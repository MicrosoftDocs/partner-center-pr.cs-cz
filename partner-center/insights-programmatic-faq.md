---
title: Běžné otázky k programu partner Insights programový přístup
description: Získejte odpovědi na nejčastější dotazy týkající se přístupu k datům o partner Insights prostřednictvím rozhraní API.
ms.topic: troubleshooting
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 5645a834c2b6a84920ba032198f7f62aa1487c47
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376442"
---
# <a name="programmatic-access-of-analytics-data-common-questions"></a>Běžné dotazy k programovému přístupu k analytickým datům

Tento článek obsahuje nejčastější dotazy týkající se programového přístupu k datům o partner Insights v partnerském centru.

## <a name="api-responses"></a>Odezvy rozhraní API

Jaké jsou různé scénáře, v rámci kterých mohu přijmout odpověď rozhraní API jinou než 200 (úspěch)?

Tato tabulka popisuje odpovědi rozhraní API a to, co dělat, když je dostanete.

|    Popis chyby     |    Kód chyby     |    Řešení potíží     |
|    ----    |    ----    |    ----    |
|    Neautorizováno     |    401     |    Toto je výjimka ověřování. ověřte správnost tokenu Azure Active Directory (AAD). Token AAD je platný po 60 minutách, po uplynutí této doby byste museli token AAD znovu vygenerovat.     |
|    Neplatný název tabulky     |    400     |    Název datové sady je chybný. Znovu ověřte název datové sady voláním rozhraní API "načíst všechny datové sady".     |
|    Nesprávný název sloupce     |    400     |    Název sloupce v dotazu je nesprávný. Znovu ověřte název sloupce voláním rozhraní API "načíst všechny datové sady", nebo se podívejte na názvy sloupců v definicích dat.    |
|    Hodnota null nebo chybějící hodnota     |    400     |    V rámci datové části požadavku rozhraní API možná chybí povinné parametry.     |
|    Neplatné parametry sestavy     |    400     |    Ujistěte se, že jsou parametry sestavy správné. Můžete například pro parametr RecurrenceInterval poskytnout hodnotu menší než 4.     |
|    Interval opakování musí být mezi 4 a 2160.     |    400     |    Ujistěte se, že hodnota parametru RecurrenceInterval Request je mezi 4 a 2160.     |
|    Neplatný QueryId     |    400     |    Znovu zkontroluje vygenerované QueryId.     |
|    Neplatné parametry sestavy pro čas vytvoření a zahájení sestavy by měly být nejméně 4 hodiny od aktuálního času UTC.     |    400     |    Parametr času spuštění jako součást datové části požadavku by neměl být v minulosti. Čas zahájení sestavy by měl být nejméně 4 hodiny od aktuálního času UTC.     |
|    Požadovaná hodnota String se nenašla.     |    400     |    Ověřte, zda jste aktualizovali parametry `callbackurl` nebo formát žádosti.     |
|    S danými filtry se nenašla žádná položka.     |    404     |    Podívejte se na parametr reportID, který se používá v rozhraní get pro spuštění sestavy.     |
|    Pro dané podmínky filtru se nevyskytla žádná spuštění. Překontrolujte reportId nebo executionId a znovu spusťte rozhraní API po plánovaném čase spuštění sestavy.     |    404     |    Ujistěte se, že je reportId správný. Po plánovaném spuštění sestavy znovu spusťte rozhraní API, jak je uvedeno v datové části požadavku.     |
|    Při vytváření sestavy došlo k vnitřní chybě. ID korelace <>     |    500     |    Ujistěte se, že je správný formát data pro pole *čas_spuštění*, *QueryStartTime* a *QueryEndTime* .     |
|    Nedostupná služba    |    500     |    Pokud trvale obdržíte nedostupnou službu (chyba 5xx), otevřete lístek podpory.    |
|        |        |        |

## <a name="no-records"></a>Žádné záznamy

Při stažení sestavy z zabezpečeného umístění se mi zobrazí odpověď rozhraní API 200. Proč nezískávám žádné záznamy?
Ověřte, zda řetězec v dotazu má jednu z přípustných hodnot pro záhlaví sloupce. Tento dotaz například vrátí nulové výsledky:

```sql
SELECT CustomerTenantId, CustomerTpId, WorkloadName, Month, MonthlyActiveUsers 
FROM OfficeUsage 
WHERE IsDuplicateRowForPGA = 'False' 
ORDER BY CustomerTenantId DESC
```

V tomto příkladu jsou povolené hodnoty pro `IsDuplicateRowForPGA` hodnotu 0 nebo 1. Všechny možné hodnoty pro různé sloupce najdete v [definicích dat](insights-data-definitions.md) .
