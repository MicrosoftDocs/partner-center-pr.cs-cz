---
title: získání všech rozhraní API datových sad – Přehledy dat
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Pomocí tohoto rozhraní API získáte podrobné informace o všech dostupných datových sadách ve službě partner Center Insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 42ff7cc1f097e2423be5f1f7f9a7f62214d64949
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376387"
---
# <a name="get-all-datasets-api"></a><span data-ttu-id="2bc03-103">Získat všechny rozhraní API datových sad</span><span class="sxs-lookup"><span data-stu-id="2bc03-103">Get all datasets API</span></span>

<span data-ttu-id="2bc03-104">Rozhraní API získat všechny datové sady získá všechny dostupné datové sady.</span><span class="sxs-lookup"><span data-stu-id="2bc03-104">The Get all datasets API gets all the available datasets.</span></span> <span data-ttu-id="2bc03-105">Datové sady vypíše tabulky, sloupce, metriky a časové rozsahy.</span><span class="sxs-lookup"><span data-stu-id="2bc03-105">Datasets list the tables, columns, metrics, and time ranges.</span></span>

<span data-ttu-id="2bc03-106">**Syntaxe žádosti**</span><span class="sxs-lookup"><span data-stu-id="2bc03-106">**Request syntax**</span></span>

|    <span data-ttu-id="2bc03-107">Metoda</span><span class="sxs-lookup"><span data-stu-id="2bc03-107">Method</span></span>    |    <span data-ttu-id="2bc03-108">Identifikátor URI žádosti</span><span class="sxs-lookup"><span data-stu-id="2bc03-108">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="2bc03-109">GET</span><span class="sxs-lookup"><span data-stu-id="2bc03-109">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset?datasetName={Dataset Name}`     |
|        |        |

<span data-ttu-id="2bc03-110">**Hlavička žádosti**</span><span class="sxs-lookup"><span data-stu-id="2bc03-110">**Request header**</span></span>

|    <span data-ttu-id="2bc03-111">Hlavička</span><span class="sxs-lookup"><span data-stu-id="2bc03-111">Header</span></span>    |    <span data-ttu-id="2bc03-112">Typ</span><span class="sxs-lookup"><span data-stu-id="2bc03-112">Type</span></span>    |    <span data-ttu-id="2bc03-113">Description</span><span class="sxs-lookup"><span data-stu-id="2bc03-113">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="2bc03-114">Autorizace</span><span class="sxs-lookup"><span data-stu-id="2bc03-114">Authorization</span></span>    |    <span data-ttu-id="2bc03-115">řetězec</span><span class="sxs-lookup"><span data-stu-id="2bc03-115">string</span></span>    |    <span data-ttu-id="2bc03-116">Povinná hodnota.</span><span class="sxs-lookup"><span data-stu-id="2bc03-116">Required.</span></span> <span data-ttu-id="2bc03-117">přístupový token pro Azure Active Directory (AAD) ve formuláři`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="2bc03-117">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="2bc03-118">Typ obsahu</span><span class="sxs-lookup"><span data-stu-id="2bc03-118">Content-Type</span></span>    |    <span data-ttu-id="2bc03-119">řetězec</span><span class="sxs-lookup"><span data-stu-id="2bc03-119">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="2bc03-120">**Parametr cesty**</span><span class="sxs-lookup"><span data-stu-id="2bc03-120">**Path parameter**</span></span>

<span data-ttu-id="2bc03-121">Žádná</span><span class="sxs-lookup"><span data-stu-id="2bc03-121">None</span></span>

<span data-ttu-id="2bc03-122">**Parametr dotazu**</span><span class="sxs-lookup"><span data-stu-id="2bc03-122">**Query parameter**</span></span>

|    <span data-ttu-id="2bc03-123">Název parametru</span><span class="sxs-lookup"><span data-stu-id="2bc03-123">Parameter Name</span></span>    |    <span data-ttu-id="2bc03-124">Typ</span><span class="sxs-lookup"><span data-stu-id="2bc03-124">Type</span></span>    |    <span data-ttu-id="2bc03-125">Vyžadováno</span><span class="sxs-lookup"><span data-stu-id="2bc03-125">Required</span></span>    |    <span data-ttu-id="2bc03-126">Popis</span><span class="sxs-lookup"><span data-stu-id="2bc03-126">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="2bc03-127">datasetName</span><span class="sxs-lookup"><span data-stu-id="2bc03-127">datasetName</span></span>    |    <span data-ttu-id="2bc03-128">řetězec</span><span class="sxs-lookup"><span data-stu-id="2bc03-128">string</span></span>    |    <span data-ttu-id="2bc03-129">No</span><span class="sxs-lookup"><span data-stu-id="2bc03-129">No</span></span>    |    <span data-ttu-id="2bc03-130">Filtr, aby se získaly podrobnosti jenom pro jednu datovou sadu</span><span class="sxs-lookup"><span data-stu-id="2bc03-130">Filter to get details of only one dataset</span></span>    |
|        |        |        |        |

<span data-ttu-id="2bc03-131">**Datová část požadavku**</span><span class="sxs-lookup"><span data-stu-id="2bc03-131">**Request payload**</span></span>

