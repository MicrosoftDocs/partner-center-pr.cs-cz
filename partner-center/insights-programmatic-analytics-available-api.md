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
# <a name="available-apis-for-partner-insights-analytics"></a><span data-ttu-id="b2cdb-103">Dostupná rozhraní API pro analýzy partnerských přehledů</span><span class="sxs-lookup"><span data-stu-id="b2cdb-103">Available APIs for partner insights analytics</span></span>

<span data-ttu-id="b2cdb-104">Následuje seznam rozhraní API pro analýzy partnerských přehledů a jejich přidružených funkcí.</span><span class="sxs-lookup"><span data-stu-id="b2cdb-104">Following are the list of APIs for partner insights analytics and their associated functionalities.</span></span>

## <a name="dataset-pull-apis"></a><span data-ttu-id="b2cdb-105">Rozhraní API pro vyžádanou datovou sadu</span><span class="sxs-lookup"><span data-stu-id="b2cdb-105">Dataset pull APIs</span></span>

<span data-ttu-id="b2cdb-106">***Tabulka 1: Rozhraní API pro vyžádanou datovou sadu***</span><span class="sxs-lookup"><span data-stu-id="b2cdb-106">***Table 1: Dataset pull APIs***</span></span>

| <span data-ttu-id="b2cdb-107">**Rozhraní API**</span><span class="sxs-lookup"><span data-stu-id="b2cdb-107">**API**</span></span> | <span data-ttu-id="b2cdb-108">**Funkce**</span><span class="sxs-lookup"><span data-stu-id="b2cdb-108">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="b2cdb-109">Získání všech datových sad</span><span class="sxs-lookup"><span data-stu-id="b2cdb-109">Get all datasets</span></span>](insights-programmatic-analytics-api-get-dataset.md) | <span data-ttu-id="b2cdb-110">Získá všechny dostupné datové sady.</span><span class="sxs-lookup"><span data-stu-id="b2cdb-110">Gets all the available datasets.</span></span> <span data-ttu-id="b2cdb-111">Datové sady obsahují tabulky, sloupce, metriky a časové rozsahy.</span><span class="sxs-lookup"><span data-stu-id="b2cdb-111">Datasets list the tables, columns, metrics, and time ranges.</span></span> |
|||

## <a name="query-management-apis"></a><span data-ttu-id="b2cdb-112">Rozhraní API pro správu dotazů</span><span class="sxs-lookup"><span data-stu-id="b2cdb-112">Query management APIs</span></span>

<span data-ttu-id="b2cdb-113">***Tabulka 2: Rozhraní API pro správu dotazů***</span><span class="sxs-lookup"><span data-stu-id="b2cdb-113">***Table 2: Query management APIs***</span></span>

