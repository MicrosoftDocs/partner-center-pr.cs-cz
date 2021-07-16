---
title: Rozhraní API pro odstranění sestavy – Přehledy data
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Pomocí tohoto rozhraní API můžete odstranit všechny sestavy v Partnerské centrum přehledy.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e060104f8f09f69c213ab1b22d4be08d58babced
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376462"
---
# <a name="delete-report-api"></a><span data-ttu-id="2dfef-103">Rozhraní API pro odstranění sestavy</span><span class="sxs-lookup"><span data-stu-id="2dfef-103">Delete report API</span></span>

<span data-ttu-id="2dfef-104">Při spuštění toto rozhraní API odstraní všechny záznamy o spuštění sestavy a sestavy.</span><span class="sxs-lookup"><span data-stu-id="2dfef-104">On execution, this API deletes all of the report and report execution records.</span></span>

<span data-ttu-id="2dfef-105">**Syntaxe požadavku**</span><span class="sxs-lookup"><span data-stu-id="2dfef-105">**Request syntax**</span></span>

|    <span data-ttu-id="2dfef-106">Metoda</span><span class="sxs-lookup"><span data-stu-id="2dfef-106">Method</span></span>    |    <span data-ttu-id="2dfef-107">Identifikátor URI žádosti</span><span class="sxs-lookup"><span data-stu-id="2dfef-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="2dfef-108">DELETE</span><span class="sxs-lookup"><span data-stu-id="2dfef-108">DELETE</span></span>    |    ` https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

<span data-ttu-id="2dfef-109">**Hlavička požadavku**</span><span class="sxs-lookup"><span data-stu-id="2dfef-109">**Request header**</span></span>

|    <span data-ttu-id="2dfef-110">Hlavička</span><span class="sxs-lookup"><span data-stu-id="2dfef-110">Header</span></span>    |    <span data-ttu-id="2dfef-111">Typ</span><span class="sxs-lookup"><span data-stu-id="2dfef-111">Type</span></span>    |    <span data-ttu-id="2dfef-112">Description</span><span class="sxs-lookup"><span data-stu-id="2dfef-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="2dfef-113">Autorizace</span><span class="sxs-lookup"><span data-stu-id="2dfef-113">Authorization</span></span>    |    <span data-ttu-id="2dfef-114">řetězec</span><span class="sxs-lookup"><span data-stu-id="2dfef-114">string</span></span>    |    <span data-ttu-id="2dfef-115">Povinná hodnota.</span><span class="sxs-lookup"><span data-stu-id="2dfef-115">Required.</span></span> <span data-ttu-id="2dfef-116">Přístupový Azure Active Directory (AAD) ve formuláři`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="2dfef-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="2dfef-117">Typ obsahu</span><span class="sxs-lookup"><span data-stu-id="2dfef-117">Content-Type</span></span>    |    <span data-ttu-id="2dfef-118">řetězec</span><span class="sxs-lookup"><span data-stu-id="2dfef-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="2dfef-119">**Parametr cesty**</span><span class="sxs-lookup"><span data-stu-id="2dfef-119">**Path parameter**</span></span>

|    <span data-ttu-id="2dfef-120">Název parametru</span><span class="sxs-lookup"><span data-stu-id="2dfef-120">Parameter Name</span></span>    |    <span data-ttu-id="2dfef-121">Typ</span><span class="sxs-lookup"><span data-stu-id="2dfef-121">Type</span></span>    |    <span data-ttu-id="2dfef-122">Vyžadováno</span><span class="sxs-lookup"><span data-stu-id="2dfef-122">Required</span></span>    |    <span data-ttu-id="2dfef-123">Popis</span><span class="sxs-lookup"><span data-stu-id="2dfef-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="2dfef-124">reportId</span><span class="sxs-lookup"><span data-stu-id="2dfef-124">reportId</span></span>     |    <span data-ttu-id="2dfef-125">řetězec</span><span class="sxs-lookup"><span data-stu-id="2dfef-125">string</span></span>    |    <span data-ttu-id="2dfef-126">No</span><span class="sxs-lookup"><span data-stu-id="2dfef-126">No</span></span>    |    <span data-ttu-id="2dfef-127">ID odstraněné sestavy</span><span class="sxs-lookup"><span data-stu-id="2dfef-127">ID of the report being deleted</span></span>    |
|        |        |        |        |

