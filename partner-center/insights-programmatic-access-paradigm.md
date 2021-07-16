---
title: programový přístup paradigma pro data Přehledy
description: Seznamte se s vysokým tokem vzoru volání rozhraní API pro programovou analýzu. Jsou zahrnutá i rozhraní API pro přístup k sestavám služby partner Insights Analytics.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: dcdd54fcc744fdb1683259203188c309a3949eff
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376393"
---
# <a name="programmatic-access-paradigm"></a><span data-ttu-id="ea3cf-104">Programové přístupové paradigma</span><span class="sxs-lookup"><span data-stu-id="ea3cf-104">Programmatic access paradigm</span></span>

<span data-ttu-id="ea3cf-105">Tento diagram znázorňuje vzor volání rozhraní API, který se používá k vytvoření nové šablony sestavy, naplánování vlastní sestavy a načtení dat o chybách.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-105">This diagram shows the API call pattern used to create a new report template, schedule the custom report and retrieve failure data.</span></span>

:::image type="content" source="images/insights/prog-acc-paradigm.png" alt-text="Tok vysoké úrovně":::
<span data-ttu-id="ea3cf-107">***Obrázek 1: tok vysoké úrovně vzoru volání rozhraní API***</span><span class="sxs-lookup"><span data-stu-id="ea3cf-107">***Figure 1: High level flow of the API call pattern***</span></span>

<span data-ttu-id="ea3cf-108">V tomto seznamu najdete další podrobnosti o obrázku 1.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-108">This list provides more details about Figure 1.</span></span>

