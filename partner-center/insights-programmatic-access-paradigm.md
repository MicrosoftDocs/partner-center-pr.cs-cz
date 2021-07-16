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
# <a name="programmatic-access-paradigm"></a>Programové přístupové paradigma

Tento diagram znázorňuje vzor volání rozhraní API, který se používá k vytvoření nové šablony sestavy, naplánování vlastní sestavy a načtení dat o chybách.

:::image type="content" source="images/insights/prog-acc-paradigm.png" alt-text="Tok vysoké úrovně":::
***Obrázek 1: tok vysoké úrovně vzoru volání rozhraní API***

V tomto seznamu najdete další podrobnosti o obrázku 1.

1. Klientská aplikace může definovat vlastní schéma a šablonu sestavy voláním [rozhraní API pro vytvoření dotazu na sestavu](#create-report-query-api). Alternativně můžete vybrat šablonu sestavy (QueryId) ze zde uvedených ukázek knihovny šablon sestav [.](insights-programmatic-system-queries.md)
2. Po úspěšném dokončení vrátí rozhraní API pro dotazování pro vytváření sestav QueryId.
3. Klientská aplikace pak musí volat [rozhraní API pro vytváření sestav](#create-report-api) pomocí QueryId spolu s počátečním datem sestavy, opakovat interval, opakování a nepovinný identifikátor URI zpětného volání.
4. Po úspěšném dokončení vrátí [rozhraní API pro vytváření sestav](#create-report-api) ReportId.
5. Klientská aplikace se pošle oznámení na adresu URL zpětného volání, jakmile budou data sestavy připravena ke stažení.
6. Klientská aplikace potom používá [rozhraní API pro spuštění sestav](#get-report-execution-api) k dotazování na stav sestavy s ID sestavy a rozsahem dat.
7. Po úspěšném dokončení se odkaz na stažení sestavy vrátí a aplikace může zahájit stahování dat.

## <a name="report-query-language-specification"></a>Specifikace jazyka dotazu sestavy

I když poskytujeme [systémové dotazy](insights-programmatic-system-queries.md) , které můžete použít k vytváření sestav, můžete také vytvářet vlastní dotazy založené na vašich obchodních potřebách. Další informace o vlastních dotazech najdete v tématu [vlastní specifikace dotazu](insights-programmatic-custom-query.md).

## <a name="create-report-query-api"></a>Vytvoření rozhraní API pro dotazování sestav

Rozhraní API pomáhá vytvářet vlastní dotazy definující datovou sadu, ze které je nutné exportovat sloupce a metriky. Rozhraní API poskytuje flexibilitu pro vytvoření nové šablony vytváření sestav na základě vašich obchodních potřeb.  

Můžete také použít [systémové dotazy](insights-programmatic-system-queries.md) , které poskytujeme. Pokud nepotřebujete vlastní šablony sestav, můžete zavolat [rozhraní API pro vytváření sestav](#create-report-api) přímo pomocí QueryIds systémových dotazů, které jsou k dispozici.  

Následující příklad ukazuje, jak vytvořit vlastní dotaz pro získání prvních 10 zákazníků podle výnosů za poslední měsíc.

### <a name="request-syntax"></a>Syntaxe žádosti

|    Metoda     |    Identifikátor URI žádosti     |
|----- | -----|
|    POST     |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries`|
|||

### <a name="request-header"></a>Hlavička požadavku

|    Hlavička     |    Typ     |    Description     |
|-------|-----|------|
|    Autorizace     |    řetězec |Povinná hodnota. přístupový token Azure Active Directory (Azure AD). Formát je  `Bearer <token>` .|
|    Typ obsahu     |řetězec |`Application/JSON` |
||||

### <a name="path-parameter"></a>Parametr cesty

Žádná

### <a name="query-parameter"></a>Parametr dotazu

Žádná

### <a name="sample-request-payload"></a>Ukázková datová část požadavku

```json
{ 
  "Name": "CustomersRevenueQuery", 
  "Description": "Query to get top 10 customers by revenue for last month", 
  "Query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH" 
}
```

### <a name="glossary"></a>Glosář

Tato tabulka poskytuje klíčové definice prvků v datové části požadavku.

|Parametr|    Povinné     |    Popis     |    Povolené hodnoty     |
|-----|    -----    |    -----    |    -----    |
|Name |    Yes     |    Popisný název dotazu     |    řetězec     |
|    Popis     |    No     |    Popis toho, co dotaz vrátí     |    řetězec     |
|    Dotaz     |    Yes     |    Řetězec dotazu sestavy     |    Datový typ: řetězec <br> [Vlastní dotaz](insights-programmatic-custom-query.md) založený na obchodních potřebách |
|        |        |        |        |

> [!Note]
> Vlastní Ukázky dotazů najdete v tématu [Příklady ukázkových dotazů.](insights-programmatic-sample-queries.md)

### <a name="sample-response"></a>Ukázková odpověď

Datová část odpovědi je strukturována takto:

Kódy odpovědí: 200, 400, 401, 403, 500

Příklad datové části odpovědi:

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

### <a name="glossary"></a>Glosář

Tato tabulka poskytuje klíčové definice prvků v datové části požadavku.

|    Parametr     |    Popis     |
|    ----    |    ----    |
|    QueryId     |    Univerzálně jedinečný identifikátor (UUID) dotazu, který jste vytvořili     |
|    Name     |    Popisný název zadaný pro dotaz v datové části požadavku     |
|    Description     |    Popis zadaný při vytváření dotazu     |
|    Dotaz     |    Dotaz na sestavu předaný jako vstup během vytváření dotazu     |
|    Typ     |    Nastavit na `userDefined`     |
|    Uživatel     |    ID uživatele, které se použilo k vytvoření dotazu     |
|    CreatedTime     |    Čas UTC, kdy byl dotaz vytvořen v tomto formátu: RRRR-MM-ddTHH: mm: ssZ     |
|    TotalCount     |    Počet datových sad v poli hodnot     |
|    StatusCode     |    Kód výsledku <br> Možné hodnoty jsou 200, 400, 401, 403, 500     |
|    zpráva     |    Stavová zpráva od spuštění rozhraní API     |
|        |        |

## <a name="create-report-api"></a>Vytvoření rozhraní API pro sestavy

Po úspěšném vytvoření vlastní šablony sestavy a přijetí QueryID jako součást odpovědi na [dotaz na vytvoření sestavy](#create-report-query-api) lze toto rozhraní API volat, aby bylo možné naplánovat spuštění dotazu v pravidelných intervalech. Můžete nastavit četnost a plán pro doručení sestavy.
Pro systémové dotazy, které poskytujeme, se dá rozhraní API pro vytváření sestav volat taky pomocí [QueryId](insights-programmatic-system-queries.md).

### <a name="callback-url"></a>Adresa URL zpětného volání

Rozhraní API pro vytvoření sestavy přijímá adresu URL zpětného volání. Tato adresa URL se bude volat, jakmile bude generování sestavy úspěšné. Adresa URL zpětného volání by měla být veřejně přístupná. Kromě adresy URL lze také zadat metodu zpětného volání. Metoda zpětného volání může být pouze GET nebo POST. Výchozí metoda, pokud se žádná hodnota předá, bude POST. ReportId, který dokončil generování, se vždy předá zpět během zpětného volání.

Zpětné volání POST: Pokud předaná adresa URL byla `https://www.contosso.com/callback` , bude volaná zpětná adresa URL . `https://www.contosso.com/callback/<reportID>` 

Zpětné volání GET: Pokud byla předaná adresa URL `https://www.contosso.com/callback` , bude volaná zpětná adresa URL `https://www.contosso.com/callback?reportId=<reportID>` 

### <a name="executenow-reports"></a>Sestavy ExecuteNow

Existuje zřízení pro generování sestavy bez plánování. Datová část rozhraní API pro vytvoření sestavy může přijmout parametr , který při volání rozhraní API zařadí sestavu do fronty, která `ExecuteNow` se má vygenerovat. Pokud `ExecuteNow` je nastavená hodnota true, pole `StartTime` , se ignorují, protože tyto sestavy nejsou `RecurrenceCount` `RecurrenceInterval` naplánované.

Pokud má hodnota true, je možné předat dvě další `ExecuteNow` pole a `QueryStartTime` `QueryEndTime` . Tato dvě pole `TIMESPAN` přepíší pole v dotazu. Tato pole se nevztahují na naplánované sestavy, protože data se budou průběžně generovat po pevné časové období, které se nemění.

### <a name="request-syntax"></a>Syntaxe požadavku

|    Metoda     |    Identifikátor URI žádosti     |
|----- | -----|
|    POST     |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport` |

### <a name="request-header"></a>Hlavička požadavku

|    Hlavička     |    Typ     |    Description     |
|-------|-----|------|
|    Autorizace     |    řetězec |Povinná hodnota. Přístupový Azure Active Directory služby Azure AD (Azure AD). Formát je  `Bearer <token>` .|
|    Typ obsahu     |řetězec |`Application/JSON` |

### <a name="path-parameter"></a>Parametr cesty

Žádná

### <a name="query-parameter"></a>Parametr dotazu

Žádná

### <a name="sample-request-payload"></a>Ukázková datová část požadavku

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

### <a name="glossary"></a>Glosář

Klíčové definice elementů v datové části požadavku jsou uvedené níže:

|    Parametr     |    Povinné     |    Popis     |    Povolené hodnoty     |
|    ----    |    ----    |    ----    |    ----    |
|    ReportName     |    Yes     |    Název, který se má k sestavě přiřadit     |    řetězec     |
|    Popis     |    No     |    Popis vytvořené sestavy     |    řetězec     |
|    ID dotazu     |    Yes     |    ID dotazu sestavy     |    řetězec     |
|    StartTime     |    Yes     |    Časové razítko UTC, ve kterém bude generování sestavy začínat. <br> Formát by měl být: rrrr-MM-ddTHH:mm:ssZ       |    řetězec     |
|    ExecuteNow     |    No     |    Tento parametr by se měl použít k vytvoření sestavy, která se spustí pouze jednou. `StartTime`A `RecurrenceInterval` `RecurrenceCount` se ignorují, pokud je nastavená hodnota true. Sestava se spustí okamžitě asynchronním způsobem.     |    true/false     |
|    Čas_spuštění_dotazu     |    No     |    Volitelně určuje čas spuštění dotazu extrahování dat. Tento parametr se vztahuje pouze na jednu sestavu spuštění, která má `ExecuteNow` nastavenou hodnotu true. Nastavení tohoto parametru `TIMESPAN` přepíše dané v dotazu. Formát by měl být rrrr-MM-ddTHH:mm:ssZ.     |    Časové razítko jako řetězec     |
|    QueryEndTime     |    No     |    Volitelně určuje koncový čas pro dotaz extrahující data. Tento parametr se vztahuje pouze na jednu sestavu spuštění, která má `ExecuteNow` nastavenou hodnotu true. Nastavení tohoto parametru `TIMESPAN` přepíše dané v dotazu. Formát by měl být rrrr-MM-ddTHH:mm:ssZ.     |    Časové razítko jako řetězec     |
|    OpakováníInterval     |    Yes     |    Frekvence v hodinách, kdy se má sestava generovat. <br> Minimální hodnota je 4 a maximální hodnota je 2 160.      |    integer     |
|    Počet opakování     |    No     |    Počet sestav, které se vygenerují     |    integer     |
|    Formát     |    No     |    Formát exportovaného souboru. <br> Výchozí hodnota je CSV.    |    "CSV"/"TSV"     |
|    CallbackUrl (Url zpětného volání)     |    No     |    Veřejně přístupná adresa URL, kterou je možné volitelně nakonfigurovat jako cíl zpětného volání     |    Řetězec (adresa URL protokolu HTTP)     |
|    Metoda zpětného volání     |    No     |    Metoda, která se má použít pro zpětné volání     |    GET/POST     |
|        |        |        |        |

### <a name="sample-response"></a>Ukázková odpověď

Datová část odpovědi je strukturována takto:

Kódy odpovědí: 200, 400, 401, 403, 404, 500

Příklad datové části odpovědi:

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

### <a name="glossary"></a>Glosář

Klíčové definice prvků v odpovědi jsou kloubově navýšené:

|    Parametr     |    Popis     |
|    ----    |    ----    |
|    ReportId     |    Univerzálně jedinečný identifikátor (UUID) sestavy, kterou jste vytvořili     |
|    ReportName     |    Název zadaný pro sestavu v datové části požadavku     |
|    Description     |    Popis zadaný při vytváření sestavy     |
|    QueryId     |    ID dotazu předané v době, kdy jste sestavu vytvořili     |
|    Dotaz     |    Text dotazu, který se spustí pro tuto sestavu     |
|    Uživatel     |    ID uživatele, které se použilo k vytvoření sestavy     |
|    CreatedTime     |    Čas UTC, kdy byla sestava vytvořena v tomto formátu: RRRR-MM-ddTHH: mm: ssZ     |
|    ModifiedTime     |    Čas UTC, kdy se sestava naposledy změnila v tomto formátu: RRRR-MM-ddTHH: mm: ssZ     |
|    ExecuteNow     |    `ExecuteNow` příznak nastavený v okamžiku vytvoření sestavy     |
|    StartTime     |    Čas UTC, kdy bude spuštění sestavy začínat v tomto formátu: RRRR-MM-ddTHH: mm: ssZ     |
|    ReportStatus     |    Stav provádění sestavy Možné hodnoty jsou `Paused` , `Active` a. `Inactive`     |
|    RecurrenceInterval     |    Interval opakování zadaný při vytváření sestavy     |
|    RecurrenceCount     |    Počet opakování poskytnutý během vytváření sestavy      |
|    CallbackUrl     |    Adresa URL zpětného volání poskytnutá v žádosti     |
|    CallbackMethod     |    Metoda zpětného volání poskytnutá v žádosti     |
|    Formát     |    Formát souborů sestav Možné hodnoty jsou `CSV` nebo `TSV` .     |
|    TotalCount     |    Počet záznamů v poli hodnot     |
|    StatusCode     |    Kód výsledku     |
|    zpráva     |    Možné hodnoty jsou 200, 400, 401, 403, 500. Stavová zpráva od spuštění rozhraní API     |
|        |        |

## <a name="get-report-execution-api"></a>Získat rozhraní API pro spuštění sestavy

Tuto metodu můžete použít k dotazování na stav spuštění sestavy pomocí ReportId přijatých z [rozhraní API pro vytvoření sestavy](#create-report-api). Metoda vrátí odkaz pro stažení sestavy, pokud je sestava připravena ke stažení. V opačném případě metoda vrátí stav. Toto rozhraní API můžete použít také k získání všech spuštění, ke kterým došlo pro danou sestavu.  

>[!IMPORTANT]
>Toto rozhraní API má výchozí parametry dotazu nastavené pro `executionStatus=Completed` a `getLatestExecution=true` . Proto volání rozhraní API před prvním úspěšným spuštěním sestavy vrátí 404. Nedokončené spouštění lze získat nastavením `executionStatus=Pending` .

### <a name="request-syntax"></a>Syntaxe žádosti

|    Metoda     |    Identifikátor URI žádosti     |
|----- | -----|
|    GET    |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/{reportId}?executionId={executionId}&executionStatus={executionStatus}&getLatestExecution={getLatestExecution}`  |

### <a name="request-header"></a>Hlavička požadavku

|    Hlavička     |    Typ     |    Description     |
|-------|-----|------|
|    Autorizace     |    řetězec |Povinná hodnota. přístupový token Azure Active Directory (Azure AD). Formát je  `Bearer <token>` .|
|    Typ obsahu     |řetězec |`Application/JSON` |

### <a name="path-parameter"></a>Parametr cesty

|    Název parametru    |    Požaduje se    |    Typ    |    Description    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId    |    Yes    |    řetězec    |    Filtr pro získání podrobností o spuštění pouze sestav s reportId, které jsou uvedeny v tomto argumentu. Více reportIds je možné zadat tak, že je oddělíte středníkem ";".    |
|        |        |        |        |

### <a name="query-parameter"></a>Parametr dotazu

|    Název parametru    |    Požaduje se    |    Typ    |    Description    |
|    ----    |    ----    |    ----    |    ----    |
|    executionId    |    No    |    řetězec    |    Filtr pro získání podrobností o pouze sestavách s executionId, které jsou uvedeny v tomto argumentu. Více executionIds je možné zadat tak, že je oddělíte středníkem ";".    |
|    executionStatus    |    No    |    Řetězec/výčet    |    Filtr pro získání podrobností o pouze sestavách s executionStatus, které jsou uvedeny v tomto argumentu. <br> Platné hodnoty jsou: `Pending` , `Running` `Paused` a `Completed` . <br> Výchozí hodnota je `Completed`. <br> Více stavů je možné zadat tak, že je oddělíte středníkem (;).    |
|    getLatestExecution    |    No    |    boolean    |    Rozhraní API vrátí podrobnosti o posledním spuštění. Ve výchozím nastavení je tento parametr nastavený na hodnotu true.<br> Pokud se rozhodnete předat hodnotu tohoto parametru jako false, vrátí rozhraní API instance provádění za posledních 90 dnů.    |
|        |        |        |        |

### <a name="sample-request-payload"></a>Ukázková datová část požadavku

Žádná

### <a name="sample-response"></a>Ukázková odpověď

Datová část odpovědi je strukturovaná takto:

Kódy odpovědí: 200, 400, 401, 403, 404, 500

Příklad datové části odpovědi:

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

Po dokončení spuštění sestavy se zobrazí `Completed` stav spuštění. Sestavu si můžete stáhnout výběrem adresy URL v `reportAccessSecureLink` .

### <a name="glossary"></a>Glosář

Klíčové definice prvků v odpovědi.

|    Parametr    |    Popis    |
|    ----    |    ----    |
|    ID spuštění    |    Univerzálně jedinečný identifikátor (UUID) instance provádění    |
|    ID sestavy    |    ID sestavy přidružené k instanci spuštění    |
|    OpakováníInterval    |    Interval opakování poskytovaný během vytváření sestavy    |
|    Počet opakování    |    Počet opakování při vytváření sestavy    |
|    CallbackUrl (Url zpětného volání)    |    Adresa URL zpětného volání přidružená k instanci provádění    |
|    Metoda zpětného volání    |    Metoda zpětného volání přidružená k instanci provádění    |
|    Formát    |    Formát generovaného souboru na konci provádění    |
|    Stav spuštění    |    Stav instance spuštění sestavy <br> Platné hodnoty: `Pending` , `Running` , `Paused` a `Completed`    |
|    ReportAccessSecureLink    |Odkaz, přes který můžete bezpečně přistupovat k sestavě        |
|    ReportExpiryTime    |    Čas UTC, po jehož uplynutí vyprší platnost odkazu na sestavu v tomto formátu: rrrr-MM-ddTHH:mm:ssZ    |
|    ReportGeneratedTime    |    Čas UTC, ve kterém byla sestava vygenerována v tomto formátu: rrrr-MM-ddTHH:mm:ssZ    |
|    TotalCount    |    Počet datových sad v poli Hodnota    |
|    Statuscode    |    Kód výsledku <br> Možné hodnoty jsou 200, 400, 401, 403, 404 a 500.    |
|    zpráva    |    Stavová zpráva z spuštění rozhraní API    |
|        |        |

## <a name="next-steps"></a>Další kroky

- Vyzkoušejte si rozhraní API prostřednictvím adresy URL rozhraní [API Swaggeru.](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)
- [První volání rozhraní API](insights-programmatic-first-api-call.md)