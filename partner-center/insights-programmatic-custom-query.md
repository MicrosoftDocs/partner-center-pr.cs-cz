---
title: Specifikace vlastních dotazů
description: Naučte se vytvářet vlastní dotazy pro extrahování dat z analytických tabulek.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 57f2109044e604dca21b0109b5be56f40170628e
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376445"
---
# <a name="custom-query-specification"></a><span data-ttu-id="51032-103">Specifikace vlastních dotazů</span><span class="sxs-lookup"><span data-stu-id="51032-103">Custom query specification</span></span>

<span data-ttu-id="51032-104">Partneři mohou tuto specifikaci dotazu použít ke snadnému formulování vlastních dotazů pro extrahování dat z analytických tabulek.</span><span class="sxs-lookup"><span data-stu-id="51032-104">Partners can use this query specification to easily formulate custom queries for extracting data from analytics tables.</span></span> <span data-ttu-id="51032-105">Dotazy lze použít k výběru pouze požadovaných sloupců a metrik, které odpovídají určitým kritériím.</span><span class="sxs-lookup"><span data-stu-id="51032-105">The queries can be used to select only the desired columns and metrics that match a certain criterion.</span></span> <span data-ttu-id="51032-106">V centru specifikace jazyka je definice datové sady, na kterou lze napsat vlastní dotaz.</span><span class="sxs-lookup"><span data-stu-id="51032-106">At the heart of the language specification is the dataset definition on which a custom query can be written.</span></span>

## <a name="datasets"></a><span data-ttu-id="51032-107">Datové sady</span><span class="sxs-lookup"><span data-stu-id="51032-107">Datasets</span></span>

<span data-ttu-id="51032-108">Stejně jako se některé dotazy spouštěly proti databázi, která obsahuje tabulky a sloupce, funguje vlastní dotaz na datové sady, které mají sloupce a metriky.</span><span class="sxs-lookup"><span data-stu-id="51032-108">In the same way that some queries are run against a database that has tables and columns, a custom query works on Datasets that have columns and metrics.</span></span> <span data-ttu-id="51032-109">Úplný seznam dostupných datových sad pro formulovat dotaz lze získat pomocí rozhraní API datových sad.</span><span class="sxs-lookup"><span data-stu-id="51032-109">The full list of available datasets for formulating a query can be obtained by using the datasets API.</span></span>

<span data-ttu-id="51032-110">Toto je příklad datové sady zobrazené jako JSON:</span><span class="sxs-lookup"><span data-stu-id="51032-110">This is an example of a dataset shown as a JSON:</span></span>

```json
{ 
      "datasetName": "OfficeUsage", 
      "selectableColumns": [ 
        "CustomerTenantId", 
        "CustomerTpid", 
        "WorkloadName", 
        "Month", 
        "PaidAvailableUnits", 
        "MonthlyActiveUsers", 
        "CustomerName", 
        "CustomerMarket", 
        "CustomerSegment",  
        "MPNId", 
        "PartnerName", 
        "PartnerLocation", 
        "PartnerAttributionType", 
        "IsDuplicateRowForPGA" 
      ], 
      "availableMetrics": [ 
        "CustomerCount", 
        "CustomerTenantCount", 
        "TotalPaidAvailableUnits", 
        "TotalMonthlyActiveUsers" 
      ], 
      "availableDateRanges": [ 
        "LAST_MONTH", 
        "LAST_3_MONTHS", 
        "LAST_6_MONTHS", 
        "LAST_1_YEAR", 
        "LIFETIME" 
      ], 
      "minimumRecurrenceInterval": 24 
    },
```

## <a name="parts-of-a-dataset"></a><span data-ttu-id="51032-111">Části datové sady</span><span class="sxs-lookup"><span data-stu-id="51032-111">Parts of a dataset</span></span>

