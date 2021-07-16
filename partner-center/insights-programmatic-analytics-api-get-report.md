---
title: získat rozhraní API pro sestavy – Přehledy dat
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Pomocí tohoto rozhraní API získáte všechny dostupné ID sestav ve službě partner Center Insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 174a2f60a36cb46b287b787b177dd32236cef4eb
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376458"
---
# <a name="get-report-api"></a><span data-ttu-id="e71e0-103">Získat rozhraní API pro sestavy</span><span class="sxs-lookup"><span data-stu-id="e71e0-103">Get report API</span></span>

<span data-ttu-id="e71e0-104">Toto rozhraní API získá všechny plánované sestavy.</span><span class="sxs-lookup"><span data-stu-id="e71e0-104">This API gets all the reports that have been scheduled.</span></span>

<span data-ttu-id="e71e0-105">**Syntaxe žádosti**</span><span class="sxs-lookup"><span data-stu-id="e71e0-105">**Request syntax**</span></span>

|    <span data-ttu-id="e71e0-106">Metoda</span><span class="sxs-lookup"><span data-stu-id="e71e0-106">Method</span></span>    |    <span data-ttu-id="e71e0-107">Identifikátor URI žádosti</span><span class="sxs-lookup"><span data-stu-id="e71e0-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="e71e0-108">GET</span><span class="sxs-lookup"><span data-stu-id="e71e0-108">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport?reportId={Report ID}&reportName={Report Name}&queryId={Query ID}` |
|        |        |

<span data-ttu-id="e71e0-109">**Hlavička žádosti**</span><span class="sxs-lookup"><span data-stu-id="e71e0-109">**Request header**</span></span>

|    <span data-ttu-id="e71e0-110">Hlavička</span><span class="sxs-lookup"><span data-stu-id="e71e0-110">Header</span></span>    |    <span data-ttu-id="e71e0-111">Typ</span><span class="sxs-lookup"><span data-stu-id="e71e0-111">Type</span></span>    |    <span data-ttu-id="e71e0-112">Description</span><span class="sxs-lookup"><span data-stu-id="e71e0-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="e71e0-113">Autorizace</span><span class="sxs-lookup"><span data-stu-id="e71e0-113">Authorization</span></span>    |    <span data-ttu-id="e71e0-114">řetězec</span><span class="sxs-lookup"><span data-stu-id="e71e0-114">string</span></span>    |    <span data-ttu-id="e71e0-115">Povinná hodnota.</span><span class="sxs-lookup"><span data-stu-id="e71e0-115">Required.</span></span> <span data-ttu-id="e71e0-116">přístupový token pro Azure Active Directory (AAD) ve formuláři`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="e71e0-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="e71e0-117">Typ obsahu</span><span class="sxs-lookup"><span data-stu-id="e71e0-117">Content-Type</span></span>    |    <span data-ttu-id="e71e0-118">řetězec</span><span class="sxs-lookup"><span data-stu-id="e71e0-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="e71e0-119">**Parametr cesty**</span><span class="sxs-lookup"><span data-stu-id="e71e0-119">**Path parameter**</span></span>

<span data-ttu-id="e71e0-120">Žádná</span><span class="sxs-lookup"><span data-stu-id="e71e0-120">None</span></span>

<span data-ttu-id="e71e0-121">**Parametr dotazu**</span><span class="sxs-lookup"><span data-stu-id="e71e0-121">**Query parameter**</span></span>

|    <span data-ttu-id="e71e0-122">Název parametru</span><span class="sxs-lookup"><span data-stu-id="e71e0-122">Parameter Name</span></span>    |    <span data-ttu-id="e71e0-123">Typ</span><span class="sxs-lookup"><span data-stu-id="e71e0-123">Type</span></span>    |    <span data-ttu-id="e71e0-124">Vyžadováno</span><span class="sxs-lookup"><span data-stu-id="e71e0-124">Required</span></span>    |    <span data-ttu-id="e71e0-125">Popis</span><span class="sxs-lookup"><span data-stu-id="e71e0-125">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="e71e0-126">reportId</span><span class="sxs-lookup"><span data-stu-id="e71e0-126">reportId</span></span>     |    <span data-ttu-id="e71e0-127">řetězec</span><span class="sxs-lookup"><span data-stu-id="e71e0-127">string</span></span>    |    <span data-ttu-id="e71e0-128">No</span><span class="sxs-lookup"><span data-stu-id="e71e0-128">No</span></span>    |    <span data-ttu-id="e71e0-129">Filtr pro získání podrobností o pouze sestavách s reportId, které jsou uvedeny v tomto argumentu</span><span class="sxs-lookup"><span data-stu-id="e71e0-129">Filter to get details of only reports with the reportId given in this argument</span></span>     |
|    <span data-ttu-id="e71e0-130">reportName</span><span class="sxs-lookup"><span data-stu-id="e71e0-130">reportName</span></span>     |    <span data-ttu-id="e71e0-131">řetězec</span><span class="sxs-lookup"><span data-stu-id="e71e0-131">string</span></span>    |    <span data-ttu-id="e71e0-132">No</span><span class="sxs-lookup"><span data-stu-id="e71e0-132">No</span></span>    |    <span data-ttu-id="e71e0-133">Filtr, který získá podrobné informace o pouze sestavách se sestavou, která je uvedena v tomto argumentu</span><span class="sxs-lookup"><span data-stu-id="e71e0-133">Filter to get details of only reports with the reportName given in this argument</span></span>     |
|    <span data-ttu-id="e71e0-134">queryId</span><span class="sxs-lookup"><span data-stu-id="e71e0-134">queryId</span></span>     |    <span data-ttu-id="e71e0-135">řetězec</span><span class="sxs-lookup"><span data-stu-id="e71e0-135">string</span></span>    |    <span data-ttu-id="e71e0-136">No</span><span class="sxs-lookup"><span data-stu-id="e71e0-136">No</span></span>    |    <span data-ttu-id="e71e0-137">Filtr pro získání podrobností o pouze sestavách s queryId, které jsou uvedeny v tomto argumentu</span><span class="sxs-lookup"><span data-stu-id="e71e0-137">Filter to get details of only reports with the queryId given in this argument</span></span>     |
|        |        |        |        |