| <span data-ttu-id="b2cdb-114">**Rozhraní API**</span><span class="sxs-lookup"><span data-stu-id="b2cdb-114">**API**</span></span> | <span data-ttu-id="b2cdb-115">**Funkce**</span><span class="sxs-lookup"><span data-stu-id="b2cdb-115">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="b2cdb-116">Vytvoření dotazu na sestavu</span><span class="sxs-lookup"><span data-stu-id="b2cdb-116">Create Report Query</span></span>](insights-programmatic-access-paradigm.md#create-report-query-api) | <span data-ttu-id="b2cdb-117">Vytvoří vlastní dotazy, které definují datovou sadu, ze které se mají exportovat sloupce a metriky.</span><span class="sxs-lookup"><span data-stu-id="b2cdb-117">Creates custom queries that define the dataset from which columns and metrics need to be exported.</span></span> |
| [<span data-ttu-id="b2cdb-118">GET Report Query</span><span class="sxs-lookup"><span data-stu-id="b2cdb-118">GET Report Query</span></span>](insights-programmatic-analytics-api-get-report-queries.md) | <span data-ttu-id="b2cdb-119">Získá všechny dotazy, které jsou k dispozici pro použití v sestavách.</span><span class="sxs-lookup"><span data-stu-id="b2cdb-119">Gets all the queries available for use in reports.</span></span> <span data-ttu-id="b2cdb-120">Ve výchozím nastavení získá všechny systémové a uživatelsky definované dotazy.</span><span class="sxs-lookup"><span data-stu-id="b2cdb-120">Gets all the system and user-defined queries by default.</span></span> |
| [<span data-ttu-id="b2cdb-121">ODSTRANĚNÍ dotazu na sestavu</span><span class="sxs-lookup"><span data-stu-id="b2cdb-121">DELETE Report Query</span></span>](insights-programmatic-analytics-api-delete-report-queries.md) | <span data-ttu-id="b2cdb-122">Odstraní uživatelsky definované dotazy.</span><span class="sxs-lookup"><span data-stu-id="b2cdb-122">Deletes user-defined queries.</span></span> |
|||

## <a name="report-management-apis"></a><span data-ttu-id="b2cdb-123">Rozhraní API pro správu sestav</span><span class="sxs-lookup"><span data-stu-id="b2cdb-123">Report management APIs</span></span>

<span data-ttu-id="b2cdb-124">***Tabulka 3: Rozhraní API pro správu sestav***</span><span class="sxs-lookup"><span data-stu-id="b2cdb-124">***Table 3: Report management APIs***</span></span>

| <span data-ttu-id="b2cdb-125">**Rozhraní API**</span><span class="sxs-lookup"><span data-stu-id="b2cdb-125">**API**</span></span> | <span data-ttu-id="b2cdb-126">**Funkce**</span><span class="sxs-lookup"><span data-stu-id="b2cdb-126">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="b2cdb-127">Vytvoření sestavy</span><span class="sxs-lookup"><span data-stu-id="b2cdb-127">Create Report</span></span>](insights-programmatic-access-paradigm.md#create-report-api) | <span data-ttu-id="b2cdb-128">Naplánuje spuštění dotazu v pravidelných intervalech.</span><span class="sxs-lookup"><span data-stu-id="b2cdb-128">Schedules a query to be executed at regular intervals.</span></span> |
| [<span data-ttu-id="b2cdb-129">TRY Report Query</span><span class="sxs-lookup"><span data-stu-id="b2cdb-129">TRY Report Query</span></span>](insights-programmatic-analytics-api-try-report-queries.md) | <span data-ttu-id="b2cdb-130">Spustí příkaz dotazu sestavy.</span><span class="sxs-lookup"><span data-stu-id="b2cdb-130">Executes a Report query statement.</span></span> <span data-ttu-id="b2cdb-131">Vrátí pouze 10 záznamů, které partner může použít k ověření, jestli jsou data podle očekávání.</span><span class="sxs-lookup"><span data-stu-id="b2cdb-131">Returns only 10 records that a partner can use to verify if the data is as expected.</span></span> |
| [<span data-ttu-id="b2cdb-132">Get Report</span><span class="sxs-lookup"><span data-stu-id="b2cdb-132">Get Report</span></span>](insights-programmatic-analytics-api-get-report.md) | <span data-ttu-id="b2cdb-133">Získejte všechny naplánované sestavy.</span><span class="sxs-lookup"><span data-stu-id="b2cdb-133">Get all the reports that have been scheduled.</span></span> |
| [<span data-ttu-id="b2cdb-134">Aktualizace sestavy</span><span class="sxs-lookup"><span data-stu-id="b2cdb-134">Update Report</span></span>](insights-programmatic-analytics-api-update-report.md) | <span data-ttu-id="b2cdb-135">Úprava parametru sestavy</span><span class="sxs-lookup"><span data-stu-id="b2cdb-135">Modify a report parameter.</span></span> |
| [<span data-ttu-id="b2cdb-136">Odstranění sestavy</span><span class="sxs-lookup"><span data-stu-id="b2cdb-136">Delete Report</span></span>](insights-programmatic-analytics-api-delete-report.md) | <span data-ttu-id="b2cdb-137">Odstraní všechny záznamy o spuštění sestavy a sestavy.</span><span class="sxs-lookup"><span data-stu-id="b2cdb-137">Deletes all the report and report execution records.</span></span> |
| [<span data-ttu-id="b2cdb-138">Pozastavení provádění sestav</span><span class="sxs-lookup"><span data-stu-id="b2cdb-138">Pause Report Executions</span></span>](insights-programmatic-analytics-api-pause-report-executions.md) | <span data-ttu-id="b2cdb-139">Pozastaví naplánované spouštění sestav.</span><span class="sxs-lookup"><span data-stu-id="b2cdb-139">Pauses the scheduled execution of reports.</span></span> |
| [<span data-ttu-id="b2cdb-140">Obnovení spouštění sestav</span><span class="sxs-lookup"><span data-stu-id="b2cdb-140">Resume Report Executions</span></span>](insights-programmatic-analytics-api-resume-report-executions.md) | <span data-ttu-id="b2cdb-141">Obnoví naplánované spuštění pozastavené sestavy.</span><span class="sxs-lookup"><span data-stu-id="b2cdb-141">Resumes the scheduled execution of a paused report.</span></span> |
|||

## <a name="report-execution-pull-apis"></a><span data-ttu-id="b2cdb-142">Rozhraní API pro zpracování sestav pro vyžádané zpracování</span><span class="sxs-lookup"><span data-stu-id="b2cdb-142">Report execution pull APIs</span></span>

<span data-ttu-id="b2cdb-143">***Tabulka 4: Rozhraní API pro vyžádané zpracování sestav***</span><span class="sxs-lookup"><span data-stu-id="b2cdb-143">***Table 4: Report execution pull APIs***</span></span>

| <span data-ttu-id="b2cdb-144">**Rozhraní API**</span><span class="sxs-lookup"><span data-stu-id="b2cdb-144">**API**</span></span> | <span data-ttu-id="b2cdb-145">**Funkce**</span><span class="sxs-lookup"><span data-stu-id="b2cdb-145">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="b2cdb-146">Získání spuštění sestav</span><span class="sxs-lookup"><span data-stu-id="b2cdb-146">Get Report Executions</span></span>](insights-programmatic-access-paradigm.md#get-report-execution-api) | <span data-ttu-id="b2cdb-147">Získejte všechna spuštění, která se pro danou sestavu odehrály.</span><span class="sxs-lookup"><span data-stu-id="b2cdb-147">Get all the executions that have happened for a given report.</span></span> |
|||

## <a name="next-steps"></a><span data-ttu-id="b2cdb-148">Další kroky</span><span class="sxs-lookup"><span data-stu-id="b2cdb-148">Next steps</span></span>

- <span data-ttu-id="b2cdb-149">Rozhraní API si můžete vyzkoušet prostřednictvím adresy URL rozhraní [API Swaggeru](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).</span><span class="sxs-lookup"><span data-stu-id="b2cdb-149">You can try out the APIs through the [Swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).</span></span>