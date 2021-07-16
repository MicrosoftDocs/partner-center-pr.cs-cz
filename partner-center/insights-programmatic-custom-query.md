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
# <a name="custom-query-specification"></a>Specifikace vlastních dotazů

Partneři mohou tuto specifikaci dotazu použít ke snadnému formulování vlastních dotazů pro extrahování dat z analytických tabulek. Dotazy lze použít k výběru pouze požadovaných sloupců a metrik, které odpovídají určitým kritériím. V centru specifikace jazyka je definice datové sady, na kterou lze napsat vlastní dotaz.

## <a name="datasets"></a>Datové sady

Stejně jako se některé dotazy spouštěly proti databázi, která obsahuje tabulky a sloupce, funguje vlastní dotaz na datové sady, které mají sloupce a metriky. Úplný seznam dostupných datových sad pro formulovat dotaz lze získat pomocí rozhraní API datových sad.

Toto je příklad datové sady zobrazené jako JSON:

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

## <a name="parts-of-a-dataset"></a>Části datové sady

- Název datové sady je jako název databázové tabulky. Například OfficeUsage. Datová sada obsahuje seznam sloupců, které je možné vybrat, například CustomerTenantId.
- Datová sada má také metriky, které jsou v databázi jako agregační funkce. Například TotalMonthlyActiveUsers.
- Existují pevná časová období, během kterých je možné data exportovat.

## <a name="formulating-a-query-on-a-dataset"></a>Formulace dotazu na datovou sadu

Toto jsou některé ukázkové dotazy, které ukazují, jak extrahovat různé typy dat.

|Dotaz|    Description    |
|----|    ----    |
|**SELECT (VYBRAT)** CustomerTenantId, PaidAvailableUnits **FROM** <br>OfficeUsage **TIMESPAN** LAST_MONTH|    Tento dotaz za poslední 1 měsíc zobrazí všechny hodnoty CusotmerTenantID a příslušné jednotky PaidAvailableUnits.    |
|**SELECT (VYBRAT)** CustomerTenantId, PaidAvailableUnits **FROM** <br>OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10|    Tento dotaz zobrazí 10 tenantů s nejvyšším počtem placených dostupných jednotek v sestupného pořadí.     |
|**SELECT (VYBRAT)** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS |    Tento dotaz zobrazí jednotky PaidAvailableUnits a MonthlyActiveUsers všech zákazníků, kteří mají monthlyActiveUsers větší než 100 000.     |
|**SELECT (VYBRAT)** CustomerTenantId, Month, MonthlyActiveUsers **FROM** <br>OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002') |    Tento dotaz zobrazí hodnotu CustomerTenantId a měsíční aktivní uživatele pro každý měsíc podle dvou hodnot CustomerTpId: '2a31c234-1f4e-4c60-909e-76d234f93161 a 80780748-3f9a-11eb-b378-0242ac130002.     |
|        |        |

## <a name="query-specification"></a>Specifikace dotazu

Tato část popisuje definici a strukturu dotazu.

## <a name="grammar-reference"></a>Referenční informace k gramatikě

Tato tabulka popisuje symboly používané v dotazech.

|    Dotaz    |    Description    |
|    ----    |    ----    |
|    `?`    |    Volitelné    |
|    `*`    |    Nula nebo více    |
|    `+`    |    Jeden nebo více    |
|    `\|`    |    Nebo / Jeden ze seznamů    |
|        |        |

## <a name="query-definition"></a>Definice dotazu

Příkaz dotazu obsahuje následující klauzule: SelectClause, FromClause, WhereClause, OrderClause, LimitClause a TimeSpan.

- **SelectClause**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`
    - **ColumOrMetricName:** Sloupce a metriky definované v rámci datové sady
- **FromClause:**`FROM DatasetName`
    - **DatasetName:** Název datové sady definovaný v datové sadě
- **WhereClause**: `WHERE FilterCondition (AND FilterCondition)`
    - **FilterCondition:** ColumOrMetricName – hodnota operátoru
        - **Operátor**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`
        - **Value**: Number | StringLiteral – | MultiNumberList – | Seznam víceřetězcových řetězců
            - **Číslo:**`-? [0-9]+ (. [0-9] [0-9]*)?`
            - **StringLiteral**:  `' [a-zA-Z0-9_]*'`
            - **MultiNumberList:**`(Number (,Number)*)`
            - **MultiStringList:**`(StringLiteral (,StringLiteral)*)`
