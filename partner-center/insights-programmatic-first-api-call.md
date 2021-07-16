---
title: Zpřístupnění vašeho prvního volání rozhraní API pro přístup k datům pro analýzu partnera Insights
description: Příklady, jak se naučit používat rozhraní API pro přístup k analytickým datům pro partnery – přehled
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d2252ccfb601ae22ce106d87fb06b67bf0927df5
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376386"
---
# <a name="make-your-first-api-call-to-access-partner-insights-analytics-data"></a>Zpřístupnění vašeho prvního volání rozhraní API pro přístup k datům pro analýzu partnera Insights

Seznam rozhraní API pro přístup k datům služby partner Insights Analytics najdete v tématu [rozhraní API pro přístup k datům služby partner Insights Analytics](insights-programmatic-analytics-available-api.md). před provedením prvního volání rozhraní API se ujistěte, že jste splnili [požadavky](insights-programmatic-prerequisites.md) pro programový přístup k partnerům Přehledy analytics data.

## <a name="token-generation"></a>Generování tokenu

před voláním některé z metod musíte nejprve získat přístupový token pro Azure Active Directory (AAD). Přístupový token služby Azure AD je potřeba předat do autorizační hlavičky každé metody v rozhraní API. Po získání přístupového tokenu máte 60 minut, než ho budete moct použít dřív, než vyprší jeho platnost. Po vypršení platnosti tokenu můžete token aktualizovat a můžete ho dál používat pro další volání rozhraní API.

Pro vygenerování tokenu použijte níže uvedený požadavek na ukázku. Tři hodnoty, které jsou požadovány pro vygenerování tokenu `clientId` , jsou, `clientSecret` a `tenantId` . Parametr prostředku by měl být nastaven na hodnotu `https://api.partnercenter.microsoft.com`

#### <a name="request-example"></a>Příklad požadavku

```console
curl --location --request POST 'https://login.microsoftonline.com/<tenantId>/oauth2/token' \
--header 'return-client-request-id: true' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Cookie: fpc=Ar2GMei7JwdKg4Y4onHrMpvxqd4FAQAAAEhU_tcOAAAA; stsservicecookie=estsfd; x-ms-gateway-slice=estsfd' \
--data-urlencode 'resource= https://api.partnercenter.microsoft.com' \
--data-urlencode 'client_id= ' \
--data-urlencode 'client_secret= ' \
--data-urlencode 'grant_type=password' \
--data-urlencode 'scope=openid' \
--data-urlencode 'username= ' \
--data-urlencode 'password= '
```

#### <a name="response-example"></a>Příklad odpovědi

```json
{
    "token_type": "Bearer",
    "expires_in": "3599",
    "ext_expires_in": "3599",
    "expires_on": "1612794445",
    "not_before": "1612790545",
    "resource": "https://api.partnercenter.microsoft.com",
    "access_token": {Token}
}
```