<span data-ttu-id="2dfef-128">**Parametr dotazu**</span><span class="sxs-lookup"><span data-stu-id="2dfef-128">**Query parameter**</span></span>

<span data-ttu-id="2dfef-129">Žádná</span><span class="sxs-lookup"><span data-stu-id="2dfef-129">None</span></span>

<span data-ttu-id="2dfef-130">**Žádost o datovou část**</span><span class="sxs-lookup"><span data-stu-id="2dfef-130">**Request payload**</span></span>

<span data-ttu-id="2dfef-131">Žádná</span><span class="sxs-lookup"><span data-stu-id="2dfef-131">None</span></span>

<span data-ttu-id="2dfef-132">**Glosář**</span><span class="sxs-lookup"><span data-stu-id="2dfef-132">**Glossary**</span></span>

<span data-ttu-id="2dfef-133">Žádná</span><span class="sxs-lookup"><span data-stu-id="2dfef-133">None</span></span>

<span data-ttu-id="2dfef-134">**Response** (Odpověď)</span><span class="sxs-lookup"><span data-stu-id="2dfef-134">**Response**</span></span>

<span data-ttu-id="2dfef-135">Datová část odpovědi je strukturovaná takto:</span><span class="sxs-lookup"><span data-stu-id="2dfef-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="2dfef-136">Kód odpovědi: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="2dfef-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="2dfef-137">Příklad datové části odpovědi:</span><span class="sxs-lookup"><span data-stu-id="2dfef-137">Response payload example:</span></span>

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

<span data-ttu-id="2dfef-138">**Glosář**</span><span class="sxs-lookup"><span data-stu-id="2dfef-138">**Glossary**</span></span>

