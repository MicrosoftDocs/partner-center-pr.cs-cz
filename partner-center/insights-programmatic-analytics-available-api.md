---
title: Seznam rozhraní API pro přístup k datům partnerských přehledů
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Seznam rozhraní API pro přístup k datům partnerských přehledů
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 71d04b6927e27b1d7a8d72bbdaa56b41cb113625
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376447"
---
# <a name="available-apis-for-partner-insights-analytics"></a>Dostupná rozhraní API pro analýzy partnerských přehledů

Následuje seznam rozhraní API pro analýzy partnerských přehledů a jejich přidružených funkcí.

## <a name="dataset-pull-apis"></a>Rozhraní API pro vyžádanou datovou sadu

***Tabulka 1: Rozhraní API pro vyžádanou datovou sadu***

| **Rozhraní API** | **Funkce** |
| --- | --- |
| [Získání všech datových sad](insights-programmatic-analytics-api-get-dataset.md) | Získá všechny dostupné datové sady. Datové sady obsahují tabulky, sloupce, metriky a časové rozsahy. |
|||

## <a name="query-management-apis"></a>Rozhraní API pro správu dotazů

***Tabulka 2: Rozhraní API pro správu dotazů***

| **Rozhraní API** | **Funkce** |
| --- | --- |
| [Vytvoření dotazu na sestavu](insights-programmatic-access-paradigm.md#create-report-query-api) | Vytvoří vlastní dotazy, které definují datovou sadu, ze které se mají exportovat sloupce a metriky. |
| [GET Report Query](insights-programmatic-analytics-api-get-report-queries.md) | Získá všechny dotazy, které jsou k dispozici pro použití v sestavách. Ve výchozím nastavení získá všechny systémové a uživatelsky definované dotazy. |
| [ODSTRANĚNÍ dotazu na sestavu](insights-programmatic-analytics-api-delete-report-queries.md) | Odstraní uživatelsky definované dotazy. |
|||

## <a name="report-management-apis"></a>Rozhraní API pro správu sestav

***Tabulka 3: Rozhraní API pro správu sestav***

| **Rozhraní API** | **Funkce** |
| --- | --- |
| [Vytvoření sestavy](insights-programmatic-access-paradigm.md#create-report-api) | Naplánuje spuštění dotazu v pravidelných intervalech. |
| [TRY Report Query](insights-programmatic-analytics-api-try-report-queries.md) | Spustí příkaz dotazu sestavy. Vrátí pouze 10 záznamů, které partner může použít k ověření, jestli jsou data podle očekávání. |
| [Get Report](insights-programmatic-analytics-api-get-report.md) | Získejte všechny naplánované sestavy. |
| [Aktualizace sestavy](insights-programmatic-analytics-api-update-report.md) | Úprava parametru sestavy |
| [Odstranění sestavy](insights-programmatic-analytics-api-delete-report.md) | Odstraní všechny záznamy o spuštění sestavy a sestavy. |
| [Pozastavení provádění sestav](insights-programmatic-analytics-api-pause-report-executions.md) | Pozastaví naplánované spouštění sestav. |
| [Obnovení spouštění sestav](insights-programmatic-analytics-api-resume-report-executions.md) | Obnoví naplánované spuštění pozastavené sestavy. |
|||

## <a name="report-execution-pull-apis"></a>Rozhraní API pro zpracování sestav pro vyžádané zpracování

***Tabulka 4: Rozhraní API pro vyžádané zpracování sestav***

| **Rozhraní API** | **Funkce** |
| --- | --- |
| [Získání spuštění sestav](insights-programmatic-access-paradigm.md#get-report-execution-api) | Získejte všechna spuštění, která se pro danou sestavu odehrály. |
|||

## <a name="next-steps"></a>Další kroky

- Rozhraní API si můžete vyzkoušet prostřednictvím adresy URL rozhraní [API Swaggeru](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).