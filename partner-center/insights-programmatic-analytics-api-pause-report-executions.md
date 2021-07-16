---
title: pozastavit spuštění sestavy rozhraní API – Přehledy dat
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Pomocí tohoto rozhraní API můžete pozastavit provádění jakékoli sestavy ve službě partner Center Insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 1e490a6d5120d729f0ea4979a201e9a80ba2991c
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376457"
---
# <a name="pause-report-executions-api"></a><span data-ttu-id="7567a-103">Pozastavit rozhraní API pro spouštění sestav</span><span class="sxs-lookup"><span data-stu-id="7567a-103">Pause report executions API</span></span>

<span data-ttu-id="7567a-104">Při spuštění toto rozhraní API pozastaví naplánované provádění sestav.</span><span class="sxs-lookup"><span data-stu-id="7567a-104">On execution, this API pauses the scheduled execution of reports.</span></span>

<span data-ttu-id="7567a-105">**Syntaxe žádosti**</span><span class="sxs-lookup"><span data-stu-id="7567a-105">**Request syntax**</span></span>

|    <span data-ttu-id="7567a-106">Metoda</span><span class="sxs-lookup"><span data-stu-id="7567a-106">Method</span></span>    |    <span data-ttu-id="7567a-107">Identifikátor URI žádosti</span><span class="sxs-lookup"><span data-stu-id="7567a-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="7567a-108">PUT</span><span class="sxs-lookup"><span data-stu-id="7567a-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/pause/{ReportID}`    |
|        |        |

<span data-ttu-id="7567a-109">**Hlavička žádosti**</span><span class="sxs-lookup"><span data-stu-id="7567a-109">**Request header**</span></span>

|    <span data-ttu-id="7567a-110">Hlavička</span><span class="sxs-lookup"><span data-stu-id="7567a-110">Header</span></span>    |    <span data-ttu-id="7567a-111">Typ</span><span class="sxs-lookup"><span data-stu-id="7567a-111">Type</span></span>    |    <span data-ttu-id="7567a-112">Description</span><span class="sxs-lookup"><span data-stu-id="7567a-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="7567a-113">Autorizace</span><span class="sxs-lookup"><span data-stu-id="7567a-113">Authorization</span></span>    |    <span data-ttu-id="7567a-114">řetězec</span><span class="sxs-lookup"><span data-stu-id="7567a-114">string</span></span>    |    <span data-ttu-id="7567a-115">Povinná hodnota.</span><span class="sxs-lookup"><span data-stu-id="7567a-115">Required.</span></span> <span data-ttu-id="7567a-116">přístupový token pro Azure Active Directory (AAD) ve formuláři`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="7567a-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="7567a-117">Typ obsahu</span><span class="sxs-lookup"><span data-stu-id="7567a-117">Content-Type</span></span>    |    <span data-ttu-id="7567a-118">řetězec</span><span class="sxs-lookup"><span data-stu-id="7567a-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="7567a-119">**Parametr cesty**</span><span class="sxs-lookup"><span data-stu-id="7567a-119">**Path parameter**</span></span>

|    <span data-ttu-id="7567a-120">Název parametru</span><span class="sxs-lookup"><span data-stu-id="7567a-120">Parameter Name</span></span>    |    <span data-ttu-id="7567a-121">Typ</span><span class="sxs-lookup"><span data-stu-id="7567a-121">Type</span></span>    |    <span data-ttu-id="7567a-122">Vyžadováno</span><span class="sxs-lookup"><span data-stu-id="7567a-122">Required</span></span>    |    <span data-ttu-id="7567a-123">Popis</span><span class="sxs-lookup"><span data-stu-id="7567a-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="7567a-124">reportId</span><span class="sxs-lookup"><span data-stu-id="7567a-124">reportId</span></span>     |    <span data-ttu-id="7567a-125">řetězec</span><span class="sxs-lookup"><span data-stu-id="7567a-125">string</span></span>    |    <span data-ttu-id="7567a-126">No</span><span class="sxs-lookup"><span data-stu-id="7567a-126">No</span></span>    |    <span data-ttu-id="7567a-127">ID upravované sestavy</span><span class="sxs-lookup"><span data-stu-id="7567a-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="7567a-128">**Parametr dotazu**</span><span class="sxs-lookup"><span data-stu-id="7567a-128">**Query parameter**</span></span>