1. <span data-ttu-id="ea3cf-109">Klientská aplikace může definovat vlastní schéma a šablonu sestavy voláním [rozhraní API pro vytvoření dotazu na sestavu](#create-report-query-api).</span><span class="sxs-lookup"><span data-stu-id="ea3cf-109">The Client Application can define the custom report schema/template by calling the [Create Report Query API](#create-report-query-api).</span></span> <span data-ttu-id="ea3cf-110">Alternativně můžete vybrat šablonu sestavy (QueryId) ze zde uvedených ukázek knihovny šablon sestav [.](insights-programmatic-system-queries.md)</span><span class="sxs-lookup"><span data-stu-id="ea3cf-110">Alternately, you can pick a report template (QueryId) from the report template library samples listed [here.](insights-programmatic-system-queries.md)</span></span>
2. <span data-ttu-id="ea3cf-111">Po úspěšném dokončení vrátí rozhraní API pro dotazování pro vytváření sestav QueryId.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-111">On success, the Create Report Query API returns the QueryId.</span></span>
3. <span data-ttu-id="ea3cf-112">Klientská aplikace pak musí volat [rozhraní API pro vytváření sestav](#create-report-api) pomocí QueryId spolu s počátečním datem sestavy, opakovat interval, opakování a nepovinný identifikátor URI zpětného volání.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-112">The client application then needs to call the [Create Report API](#create-report-api) using the QueryId along with the report start date, Repeat Interval, Recurrence, and an optional Callback URI.</span></span>
4. <span data-ttu-id="ea3cf-113">Po úspěšném dokončení vrátí [rozhraní API pro vytváření sestav](#create-report-api) ReportId.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-113">On Success, the [Create Report API](#create-report-api) returns the ReportId.</span></span>
5. <span data-ttu-id="ea3cf-114">Klientská aplikace se pošle oznámení na adresu URL zpětného volání, jakmile budou data sestavy připravena ke stažení.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-114">The client application gets notified at the callback URL as soon as the report data is ready for download.</span></span>
6. <span data-ttu-id="ea3cf-115">Klientská aplikace potom používá [rozhraní API pro spuštění sestav](#get-report-execution-api) k dotazování na stav sestavy s ID sestavy a rozsahem dat.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-115">The client application then uses the [Get Report Executions API](#get-report-execution-api) to query the status of the report with the Report ID and date range.</span></span>
7. <span data-ttu-id="ea3cf-116">Po úspěšném dokončení se odkaz na stažení sestavy vrátí a aplikace může zahájit stahování dat.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-116">On success, the report download link is returned and the application can initiate download of the data.</span></span>

## <a name="report-query-language-specification"></a><span data-ttu-id="ea3cf-117">Specifikace jazyka dotazu sestavy</span><span class="sxs-lookup"><span data-stu-id="ea3cf-117">Report query language specification</span></span>

<span data-ttu-id="ea3cf-118">I když poskytujeme [systémové dotazy](insights-programmatic-system-queries.md) , které můžete použít k vytváření sestav, můžete také vytvářet vlastní dotazy založené na vašich obchodních potřebách.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-118">While we do provide [system queries](insights-programmatic-system-queries.md) you can use to create reports, you can also create your own queries based on your business needs.</span></span> <span data-ttu-id="ea3cf-119">Další informace o vlastních dotazech najdete v tématu [vlastní specifikace dotazu](insights-programmatic-custom-query.md).</span><span class="sxs-lookup"><span data-stu-id="ea3cf-119">To learn more about custom queries, see [Custom Query Specification](insights-programmatic-custom-query.md).</span></span>

## <a name="create-report-query-api"></a><span data-ttu-id="ea3cf-120">Vytvoření rozhraní API pro dotazování sestav</span><span class="sxs-lookup"><span data-stu-id="ea3cf-120">Create report query API</span></span>

<span data-ttu-id="ea3cf-121">Rozhraní API pomáhá vytvářet vlastní dotazy definující datovou sadu, ze které je nutné exportovat sloupce a metriky.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-121">The API helps to create custom queries that define the dataset from which columns and metrics need to be exported.</span></span> <span data-ttu-id="ea3cf-122">Rozhraní API poskytuje flexibilitu pro vytvoření nové šablony vytváření sestav na základě vašich obchodních potřeb.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-122">The API provides the flexibility to create a new reporting template based on your business needs.</span></span>  

<span data-ttu-id="ea3cf-123">Můžete také použít [systémové dotazy](insights-programmatic-system-queries.md) , které poskytujeme.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-123">You can also use the [system queries](insights-programmatic-system-queries.md) we provide.</span></span> <span data-ttu-id="ea3cf-124">Pokud nepotřebujete vlastní šablony sestav, můžete zavolat [rozhraní API pro vytváření sestav](#create-report-api) přímo pomocí QueryIds systémových dotazů, které jsou k dispozici.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-124">When custom report templates are not needed, you can call [Create Report API](#create-report-api) directly using the QueryIds of the system queries that are provided.</span></span>  

<span data-ttu-id="ea3cf-125">Následující příklad ukazuje, jak vytvořit vlastní dotaz pro získání prvních 10 zákazníků podle výnosů za poslední měsíc.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-125">The following example shows how to create a custom query to get top 10 customers by revenue for last month.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="ea3cf-126">Syntaxe žádosti</span><span class="sxs-lookup"><span data-stu-id="ea3cf-126">Request syntax</span></span>

|    <span data-ttu-id="ea3cf-127">Metoda</span><span class="sxs-lookup"><span data-stu-id="ea3cf-127">Method</span></span>     |    <span data-ttu-id="ea3cf-128">Identifikátor URI žádosti</span><span class="sxs-lookup"><span data-stu-id="ea3cf-128">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="ea3cf-129">POST</span><span class="sxs-lookup"><span data-stu-id="ea3cf-129">POST</span></span>     |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries`|
|||

### <a name="request-header"></a><span data-ttu-id="ea3cf-130">Hlavička požadavku</span><span class="sxs-lookup"><span data-stu-id="ea3cf-130">Request header</span></span>

|    <span data-ttu-id="ea3cf-131">Hlavička</span><span class="sxs-lookup"><span data-stu-id="ea3cf-131">Header</span></span>     |    <span data-ttu-id="ea3cf-132">Typ</span><span class="sxs-lookup"><span data-stu-id="ea3cf-132">Type</span></span>     |    <span data-ttu-id="ea3cf-133">Description</span><span class="sxs-lookup"><span data-stu-id="ea3cf-133">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="ea3cf-134">Autorizace</span><span class="sxs-lookup"><span data-stu-id="ea3cf-134">Authorization</span></span>     |    <span data-ttu-id="ea3cf-135">řetězec</span><span class="sxs-lookup"><span data-stu-id="ea3cf-135">string</span></span> |<span data-ttu-id="ea3cf-136">Povinná hodnota.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-136">Required.</span></span> <span data-ttu-id="ea3cf-137">přístupový token Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="ea3cf-137">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="ea3cf-138">Formát je  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="ea3cf-138">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="ea3cf-139">Typ obsahu</span><span class="sxs-lookup"><span data-stu-id="ea3cf-139">Content-Type</span></span>     |<span data-ttu-id="ea3cf-140">řetězec</span><span class="sxs-lookup"><span data-stu-id="ea3cf-140">string</span></span> |`Application/JSON` |
||||

### <a name="path-parameter"></a><span data-ttu-id="ea3cf-141">Parametr cesty</span><span class="sxs-lookup"><span data-stu-id="ea3cf-141">Path parameter</span></span>

<span data-ttu-id="ea3cf-142">Žádná</span><span class="sxs-lookup"><span data-stu-id="ea3cf-142">None</span></span>

### <a name="query-parameter"></a><span data-ttu-id="ea3cf-143">Parametr dotazu</span><span class="sxs-lookup"><span data-stu-id="ea3cf-143">Query parameter</span></span>

<span data-ttu-id="ea3cf-144">Žádná</span><span class="sxs-lookup"><span data-stu-id="ea3cf-144">None</span></span>

### <a name="sample-request-payload"></a><span data-ttu-id="ea3cf-145">Ukázková datová část požadavku</span><span class="sxs-lookup"><span data-stu-id="ea3cf-145">Sample request payload</span></span>

```json
{ 
  "Name": "CustomersRevenueQuery", 
  "Description": "Query to get top 10 customers by revenue for last month", 
  "Query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH" 
}
```

### <a name="glossary"></a><span data-ttu-id="ea3cf-146">Glosář</span><span class="sxs-lookup"><span data-stu-id="ea3cf-146">Glossary</span></span>

<span data-ttu-id="ea3cf-147">Tato tabulka poskytuje klíčové definice prvků v datové části požadavku.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-147">This table provides the key definitions of elements in the request payload.</span></span>

|<span data-ttu-id="ea3cf-148">Parametr</span><span class="sxs-lookup"><span data-stu-id="ea3cf-148">Parameter</span></span>|    <span data-ttu-id="ea3cf-149">Povinné</span><span class="sxs-lookup"><span data-stu-id="ea3cf-149">Required</span></span>     |    <span data-ttu-id="ea3cf-150">Popis</span><span class="sxs-lookup"><span data-stu-id="ea3cf-150">Description</span></span>     |    <span data-ttu-id="ea3cf-151">Povolené hodnoty</span><span class="sxs-lookup"><span data-stu-id="ea3cf-151">Allowed Values</span></span>     |
|-----|    -----    |    -----    |    -----    |
|<span data-ttu-id="ea3cf-152">Name</span><span class="sxs-lookup"><span data-stu-id="ea3cf-152">Name</span></span> |    <span data-ttu-id="ea3cf-153">Yes</span><span class="sxs-lookup"><span data-stu-id="ea3cf-153">Yes</span></span>     |    <span data-ttu-id="ea3cf-154">Popisný název dotazu</span><span class="sxs-lookup"><span data-stu-id="ea3cf-154">Friendly name of the query</span></span>     |    <span data-ttu-id="ea3cf-155">řetězec</span><span class="sxs-lookup"><span data-stu-id="ea3cf-155">string</span></span>     |
|    <span data-ttu-id="ea3cf-156">Popis</span><span class="sxs-lookup"><span data-stu-id="ea3cf-156">Description</span></span>     |    <span data-ttu-id="ea3cf-157">No</span><span class="sxs-lookup"><span data-stu-id="ea3cf-157">No</span></span>     |    <span data-ttu-id="ea3cf-158">Popis toho, co dotaz vrátí</span><span class="sxs-lookup"><span data-stu-id="ea3cf-158">Description of what the query returns</span></span>     |    <span data-ttu-id="ea3cf-159">řetězec</span><span class="sxs-lookup"><span data-stu-id="ea3cf-159">string</span></span>     |
|    <span data-ttu-id="ea3cf-160">Dotaz</span><span class="sxs-lookup"><span data-stu-id="ea3cf-160">Query</span></span>     |    <span data-ttu-id="ea3cf-161">Yes</span><span class="sxs-lookup"><span data-stu-id="ea3cf-161">Yes</span></span>     |    <span data-ttu-id="ea3cf-162">Řetězec dotazu sestavy</span><span class="sxs-lookup"><span data-stu-id="ea3cf-162">Report query string</span></span>     |    <span data-ttu-id="ea3cf-163">Datový typ: řetězec</span><span class="sxs-lookup"><span data-stu-id="ea3cf-163">Data type: string</span></span> <br> <span data-ttu-id="ea3cf-164">[Vlastní dotaz](insights-programmatic-custom-query.md) založený na obchodních potřebách</span><span class="sxs-lookup"><span data-stu-id="ea3cf-164">[Custom query](insights-programmatic-custom-query.md) based on business need</span></span> |
|        |        |        |        |

> [!Note]
> <span data-ttu-id="ea3cf-165">Vlastní Ukázky dotazů najdete v tématu [Příklady ukázkových dotazů.](insights-programmatic-sample-queries.md)</span><span class="sxs-lookup"><span data-stu-id="ea3cf-165">For custom query samples, see [Examples of sample queries.](insights-programmatic-sample-queries.md)</span></span>

### <a name="sample-response"></a><span data-ttu-id="ea3cf-166">Ukázková odpověď</span><span class="sxs-lookup"><span data-stu-id="ea3cf-166">Sample response</span></span>

<span data-ttu-id="ea3cf-167">Datová část odpovědi je strukturována takto:</span><span class="sxs-lookup"><span data-stu-id="ea3cf-167">The response payload is structured as follows:</span></span>

<span data-ttu-id="ea3cf-168">Kódy odpovědí: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="ea3cf-168">Response Codes: 200, 400, 401, 403, 500</span></span>

<span data-ttu-id="ea3cf-169">Příklad datové části odpovědi:</span><span class="sxs-lookup"><span data-stu-id="ea3cf-169">Response payload example:</span></span>

```json
{ 
  "value": [ 
    { 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
      "name": "CustomersRevenueQuery",
      "description": "Query to get top 10 customers by revenue for last month",
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T12:52:39Z" 
    }
  ], 
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
} 
```

### <a name="glossary"></a><span data-ttu-id="ea3cf-170">Glosář</span><span class="sxs-lookup"><span data-stu-id="ea3cf-170">Glossary</span></span>

<span data-ttu-id="ea3cf-171">Tato tabulka poskytuje klíčové definice prvků v datové části požadavku.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-171">This table provides the key definitions of elements in the request payload.</span></span>

|    <span data-ttu-id="ea3cf-172">Parametr</span><span class="sxs-lookup"><span data-stu-id="ea3cf-172">Parameter</span></span>     |    <span data-ttu-id="ea3cf-173">Popis</span><span class="sxs-lookup"><span data-stu-id="ea3cf-173">Description</span></span>     |
|    ----    |    ----    |
|    <span data-ttu-id="ea3cf-174">QueryId</span><span class="sxs-lookup"><span data-stu-id="ea3cf-174">QueryId</span></span>     |    <span data-ttu-id="ea3cf-175">Univerzálně jedinečný identifikátor (UUID) dotazu, který jste vytvořili</span><span class="sxs-lookup"><span data-stu-id="ea3cf-175">Universally unique identifier (UUID) of the query you created</span></span>     |
|    <span data-ttu-id="ea3cf-176">Name</span><span class="sxs-lookup"><span data-stu-id="ea3cf-176">Name</span></span>     |    <span data-ttu-id="ea3cf-177">Popisný název zadaný pro dotaz v datové části požadavku</span><span class="sxs-lookup"><span data-stu-id="ea3cf-177">Friendly name given to the query in the request payload</span></span>     |
|    <span data-ttu-id="ea3cf-178">Description</span><span class="sxs-lookup"><span data-stu-id="ea3cf-178">Description</span></span>     |    <span data-ttu-id="ea3cf-179">Popis zadaný při vytváření dotazu</span><span class="sxs-lookup"><span data-stu-id="ea3cf-179">Description given during creation of the query</span></span>     |
|    <span data-ttu-id="ea3cf-180">Dotaz</span><span class="sxs-lookup"><span data-stu-id="ea3cf-180">Query</span></span>     |    <span data-ttu-id="ea3cf-181">Dotaz na sestavu předaný jako vstup během vytváření dotazu</span><span class="sxs-lookup"><span data-stu-id="ea3cf-181">Report query passed as input during query creation</span></span>     |
|    <span data-ttu-id="ea3cf-182">Typ</span><span class="sxs-lookup"><span data-stu-id="ea3cf-182">Type</span></span>     |    <span data-ttu-id="ea3cf-183">Nastavit na `userDefined`</span><span class="sxs-lookup"><span data-stu-id="ea3cf-183">Set to `userDefined`</span></span>     |
|    <span data-ttu-id="ea3cf-184">Uživatel</span><span class="sxs-lookup"><span data-stu-id="ea3cf-184">User</span></span>     |    <span data-ttu-id="ea3cf-185">ID uživatele, které se použilo k vytvoření dotazu</span><span class="sxs-lookup"><span data-stu-id="ea3cf-185">User ID used to create of the query</span></span>     |
|    <span data-ttu-id="ea3cf-186">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="ea3cf-186">CreatedTime</span></span>     |    <span data-ttu-id="ea3cf-187">Čas UTC, kdy byl dotaz vytvořen v tomto formátu: RRRR-MM-ddTHH: mm: ssZ</span><span class="sxs-lookup"><span data-stu-id="ea3cf-187">UTC Time the query was created in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="ea3cf-188">TotalCount</span><span class="sxs-lookup"><span data-stu-id="ea3cf-188">TotalCount</span></span>     |    <span data-ttu-id="ea3cf-189">Počet datových sad v poli hodnot</span><span class="sxs-lookup"><span data-stu-id="ea3cf-189">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="ea3cf-190">StatusCode</span><span class="sxs-lookup"><span data-stu-id="ea3cf-190">StatusCode</span></span>     |    <span data-ttu-id="ea3cf-191">Kód výsledku</span><span class="sxs-lookup"><span data-stu-id="ea3cf-191">Result Code</span></span> <br> <span data-ttu-id="ea3cf-192">Možné hodnoty jsou 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="ea3cf-192">The possible values are 200, 400, 401, 403, 500</span></span>     |
|    <span data-ttu-id="ea3cf-193">zpráva</span><span class="sxs-lookup"><span data-stu-id="ea3cf-193">message</span></span>     |    <span data-ttu-id="ea3cf-194">Stavová zpráva od spuštění rozhraní API</span><span class="sxs-lookup"><span data-stu-id="ea3cf-194">Status message from the execution of the API</span></span>     |
|        |        |

## <a name="create-report-api"></a><span data-ttu-id="ea3cf-195">Vytvoření rozhraní API pro sestavy</span><span class="sxs-lookup"><span data-stu-id="ea3cf-195">Create report API</span></span>

<span data-ttu-id="ea3cf-196">Po úspěšném vytvoření vlastní šablony sestavy a přijetí QueryID jako součást odpovědi na [dotaz na vytvoření sestavy](#create-report-query-api) lze toto rozhraní API volat, aby bylo možné naplánovat spuštění dotazu v pravidelných intervalech.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-196">On creating a custom report template successfully and receiving the QueryID as part of [Create Report Query](#create-report-query-api) response, this API can be called to schedule a query to be executed at regular intervals.</span></span> <span data-ttu-id="ea3cf-197">Můžete nastavit četnost a plán pro doručení sestavy.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-197">You can set a frequency and schedule for the report to be delivered.</span></span>
<span data-ttu-id="ea3cf-198">Pro systémové dotazy, které poskytujeme, se dá rozhraní API pro vytváření sestav volat taky pomocí [QueryId](insights-programmatic-system-queries.md).</span><span class="sxs-lookup"><span data-stu-id="ea3cf-198">For system queries we provide, the Create Report API can also be called with [QueryId](insights-programmatic-system-queries.md).</span></span>

### <a name="callback-url"></a><span data-ttu-id="ea3cf-199">Adresa URL zpětného volání</span><span class="sxs-lookup"><span data-stu-id="ea3cf-199">Callback URL</span></span>

<span data-ttu-id="ea3cf-200">Rozhraní API pro vytvoření sestavy přijímá adresu URL zpětného volání.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-200">The create report API accepts a callback URL.</span></span> <span data-ttu-id="ea3cf-201">Tato adresa URL se bude volat, jakmile bude generování sestavy úspěšné.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-201">This URL will be called once the report generation is successful.</span></span> <span data-ttu-id="ea3cf-202">Adresa URL zpětného volání by měla být veřejně přístupná.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-202">The callback URL should be publicly reachable.</span></span> <span data-ttu-id="ea3cf-203">Kromě adresy URL lze také zadat metodu zpětného volání.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-203">In addition to the URL a callback method can also be given.</span></span> <span data-ttu-id="ea3cf-204">Metoda zpětného volání může být pouze GET nebo POST.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-204">The callback method can only be "GET" or "POST".</span></span> <span data-ttu-id="ea3cf-205">Výchozí metoda, pokud se žádná hodnota předá, bude POST.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-205">The default method if no value is passed will be "POST".</span></span> <span data-ttu-id="ea3cf-206">ReportId, který dokončil generování, se vždy předá zpět během zpětného volání.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-206">The reportId that has completed generation will always be passed back during the callback.</span></span>

<span data-ttu-id="ea3cf-207">Zpětné volání POST: Pokud předaná adresa URL byla `https://www.contosso.com/callback` , bude volaná zpětná adresa URL . `https://www.contosso.com/callback/<reportID>`</span><span class="sxs-lookup"><span data-stu-id="ea3cf-207">POST callback: If the URL passed was `https://www.contosso.com/callback`, then the called back URL will be `https://www.contosso.com/callback/<reportID>`</span></span> 

<span data-ttu-id="ea3cf-208">Zpětné volání GET: Pokud byla předaná adresa URL `https://www.contosso.com/callback` , bude volaná zpětná adresa URL `https://www.contosso.com/callback?reportId=<reportID>`</span><span class="sxs-lookup"><span data-stu-id="ea3cf-208">GET callback: If the URL passed was `https://www.contosso.com/callback`, then the called back URL will be `https://www.contosso.com/callback?reportId=<reportID>`</span></span> 

### <a name="executenow-reports"></a><span data-ttu-id="ea3cf-209">Sestavy ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="ea3cf-209">ExecuteNow reports</span></span>

<span data-ttu-id="ea3cf-210">Existuje zřízení pro generování sestavy bez plánování.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-210">There is a provision to generate a report without scheduling.</span></span> <span data-ttu-id="ea3cf-211">Datová část rozhraní API pro vytvoření sestavy může přijmout parametr , který při volání rozhraní API zařadí sestavu do fronty, která `ExecuteNow` se má vygenerovat.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-211">The report create API payload can accept a parameter `ExecuteNow`, which will enqueue the report to be generated as soon as the API is called.</span></span> <span data-ttu-id="ea3cf-212">Pokud `ExecuteNow` je nastavená hodnota true, pole `StartTime` , se ignorují, protože tyto sestavy nejsou `RecurrenceCount` `RecurrenceInterval` naplánované.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-212">When `ExecuteNow` is set to true, the fields: `StartTime`, `RecurrenceCount`, `RecurrenceInterval` are ignored as these reports are not scheduled.</span></span>

<span data-ttu-id="ea3cf-213">Pokud má hodnota true, je možné předat dvě další `ExecuteNow` pole a `QueryStartTime` `QueryEndTime` .</span><span class="sxs-lookup"><span data-stu-id="ea3cf-213">Two additional fields can be passed when `ExecuteNow` is true, `QueryStartTime` and `QueryEndTime`.</span></span> <span data-ttu-id="ea3cf-214">Tato dvě pole `TIMESPAN` přepíší pole v dotazu.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-214">These two fields will override the `TIMESPAN` field in the query.</span></span> <span data-ttu-id="ea3cf-215">Tato pole se nevztahují na naplánované sestavy, protože data se budou průběžně generovat po pevné časové období, které se nemění.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-215">These fields are not applicable for scheduled reports as data will get continuously generated for a fixed time period that does not change.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="ea3cf-216">Syntaxe požadavku</span><span class="sxs-lookup"><span data-stu-id="ea3cf-216">Request syntax</span></span>

|    <span data-ttu-id="ea3cf-217">Metoda</span><span class="sxs-lookup"><span data-stu-id="ea3cf-217">Method</span></span>     |    <span data-ttu-id="ea3cf-218">Identifikátor URI žádosti</span><span class="sxs-lookup"><span data-stu-id="ea3cf-218">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="ea3cf-219">POST</span><span class="sxs-lookup"><span data-stu-id="ea3cf-219">POST</span></span>     |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport` |

### <a name="request-header"></a><span data-ttu-id="ea3cf-220">Hlavička požadavku</span><span class="sxs-lookup"><span data-stu-id="ea3cf-220">Request header</span></span>

|    <span data-ttu-id="ea3cf-221">Hlavička</span><span class="sxs-lookup"><span data-stu-id="ea3cf-221">Header</span></span>     |    <span data-ttu-id="ea3cf-222">Typ</span><span class="sxs-lookup"><span data-stu-id="ea3cf-222">Type</span></span>     |    <span data-ttu-id="ea3cf-223">Description</span><span class="sxs-lookup"><span data-stu-id="ea3cf-223">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="ea3cf-224">Autorizace</span><span class="sxs-lookup"><span data-stu-id="ea3cf-224">Authorization</span></span>     |    <span data-ttu-id="ea3cf-225">řetězec</span><span class="sxs-lookup"><span data-stu-id="ea3cf-225">string</span></span> |<span data-ttu-id="ea3cf-226">Povinná hodnota.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-226">Required.</span></span> <span data-ttu-id="ea3cf-227">Přístupový Azure Active Directory služby Azure AD (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="ea3cf-227">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="ea3cf-228">Formát je  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="ea3cf-228">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="ea3cf-229">Typ obsahu</span><span class="sxs-lookup"><span data-stu-id="ea3cf-229">Content-Type</span></span>     |<span data-ttu-id="ea3cf-230">řetězec</span><span class="sxs-lookup"><span data-stu-id="ea3cf-230">string</span></span> |`Application/JSON` |

### <a name="path-parameter"></a><span data-ttu-id="ea3cf-231">Parametr cesty</span><span class="sxs-lookup"><span data-stu-id="ea3cf-231">Path Parameter</span></span>

<span data-ttu-id="ea3cf-232">Žádná</span><span class="sxs-lookup"><span data-stu-id="ea3cf-232">None</span></span>

### <a name="query-parameter"></a><span data-ttu-id="ea3cf-233">Parametr dotazu</span><span class="sxs-lookup"><span data-stu-id="ea3cf-233">Query Parameter</span></span>

<span data-ttu-id="ea3cf-234">Žádná</span><span class="sxs-lookup"><span data-stu-id="ea3cf-234">None</span></span>

### <a name="sample-request-payload"></a><span data-ttu-id="ea3cf-235">Ukázková datová část požadavku</span><span class="sxs-lookup"><span data-stu-id="ea3cf-235">Sample request payload</span></span>

```json
{
  "ReportName": "Top10_CustomersReport",
  "Description": "Top 10 customers by revenue for last month",
  "QueryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
  "StartTime": "2021-03-31T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": null,
  "QueryEndTime": null,
  "RecurrenceInterval": 24,
  "RecurrenceCount": 100,
  "Format": "CSV",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}
```

### <a name="glossary"></a><span data-ttu-id="ea3cf-236">Glosář</span><span class="sxs-lookup"><span data-stu-id="ea3cf-236">Glossary</span></span>

<span data-ttu-id="ea3cf-237">Klíčové definice elementů v datové části požadavku jsou uvedené níže:</span><span class="sxs-lookup"><span data-stu-id="ea3cf-237">Key definitions of elements in the request payload are articulated below:</span></span>

|    <span data-ttu-id="ea3cf-238">Parametr</span><span class="sxs-lookup"><span data-stu-id="ea3cf-238">Parameter</span></span>     |    <span data-ttu-id="ea3cf-239">Povinné</span><span class="sxs-lookup"><span data-stu-id="ea3cf-239">Required</span></span>     |    <span data-ttu-id="ea3cf-240">Popis</span><span class="sxs-lookup"><span data-stu-id="ea3cf-240">Description</span></span>     |    <span data-ttu-id="ea3cf-241">Povolené hodnoty</span><span class="sxs-lookup"><span data-stu-id="ea3cf-241">Allowed Values</span></span>     |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="ea3cf-242">ReportName</span><span class="sxs-lookup"><span data-stu-id="ea3cf-242">ReportName</span></span>     |    <span data-ttu-id="ea3cf-243">Yes</span><span class="sxs-lookup"><span data-stu-id="ea3cf-243">Yes</span></span>     |    <span data-ttu-id="ea3cf-244">Název, který se má k sestavě přiřadit</span><span class="sxs-lookup"><span data-stu-id="ea3cf-244">Name to be assigned to the report</span></span>     |    <span data-ttu-id="ea3cf-245">řetězec</span><span class="sxs-lookup"><span data-stu-id="ea3cf-245">string</span></span>     |
|    <span data-ttu-id="ea3cf-246">Popis</span><span class="sxs-lookup"><span data-stu-id="ea3cf-246">Description</span></span>     |    <span data-ttu-id="ea3cf-247">No</span><span class="sxs-lookup"><span data-stu-id="ea3cf-247">No</span></span>     |    <span data-ttu-id="ea3cf-248">Popis vytvořené sestavy</span><span class="sxs-lookup"><span data-stu-id="ea3cf-248">Description of the created report</span></span>     |    <span data-ttu-id="ea3cf-249">řetězec</span><span class="sxs-lookup"><span data-stu-id="ea3cf-249">string</span></span>     |
|    <span data-ttu-id="ea3cf-250">ID dotazu</span><span class="sxs-lookup"><span data-stu-id="ea3cf-250">QueryId</span></span>     |    <span data-ttu-id="ea3cf-251">Yes</span><span class="sxs-lookup"><span data-stu-id="ea3cf-251">Yes</span></span>     |    <span data-ttu-id="ea3cf-252">ID dotazu sestavy</span><span class="sxs-lookup"><span data-stu-id="ea3cf-252">Report query ID</span></span>     |    <span data-ttu-id="ea3cf-253">řetězec</span><span class="sxs-lookup"><span data-stu-id="ea3cf-253">string</span></span>     |
|    <span data-ttu-id="ea3cf-254">StartTime</span><span class="sxs-lookup"><span data-stu-id="ea3cf-254">StartTime</span></span>     |    <span data-ttu-id="ea3cf-255">Yes</span><span class="sxs-lookup"><span data-stu-id="ea3cf-255">Yes</span></span>     |    <span data-ttu-id="ea3cf-256">Časové razítko UTC, ve kterém bude generování sestavy začínat.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-256">UTC Timestamp at which the report generation will begin.</span></span> <br> <span data-ttu-id="ea3cf-257">Formát by měl být: rrrr-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="ea3cf-257">The format should be: yyyy-MM-ddTHH:mm:ssZ</span></span>       |    <span data-ttu-id="ea3cf-258">řetězec</span><span class="sxs-lookup"><span data-stu-id="ea3cf-258">string</span></span>     |
|    <span data-ttu-id="ea3cf-259">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="ea3cf-259">ExecuteNow</span></span>     |    <span data-ttu-id="ea3cf-260">No</span><span class="sxs-lookup"><span data-stu-id="ea3cf-260">No</span></span>     |    <span data-ttu-id="ea3cf-261">Tento parametr by se měl použít k vytvoření sestavy, která se spustí pouze jednou.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-261">This parameter should be used to create a report that will be executed only once.</span></span> <span data-ttu-id="ea3cf-262">`StartTime`A `RecurrenceInterval` `RecurrenceCount` se ignorují, pokud je nastavená hodnota true.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-262">`StartTime`, `RecurrenceInterval` and `RecurrenceCount` are ignored if this is set to true.</span></span> <span data-ttu-id="ea3cf-263">Sestava se spustí okamžitě asynchronním způsobem.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-263">The report is executed immediately in an asynchronous fashion</span></span>     |    <span data-ttu-id="ea3cf-264">true/false</span><span class="sxs-lookup"><span data-stu-id="ea3cf-264">true/false</span></span>     |
|    <span data-ttu-id="ea3cf-265">Čas_spuštění_dotazu</span><span class="sxs-lookup"><span data-stu-id="ea3cf-265">QueryStartTime</span></span>     |    <span data-ttu-id="ea3cf-266">No</span><span class="sxs-lookup"><span data-stu-id="ea3cf-266">No</span></span>     |    <span data-ttu-id="ea3cf-267">Volitelně určuje čas spuštění dotazu extrahování dat.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-267">Optionally specifies the start time for the query extracting the data.</span></span> <span data-ttu-id="ea3cf-268">Tento parametr se vztahuje pouze na jednu sestavu spuštění, která má `ExecuteNow` nastavenou hodnotu true.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-268">This parameter is applicable only for one time execution report that have `ExecuteNow` set to true.</span></span> <span data-ttu-id="ea3cf-269">Nastavení tohoto parametru `TIMESPAN` přepíše dané v dotazu.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-269">Setting this parameter overrides `TIMESPAN` given in the query.</span></span> <span data-ttu-id="ea3cf-270">Formát by měl být rrrr-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-270">The format should be yyyy-MM-ddTHH:mm:ssZ</span></span>     |    <span data-ttu-id="ea3cf-271">Časové razítko jako řetězec</span><span class="sxs-lookup"><span data-stu-id="ea3cf-271">Timestamp as string</span></span>     |
|    <span data-ttu-id="ea3cf-272">QueryEndTime</span><span class="sxs-lookup"><span data-stu-id="ea3cf-272">QueryEndTime</span></span>     |    <span data-ttu-id="ea3cf-273">No</span><span class="sxs-lookup"><span data-stu-id="ea3cf-273">No</span></span>     |    <span data-ttu-id="ea3cf-274">Volitelně určuje koncový čas pro dotaz extrahující data.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-274">Optionally specifies the end time for the query extracting the data.</span></span> <span data-ttu-id="ea3cf-275">Tento parametr se vztahuje pouze na jednu sestavu spuštění, která má `ExecuteNow` nastavenou hodnotu true.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-275">This parameter is applicable only for one time execution report that have `ExecuteNow` set to true.</span></span> <span data-ttu-id="ea3cf-276">Nastavení tohoto parametru `TIMESPAN` přepíše dané v dotazu.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-276">Setting this parameter overrides `TIMESPAN` given in the query.</span></span> <span data-ttu-id="ea3cf-277">Formát by měl být rrrr-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-277">The format should be yyyy-MM-ddTHH:mm:ssZ</span></span>     |    <span data-ttu-id="ea3cf-278">Časové razítko jako řetězec</span><span class="sxs-lookup"><span data-stu-id="ea3cf-278">Timestamp as string</span></span>     |
|    <span data-ttu-id="ea3cf-279">OpakováníInterval</span><span class="sxs-lookup"><span data-stu-id="ea3cf-279">RecurrenceInterval</span></span>     |    <span data-ttu-id="ea3cf-280">Yes</span><span class="sxs-lookup"><span data-stu-id="ea3cf-280">Yes</span></span>     |    <span data-ttu-id="ea3cf-281">Frekvence v hodinách, kdy se má sestava generovat.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-281">Frequency in hours at which the report should be generated.</span></span> <br> <span data-ttu-id="ea3cf-282">Minimální hodnota je 4 a maximální hodnota je 2 160.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-282">Minimum value is 4 and Maximum value is 2160.</span></span>      |    <span data-ttu-id="ea3cf-283">integer</span><span class="sxs-lookup"><span data-stu-id="ea3cf-283">integer</span></span>     |
|    <span data-ttu-id="ea3cf-284">Počet opakování</span><span class="sxs-lookup"><span data-stu-id="ea3cf-284">RecurrenceCount</span></span>     |    <span data-ttu-id="ea3cf-285">No</span><span class="sxs-lookup"><span data-stu-id="ea3cf-285">No</span></span>     |    <span data-ttu-id="ea3cf-286">Počet sestav, které se vygenerují</span><span class="sxs-lookup"><span data-stu-id="ea3cf-286">Number of reports to be generated.</span></span>     |    <span data-ttu-id="ea3cf-287">integer</span><span class="sxs-lookup"><span data-stu-id="ea3cf-287">integer</span></span>     |
|    <span data-ttu-id="ea3cf-288">Formát</span><span class="sxs-lookup"><span data-stu-id="ea3cf-288">Format</span></span>     |    <span data-ttu-id="ea3cf-289">No</span><span class="sxs-lookup"><span data-stu-id="ea3cf-289">No</span></span>     |    <span data-ttu-id="ea3cf-290">Formát exportovaného souboru.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-290">File format of the exported file.</span></span> <br> <span data-ttu-id="ea3cf-291">Výchozí hodnota je CSV.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-291">Default is CSV.</span></span>    |    <span data-ttu-id="ea3cf-292">"CSV"/"TSV"</span><span class="sxs-lookup"><span data-stu-id="ea3cf-292">"CSV"/"TSV"</span></span>     |
|    <span data-ttu-id="ea3cf-293">CallbackUrl (Url zpětného volání)</span><span class="sxs-lookup"><span data-stu-id="ea3cf-293">CallbackUrl</span></span>     |    <span data-ttu-id="ea3cf-294">No</span><span class="sxs-lookup"><span data-stu-id="ea3cf-294">No</span></span>     |    <span data-ttu-id="ea3cf-295">Veřejně přístupná adresa URL, kterou je možné volitelně nakonfigurovat jako cíl zpětného volání</span><span class="sxs-lookup"><span data-stu-id="ea3cf-295">Publicly reachable URL that can be optionally configured as callback destination</span></span>     |    <span data-ttu-id="ea3cf-296">Řetězec (adresa URL protokolu HTTP)</span><span class="sxs-lookup"><span data-stu-id="ea3cf-296">String (http URL)</span></span>     |
|    <span data-ttu-id="ea3cf-297">Metoda zpětného volání</span><span class="sxs-lookup"><span data-stu-id="ea3cf-297">CallbackMethod</span></span>     |    <span data-ttu-id="ea3cf-298">No</span><span class="sxs-lookup"><span data-stu-id="ea3cf-298">No</span></span>     |    <span data-ttu-id="ea3cf-299">Metoda, která se má použít pro zpětné volání</span><span class="sxs-lookup"><span data-stu-id="ea3cf-299">The method to be used for callback</span></span>     |    <span data-ttu-id="ea3cf-300">GET/POST</span><span class="sxs-lookup"><span data-stu-id="ea3cf-300">GET/POST</span></span>     |
|        |        |        |        |

### <a name="sample-response"></a><span data-ttu-id="ea3cf-301">Ukázková odpověď</span><span class="sxs-lookup"><span data-stu-id="ea3cf-301">Sample response</span></span>

<span data-ttu-id="ea3cf-302">Datová část odpovědi je strukturována takto:</span><span class="sxs-lookup"><span data-stu-id="ea3cf-302">The response payload is structured as follows:</span></span>

<span data-ttu-id="ea3cf-303">Kódy odpovědí: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="ea3cf-303">Response Codes: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="ea3cf-304">Příklad datové části odpovědi:</span><span class="sxs-lookup"><span data-stu-id="ea3cf-304">Response payload example:</span></span>

```json
{ 
  "value": [
    { 
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf", 
      "reportName": "Top10_CustomersReport", 
      "description": "Top 10 customers by revenue for last month", 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033", 
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH", 
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T13:11:58Z", 
      "modifiedTime": null, 
      "executeNow": false, 
      "startTime": "2021-03-31T18:41:00Z", 
      "reportStatus": "Active", 
      "recurrenceInterval": 24, 
      "recurrenceCount": 100, 
      "callbackUrl": "https://<SampleCallbackUrl>", 
      "callbackMethod": "GET", 
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

### <a name="glossary"></a><span data-ttu-id="ea3cf-305">Glosář</span><span class="sxs-lookup"><span data-stu-id="ea3cf-305">Glossary</span></span>

<span data-ttu-id="ea3cf-306">Klíčové definice prvků v odpovědi jsou kloubově navýšené:</span><span class="sxs-lookup"><span data-stu-id="ea3cf-306">Key definitions of elements in the response are articulated below:</span></span>

|    <span data-ttu-id="ea3cf-307">Parametr</span><span class="sxs-lookup"><span data-stu-id="ea3cf-307">Parameter</span></span>     |    <span data-ttu-id="ea3cf-308">Popis</span><span class="sxs-lookup"><span data-stu-id="ea3cf-308">Description</span></span>     |
|    ----    |    ----    |
|    <span data-ttu-id="ea3cf-309">ReportId</span><span class="sxs-lookup"><span data-stu-id="ea3cf-309">ReportId</span></span>     |    <span data-ttu-id="ea3cf-310">Univerzálně jedinečný identifikátor (UUID) sestavy, kterou jste vytvořili</span><span class="sxs-lookup"><span data-stu-id="ea3cf-310">Universally unique identifier (UUID) of the report you created</span></span>     |
|    <span data-ttu-id="ea3cf-311">ReportName</span><span class="sxs-lookup"><span data-stu-id="ea3cf-311">ReportName</span></span>     |    <span data-ttu-id="ea3cf-312">Název zadaný pro sestavu v datové části požadavku</span><span class="sxs-lookup"><span data-stu-id="ea3cf-312">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="ea3cf-313">Description</span><span class="sxs-lookup"><span data-stu-id="ea3cf-313">Description</span></span>     |    <span data-ttu-id="ea3cf-314">Popis zadaný při vytváření sestavy</span><span class="sxs-lookup"><span data-stu-id="ea3cf-314">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="ea3cf-315">QueryId</span><span class="sxs-lookup"><span data-stu-id="ea3cf-315">QueryId</span></span>     |    <span data-ttu-id="ea3cf-316">ID dotazu předané v době, kdy jste sestavu vytvořili</span><span class="sxs-lookup"><span data-stu-id="ea3cf-316">Query ID passed at the time you created the report</span></span>     |
|    <span data-ttu-id="ea3cf-317">Dotaz</span><span class="sxs-lookup"><span data-stu-id="ea3cf-317">Query</span></span>     |    <span data-ttu-id="ea3cf-318">Text dotazu, který se spustí pro tuto sestavu</span><span class="sxs-lookup"><span data-stu-id="ea3cf-318">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="ea3cf-319">Uživatel</span><span class="sxs-lookup"><span data-stu-id="ea3cf-319">User</span></span>     |    <span data-ttu-id="ea3cf-320">ID uživatele, které se použilo k vytvoření sestavy</span><span class="sxs-lookup"><span data-stu-id="ea3cf-320">User ID used to create the report</span></span>     |
|    <span data-ttu-id="ea3cf-321">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="ea3cf-321">CreatedTime</span></span>     |    <span data-ttu-id="ea3cf-322">Čas UTC, kdy byla sestava vytvořena v tomto formátu: RRRR-MM-ddTHH: mm: ssZ</span><span class="sxs-lookup"><span data-stu-id="ea3cf-322">UTC Time the report was created in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="ea3cf-323">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="ea3cf-323">ModifiedTime</span></span>     |    <span data-ttu-id="ea3cf-324">Čas UTC, kdy se sestava naposledy změnila v tomto formátu: RRRR-MM-ddTHH: mm: ssZ</span><span class="sxs-lookup"><span data-stu-id="ea3cf-324">UTC Time the report was last modified in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="ea3cf-325">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="ea3cf-325">ExecuteNow</span></span>     |    <span data-ttu-id="ea3cf-326">`ExecuteNow` příznak nastavený v okamžiku vytvoření sestavy</span><span class="sxs-lookup"><span data-stu-id="ea3cf-326">`ExecuteNow` flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="ea3cf-327">StartTime</span><span class="sxs-lookup"><span data-stu-id="ea3cf-327">StartTime</span></span>     |    <span data-ttu-id="ea3cf-328">Čas UTC, kdy bude spuštění sestavy začínat v tomto formátu: RRRR-MM-ddTHH: mm: ssZ</span><span class="sxs-lookup"><span data-stu-id="ea3cf-328">UTC Time the report execution will begin in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="ea3cf-329">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="ea3cf-329">ReportStatus</span></span>     |    <span data-ttu-id="ea3cf-330">Stav provádění sestavy</span><span class="sxs-lookup"><span data-stu-id="ea3cf-330">Status of the report execution.</span></span> <span data-ttu-id="ea3cf-331">Možné hodnoty jsou `Paused` , `Active` a. `Inactive`</span><span class="sxs-lookup"><span data-stu-id="ea3cf-331">The possible values are `Paused`, `Active`, and `Inactive`</span></span>     |
|    <span data-ttu-id="ea3cf-332">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="ea3cf-332">RecurrenceInterval</span></span>     |    <span data-ttu-id="ea3cf-333">Interval opakování zadaný při vytváření sestavy</span><span class="sxs-lookup"><span data-stu-id="ea3cf-333">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="ea3cf-334">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="ea3cf-334">RecurrenceCount</span></span>     |    <span data-ttu-id="ea3cf-335">Počet opakování poskytnutý během vytváření sestavy</span><span class="sxs-lookup"><span data-stu-id="ea3cf-335">Recurrence count provided during report creation.</span></span>      |
|    <span data-ttu-id="ea3cf-336">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="ea3cf-336">CallbackUrl</span></span>     |    <span data-ttu-id="ea3cf-337">Adresa URL zpětného volání poskytnutá v žádosti</span><span class="sxs-lookup"><span data-stu-id="ea3cf-337">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="ea3cf-338">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="ea3cf-338">CallbackMethod</span></span>     |    <span data-ttu-id="ea3cf-339">Metoda zpětného volání poskytnutá v žádosti</span><span class="sxs-lookup"><span data-stu-id="ea3cf-339">Callback method provided in the request</span></span>     |
|    <span data-ttu-id="ea3cf-340">Formát</span><span class="sxs-lookup"><span data-stu-id="ea3cf-340">Format</span></span>     |    <span data-ttu-id="ea3cf-341">Formát souborů sestav</span><span class="sxs-lookup"><span data-stu-id="ea3cf-341">Format of the report files.</span></span> <span data-ttu-id="ea3cf-342">Možné hodnoty jsou `CSV` nebo `TSV` .</span><span class="sxs-lookup"><span data-stu-id="ea3cf-342">The possible values are `CSV` or `TSV`.</span></span>     |
|    <span data-ttu-id="ea3cf-343">TotalCount</span><span class="sxs-lookup"><span data-stu-id="ea3cf-343">TotalCount</span></span>     |    <span data-ttu-id="ea3cf-344">Počet záznamů v poli hodnot</span><span class="sxs-lookup"><span data-stu-id="ea3cf-344">Number of records in the Value array</span></span>     |
|    <span data-ttu-id="ea3cf-345">StatusCode</span><span class="sxs-lookup"><span data-stu-id="ea3cf-345">StatusCode</span></span>     |    <span data-ttu-id="ea3cf-346">Kód výsledku</span><span class="sxs-lookup"><span data-stu-id="ea3cf-346">Result Code</span></span>     |
|    <span data-ttu-id="ea3cf-347">zpráva</span><span class="sxs-lookup"><span data-stu-id="ea3cf-347">message</span></span>     |    <span data-ttu-id="ea3cf-348">Možné hodnoty jsou 200, 400, 401, 403, 500.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-348">The possible values are 200, 400, 401, 403, 500.</span></span> <span data-ttu-id="ea3cf-349">Stavová zpráva od spuštění rozhraní API</span><span class="sxs-lookup"><span data-stu-id="ea3cf-349">Status message from the execution of the API</span></span>     |
|        |        |

## <a name="get-report-execution-api"></a><span data-ttu-id="ea3cf-350">Získat rozhraní API pro spuštění sestavy</span><span class="sxs-lookup"><span data-stu-id="ea3cf-350">Get report execution API</span></span>

<span data-ttu-id="ea3cf-351">Tuto metodu můžete použít k dotazování na stav spuštění sestavy pomocí ReportId přijatých z [rozhraní API pro vytvoření sestavy](#create-report-api).</span><span class="sxs-lookup"><span data-stu-id="ea3cf-351">You can use this method to query the status of a report execution using the ReportId received from [Create Report API](#create-report-api).</span></span> <span data-ttu-id="ea3cf-352">Metoda vrátí odkaz pro stažení sestavy, pokud je sestava připravena ke stažení.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-352">The method returns the report download link if the report is ready for download.</span></span> <span data-ttu-id="ea3cf-353">V opačném případě metoda vrátí stav.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-353">Otherwise, the method returns the status.</span></span> <span data-ttu-id="ea3cf-354">Toto rozhraní API můžete použít také k získání všech spuštění, ke kterým došlo pro danou sestavu.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-354">You can also use this API to get all the executions that have happened for a given report.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="ea3cf-355">Toto rozhraní API má výchozí parametry dotazu nastavené pro `executionStatus=Completed` a `getLatestExecution=true` .</span><span class="sxs-lookup"><span data-stu-id="ea3cf-355">This API has default query parameters set for `executionStatus=Completed` and `getLatestExecution=true`.</span></span> <span data-ttu-id="ea3cf-356">Proto volání rozhraní API před prvním úspěšným spuštěním sestavy vrátí 404.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-356">Hence, calling the API before the first successful execution of the report will return 404.</span></span> <span data-ttu-id="ea3cf-357">Nedokončené spouštění lze získat nastavením `executionStatus=Pending` .</span><span class="sxs-lookup"><span data-stu-id="ea3cf-357">Pending executions can be obtained by setting `executionStatus=Pending`.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="ea3cf-358">Syntaxe žádosti</span><span class="sxs-lookup"><span data-stu-id="ea3cf-358">Request syntax</span></span>

|    <span data-ttu-id="ea3cf-359">Metoda</span><span class="sxs-lookup"><span data-stu-id="ea3cf-359">Method</span></span>     |    <span data-ttu-id="ea3cf-360">Identifikátor URI žádosti</span><span class="sxs-lookup"><span data-stu-id="ea3cf-360">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="ea3cf-361">GET</span><span class="sxs-lookup"><span data-stu-id="ea3cf-361">GET</span></span>    |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/{reportId}?executionId={executionId}&executionStatus={executionStatus}&getLatestExecution={getLatestExecution}`  |

### <a name="request-header"></a><span data-ttu-id="ea3cf-362">Hlavička požadavku</span><span class="sxs-lookup"><span data-stu-id="ea3cf-362">Request header</span></span>

|    <span data-ttu-id="ea3cf-363">Hlavička</span><span class="sxs-lookup"><span data-stu-id="ea3cf-363">Header</span></span>     |    <span data-ttu-id="ea3cf-364">Typ</span><span class="sxs-lookup"><span data-stu-id="ea3cf-364">Type</span></span>     |    <span data-ttu-id="ea3cf-365">Description</span><span class="sxs-lookup"><span data-stu-id="ea3cf-365">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="ea3cf-366">Autorizace</span><span class="sxs-lookup"><span data-stu-id="ea3cf-366">Authorization</span></span>     |    <span data-ttu-id="ea3cf-367">řetězec</span><span class="sxs-lookup"><span data-stu-id="ea3cf-367">string</span></span> |<span data-ttu-id="ea3cf-368">Povinná hodnota.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-368">Required.</span></span> <span data-ttu-id="ea3cf-369">přístupový token Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="ea3cf-369">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="ea3cf-370">Formát je  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="ea3cf-370">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="ea3cf-371">Typ obsahu</span><span class="sxs-lookup"><span data-stu-id="ea3cf-371">Content-Type</span></span>     |<span data-ttu-id="ea3cf-372">řetězec</span><span class="sxs-lookup"><span data-stu-id="ea3cf-372">string</span></span> |`Application/JSON` |

### <a name="path-parameter"></a><span data-ttu-id="ea3cf-373">Parametr cesty</span><span class="sxs-lookup"><span data-stu-id="ea3cf-373">Path parameter</span></span>

|    <span data-ttu-id="ea3cf-374">Název parametru</span><span class="sxs-lookup"><span data-stu-id="ea3cf-374">Parameter Name</span></span>    |    <span data-ttu-id="ea3cf-375">Požaduje se</span><span class="sxs-lookup"><span data-stu-id="ea3cf-375">Required</span></span>    |    <span data-ttu-id="ea3cf-376">Typ</span><span class="sxs-lookup"><span data-stu-id="ea3cf-376">Type</span></span>    |    <span data-ttu-id="ea3cf-377">Description</span><span class="sxs-lookup"><span data-stu-id="ea3cf-377">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="ea3cf-378">reportId</span><span class="sxs-lookup"><span data-stu-id="ea3cf-378">reportId</span></span>    |    <span data-ttu-id="ea3cf-379">Yes</span><span class="sxs-lookup"><span data-stu-id="ea3cf-379">Yes</span></span>    |    <span data-ttu-id="ea3cf-380">řetězec</span><span class="sxs-lookup"><span data-stu-id="ea3cf-380">string</span></span>    |    <span data-ttu-id="ea3cf-381">Filtr pro získání podrobností o spuštění pouze sestav s reportId, které jsou uvedeny v tomto argumentu.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-381">Filter to get execution details of only reports with the reportId given in this argument.</span></span> <span data-ttu-id="ea3cf-382">Více reportIds je možné zadat tak, že je oddělíte středníkem ";".</span><span class="sxs-lookup"><span data-stu-id="ea3cf-382">Multiple reportIds can be specified by separating them with a semicolon ";".</span></span>    |
|        |        |        |        |

### <a name="query-parameter"></a><span data-ttu-id="ea3cf-383">Parametr dotazu</span><span class="sxs-lookup"><span data-stu-id="ea3cf-383">Query parameter</span></span>

|    <span data-ttu-id="ea3cf-384">Název parametru</span><span class="sxs-lookup"><span data-stu-id="ea3cf-384">Parameter Name</span></span>    |    <span data-ttu-id="ea3cf-385">Požaduje se</span><span class="sxs-lookup"><span data-stu-id="ea3cf-385">Required</span></span>    |    <span data-ttu-id="ea3cf-386">Typ</span><span class="sxs-lookup"><span data-stu-id="ea3cf-386">Type</span></span>    |    <span data-ttu-id="ea3cf-387">Description</span><span class="sxs-lookup"><span data-stu-id="ea3cf-387">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="ea3cf-388">executionId</span><span class="sxs-lookup"><span data-stu-id="ea3cf-388">executionId</span></span>    |    <span data-ttu-id="ea3cf-389">No</span><span class="sxs-lookup"><span data-stu-id="ea3cf-389">No</span></span>    |    <span data-ttu-id="ea3cf-390">řetězec</span><span class="sxs-lookup"><span data-stu-id="ea3cf-390">string</span></span>    |    <span data-ttu-id="ea3cf-391">Filtr pro získání podrobností o pouze sestavách s executionId, které jsou uvedeny v tomto argumentu.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-391">Filter to get details of only reports with the executionId given in this argument.</span></span> <span data-ttu-id="ea3cf-392">Více executionIds je možné zadat tak, že je oddělíte středníkem ";".</span><span class="sxs-lookup"><span data-stu-id="ea3cf-392">Multiple executionIds can be specified by separating them with a semicolon ";".</span></span>    |
|    <span data-ttu-id="ea3cf-393">executionStatus</span><span class="sxs-lookup"><span data-stu-id="ea3cf-393">executionStatus</span></span>    |    <span data-ttu-id="ea3cf-394">No</span><span class="sxs-lookup"><span data-stu-id="ea3cf-394">No</span></span>    |    <span data-ttu-id="ea3cf-395">Řetězec/výčet</span><span class="sxs-lookup"><span data-stu-id="ea3cf-395">String/enum</span></span>    |    <span data-ttu-id="ea3cf-396">Filtr pro získání podrobností o pouze sestavách s executionStatus, které jsou uvedeny v tomto argumentu.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-396">Filter to get details of only reports with the executionStatus given in this argument.</span></span> <br> <span data-ttu-id="ea3cf-397">Platné hodnoty jsou: `Pending` , `Running` `Paused` a `Completed` .</span><span class="sxs-lookup"><span data-stu-id="ea3cf-397">Valid values are: `Pending`, `Running`, `Paused` and `Completed`.</span></span> <br> <span data-ttu-id="ea3cf-398">Výchozí hodnota je `Completed`.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-398">The default value is `Completed`.</span></span> <br> <span data-ttu-id="ea3cf-399">Více stavů je možné zadat tak, že je oddělíte středníkem (;).</span><span class="sxs-lookup"><span data-stu-id="ea3cf-399">Multiple statuses can be specified by separating them with a semicolon ";".</span></span>    |
|    <span data-ttu-id="ea3cf-400">getLatestExecution</span><span class="sxs-lookup"><span data-stu-id="ea3cf-400">getLatestExecution</span></span>    |    <span data-ttu-id="ea3cf-401">No</span><span class="sxs-lookup"><span data-stu-id="ea3cf-401">No</span></span>    |    <span data-ttu-id="ea3cf-402">boolean</span><span class="sxs-lookup"><span data-stu-id="ea3cf-402">boolean</span></span>    |    <span data-ttu-id="ea3cf-403">Rozhraní API vrátí podrobnosti o posledním spuštění.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-403">The API will return details of the latest execution.</span></span> <span data-ttu-id="ea3cf-404">Ve výchozím nastavení je tento parametr nastavený na hodnotu true.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-404">By default, this parameter is set to true.</span></span><br> <span data-ttu-id="ea3cf-405">Pokud se rozhodnete předat hodnotu tohoto parametru jako false, vrátí rozhraní API instance provádění za posledních 90 dnů.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-405">If you choose to pass the value of this parameter as false, then the API will return the last 90 days execution instances.</span></span>    |
|        |        |        |        |

### <a name="sample-request-payload"></a><span data-ttu-id="ea3cf-406">Ukázková datová část požadavku</span><span class="sxs-lookup"><span data-stu-id="ea3cf-406">Sample Request Payload</span></span>

<span data-ttu-id="ea3cf-407">Žádná</span><span class="sxs-lookup"><span data-stu-id="ea3cf-407">None</span></span>

### <a name="sample-response"></a><span data-ttu-id="ea3cf-408">Ukázková odpověď</span><span class="sxs-lookup"><span data-stu-id="ea3cf-408">Sample Response</span></span>

<span data-ttu-id="ea3cf-409">Datová část odpovědi je strukturovaná takto:</span><span class="sxs-lookup"><span data-stu-id="ea3cf-409">The response payload is structured as follows:</span></span>

<span data-ttu-id="ea3cf-410">Kódy odpovědí: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="ea3cf-410">Response Codes: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="ea3cf-411">Příklad datové části odpovědi:</span><span class="sxs-lookup"><span data-stu-id="ea3cf-411">Response payload example:</span></span>

```json
{
  "value": [
    {
      "executionId": "906931dc-4f2f-4195-bbb2-d7295c7550d3",
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf",
      "recurrenceInterval": 24,
      "recurrenceCount": 100,
      "callbackUrl": null,
      "callbackMethod": null,
      "format": "csv",
      "executionStatus": "Completed",
      "reportLocation": null,
      "reportAccessSecureLink": "https://<path to report for download>",
      "reportExpiryTime": null,
      "reportGeneratedTime": "2021-03-31T18:41:00Z"
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

<span data-ttu-id="ea3cf-412">Po dokončení spuštění sestavy se zobrazí `Completed` stav spuštění.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-412">Once report execution is complete, the execution status `Completed` is shown.</span></span> <span data-ttu-id="ea3cf-413">Sestavu si můžete stáhnout výběrem adresy URL v `reportAccessSecureLink` .</span><span class="sxs-lookup"><span data-stu-id="ea3cf-413">You can download the report by selecting the URL in the `reportAccessSecureLink`.</span></span>

### <a name="glossary"></a><span data-ttu-id="ea3cf-414">Glosář</span><span class="sxs-lookup"><span data-stu-id="ea3cf-414">Glossary</span></span>

<span data-ttu-id="ea3cf-415">Klíčové definice prvků v odpovědi.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-415">Key definitions of elements in the response.</span></span>

|    <span data-ttu-id="ea3cf-416">Parametr</span><span class="sxs-lookup"><span data-stu-id="ea3cf-416">Parameter</span></span>    |    <span data-ttu-id="ea3cf-417">Popis</span><span class="sxs-lookup"><span data-stu-id="ea3cf-417">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="ea3cf-418">ID spuštění</span><span class="sxs-lookup"><span data-stu-id="ea3cf-418">ExecutionId</span></span>    |    <span data-ttu-id="ea3cf-419">Univerzálně jedinečný identifikátor (UUID) instance provádění</span><span class="sxs-lookup"><span data-stu-id="ea3cf-419">Universally unique identifier (UUID) of the execution instance</span></span>    |
|    <span data-ttu-id="ea3cf-420">ID sestavy</span><span class="sxs-lookup"><span data-stu-id="ea3cf-420">ReportId</span></span>    |    <span data-ttu-id="ea3cf-421">ID sestavy přidružené k instanci spuštění</span><span class="sxs-lookup"><span data-stu-id="ea3cf-421">Report ID associated with the execution instance</span></span>    |
|    <span data-ttu-id="ea3cf-422">OpakováníInterval</span><span class="sxs-lookup"><span data-stu-id="ea3cf-422">RecurrenceInterval</span></span>    |    <span data-ttu-id="ea3cf-423">Interval opakování poskytovaný během vytváření sestavy</span><span class="sxs-lookup"><span data-stu-id="ea3cf-423">Recurrence interval provided during report creation</span></span>    |
|    <span data-ttu-id="ea3cf-424">Počet opakování</span><span class="sxs-lookup"><span data-stu-id="ea3cf-424">RecurrenceCount</span></span>    |    <span data-ttu-id="ea3cf-425">Počet opakování při vytváření sestavy</span><span class="sxs-lookup"><span data-stu-id="ea3cf-425">Recurrence count provided during report creation</span></span>    |
|    <span data-ttu-id="ea3cf-426">CallbackUrl (Url zpětného volání)</span><span class="sxs-lookup"><span data-stu-id="ea3cf-426">CallbackUrl</span></span>    |    <span data-ttu-id="ea3cf-427">Adresa URL zpětného volání přidružená k instanci provádění</span><span class="sxs-lookup"><span data-stu-id="ea3cf-427">Callback URL associated with the execution instance</span></span>    |
|    <span data-ttu-id="ea3cf-428">Metoda zpětného volání</span><span class="sxs-lookup"><span data-stu-id="ea3cf-428">CallbackMethod</span></span>    |    <span data-ttu-id="ea3cf-429">Metoda zpětného volání přidružená k instanci provádění</span><span class="sxs-lookup"><span data-stu-id="ea3cf-429">Callback method associated with the execution instance</span></span>    |
|    <span data-ttu-id="ea3cf-430">Formát</span><span class="sxs-lookup"><span data-stu-id="ea3cf-430">Format</span></span>    |    <span data-ttu-id="ea3cf-431">Formát generovaného souboru na konci provádění</span><span class="sxs-lookup"><span data-stu-id="ea3cf-431">Format of the generated file at the end of execution</span></span>    |
|    <span data-ttu-id="ea3cf-432">Stav spuštění</span><span class="sxs-lookup"><span data-stu-id="ea3cf-432">ExecutionStatus</span></span>    |    <span data-ttu-id="ea3cf-433">Stav instance spuštění sestavy</span><span class="sxs-lookup"><span data-stu-id="ea3cf-433">Status of the report execution instance.</span></span> <br> <span data-ttu-id="ea3cf-434">Platné hodnoty: `Pending` , `Running` , `Paused` a `Completed`</span><span class="sxs-lookup"><span data-stu-id="ea3cf-434">Valid values are: `Pending`, `Running`, `Paused`, and `Completed`</span></span>    |
|    <span data-ttu-id="ea3cf-435">ReportAccessSecureLink</span><span class="sxs-lookup"><span data-stu-id="ea3cf-435">ReportAccessSecureLink</span></span>    |<span data-ttu-id="ea3cf-436">Odkaz, přes který můžete bezpečně přistupovat k sestavě</span><span class="sxs-lookup"><span data-stu-id="ea3cf-436">Link through which the report can be accessed securely</span></span>        |
|    <span data-ttu-id="ea3cf-437">ReportExpiryTime</span><span class="sxs-lookup"><span data-stu-id="ea3cf-437">ReportExpiryTime</span></span>    |    <span data-ttu-id="ea3cf-438">Čas UTC, po jehož uplynutí vyprší platnost odkazu na sestavu v tomto formátu: rrrr-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="ea3cf-438">UTC Time after which the report link will expire in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>    |
|    <span data-ttu-id="ea3cf-439">ReportGeneratedTime</span><span class="sxs-lookup"><span data-stu-id="ea3cf-439">ReportGeneratedTime</span></span>    |    <span data-ttu-id="ea3cf-440">Čas UTC, ve kterém byla sestava vygenerována v tomto formátu: rrrr-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="ea3cf-440">UTC Time at which the report was generated in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>    |
|    <span data-ttu-id="ea3cf-441">TotalCount</span><span class="sxs-lookup"><span data-stu-id="ea3cf-441">TotalCount</span></span>    |    <span data-ttu-id="ea3cf-442">Počet datových sad v poli Hodnota</span><span class="sxs-lookup"><span data-stu-id="ea3cf-442">Number of datasets in the Value array</span></span>    |
|    <span data-ttu-id="ea3cf-443">Statuscode</span><span class="sxs-lookup"><span data-stu-id="ea3cf-443">StatusCode</span></span>    |    <span data-ttu-id="ea3cf-444">Kód výsledku</span><span class="sxs-lookup"><span data-stu-id="ea3cf-444">Result Code</span></span> <br> <span data-ttu-id="ea3cf-445">Možné hodnoty jsou 200, 400, 401, 403, 404 a 500.</span><span class="sxs-lookup"><span data-stu-id="ea3cf-445">The possible values are 200, 400, 401, 403, 404 and 500</span></span>    |
|    <span data-ttu-id="ea3cf-446">zpráva</span><span class="sxs-lookup"><span data-stu-id="ea3cf-446">message</span></span>    |    <span data-ttu-id="ea3cf-447">Stavová zpráva z spuštění rozhraní API</span><span class="sxs-lookup"><span data-stu-id="ea3cf-447">Status message from the execution of the API</span></span>    |
|        |        |

## <a name="next-steps"></a><span data-ttu-id="ea3cf-448">Další kroky</span><span class="sxs-lookup"><span data-stu-id="ea3cf-448">Next steps</span></span>

- <span data-ttu-id="ea3cf-449">Vyzkoušejte si rozhraní API prostřednictvím adresy URL rozhraní [API Swaggeru.](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span><span class="sxs-lookup"><span data-stu-id="ea3cf-449">Try out the APIs through the [swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span></span>
- [<span data-ttu-id="ea3cf-450">První volání rozhraní API</span><span class="sxs-lookup"><span data-stu-id="ea3cf-450">Make your first API call</span></span>](insights-programmatic-first-api-call.md)