<span data-ttu-id="2dfef-139">Tato tabulka definuje klíčové prvky v odpovědi:</span><span class="sxs-lookup"><span data-stu-id="2dfef-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="2dfef-140">Parametr</span><span class="sxs-lookup"><span data-stu-id="2dfef-140">Parameter</span></span>    |    <span data-ttu-id="2dfef-141">Popis</span><span class="sxs-lookup"><span data-stu-id="2dfef-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="2dfef-142">ID sestavy</span><span class="sxs-lookup"><span data-stu-id="2dfef-142">ReportId</span></span>     |    <span data-ttu-id="2dfef-143">Univerzálně jedinečný identifikátor (UUID) odstraněné sestavy</span><span class="sxs-lookup"><span data-stu-id="2dfef-143">Universally unique identifier (UUID) of the deleted report</span></span>     |
|    <span data-ttu-id="2dfef-144">ReportName</span><span class="sxs-lookup"><span data-stu-id="2dfef-144">ReportName</span></span>     |    <span data-ttu-id="2dfef-145">Název přidán sestavě během vytváření</span><span class="sxs-lookup"><span data-stu-id="2dfef-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="2dfef-146">Description</span><span class="sxs-lookup"><span data-stu-id="2dfef-146">Description</span></span>     |    <span data-ttu-id="2dfef-147">Popis při vytváření sestavy</span><span class="sxs-lookup"><span data-stu-id="2dfef-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="2dfef-148">ID dotazu</span><span class="sxs-lookup"><span data-stu-id="2dfef-148">QueryId</span></span>     |    <span data-ttu-id="2dfef-149">ID dotazu předané v době vytvoření sestavy</span><span class="sxs-lookup"><span data-stu-id="2dfef-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="2dfef-150">Dotaz</span><span class="sxs-lookup"><span data-stu-id="2dfef-150">Query</span></span>     |    <span data-ttu-id="2dfef-151">Text dotazu, který se provede pro tuto sestavu</span><span class="sxs-lookup"><span data-stu-id="2dfef-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="2dfef-152">Uživatel</span><span class="sxs-lookup"><span data-stu-id="2dfef-152">User</span></span>     |    <span data-ttu-id="2dfef-153">ID uživatele použité k vytvoření sestavy</span><span class="sxs-lookup"><span data-stu-id="2dfef-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="2dfef-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="2dfef-154">CreatedTime</span></span>     |    <span data-ttu-id="2dfef-155">Čas vytvoření sestavy</span><span class="sxs-lookup"><span data-stu-id="2dfef-155">Time the report was created.</span></span> <span data-ttu-id="2dfef-156">Formát času je rrrr-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="2dfef-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="2dfef-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="2dfef-157">ModifiedTime</span></span>     |    <span data-ttu-id="2dfef-158">Čas poslední změny sestavy</span><span class="sxs-lookup"><span data-stu-id="2dfef-158">Time the report was last modified.</span></span> <span data-ttu-id="2dfef-159">Formát času je rrrr-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="2dfef-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="2dfef-160">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="2dfef-160">ExecuteNow</span></span>     |    <span data-ttu-id="2dfef-161">Příznak ExecuteNow nastavený v době vytvoření sestavy</span><span class="sxs-lookup"><span data-stu-id="2dfef-161">ExecuteNow flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="2dfef-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="2dfef-162">StartTime</span></span>     |    <span data-ttu-id="2dfef-163">Čas zahájení provádění sestavy</span><span class="sxs-lookup"><span data-stu-id="2dfef-163">Time the report execution will begin.</span></span> <span data-ttu-id="2dfef-164">Formát času je rrrr-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="2dfef-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="2dfef-165">Stav sestavy</span><span class="sxs-lookup"><span data-stu-id="2dfef-165">ReportStatus</span></span>     |    <span data-ttu-id="2dfef-166">Stav spuštění sestavy</span><span class="sxs-lookup"><span data-stu-id="2dfef-166">Status of the report execution.</span></span> <span data-ttu-id="2dfef-167">Možné hodnoty jsou Pozastaveno, Aktivní a Neaktivní.</span><span class="sxs-lookup"><span data-stu-id="2dfef-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="2dfef-168">OpakováníInterval</span><span class="sxs-lookup"><span data-stu-id="2dfef-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="2dfef-169">Interval opakování poskytovaný během vytváření sestavy</span><span class="sxs-lookup"><span data-stu-id="2dfef-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="2dfef-170">Počet opakování</span><span class="sxs-lookup"><span data-stu-id="2dfef-170">RecurrenceCount</span></span>     |    <span data-ttu-id="2dfef-171">Počet opakování při vytváření sestavy</span><span class="sxs-lookup"><span data-stu-id="2dfef-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="2dfef-172">CallbackUrl (Url zpětného volání)</span><span class="sxs-lookup"><span data-stu-id="2dfef-172">CallbackUrl</span></span>     |    <span data-ttu-id="2dfef-173">Adresa URL zpětného volání zadaná v požadavku</span><span class="sxs-lookup"><span data-stu-id="2dfef-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="2dfef-174">Metoda zpětného volání</span><span class="sxs-lookup"><span data-stu-id="2dfef-174">CallbackMethod</span></span>    |    <span data-ttu-id="2dfef-175">Metoda zpětného volání poskytnutá v požadavku</span><span class="sxs-lookup"><span data-stu-id="2dfef-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="2dfef-176">Formát</span><span class="sxs-lookup"><span data-stu-id="2dfef-176">Format</span></span>     |    <span data-ttu-id="2dfef-177">Formát souborů sestav</span><span class="sxs-lookup"><span data-stu-id="2dfef-177">Format of the report files</span></span>     |
|    <span data-ttu-id="2dfef-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="2dfef-178">TotalCount</span></span>     |    <span data-ttu-id="2dfef-179">Počet datových sad v poli Hodnota</span><span class="sxs-lookup"><span data-stu-id="2dfef-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="2dfef-180">Zpráva</span><span class="sxs-lookup"><span data-stu-id="2dfef-180">Message</span></span>     |    <span data-ttu-id="2dfef-181">Stavová zpráva z spuštění rozhraní API</span><span class="sxs-lookup"><span data-stu-id="2dfef-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="2dfef-182">Statuscode</span><span class="sxs-lookup"><span data-stu-id="2dfef-182">StatusCode</span></span>     |    <span data-ttu-id="2dfef-183">Kód výsledku.</span><span class="sxs-lookup"><span data-stu-id="2dfef-183">Result Code.</span></span> <span data-ttu-id="2dfef-184">Možné hodnoty jsou 200, 400, 401, 403, 500.</span><span class="sxs-lookup"><span data-stu-id="2dfef-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