<span data-ttu-id="2bc03-132">Žádná</span><span class="sxs-lookup"><span data-stu-id="2bc03-132">None</span></span>

<span data-ttu-id="2bc03-133">**Glosář**</span><span class="sxs-lookup"><span data-stu-id="2bc03-133">**Glossary**</span></span>

<span data-ttu-id="2bc03-134">Žádná</span><span class="sxs-lookup"><span data-stu-id="2bc03-134">None</span></span>

<span data-ttu-id="2bc03-135">**Response** (Odpověď)</span><span class="sxs-lookup"><span data-stu-id="2bc03-135">**Response**</span></span>

<span data-ttu-id="2bc03-136">Datová část odpovědi je strukturována takto:</span><span class="sxs-lookup"><span data-stu-id="2bc03-136">The response payload is structured as follows:</span></span>

<span data-ttu-id="2bc03-137">Kód odpovědi: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="2bc03-137">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="2bc03-138">Příklad datové části odpovědi:</span><span class="sxs-lookup"><span data-stu-id="2bc03-138">Response payload example:</span></span>

```json
{ 
   "Value":[ 
      { 
         "DatasetName ":"string", 
         "SelectableColumns":[ 
            "string" 
         ], 
         "AvailableMetrics":[ 
            "string" 
         ], 
         "AvailableDateRanges":[ 
            "string" 
         ], 
         "minimumRecurrenceInterval":0 
      } 
   ], 
   "TotalCount":0, 
   "Message":"<Error Message>", 
   "StatusCode": 0, 
} 
```

<span data-ttu-id="2bc03-139">**Glosář**</span><span class="sxs-lookup"><span data-stu-id="2bc03-139">**Glossary**</span></span>

<span data-ttu-id="2bc03-140">Tato tabulka definuje klíčové prvky v odpovědi:</span><span class="sxs-lookup"><span data-stu-id="2bc03-140">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="2bc03-141">Parametr</span><span class="sxs-lookup"><span data-stu-id="2bc03-141">Parameter</span></span>    |    <span data-ttu-id="2bc03-142">Popis</span><span class="sxs-lookup"><span data-stu-id="2bc03-142">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="2bc03-143">DatasetName</span><span class="sxs-lookup"><span data-stu-id="2bc03-143">DatasetName</span></span>     |    <span data-ttu-id="2bc03-144">Název datové sady, kterou tento objekt pole definuje</span><span class="sxs-lookup"><span data-stu-id="2bc03-144">Name of the dataset that this array object defines</span></span>     |
|    <span data-ttu-id="2bc03-145">SelectableColumns</span><span class="sxs-lookup"><span data-stu-id="2bc03-145">SelectableColumns</span></span>     |    <span data-ttu-id="2bc03-146">Nezpracované sloupce, které se dají zadat ve sloupcích pro výběr</span><span class="sxs-lookup"><span data-stu-id="2bc03-146">Raw columns that can be specified in the select columns</span></span>     |
|    <span data-ttu-id="2bc03-147">AvailableMetrics</span><span class="sxs-lookup"><span data-stu-id="2bc03-147">AvailableMetrics</span></span>     |    <span data-ttu-id="2bc03-148">Názvy sloupců agregace a metriky, které lze zadat ve sloupcích výběr</span><span class="sxs-lookup"><span data-stu-id="2bc03-148">Aggregation/metric column names that can be specified in the select columns</span></span>     |
|    <span data-ttu-id="2bc03-149">AvailableDateRanges</span><span class="sxs-lookup"><span data-stu-id="2bc03-149">AvailableDateRanges</span></span>     |    <span data-ttu-id="2bc03-150">Rozsah dat, který lze použít v dotazech sestavy pro datovou sadu</span><span class="sxs-lookup"><span data-stu-id="2bc03-150">Date range that can be used in report queries for the dataset</span></span>     |
|    <span data-ttu-id="2bc03-151">minimumRecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="2bc03-151">minimumRecurrenceInterval</span></span>     |    <span data-ttu-id="2bc03-152">Minimální hodnota intervalu opakování</span><span class="sxs-lookup"><span data-stu-id="2bc03-152">Minimum value of Recurrence Interval</span></span>     |
|    <span data-ttu-id="2bc03-153">TotalCount</span><span class="sxs-lookup"><span data-stu-id="2bc03-153">TotalCount</span></span>     |    <span data-ttu-id="2bc03-154">Počet datových sad v poli hodnot</span><span class="sxs-lookup"><span data-stu-id="2bc03-154">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="2bc03-155">Zpráva</span><span class="sxs-lookup"><span data-stu-id="2bc03-155">Message</span></span>     |    <span data-ttu-id="2bc03-156">Stavová zpráva od spuštění rozhraní API</span><span class="sxs-lookup"><span data-stu-id="2bc03-156">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="2bc03-157">StatusCode</span><span class="sxs-lookup"><span data-stu-id="2bc03-157">StatusCode</span></span>     |    <span data-ttu-id="2bc03-158">Kód výsledku.</span><span class="sxs-lookup"><span data-stu-id="2bc03-158">Result Code.</span></span> <span data-ttu-id="2bc03-159">Možné hodnoty jsou 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="2bc03-159">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