Další informace o tom, jak získat token Azure AD pro vaši aplikaci, najdete v tématu [přístup k datům Analytics pomocí služby Store.](/windows/uwp/monetize/access-analytics-data-using-windows-store-services#step-2-obtain-an-azure-ad-access-token)

## <a name="programmatic-api-call"></a>Programové volání rozhraní API

Po získání tokenu AAD, jak je popsáno v předchozí části, postupujte podle těchto kroků a vytvořte první sestavu programového přístupu.

Data je možné stáhnout z následujících datových sad (DataSet):

- CustomersAndTenants
- SeatsSubscriptionsAndRevenue
- AzureUsage
- MSLearn
- OfficeUsage
- Profil
- TrainingCompletions
- DynamicsUsage
- CompetencySummaryHistory
- PowerBIUsage
- EMSUsage
- CompetencyPeformanceRequirement
- ResellerPerformance
- CLASAgreementRenewalsPropensity
- CLASAzurePropensity
- CLASD365Propensity
- CLASM365Propensity
- TeamsUsage3PApps
- TeamsUsageWorkload
- TeamsUsageMeetingsAndCalls

V následující části se zobrazí příklady, jak programově přistupovat `SubscriptionId` z datové sady DynamicsUsage.

### <a name="step-1-make-a-rest-call-using-the-get-datasets-api"></a>Krok 1: vytvoření volání REST pomocí rozhraní API získat datové sady

Odpověď rozhraní API poskytuje název datové sady, ze kterého si můžete sestavu stáhnout. V případě konkrétní datové sady poskytuje odpověď rozhraní API také seznam volitelných sloupců, které lze použít pro vlastní šablonu sestavy. Můžete také odkazovat na [definice dat](insights-data-definitions.md) a získat názvy sloupců.

#### <a name="request-example"></a>Příklad požadavku

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset'\
--header 'Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a>Příklad odpovědi

```json
{
  "value": [
    {
      "datasetName": "DynamicsUsage",
      "selectableColumns": [
        "PGAMpnId",
        "SubscriptionId",
        "SubscriptionStartDate",
        "SubscriptionEndDate",
        "SubscriptionStatus",
        "Month",
        "RevSumDivisionName",
        "RevSumCategoryName",
        "SKU",
        "SKUId",
        "FreeVsPaidSKU",
        "SalesModel",
        "DetailedSalesModel",
        "CustomerName",
        "CustomerTenantId",
        "CustomerTpid",
        "CustomerSegment",
        "CustomerMarket",
        "MPNId",
        "PartnerName",
        "PartnerLocation",
        "PartnerAttachType",
        "AvailableSeats",
        "AssignedSeats",
        "ActiveSeats",
        "DeploymentOpportunity",
        "ActiveUsagePercent"
      ],
      "availableMetrics": [
        "SubscriptionCount",
        "TotalAssignedSeats",
        "TotalSoldSeats",
        "TotalActiveSeats",
        "TotalRevenueAndACR",
        "CustomerCount",
        "CustomerTenantCount"
      ],
      "availableDateRanges": [
        "LAST_MONTH",
        "LAST_3_MONTHS",
        "LAST_6_MONTHS",
        "LAST_1_YEAR",
        "LIFETIME"
      ],
      "minimumRecurrenceInterval": 24
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Dataset fetched successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

### <a name="step-2-create-the-custom-query"></a>Krok 2: Vytvoření vlastního dotazu

V tomto kroku použijeme SubscriptionId z datové sady DynamicsUsage k vytvoření vlastního dotazu pro sestavu, kterou chceme. Výchozí časový interval, pokud není zadaný v dotazu, je 6 měsíců.

#### <a name="request-example"></a>Příklad požadavku

```cli
curl 
--location 
--request POST 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries' \ 
--header ' Authorization: Bearer <AADToken>' \ 
--header 'Content-Type: application/json' \ 
--data-raw 
{
  "Name": "SubscriptionId Dynamics ",
  "Description": "List of Subscription Id from DynamicsUsage",
  "Query": "SELECT SubscriptionId from DynamicsUsage "
            }"
```

#### <a name="response-example"></a>Příklad odpovědi

```json
{
  "value": [
    {
      "queryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
      "name": "SubscriptionId Dynamics",
      "description": "List of Subscription Id from DynamicsUsage",
      "query": "SELECT SubscriptionId from DynamicsUsage",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net",
      "createdTime": "2021-03-31T07:28:37Z"
    }
 ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

Po úspěšném provedení dotazu `queryId` se vygeneruje, který se musí použít k vygenerování sestavy.

### <a name="step-3-execute-test-query-api"></a>Krok 3: spuštění rozhraní API pro test dotazů

V tomto kroku použijeme rozhraní test Query API k získání prvních 100 řádků pro vytvořený dotaz.

#### <a name="request-example"></a>Příklad požadavku

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?queryId=7d19305c-56db-4edc-b776-428340e3a9c8' \
--header ' Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a>Příklad odpovědi

```json
{
  "value": [
    {
      "SubscriptionId": "251DE3D4-8868-4032-B518-F142DA50522F"
    },
    {
      "SubscriptionId": "758A0647-790C-435B-BEAA-652DF47E327C"
    },
    {
      "SubscriptionId": "ACE5A84B-9794-4480-82C5-AF9462DE2589"
    },
    {
      "SubscriptionId": "C75163EE-A0CA-4822-8275-E29E2490FF1C"
    },
    {
      "SubscriptionId": "082A8A18-0834-4376-A9A4-3AA4ECD02826"
    },
    .
    .
    .
    {
      "SubscriptionId": "5E10B817-7FCB-43CE-9F32-9CB60CF14658"
    },
    {
      "SubscriptionId": "7578872A-18C1-4E6B-8F51-469555337389"
    },
    {
      "SubscriptionId": "00601E10-4C05-4BA2-B977-6578F5C81D69"
    },
    {
      "SubscriptionId": "7EBFC3A9-D502-4EA2-87E7-C42971639E8C"
    },
    {
      "SubscriptionId": "2AC30AE1-5934-48FB-A0E5-EF6985761138"
    }
  ],
  "nextLink": null,
  "totalCount": 100,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

### <a name="step-4-create-the-report"></a>Krok 4: Vytvoření sestavy

V tomto kroku použijeme dříve vygenerovanou QueryId k vytvoření sestavy.

#### <a name="request-example"></a>Příklad požadavku

```cli
curl 
--location 
--request POST 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport'\
--header ' Authorization: Bearer <AADToken>' \ 
--header 'Content-Type: application/json' \ 
--data-raw 
'{
  "ReportName": "DynamicsUsage Subscription ID Report",
  "Description": "Report for getting list of Subscription Id for Dynamics Usage",
  "QueryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
  "StartTime": "2021-04-01T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": "2021-03-31T18:41:00Z",
  "QueryEndTime": "2021-06-30T18:41:00Z",
  "RecurrenceInterval": 48,
  "RecurrenceCount": 20,
  "Format": "csv",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}'
```

#### <a name="response-example"></a>Příklad odpovědi

```json
{
  "value": [
    {
      "reportId": "cdc61cfe-d028-4333-a215-a1df51ccbfd4",
      "reportName": "DynamicsUsage Subscription ID Report",
      "description": "Report for getting list of Subscription Id for Dynamics Usage",
      "queryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
      "query": "SELECT SubscriptionId from DynamicsUsage",
      "user": "GAUser@PITEST2.ccsctp.net",
      "createdTime": "2021-03-31T08:15:15Z",
      "modifiedTime": null,
      "executeNow": false,
      "startTime": "2021-04-01T18:41:00Z",
      "reportStatus": "Active",
      "recurrenceInterval": 48,
      "recurrenceCount": 20,
      "callbackUrl": "https://<SampleCallbackUrl>",
      "CallbackMethod": "GET",
      "format": "csv"
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Report created successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

Po úspěšném spuštění `reportId` se vygeneruje, který se musí použít k naplánování stažení sestavy.

### <a name="step-5-execute-report-executions-api"></a>Krok 5: spouštění rozhraní API pro spouštění sestav

V tomto kroku použijeme rozhraní API pro spouštění sestav k získání zabezpečeného umístění (URL) sestavy.

#### <a name="request-example"></a>Příklad požadavku

```cli
Curl
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/ cdc61cfe-d028-4333-a215-a1df51ccbfd4?getLatestExecution=true'\
--header ' Authorization: Bearer <AADToken>' \
```

#### <a name="response-example"></a>Příklad odpovědi

```json
{
  "value": [
    {
      "executionId": "315eb63e-e2b2-41a2-ad8e-790b040fdce3",
      "reportId": "cdc61cfe-d028-4333-a215-a1df51ccbfd4",
      "recurrenceInterval": 48,
      "recurrenceCount": 20,
      "callbackUrl": null,
      "CallbackMethod": null,
      "format": "csv",
      "executionStatus": "Pending",
      "reportLocation": null,
      "reportAccessSecureLink": null,
      "reportExpiryTime": null,
      "reportGeneratedTime": null
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

## <a name="next-steps"></a>Další kroky

- Vyzkoušejte si rozhraní API prostřednictvím [adresy URL rozhraní Swagger API](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html) .