- <span data-ttu-id="51032-112">Název datové sady je jako název databázové tabulky.</span><span class="sxs-lookup"><span data-stu-id="51032-112">A dataset name is like a database table name.</span></span> <span data-ttu-id="51032-113">Například OfficeUsage.</span><span class="sxs-lookup"><span data-stu-id="51032-113">For example, OfficeUsage.</span></span> <span data-ttu-id="51032-114">Datová sada obsahuje seznam sloupců, které je možné vybrat, například CustomerTenantId.</span><span class="sxs-lookup"><span data-stu-id="51032-114">A dataset has a list of columns that can be selected, such as CustomerTenantId.</span></span>
- <span data-ttu-id="51032-115">Datová sada má také metriky, které jsou v databázi jako agregační funkce.</span><span class="sxs-lookup"><span data-stu-id="51032-115">A dataset also has metrics, which are like aggregation functions in a database.</span></span> <span data-ttu-id="51032-116">Například TotalMonthlyActiveUsers.</span><span class="sxs-lookup"><span data-stu-id="51032-116">For example, TotalMonthlyActiveUsers.</span></span>
- <span data-ttu-id="51032-117">Existují pevná časová období, během kterých je možné data exportovat.</span><span class="sxs-lookup"><span data-stu-id="51032-117">There are fixed time spans over which data can be exported.</span></span>

## <a name="formulating-a-query-on-a-dataset"></a><span data-ttu-id="51032-118">Formulace dotazu na datovou sadu</span><span class="sxs-lookup"><span data-stu-id="51032-118">Formulating a query on a dataset</span></span>

<span data-ttu-id="51032-119">Toto jsou některé ukázkové dotazy, které ukazují, jak extrahovat různé typy dat.</span><span class="sxs-lookup"><span data-stu-id="51032-119">These are some sample queries that show how to extract various types of data.</span></span>

|<span data-ttu-id="51032-120">Dotaz</span><span class="sxs-lookup"><span data-stu-id="51032-120">Query</span></span>|    <span data-ttu-id="51032-121">Description</span><span class="sxs-lookup"><span data-stu-id="51032-121">Description</span></span>    |
|----|    ----    |
|<span data-ttu-id="51032-122">**SELECT (VYBRAT)** CustomerTenantId, PaidAvailableUnits **FROM**</span><span class="sxs-lookup"><span data-stu-id="51032-122">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span></span> <br><span data-ttu-id="51032-123">OfficeUsage **TIMESPAN** LAST_MONTH</span><span class="sxs-lookup"><span data-stu-id="51032-123">OfficeUsage **TIMESPAN** LAST_MONTH</span></span>|    <span data-ttu-id="51032-124">Tento dotaz za poslední 1 měsíc zobrazí všechny hodnoty CusotmerTenantID a příslušné jednotky PaidAvailableUnits.</span><span class="sxs-lookup"><span data-stu-id="51032-124">This query will get every CusotmerTenantID and its corresponding PaidAvailableUnits in the last 1 month.</span></span>    |
|<span data-ttu-id="51032-125">**SELECT (VYBRAT)** CustomerTenantId, PaidAvailableUnits **FROM**</span><span class="sxs-lookup"><span data-stu-id="51032-125">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span></span> <br><span data-ttu-id="51032-126">OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10</span><span class="sxs-lookup"><span data-stu-id="51032-126">OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10</span></span>|    <span data-ttu-id="51032-127">Tento dotaz zobrazí 10 tenantů s nejvyšším počtem placených dostupných jednotek v sestupného pořadí.</span><span class="sxs-lookup"><span data-stu-id="51032-127">This query will get the top 10 customer tenants in decreasing order of the number of paid available units.</span></span>     |
|<span data-ttu-id="51032-128">**SELECT (VYBRAT)** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS</span><span class="sxs-lookup"><span data-stu-id="51032-128">**SELECT** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS</span></span> |    <span data-ttu-id="51032-129">Tento dotaz zobrazí jednotky PaidAvailableUnits a MonthlyActiveUsers všech zákazníků, kteří mají monthlyActiveUsers větší než 100 000.</span><span class="sxs-lookup"><span data-stu-id="51032-129">This query will get the PaidAvailableUnits and MonthlyActiveUsers of all the Customers who have MonthlyActiveUsers greater than 100,000.</span></span>     |
|<span data-ttu-id="51032-130">**SELECT (VYBRAT)** CustomerTenantId, Month, MonthlyActiveUsers **FROM**</span><span class="sxs-lookup"><span data-stu-id="51032-130">**SELECT** CustomerTenantId, Month, MonthlyActiveUsers **FROM**</span></span> <br><span data-ttu-id="51032-131">OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002')</span><span class="sxs-lookup"><span data-stu-id="51032-131">OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002')</span></span> |    <span data-ttu-id="51032-132">Tento dotaz zobrazí hodnotu CustomerTenantId a měsíční aktivní uživatele pro každý měsíc podle dvou hodnot CustomerTpId: '2a31c234-1f4e-4c60-909e-76d234f93161 a 80780748-3f9a-11eb-b378-0242ac130002.</span><span class="sxs-lookup"><span data-stu-id="51032-132">This query will get the CustomerTenantId and the monthly active users for every month by the two CustomerTpId values: '2a31c234-1f4e-4c60-909e-76d234f93161' and '80780748-3f9a-11eb-b378-0242ac130002'.</span></span>     |
|        |        |