<span data-ttu-id="7567a-129">Žádná</span><span class="sxs-lookup"><span data-stu-id="7567a-129">None</span></span>

<span data-ttu-id="7567a-130">**Datová část požadavku**</span><span class="sxs-lookup"><span data-stu-id="7567a-130">**Request payload**</span></span>

<span data-ttu-id="7567a-131">Žádná</span><span class="sxs-lookup"><span data-stu-id="7567a-131">None</span></span>

<span data-ttu-id="7567a-132">**Glosář**</span><span class="sxs-lookup"><span data-stu-id="7567a-132">**Glossary**</span></span>

<span data-ttu-id="7567a-133">Žádná</span><span class="sxs-lookup"><span data-stu-id="7567a-133">None</span></span>

<span data-ttu-id="7567a-134">**Response** (Odpověď)</span><span class="sxs-lookup"><span data-stu-id="7567a-134">**Response**</span></span>

<span data-ttu-id="7567a-135">Datová část odpovědi je strukturována takto:</span><span class="sxs-lookup"><span data-stu-id="7567a-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="7567a-136">Kód odpovědi: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="7567a-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="7567a-137">Příklad datové části odpovědi:</span><span class="sxs-lookup"><span data-stu-id="7567a-137">Response payload example:</span></span>

```json
{ 
  "Value": [ 
    { 
      "ReportId": "string", 
      "ReportName": "string", 
      "Description": "string", 
      "QueryId": "string", 
      "Query": "string", 
      "User": "string", 
      "CreatedTime": "string", 
      "ModifiedTime": "string", 
      "ExecuteNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      "RecurrenceCount": 0, 
      "CallbackUrl": "string", 
      "CallbackMethod": "string", 
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="7567a-138">**Glosář**</span><span class="sxs-lookup"><span data-stu-id="7567a-138">**Glossary**</span></span>

<span data-ttu-id="7567a-139">Tato tabulka definuje klíčové prvky v odpovědi:</span><span class="sxs-lookup"><span data-stu-id="7567a-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="7567a-140">Parametr</span><span class="sxs-lookup"><span data-stu-id="7567a-140">Parameter</span></span>    |    <span data-ttu-id="7567a-141">Popis</span><span class="sxs-lookup"><span data-stu-id="7567a-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="7567a-142">ReportId</span><span class="sxs-lookup"><span data-stu-id="7567a-142">ReportId</span></span>     |    <span data-ttu-id="7567a-143">Univerzálně jedinečný identifikátor (UUID) pozastavené sestavy</span><span class="sxs-lookup"><span data-stu-id="7567a-143">Universally unique identifier (UUID) of the paused report</span></span>     |
|    <span data-ttu-id="7567a-144">ReportName</span><span class="sxs-lookup"><span data-stu-id="7567a-144">ReportName</span></span>     |    <span data-ttu-id="7567a-145">Název zadaný pro sestavu během vytváření</span><span class="sxs-lookup"><span data-stu-id="7567a-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="7567a-146">Description</span><span class="sxs-lookup"><span data-stu-id="7567a-146">Description</span></span>     |    <span data-ttu-id="7567a-147">Popis zadaný při vytváření sestavy</span><span class="sxs-lookup"><span data-stu-id="7567a-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="7567a-148">QueryId</span><span class="sxs-lookup"><span data-stu-id="7567a-148">QueryId</span></span>     |    <span data-ttu-id="7567a-149">ID dotazu předané v okamžiku vytvoření sestavy</span><span class="sxs-lookup"><span data-stu-id="7567a-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="7567a-150">Dotaz</span><span class="sxs-lookup"><span data-stu-id="7567a-150">Query</span></span>     |    <span data-ttu-id="7567a-151">Text dotazu, který se spustí pro tuto sestavu</span><span class="sxs-lookup"><span data-stu-id="7567a-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="7567a-152">Uživatel</span><span class="sxs-lookup"><span data-stu-id="7567a-152">User</span></span>     |    <span data-ttu-id="7567a-153">ID uživatele, které se použilo k vytvoření sestavy</span><span class="sxs-lookup"><span data-stu-id="7567a-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="7567a-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="7567a-154">CreatedTime</span></span>     |    <span data-ttu-id="7567a-155">Čas, kdy byla sestava vytvořena.</span><span class="sxs-lookup"><span data-stu-id="7567a-155">Time the report was created.</span></span> <span data-ttu-id="7567a-156">Formát času je RRRR-MM-ddTHH: mm: ssZ</span><span class="sxs-lookup"><span data-stu-id="7567a-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="7567a-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="7567a-157">ModifiedTime</span></span>     |    <span data-ttu-id="7567a-158">Čas poslední změny sestavy</span><span class="sxs-lookup"><span data-stu-id="7567a-158">Time the report was last modified.</span></span> <span data-ttu-id="7567a-159">Formát času je RRRR-MM-ddTHH: mm: ssZ</span><span class="sxs-lookup"><span data-stu-id="7567a-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="7567a-160">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="7567a-160">ExecuteNow</span></span>     |    <span data-ttu-id="7567a-161">Příznak ExecuteNow se nastavil v okamžiku vytvoření sestavy.</span><span class="sxs-lookup"><span data-stu-id="7567a-161">ExecuteNow flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="7567a-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="7567a-162">StartTime</span></span>     |    <span data-ttu-id="7567a-163">Čas, kdy se spustí spuštění sestavy.</span><span class="sxs-lookup"><span data-stu-id="7567a-163">Time the report execution will begin.</span></span> <span data-ttu-id="7567a-164">Formát času je RRRR-MM-ddTHH: mm: ssZ</span><span class="sxs-lookup"><span data-stu-id="7567a-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="7567a-165">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="7567a-165">ReportStatus</span></span>     |    <span data-ttu-id="7567a-166">Stav provádění sestavy</span><span class="sxs-lookup"><span data-stu-id="7567a-166">Status of the report execution.</span></span> <span data-ttu-id="7567a-167">Možné hodnoty jsou pozastavené, aktivní a neaktivní.</span><span class="sxs-lookup"><span data-stu-id="7567a-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="7567a-168">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="7567a-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="7567a-169">Interval opakování zadaný při vytváření sestavy</span><span class="sxs-lookup"><span data-stu-id="7567a-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="7567a-170">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="7567a-170">RecurrenceCount</span></span>     |    <span data-ttu-id="7567a-171">Počet opakování poskytnutý během vytváření sestavy</span><span class="sxs-lookup"><span data-stu-id="7567a-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="7567a-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="7567a-172">CallbackUrl</span></span>     |    <span data-ttu-id="7567a-173">Adresa URL zpětného volání poskytnutá v žádosti</span><span class="sxs-lookup"><span data-stu-id="7567a-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="7567a-174">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="7567a-174">CallbackMethod</span></span>    |    <span data-ttu-id="7567a-175">Metoda zpětného volání poskytnutá v žádosti</span><span class="sxs-lookup"><span data-stu-id="7567a-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="7567a-176">Formát</span><span class="sxs-lookup"><span data-stu-id="7567a-176">Format</span></span>     |    <span data-ttu-id="7567a-177">Formát souborů sestav</span><span class="sxs-lookup"><span data-stu-id="7567a-177">Format of the report files</span></span>     |
|    <span data-ttu-id="7567a-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="7567a-178">TotalCount</span></span>     |    <span data-ttu-id="7567a-179">Počet datových sad v poli hodnot</span><span class="sxs-lookup"><span data-stu-id="7567a-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="7567a-180">Zpráva</span><span class="sxs-lookup"><span data-stu-id="7567a-180">Message</span></span>     |    <span data-ttu-id="7567a-181">Stavová zpráva od spuštění rozhraní API</span><span class="sxs-lookup"><span data-stu-id="7567a-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="7567a-182">StatusCode</span><span class="sxs-lookup"><span data-stu-id="7567a-182">StatusCode</span></span>     |    <span data-ttu-id="7567a-183">Kód výsledku.</span><span class="sxs-lookup"><span data-stu-id="7567a-183">Result Code.</span></span> <span data-ttu-id="7567a-184">Možné hodnoty jsou 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="7567a-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