- **OrderClause:**`ORDER BY OrderCondition (,OrderCondition)`
    - **OrderCondition**: `ColumOrMetricName (ASC | DESC)*`
- **LimitClause:**`LIMIT [0-9]+`
- **TimeSpan**: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`

## <a name="query-structure"></a>Struktura dotazů

Dotaz sestavy se sýtá z několika částí:
- `SELECT`
- `FROM`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `TIMESPAN`

Jednotlivé části jsou popsány níže.

### `SELECT`

Tato část dotazu určuje sloupce, které se mají exportovat. Sloupce, které je možné vybrat, jsou pole uvedená v *oddílech selectableColumns* a *availableMetrics* datové sady.

Volitelně můžete `DISTINCT` zadat klíčové slovo za `SELECT` . Pokud `DISTINCT` je zadaný parametr , budou konečné exportované řádky vždy obsahovat odlišné hodnoty vybraných sloupců. Metriky se budou počítat pro každou odlišnou kombinaci vybraných sloupců, takže klíčové slovo se nevyžaduje, pokud je sloupec metriky zahrnutý v `DISTINCT` seznamu vybraných sloupců.

**Příklad:**

```sql
SELECT CustomerTenantId, PaidAvailableUnits; 
SELECT DISTINCT CustomerTenantId
```

### `FROM`

Tato část dotazu označuje datovou sadu, ze které se mají data exportovat. Název datové sady, který tady najdete, musí být platným názvem datové sady vrácený rozhraním API datových sad.

**Příklad:**

- `FROM  OfficeUsage`
- `FROM  AzureUsage`

### `WHERE`

Tato část dotazu slouží k určení podmínek filtru pro datovou sadu. V posledním exportovaného souboru budou k dispozici pouze řádky, které odpovídají všem podmínkám uvedeným v této klauzuli. Podmínka filtru může být u libovolného sloupce uvedeného ve *sloupcích selectableColumns* a *availableMetrics*. Hodnoty zadané v podměně filtru mohou být seznam čísel nebo seznam řetězců pouze v případě, že operátor je `IN` nebo `NOT IN` . Hodnoty lze vždy zadat jako řetězec literálu a budou převedeny na nativní typy sloupců. Více podmínek filtru musí být odděleno operací AND.

**Příklad:**

- `CustomerTenantId= '868368da-957d-4959-8992-3c12dc7e6260'`
- `CustomerName LIKE '%Contoso%'`
- `CustomerId NOT IN (1000, 1001, 1002)`
- `OrderQuantity=100`
- `CustomerTenantId='7b487ac0-ce12-b732-dcd6-91a1e4e74a50' AND CustomerTpId=' 0f8b7fa0-eb83-a183-1225-ca153ef807aa'`

### `ORDER BY`

Tato část dotazu určuje kritéria pořadí pro exportované řádky. Sloupce, ve kterých je možné definovat řazení, musí být ze *sloupců selectableColumns* a *availableMetrics* datové sady. Pokud není zadaný žádný směr řazení, bude ve sloupci ve výchozím nastavení DESC. Řazení lze definovat na více sloupcích oddělením kritérií čárkou.

**Příklad:**

- `ORDER BY  MonthlyActiveUsers ASC,  Month DESC`
- `ORDER BY CustomerName ASC,  Month`

### `LIMIT`

Tato část dotazu určuje počet řádků, které se budou exportovat. Číslo, které zadáte, musí být kladné nenulové celé číslo.

### `TIMESPAN`

Tato část dotazu určuje dobu trvání, po kterou je potřeba data exportovat. Možné hodnoty by měly být z *pole availableDateRanges* v definici datové sady.

### <a name="case-sensitivity-in-query-specification"></a>Rozlišování velkých a malých písmen ve specifikaci dotazu

Specifikace zcela rozlišuje malá a velká písmena. Předdefinovaná klíčová slova, názvy sloupců a hodnoty lze zadat velkými nebo velkými písmeny.

## <a name="next-steps"></a>Další kroky

- [Seznam systémových dotazů](insights-programmatic-system-queries.md)
- [Seznam ukázkových dotazů](insights-programmatic-sample-queries.md)