## <a name="query-specification"></a><span data-ttu-id="51032-133">Specifikace dotazu</span><span class="sxs-lookup"><span data-stu-id="51032-133">Query specification</span></span>

<span data-ttu-id="51032-134">Tato část popisuje definici a strukturu dotazu.</span><span class="sxs-lookup"><span data-stu-id="51032-134">This section describes the query definition and structure.</span></span>

## <a name="grammar-reference"></a><span data-ttu-id="51032-135">Referenční informace k gramatikě</span><span class="sxs-lookup"><span data-stu-id="51032-135">Grammar reference</span></span>

<span data-ttu-id="51032-136">Tato tabulka popisuje symboly používané v dotazech.</span><span class="sxs-lookup"><span data-stu-id="51032-136">This table describes the symbols used in queries.</span></span>

|    <span data-ttu-id="51032-137">Dotaz</span><span class="sxs-lookup"><span data-stu-id="51032-137">Query</span></span>    |    <span data-ttu-id="51032-138">Description</span><span class="sxs-lookup"><span data-stu-id="51032-138">Description</span></span>    |
|    ----    |    ----    |
|    `?`    |    <span data-ttu-id="51032-139">Volitelné</span><span class="sxs-lookup"><span data-stu-id="51032-139">Optional</span></span>    |
|    `*`    |    <span data-ttu-id="51032-140">Nula nebo více</span><span class="sxs-lookup"><span data-stu-id="51032-140">Zero or more</span></span>    |
|    `+`    |    <span data-ttu-id="51032-141">Jeden nebo více</span><span class="sxs-lookup"><span data-stu-id="51032-141">One or more</span></span>    |
|    `\|`    |    <span data-ttu-id="51032-142">Nebo / Jeden ze seznamů</span><span class="sxs-lookup"><span data-stu-id="51032-142">Or / One of the lists</span></span>    |
|        |        |

## <a name="query-definition"></a><span data-ttu-id="51032-143">Definice dotazu</span><span class="sxs-lookup"><span data-stu-id="51032-143">Query definition</span></span>

<span data-ttu-id="51032-144">Příkaz dotazu obsahuje následující klauzule: SelectClause, FromClause, WhereClause, OrderClause, LimitClause a TimeSpan.</span><span class="sxs-lookup"><span data-stu-id="51032-144">The query statement has the following clauses: SelectClause, FromClause, WhereClause, OrderClause, LimitClause, and TimeSpan.</span></span>

- <span data-ttu-id="51032-145">**SelectClause**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`</span><span class="sxs-lookup"><span data-stu-id="51032-145">**SelectClause**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`</span></span>
    - <span data-ttu-id="51032-146">**ColumOrMetricName:** Sloupce a metriky definované v rámci datové sady</span><span class="sxs-lookup"><span data-stu-id="51032-146">**ColumOrMetricName**: Columns and Metrics defined within the Dataset</span></span>
- <span data-ttu-id="51032-147">**FromClause:**`FROM DatasetName`</span><span class="sxs-lookup"><span data-stu-id="51032-147">**FromClause**: `FROM DatasetName`</span></span>
    - <span data-ttu-id="51032-148">**DatasetName:** Název datové sady definovaný v datové sadě</span><span class="sxs-lookup"><span data-stu-id="51032-148">**DatasetName**: Dataset name defined within the Dataset</span></span>