<span data-ttu-id="e71e0-138">**Datová část požadavku**</span><span class="sxs-lookup"><span data-stu-id="e71e0-138">**Request payload**</span></span>

<span data-ttu-id="e71e0-139">Žádná</span><span class="sxs-lookup"><span data-stu-id="e71e0-139">None</span></span>

<span data-ttu-id="e71e0-140">**Glosář**</span><span class="sxs-lookup"><span data-stu-id="e71e0-140">**Glossary**</span></span>

<span data-ttu-id="e71e0-141">Žádná</span><span class="sxs-lookup"><span data-stu-id="e71e0-141">None</span></span>

<span data-ttu-id="e71e0-142">**Response** (Odpověď)</span><span class="sxs-lookup"><span data-stu-id="e71e0-142">**Response**</span></span>

<span data-ttu-id="e71e0-143">Datová část odpovědi je strukturována takto:</span><span class="sxs-lookup"><span data-stu-id="e71e0-143">The response payload is structured as follows:</span></span>

<span data-ttu-id="e71e0-144">Kód odpovědi: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="e71e0-144">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="e71e0-145">Příklad datové části odpovědi:</span><span class="sxs-lookup"><span data-stu-id="e71e0-145">Response payload example:</span></span>

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
      "executeNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      " RecurrenceCount": 0, 
      "CallbackUrl": "string",
      "CallbackMethod": null,
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0 
}
```

<span data-ttu-id="e71e0-146">**Glosář**</span><span class="sxs-lookup"><span data-stu-id="e71e0-146">**Glossary**</span></span>

<span data-ttu-id="e71e0-147">Tato tabulka definuje klíčové prvky v odpovědi:</span><span class="sxs-lookup"><span data-stu-id="e71e0-147">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="e71e0-148">Parametr</span><span class="sxs-lookup"><span data-stu-id="e71e0-148">Parameter</span></span>    |    <span data-ttu-id="e71e0-149">Popis</span><span class="sxs-lookup"><span data-stu-id="e71e0-149">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="e71e0-150">ReportId</span><span class="sxs-lookup"><span data-stu-id="e71e0-150">ReportId</span></span>     |    <span data-ttu-id="e71e0-151">Jedinečný identifikátor UUID sestavy, která byla vytvořena</span><span class="sxs-lookup"><span data-stu-id="e71e0-151">Unique UUID of the report that was created</span></span>     |
|    <span data-ttu-id="e71e0-152">ReportName</span><span class="sxs-lookup"><span data-stu-id="e71e0-152">ReportName</span></span>     |    <span data-ttu-id="e71e0-153">Název zadaný pro sestavu v datové části požadavku</span><span class="sxs-lookup"><span data-stu-id="e71e0-153">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="e71e0-154">Description</span><span class="sxs-lookup"><span data-stu-id="e71e0-154">Description</span></span>     |    <span data-ttu-id="e71e0-155">Popis zadaný při vytvoření sestavy</span><span class="sxs-lookup"><span data-stu-id="e71e0-155">Description given when the report was created</span></span>     |
|    <span data-ttu-id="e71e0-156">QueryId</span><span class="sxs-lookup"><span data-stu-id="e71e0-156">QueryId</span></span>     |    <span data-ttu-id="e71e0-157">ID dotazu předané v okamžiku vytvoření sestavy</span><span class="sxs-lookup"><span data-stu-id="e71e0-157">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="e71e0-158">Dotaz</span><span class="sxs-lookup"><span data-stu-id="e71e0-158">Query</span></span>     |    <span data-ttu-id="e71e0-159">Text dotazu, který se spustí pro tuto sestavu</span><span class="sxs-lookup"><span data-stu-id="e71e0-159">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="e71e0-160">Uživatel</span><span class="sxs-lookup"><span data-stu-id="e71e0-160">User</span></span>     |    <span data-ttu-id="e71e0-161">ID uživatele, které se použilo k vytvoření sestavy</span><span class="sxs-lookup"><span data-stu-id="e71e0-161">User ID used to create the report</span></span>     |
|    <span data-ttu-id="e71e0-162">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="e71e0-162">CreatedTime</span></span>     |    <span data-ttu-id="e71e0-163">Čas, kdy byla sestava vytvořena.</span><span class="sxs-lookup"><span data-stu-id="e71e0-163">Time the report was created.</span></span> <span data-ttu-id="e71e0-164">Formát času je RRRR-MM-ddTHH: mm: ssZ</span><span class="sxs-lookup"><span data-stu-id="e71e0-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="e71e0-165">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="e71e0-165">ModifiedTime</span></span>     |    <span data-ttu-id="e71e0-166">Čas poslední změny sestavy</span><span class="sxs-lookup"><span data-stu-id="e71e0-166">Time the report was last modified.</span></span> <span data-ttu-id="e71e0-167">Formát času je RRRR-MM-ddTHH: mm: ssZ</span><span class="sxs-lookup"><span data-stu-id="e71e0-167">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="e71e0-168">executeNow</span><span class="sxs-lookup"><span data-stu-id="e71e0-168">executeNow</span></span>     |    <span data-ttu-id="e71e0-169">Příznak ExecuteNow se nastavil v okamžiku vytvoření sestavy.</span><span class="sxs-lookup"><span data-stu-id="e71e0-169">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="e71e0-170">StartTime</span><span class="sxs-lookup"><span data-stu-id="e71e0-170">StartTime</span></span>     |    <span data-ttu-id="e71e0-171">Čas, kdy se spustí spuštění.</span><span class="sxs-lookup"><span data-stu-id="e71e0-171">Time execution will begin.</span></span> <span data-ttu-id="e71e0-172">Formát času je RRRR-MM-ddTHH: mm: ssZ</span><span class="sxs-lookup"><span data-stu-id="e71e0-172">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="e71e0-173">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="e71e0-173">ReportStatus</span></span>     |    <span data-ttu-id="e71e0-174">Stav provádění sestavy</span><span class="sxs-lookup"><span data-stu-id="e71e0-174">Status of the report execution.</span></span> <span data-ttu-id="e71e0-175">Možné hodnoty jsou pozastavené, aktivní a neaktivní.</span><span class="sxs-lookup"><span data-stu-id="e71e0-175">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="e71e0-176">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="e71e0-176">RecurrenceInterval</span></span>     |    <span data-ttu-id="e71e0-177">Interval opakování zadaný při vytváření sestavy</span><span class="sxs-lookup"><span data-stu-id="e71e0-177">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="e71e0-178">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="e71e0-178">RecurrenceCount</span></span>     |    <span data-ttu-id="e71e0-179">Počet opakování poskytnutý během vytváření sestavy</span><span class="sxs-lookup"><span data-stu-id="e71e0-179">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="e71e0-180">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="e71e0-180">CallbackUrl</span></span>     |    <span data-ttu-id="e71e0-181">Adresa URL zpětného volání poskytnutá v žádosti</span><span class="sxs-lookup"><span data-stu-id="e71e0-181">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="e71e0-182">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="e71e0-182">CallbackMethod</span></span>    |    <span data-ttu-id="e71e0-183">Metoda zpětného volání poskytnutá v žádosti</span><span class="sxs-lookup"><span data-stu-id="e71e0-183">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="e71e0-184">Formát</span><span class="sxs-lookup"><span data-stu-id="e71e0-184">Format</span></span>     |    <span data-ttu-id="e71e0-185">Formát souborů sestav</span><span class="sxs-lookup"><span data-stu-id="e71e0-185">Format of the report files</span></span>     |
|    <span data-ttu-id="e71e0-186">TotalCount</span><span class="sxs-lookup"><span data-stu-id="e71e0-186">TotalCount</span></span>     |    <span data-ttu-id="e71e0-187">Počet datových sad v poli hodnot</span><span class="sxs-lookup"><span data-stu-id="e71e0-187">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="e71e0-188">Zpráva</span><span class="sxs-lookup"><span data-stu-id="e71e0-188">Message</span></span>     |    <span data-ttu-id="e71e0-189">Stavová zpráva od spuštění rozhraní API</span><span class="sxs-lookup"><span data-stu-id="e71e0-189">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="e71e0-190">StatusCode</span><span class="sxs-lookup"><span data-stu-id="e71e0-190">StatusCode</span></span>     |    <span data-ttu-id="e71e0-191">Kód výsledku.</span><span class="sxs-lookup"><span data-stu-id="e71e0-191">Result Code.</span></span> <span data-ttu-id="e71e0-192">Možné hodnoty jsou 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="e71e0-192">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |