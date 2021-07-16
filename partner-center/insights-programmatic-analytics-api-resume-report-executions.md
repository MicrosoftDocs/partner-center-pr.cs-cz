---
title: obnovit rozhraní API pro spouštění sestav – Přehledy dat
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Pomocí tohoto rozhraní API můžete pokračovat v provádění všech pozastavených sestav ve službě partner Center – přehledy.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 1372823425f3aefd025ffc3441623c1ceee34e1e
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376455"
---
# <a name="resume-report-executions-api"></a><span data-ttu-id="cc26f-103">Obnovit rozhraní API pro spouštění sestav</span><span class="sxs-lookup"><span data-stu-id="cc26f-103">Resume report executions API</span></span>

<span data-ttu-id="cc26f-104">Po spuštění toto rozhraní API obnoví plánované provádění pozastavené sestavy.</span><span class="sxs-lookup"><span data-stu-id="cc26f-104">On execution, this API resumes the scheduled execution of a paused report.</span></span>

<span data-ttu-id="cc26f-105">**Syntaxe žádosti**</span><span class="sxs-lookup"><span data-stu-id="cc26f-105">**Request syntax**</span></span>

|    <span data-ttu-id="cc26f-106">Metoda</span><span class="sxs-lookup"><span data-stu-id="cc26f-106">Method</span></span>    |    <span data-ttu-id="cc26f-107">Identifikátor URI žádosti</span><span class="sxs-lookup"><span data-stu-id="cc26f-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="cc26f-108">PUT</span><span class="sxs-lookup"><span data-stu-id="cc26f-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/resume/{ReportID}`    |
|        |        |

<span data-ttu-id="cc26f-109">**Hlavička žádosti**</span><span class="sxs-lookup"><span data-stu-id="cc26f-109">**Request header**</span></span>

|    <span data-ttu-id="cc26f-110">Hlavička</span><span class="sxs-lookup"><span data-stu-id="cc26f-110">Header</span></span>    |    <span data-ttu-id="cc26f-111">Typ</span><span class="sxs-lookup"><span data-stu-id="cc26f-111">Type</span></span>    |    <span data-ttu-id="cc26f-112">Description</span><span class="sxs-lookup"><span data-stu-id="cc26f-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="cc26f-113">Autorizace</span><span class="sxs-lookup"><span data-stu-id="cc26f-113">Authorization</span></span>    |    <span data-ttu-id="cc26f-114">řetězec</span><span class="sxs-lookup"><span data-stu-id="cc26f-114">string</span></span>    |    <span data-ttu-id="cc26f-115">Povinná hodnota.</span><span class="sxs-lookup"><span data-stu-id="cc26f-115">Required.</span></span> <span data-ttu-id="cc26f-116">přístupový token pro Azure Active Directory (AAD) ve formuláři`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="cc26f-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="cc26f-117">Typ obsahu</span><span class="sxs-lookup"><span data-stu-id="cc26f-117">Content-Type</span></span>    |    <span data-ttu-id="cc26f-118">řetězec</span><span class="sxs-lookup"><span data-stu-id="cc26f-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="cc26f-119">**Parametr cesty**</span><span class="sxs-lookup"><span data-stu-id="cc26f-119">**Path parameter**</span></span>

|    <span data-ttu-id="cc26f-120">Název parametru</span><span class="sxs-lookup"><span data-stu-id="cc26f-120">Parameter Name</span></span>    |    <span data-ttu-id="cc26f-121">Typ</span><span class="sxs-lookup"><span data-stu-id="cc26f-121">Type</span></span>    |    <span data-ttu-id="cc26f-122">Vyžadováno</span><span class="sxs-lookup"><span data-stu-id="cc26f-122">Required</span></span>    |    <span data-ttu-id="cc26f-123">Popis</span><span class="sxs-lookup"><span data-stu-id="cc26f-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="cc26f-124">reportId</span><span class="sxs-lookup"><span data-stu-id="cc26f-124">reportId</span></span>     |    <span data-ttu-id="cc26f-125">řetězec</span><span class="sxs-lookup"><span data-stu-id="cc26f-125">string</span></span>    |    <span data-ttu-id="cc26f-126">No</span><span class="sxs-lookup"><span data-stu-id="cc26f-126">No</span></span>    |    <span data-ttu-id="cc26f-127">ID upravované sestavy</span><span class="sxs-lookup"><span data-stu-id="cc26f-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="cc26f-128">**Parametr dotazu**</span><span class="sxs-lookup"><span data-stu-id="cc26f-128">**Query parameter**</span></span>

<span data-ttu-id="cc26f-129">Žádná</span><span class="sxs-lookup"><span data-stu-id="cc26f-129">None</span></span>

<span data-ttu-id="cc26f-130">**Datová část požadavku**</span><span class="sxs-lookup"><span data-stu-id="cc26f-130">**Request payload**</span></span>

<span data-ttu-id="cc26f-131">Žádná</span><span class="sxs-lookup"><span data-stu-id="cc26f-131">None</span></span>

<span data-ttu-id="cc26f-132">**Glosář**</span><span class="sxs-lookup"><span data-stu-id="cc26f-132">**Glossary**</span></span>

<span data-ttu-id="cc26f-133">Žádná</span><span class="sxs-lookup"><span data-stu-id="cc26f-133">None</span></span>

<span data-ttu-id="cc26f-134">**Response** (Odpověď)</span><span class="sxs-lookup"><span data-stu-id="cc26f-134">**Response**</span></span>

<span data-ttu-id="cc26f-135">Datová část odpovědi je strukturována takto:</span><span class="sxs-lookup"><span data-stu-id="cc26f-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="cc26f-136">Kód odpovědi: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="cc26f-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="cc26f-137">Příklad datové části odpovědi:</span><span class="sxs-lookup"><span data-stu-id="cc26f-137">Response payload example:</span></span>

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

<span data-ttu-id="cc26f-138">**Glosář**</span><span class="sxs-lookup"><span data-stu-id="cc26f-138">**Glossary**</span></span>

<span data-ttu-id="cc26f-139">Tato tabulka definuje klíčové prvky v odpovědi:</span><span class="sxs-lookup"><span data-stu-id="cc26f-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="cc26f-140">Parametr</span><span class="sxs-lookup"><span data-stu-id="cc26f-140">Parameter</span></span>    |    <span data-ttu-id="cc26f-141">Popis</span><span class="sxs-lookup"><span data-stu-id="cc26f-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="cc26f-142">ReportId</span><span class="sxs-lookup"><span data-stu-id="cc26f-142">ReportId</span></span>     |    <span data-ttu-id="cc26f-143">Univerzálně jedinečný identifikátor (UUID) obnovené sestavy</span><span class="sxs-lookup"><span data-stu-id="cc26f-143">Universally unique identifier (UUID) of the resumed report</span></span>     |
|    <span data-ttu-id="cc26f-144">ReportName</span><span class="sxs-lookup"><span data-stu-id="cc26f-144">ReportName</span></span>     |    <span data-ttu-id="cc26f-145">Název zadaný pro sestavu během vytváření</span><span class="sxs-lookup"><span data-stu-id="cc26f-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="cc26f-146">Description</span><span class="sxs-lookup"><span data-stu-id="cc26f-146">Description</span></span>     |    <span data-ttu-id="cc26f-147">Popis zadaný při vytváření sestavy</span><span class="sxs-lookup"><span data-stu-id="cc26f-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="cc26f-148">QueryId</span><span class="sxs-lookup"><span data-stu-id="cc26f-148">QueryId</span></span>     |    <span data-ttu-id="cc26f-149">ID dotazu předané v okamžiku vytvoření sestavy</span><span class="sxs-lookup"><span data-stu-id="cc26f-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="cc26f-150">Dotaz</span><span class="sxs-lookup"><span data-stu-id="cc26f-150">Query</span></span>     |    <span data-ttu-id="cc26f-151">Text dotazu, který se spustí pro tuto sestavu</span><span class="sxs-lookup"><span data-stu-id="cc26f-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="cc26f-152">Uživatel</span><span class="sxs-lookup"><span data-stu-id="cc26f-152">User</span></span>     |    <span data-ttu-id="cc26f-153">ID uživatele, které se použilo k vytvoření sestavy</span><span class="sxs-lookup"><span data-stu-id="cc26f-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="cc26f-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="cc26f-154">CreatedTime</span></span>     |    <span data-ttu-id="cc26f-155">Čas, kdy byla sestava vytvořena.</span><span class="sxs-lookup"><span data-stu-id="cc26f-155">Time the report was created.</span></span> <span data-ttu-id="cc26f-156">Formát času je RRRR-MM-ddTHH: mm: ssZ</span><span class="sxs-lookup"><span data-stu-id="cc26f-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="cc26f-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="cc26f-157">ModifiedTime</span></span>     |    <span data-ttu-id="cc26f-158">Čas poslední změny sestavy</span><span class="sxs-lookup"><span data-stu-id="cc26f-158">Time the report was last modified.</span></span> <span data-ttu-id="cc26f-159">Formát času je RRRR-MM-ddTHH: mm: ssZ</span><span class="sxs-lookup"><span data-stu-id="cc26f-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="cc26f-160">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="cc26f-160">ExecuteNow</span></span>     |    <span data-ttu-id="cc26f-161">Příznak ExecuteNow se nastavil v okamžiku vytvoření sestavy.</span><span class="sxs-lookup"><span data-stu-id="cc26f-161">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="cc26f-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="cc26f-162">StartTime</span></span>     |    <span data-ttu-id="cc26f-163">Čas, kdy se spustí spuštění sestavy.</span><span class="sxs-lookup"><span data-stu-id="cc26f-163">Time the report execution will begin.</span></span> <span data-ttu-id="cc26f-164">Formát času je RRRR-MM-ddTHH: mm: ssZ</span><span class="sxs-lookup"><span data-stu-id="cc26f-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="cc26f-165">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="cc26f-165">ReportStatus</span></span>     |    <span data-ttu-id="cc26f-166">Stav provádění sestavy</span><span class="sxs-lookup"><span data-stu-id="cc26f-166">Status of the report execution.</span></span> <span data-ttu-id="cc26f-167">Možné hodnoty jsou pozastavené, aktivní a neaktivní.</span><span class="sxs-lookup"><span data-stu-id="cc26f-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="cc26f-168">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="cc26f-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="cc26f-169">Interval opakování zadaný při vytváření sestavy</span><span class="sxs-lookup"><span data-stu-id="cc26f-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="cc26f-170">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="cc26f-170">RecurrenceCount</span></span>     |    <span data-ttu-id="cc26f-171">Počet opakování poskytnutý během vytváření sestavy</span><span class="sxs-lookup"><span data-stu-id="cc26f-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="cc26f-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="cc26f-172">CallbackUrl</span></span>     |    <span data-ttu-id="cc26f-173">Adresa URL zpětného volání poskytnutá v žádosti</span><span class="sxs-lookup"><span data-stu-id="cc26f-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="cc26f-174">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="cc26f-174">CallbackMethod</span></span>    |    <span data-ttu-id="cc26f-175">Metoda zpětného volání poskytnutá v žádosti</span><span class="sxs-lookup"><span data-stu-id="cc26f-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="cc26f-176">Formát</span><span class="sxs-lookup"><span data-stu-id="cc26f-176">Format</span></span>     |    <span data-ttu-id="cc26f-177">Formát souborů sestav</span><span class="sxs-lookup"><span data-stu-id="cc26f-177">Format of the report files</span></span>     |
|    <span data-ttu-id="cc26f-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="cc26f-178">TotalCount</span></span>     |    <span data-ttu-id="cc26f-179">Počet datových sad v poli hodnot</span><span class="sxs-lookup"><span data-stu-id="cc26f-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="cc26f-180">Zpráva</span><span class="sxs-lookup"><span data-stu-id="cc26f-180">Message</span></span>     |    <span data-ttu-id="cc26f-181">Stavová zpráva od spuštění rozhraní API</span><span class="sxs-lookup"><span data-stu-id="cc26f-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="cc26f-182">StatusCode</span><span class="sxs-lookup"><span data-stu-id="cc26f-182">StatusCode</span></span>     |    <span data-ttu-id="cc26f-183">Kód výsledku.</span><span class="sxs-lookup"><span data-stu-id="cc26f-183">Result Code.</span></span> <span data-ttu-id="cc26f-184">Možné hodnoty jsou 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="cc26f-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