- <span data-ttu-id="51032-149">**WhereClause**: `WHERE FilterCondition (AND FilterCondition)`</span><span class="sxs-lookup"><span data-stu-id="51032-149">**WhereClause**: `WHERE FilterCondition (AND FilterCondition)`</span></span>
    - <span data-ttu-id="51032-150">**FilterCondition:** ColumOrMetricName – hodnota operátoru</span><span class="sxs-lookup"><span data-stu-id="51032-150">**FilterCondition**: ColumOrMetricName Operator Value</span></span>
        - <span data-ttu-id="51032-151">**Operátor**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`</span><span class="sxs-lookup"><span data-stu-id="51032-151">**Operator**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`</span></span>
        - <span data-ttu-id="51032-152">**Value**: Number | StringLiteral – | MultiNumberList – | Seznam víceřetězcových řetězců</span><span class="sxs-lookup"><span data-stu-id="51032-152">**Value**: Number | StringLiteral | MultiNumberList | MultiStringList</span></span>
            - <span data-ttu-id="51032-153">**Číslo:**`-? [0-9]+ (. [0-9] [0-9]*)?`</span><span class="sxs-lookup"><span data-stu-id="51032-153">**Number**: `-? [0-9]+ (. [0-9] [0-9]*)?`</span></span>
            - <span data-ttu-id="51032-154">**StringLiteral**:  `' [a-zA-Z0-9_]*'`</span><span class="sxs-lookup"><span data-stu-id="51032-154">**StringLiteral**:  `' [a-zA-Z0-9_]*'`</span></span>
            - <span data-ttu-id="51032-155">**MultiNumberList:**`(Number (,Number)*)`</span><span class="sxs-lookup"><span data-stu-id="51032-155">**MultiNumberList**: `(Number (,Number)*)`</span></span>
            - <span data-ttu-id="51032-156">**MultiStringList:**`(StringLiteral (,StringLiteral)*)`</span><span class="sxs-lookup"><span data-stu-id="51032-156">**MultiStringList**: `(StringLiteral (,StringLiteral)*)`</span></span>
- <span data-ttu-id="51032-157">**OrderClause:**`ORDER BY OrderCondition (,OrderCondition)`</span><span class="sxs-lookup"><span data-stu-id="51032-157">**OrderClause**: `ORDER BY OrderCondition (,OrderCondition)`</span></span>
    - <span data-ttu-id="51032-158">**OrderCondition**: `ColumOrMetricName (ASC | DESC)*`</span><span class="sxs-lookup"><span data-stu-id="51032-158">**OrderCondition**: `ColumOrMetricName (ASC | DESC)*`</span></span>
- <span data-ttu-id="51032-159">**LimitClause:**`LIMIT [0-9]+`</span><span class="sxs-lookup"><span data-stu-id="51032-159">**LimitClause**: `LIMIT [0-9]+`</span></span>
- <span data-ttu-id="51032-160">**TimeSpan**: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`</span><span class="sxs-lookup"><span data-stu-id="51032-160">**TimeSpan**: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`</span></span>

## <a name="query-structure"></a><span data-ttu-id="51032-161">Struktura dotazů</span><span class="sxs-lookup"><span data-stu-id="51032-161">Query Structure</span></span>

<span data-ttu-id="51032-162">Dotaz sestavy se sýtá z několika částí:</span><span class="sxs-lookup"><span data-stu-id="51032-162">A Report query is made up of multiple parts:</span></span>
- `SELECT`
- `FROM`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `TIMESPAN`

<span data-ttu-id="51032-163">Jednotlivé části jsou popsány níže.</span><span class="sxs-lookup"><span data-stu-id="51032-163">Each part is described below.</span></span>

### `SELECT`

<span data-ttu-id="51032-164">Tato část dotazu určuje sloupce, které se mají exportovat.</span><span class="sxs-lookup"><span data-stu-id="51032-164">This part of the query specifies the columns that will get exported.</span></span> <span data-ttu-id="51032-165">Sloupce, které je možné vybrat, jsou pole uvedená v *oddílech selectableColumns* a *availableMetrics* datové sady.</span><span class="sxs-lookup"><span data-stu-id="51032-165">The columns that can be selected are the fields listed in *selectableColumns* and *availableMetrics* sections of a dataset.</span></span>

<span data-ttu-id="51032-166">Volitelně můžete `DISTINCT` zadat klíčové slovo za `SELECT` .</span><span class="sxs-lookup"><span data-stu-id="51032-166">Optionally, `DISTINCT` keyword can be specified after `SELECT`.</span></span> <span data-ttu-id="51032-167">Pokud `DISTINCT` je zadaný parametr , budou konečné exportované řádky vždy obsahovat odlišné hodnoty vybraných sloupců.</span><span class="sxs-lookup"><span data-stu-id="51032-167">If `DISTINCT` is specified, then the final exported rows will always contain distinct values of the selected columns.</span></span> <span data-ttu-id="51032-168">Metriky se budou počítat pro každou odlišnou kombinaci vybraných sloupců, takže klíčové slovo se nevyžaduje, pokud je sloupec metriky zahrnutý v `DISTINCT` seznamu vybraných sloupců.</span><span class="sxs-lookup"><span data-stu-id="51032-168">Metrics will be calculated for every distinct combination of the selected columns, hence `DISTINCT` keyword is not required when a metric column is included in the select column list.</span></span>

<span data-ttu-id="51032-169">**Příklad:**</span><span class="sxs-lookup"><span data-stu-id="51032-169">**Example:**</span></span>

```sql
SELECT CustomerTenantId, PaidAvailableUnits; 
SELECT DISTINCT CustomerTenantId
```

### `FROM`

<span data-ttu-id="51032-170">Tato část dotazu označuje datovou sadu, ze které se mají data exportovat.</span><span class="sxs-lookup"><span data-stu-id="51032-170">This part of the query indicates the dataset from which data needs to be exported.</span></span> <span data-ttu-id="51032-171">Název datové sady, který tady najdete, musí být platným názvem datové sady vrácený rozhraním API datových sad.</span><span class="sxs-lookup"><span data-stu-id="51032-171">The dataset name given here needs to be a valid dataset name returned by the datasets API.</span></span>

<span data-ttu-id="51032-172">**Příklad:**</span><span class="sxs-lookup"><span data-stu-id="51032-172">**Example:**</span></span>

- `FROM  OfficeUsage`
- `FROM  AzureUsage`

### `WHERE`

<span data-ttu-id="51032-173">Tato část dotazu slouží k určení podmínek filtru pro datovou sadu.</span><span class="sxs-lookup"><span data-stu-id="51032-173">This part of the query is used to specify filter conditions on the dataset.</span></span> <span data-ttu-id="51032-174">V posledním exportovaného souboru budou k dispozici pouze řádky, které odpovídají všem podmínkám uvedeným v této klauzuli.</span><span class="sxs-lookup"><span data-stu-id="51032-174">Only rows matching all the conditions listed in this clause will be present in the final exported file.</span></span> <span data-ttu-id="51032-175">Podmínka filtru může být u libovolného sloupce uvedeného ve *sloupcích selectableColumns* a *availableMetrics*.</span><span class="sxs-lookup"><span data-stu-id="51032-175">The filter condition can be on any of the columns listed in *selectableColumns* and *availableMetrics*.</span></span> <span data-ttu-id="51032-176">Hodnoty zadané v podměně filtru mohou být seznam čísel nebo seznam řetězců pouze v případě, že operátor je `IN` nebo `NOT IN` .</span><span class="sxs-lookup"><span data-stu-id="51032-176">The values specified in the filter condition can be a list of numbers or a list of strings only when the operator is `IN` or `NOT IN`.</span></span> <span data-ttu-id="51032-177">Hodnoty lze vždy zadat jako řetězec literálu a budou převedeny na nativní typy sloupců.</span><span class="sxs-lookup"><span data-stu-id="51032-177">The values can always be given as a literal string and they will be converted to the native types of columns.</span></span> <span data-ttu-id="51032-178">Více podmínek filtru musí být odděleno operací AND.</span><span class="sxs-lookup"><span data-stu-id="51032-178">Multiple filter conditions need to be separated with an AND operation.</span></span>

<span data-ttu-id="51032-179">**Příklad:**</span><span class="sxs-lookup"><span data-stu-id="51032-179">**Example:**</span></span>

- `CustomerTenantId= '868368da-957d-4959-8992-3c12dc7e6260'`
- `CustomerName LIKE '%Contoso%'`
- `CustomerId NOT IN (1000, 1001, 1002)`
- `OrderQuantity=100`
- `CustomerTenantId='7b487ac0-ce12-b732-dcd6-91a1e4e74a50' AND CustomerTpId=' 0f8b7fa0-eb83-a183-1225-ca153ef807aa'`

### `ORDER BY`

<span data-ttu-id="51032-180">Tato část dotazu určuje kritéria pořadí pro exportované řádky.</span><span class="sxs-lookup"><span data-stu-id="51032-180">This part of the query specifies the ordering criteria for the exported rows.</span></span> <span data-ttu-id="51032-181">Sloupce, ve kterých je možné definovat řazení, musí být ze *sloupců selectableColumns* a *availableMetrics* datové sady.</span><span class="sxs-lookup"><span data-stu-id="51032-181">The columns on which ordering can be defined need to be from the *selectableColumns* and *availableMetrics* of the dataset.</span></span> <span data-ttu-id="51032-182">Pokud není zadaný žádný směr řazení, bude ve sloupci ve výchozím nastavení DESC.</span><span class="sxs-lookup"><span data-stu-id="51032-182">If there is no ordering direction specified, it will be defaulted to DESC on the column.</span></span> <span data-ttu-id="51032-183">Řazení lze definovat na více sloupcích oddělením kritérií čárkou.</span><span class="sxs-lookup"><span data-stu-id="51032-183">Ordering can be defined on multiple columns by separating the criteria with a comma.</span></span>

<span data-ttu-id="51032-184">**Příklad:**</span><span class="sxs-lookup"><span data-stu-id="51032-184">**Example:**</span></span>

- `ORDER BY  MonthlyActiveUsers ASC,  Month DESC`
- `ORDER BY CustomerName ASC,  Month`

### `LIMIT`

<span data-ttu-id="51032-185">Tato část dotazu určuje počet řádků, které se budou exportovat.</span><span class="sxs-lookup"><span data-stu-id="51032-185">This part of the query specifies the number of rows that will be exported.</span></span> <span data-ttu-id="51032-186">Číslo, které zadáte, musí být kladné nenulové celé číslo.</span><span class="sxs-lookup"><span data-stu-id="51032-186">The number you specify needs to be a positive nonzero integer.</span></span>

### `TIMESPAN`

<span data-ttu-id="51032-187">Tato část dotazu určuje dobu trvání, po kterou je potřeba data exportovat.</span><span class="sxs-lookup"><span data-stu-id="51032-187">This part of the query specifies the time duration for which the data needs to be exported.</span></span> <span data-ttu-id="51032-188">Možné hodnoty by měly být z *pole availableDateRanges* v definici datové sady.</span><span class="sxs-lookup"><span data-stu-id="51032-188">The possible values should be from the *availableDateRanges* field in the dataset definition.</span></span>

### <a name="case-sensitivity-in-query-specification"></a><span data-ttu-id="51032-189">Rozlišování velkých a malých písmen ve specifikaci dotazu</span><span class="sxs-lookup"><span data-stu-id="51032-189">Case sensitivity in query specification</span></span>

<span data-ttu-id="51032-190">Specifikace zcela rozlišuje malá a velká písmena.</span><span class="sxs-lookup"><span data-stu-id="51032-190">The specification is completely case insensitive.</span></span> <span data-ttu-id="51032-191">Předdefinovaná klíčová slova, názvy sloupců a hodnoty lze zadat velkými nebo velkými písmeny.</span><span class="sxs-lookup"><span data-stu-id="51032-191">Predefined keywords, column names and values can be specified using upper or lower case.</span></span>

## <a name="next-steps"></a><span data-ttu-id="51032-192">Další kroky</span><span class="sxs-lookup"><span data-stu-id="51032-192">Next steps</span></span>

- [<span data-ttu-id="51032-193">Seznam systémových dotazů</span><span class="sxs-lookup"><span data-stu-id="51032-193">List of system queries</span></span>](insights-programmatic-system-queries.md)
- [<span data-ttu-id="51032-194">Seznam ukázkových dotazů</span><span class="sxs-lookup"><span data-stu-id="51032-194">List of sample queries</span></span>](insights-programmatic-sample-queries.md)