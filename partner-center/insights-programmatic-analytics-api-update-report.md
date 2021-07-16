---
title: Aktualizace rozhraní API pro sestavy
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Pomocí tohoto rozhraní API můžete aktualizovat parametry sestavy v Partnerské centrum přehledech.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: c5ab1059e9be9b42918d268da6a6c1a3cbfe52af
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376450"
---
# <a name="update-report-api"></a><span data-ttu-id="1a60a-103">Aktualizace rozhraní API pro sestavy</span><span class="sxs-lookup"><span data-stu-id="1a60a-103">Update report API</span></span>

<span data-ttu-id="1a60a-104">Toto rozhraní API vám pomůže upravit parametr sestavy.</span><span class="sxs-lookup"><span data-stu-id="1a60a-104">This API helps you modify a report parameter.</span></span>

<span data-ttu-id="1a60a-105">**Syntaxe požadavku**</span><span class="sxs-lookup"><span data-stu-id="1a60a-105">**Request syntax**</span></span>

|    <span data-ttu-id="1a60a-106">Metoda</span><span class="sxs-lookup"><span data-stu-id="1a60a-106">Method</span></span>    |    <span data-ttu-id="1a60a-107">Identifikátor URI žádosti</span><span class="sxs-lookup"><span data-stu-id="1a60a-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="1a60a-108">PUT</span><span class="sxs-lookup"><span data-stu-id="1a60a-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

<span data-ttu-id="1a60a-109">**Hlavička požadavku**</span><span class="sxs-lookup"><span data-stu-id="1a60a-109">**Request header**</span></span>

|    <span data-ttu-id="1a60a-110">Hlavička</span><span class="sxs-lookup"><span data-stu-id="1a60a-110">Header</span></span>    |    <span data-ttu-id="1a60a-111">Typ</span><span class="sxs-lookup"><span data-stu-id="1a60a-111">Type</span></span>    |    <span data-ttu-id="1a60a-112">Description</span><span class="sxs-lookup"><span data-stu-id="1a60a-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="1a60a-113">Autorizace</span><span class="sxs-lookup"><span data-stu-id="1a60a-113">Authorization</span></span>    |    <span data-ttu-id="1a60a-114">řetězec</span><span class="sxs-lookup"><span data-stu-id="1a60a-114">string</span></span>    |    <span data-ttu-id="1a60a-115">Povinná hodnota.</span><span class="sxs-lookup"><span data-stu-id="1a60a-115">Required.</span></span> <span data-ttu-id="1a60a-116">Přístupový Azure Active Directory (AAD) ve formuláři`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="1a60a-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="1a60a-117">Typ obsahu</span><span class="sxs-lookup"><span data-stu-id="1a60a-117">Content-Type</span></span>    |    <span data-ttu-id="1a60a-118">řetězec</span><span class="sxs-lookup"><span data-stu-id="1a60a-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="1a60a-119">**Parametr cesty**</span><span class="sxs-lookup"><span data-stu-id="1a60a-119">**Path parameter**</span></span>

|    <span data-ttu-id="1a60a-120">Název parametru</span><span class="sxs-lookup"><span data-stu-id="1a60a-120">Parameter Name</span></span>    |    <span data-ttu-id="1a60a-121">Typ</span><span class="sxs-lookup"><span data-stu-id="1a60a-121">Type</span></span>    |    <span data-ttu-id="1a60a-122">Vyžadováno</span><span class="sxs-lookup"><span data-stu-id="1a60a-122">Required</span></span>    |    <span data-ttu-id="1a60a-123">Popis</span><span class="sxs-lookup"><span data-stu-id="1a60a-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="1a60a-124">reportId</span><span class="sxs-lookup"><span data-stu-id="1a60a-124">reportId</span></span>     |    <span data-ttu-id="1a60a-125">řetězec</span><span class="sxs-lookup"><span data-stu-id="1a60a-125">string</span></span>    |    <span data-ttu-id="1a60a-126">No</span><span class="sxs-lookup"><span data-stu-id="1a60a-126">No</span></span>    |    <span data-ttu-id="1a60a-127">ID upravované sestavy</span><span class="sxs-lookup"><span data-stu-id="1a60a-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="1a60a-128">**Parametr dotazu**</span><span class="sxs-lookup"><span data-stu-id="1a60a-128">**Query parameter**</span></span>

<span data-ttu-id="1a60a-129">Žádná</span><span class="sxs-lookup"><span data-stu-id="1a60a-129">None</span></span>

<span data-ttu-id="1a60a-130">**Žádost o datovou část**</span><span class="sxs-lookup"><span data-stu-id="1a60a-130">**Request payload**</span></span>

```json
{ 
  "ReportName": "string", 
  "Description": "string", 
  "StartTime": "string", 
  "RecurrenceInterval": 0, 
  "RecurrenceCount": 0, 
  "Format": "string", 
  "CallbackUrl": "string",
 "CallbackMethod": "string"
}
```

<span data-ttu-id="1a60a-131">**Glosář**</span><span class="sxs-lookup"><span data-stu-id="1a60a-131">**Glossary**</span></span>

<span data-ttu-id="1a60a-132">Tato tabulka obsahuje seznam klíčových definic elementů v odpovědi.</span><span class="sxs-lookup"><span data-stu-id="1a60a-132">This table lists the key definitions of elements in the response.</span></span>

|    <span data-ttu-id="1a60a-133">Parametr</span><span class="sxs-lookup"><span data-stu-id="1a60a-133">Parameter</span></span>    |    <span data-ttu-id="1a60a-134">Povinné</span><span class="sxs-lookup"><span data-stu-id="1a60a-134">Required</span></span>    |    <span data-ttu-id="1a60a-135">Popis</span><span class="sxs-lookup"><span data-stu-id="1a60a-135">Description</span></span>    |    <span data-ttu-id="1a60a-136">Povolené hodnoty</span><span class="sxs-lookup"><span data-stu-id="1a60a-136">Allowed Values</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="1a60a-137">ReportName</span><span class="sxs-lookup"><span data-stu-id="1a60a-137">ReportName</span></span>     |    <span data-ttu-id="1a60a-138">Yes</span><span class="sxs-lookup"><span data-stu-id="1a60a-138">Yes</span></span>     |    <span data-ttu-id="1a60a-139">Název, který se má k sestavě přiřadit</span><span class="sxs-lookup"><span data-stu-id="1a60a-139">Name to be assigned to the report</span></span>     |    <span data-ttu-id="1a60a-140">Řetězec</span><span class="sxs-lookup"><span data-stu-id="1a60a-140">String</span></span>     |
|    <span data-ttu-id="1a60a-141">Popis</span><span class="sxs-lookup"><span data-stu-id="1a60a-141">Description</span></span>     |    <span data-ttu-id="1a60a-142">No</span><span class="sxs-lookup"><span data-stu-id="1a60a-142">No</span></span>     |    <span data-ttu-id="1a60a-143">Popis vytvořené sestavy</span><span class="sxs-lookup"><span data-stu-id="1a60a-143">Description of the created report</span></span>     |    <span data-ttu-id="1a60a-144">Řetězec</span><span class="sxs-lookup"><span data-stu-id="1a60a-144">String</span></span>     |
|    <span data-ttu-id="1a60a-145">StartTime</span><span class="sxs-lookup"><span data-stu-id="1a60a-145">StartTime</span></span>     |    <span data-ttu-id="1a60a-146">Yes</span><span class="sxs-lookup"><span data-stu-id="1a60a-146">Yes</span></span>    |    <span data-ttu-id="1a60a-147">Časové razítko, po kterém začne generování sestavy</span><span class="sxs-lookup"><span data-stu-id="1a60a-147">Timestamp after which the report generation will begin</span></span>     |    <span data-ttu-id="1a60a-148">Řetězec</span><span class="sxs-lookup"><span data-stu-id="1a60a-148">String</span></span>     |
|    <span data-ttu-id="1a60a-149">OpakováníInterval</span><span class="sxs-lookup"><span data-stu-id="1a60a-149">RecurrenceInterval</span></span>     |    <span data-ttu-id="1a60a-150">No</span><span class="sxs-lookup"><span data-stu-id="1a60a-150">No</span></span>     |    <span data-ttu-id="1a60a-151">Frekvence generování sestavy v hodinách</span><span class="sxs-lookup"><span data-stu-id="1a60a-151">Frequency at which the report should be generated in hours.</span></span> <span data-ttu-id="1a60a-152">Minimální hodnota je 4</span><span class="sxs-lookup"><span data-stu-id="1a60a-152">Minimum value is 4</span></span>     |    <span data-ttu-id="1a60a-153">Integer</span><span class="sxs-lookup"><span data-stu-id="1a60a-153">Integer</span></span>     |
|    <span data-ttu-id="1a60a-154">Počet opakování</span><span class="sxs-lookup"><span data-stu-id="1a60a-154">RecurrenceCount</span></span>     |    <span data-ttu-id="1a60a-155">No</span><span class="sxs-lookup"><span data-stu-id="1a60a-155">No</span></span>     |    <span data-ttu-id="1a60a-156">Čísla sestav, které se budou generovat</span><span class="sxs-lookup"><span data-stu-id="1a60a-156">Numbers of report to be generated.</span></span> <span data-ttu-id="1a60a-157">Výchozí hodnota je neurčitý.</span><span class="sxs-lookup"><span data-stu-id="1a60a-157">Default is indefinite.</span></span>     |    <span data-ttu-id="1a60a-158">Integer</span><span class="sxs-lookup"><span data-stu-id="1a60a-158">Integer</span></span>     |
|    <span data-ttu-id="1a60a-159">Formát</span><span class="sxs-lookup"><span data-stu-id="1a60a-159">Format</span></span>     |    <span data-ttu-id="1a60a-160">No</span><span class="sxs-lookup"><span data-stu-id="1a60a-160">No</span></span>    |    <span data-ttu-id="1a60a-161">Formát exportovaného souboru.</span><span class="sxs-lookup"><span data-stu-id="1a60a-161">File format of the exported file.</span></span> <span data-ttu-id="1a60a-162">Výchozí hodnota je CSV.</span><span class="sxs-lookup"><span data-stu-id="1a60a-162">Default is CSV</span></span>     |    <span data-ttu-id="1a60a-163">CSV/TSV</span><span class="sxs-lookup"><span data-stu-id="1a60a-163">CSV/TSV</span></span>     |
|    <span data-ttu-id="1a60a-164">CallbackURL</span><span class="sxs-lookup"><span data-stu-id="1a60a-164">CallbackURL</span></span>     |    <span data-ttu-id="1a60a-165">No</span><span class="sxs-lookup"><span data-stu-id="1a60a-165">No</span></span>     |    <span data-ttu-id="1a60a-166">Adresa URL zpětného volání https, která se má volat při generování sestav</span><span class="sxs-lookup"><span data-stu-id="1a60a-166">https callback URL to be called on report generation</span></span>     |    <span data-ttu-id="1a60a-167">Řetězec</span><span class="sxs-lookup"><span data-stu-id="1a60a-167">String</span></span>     |
|    <span data-ttu-id="1a60a-168">Metoda zpětného volání</span><span class="sxs-lookup"><span data-stu-id="1a60a-168">CallbackMethod</span></span>    |    <span data-ttu-id="1a60a-169">No</span><span class="sxs-lookup"><span data-stu-id="1a60a-169">No</span></span>    |    <span data-ttu-id="1a60a-170">Metoda HTTP, která se má použít pro zpětné volání</span><span class="sxs-lookup"><span data-stu-id="1a60a-170">Http method to be used for callback</span></span>    |    <span data-ttu-id="1a60a-171">GET/POST</span><span class="sxs-lookup"><span data-stu-id="1a60a-171">GET/POST</span></span>    |
|        |        |        |        |


<span data-ttu-id="1a60a-172">**Response** (Odpověď)</span><span class="sxs-lookup"><span data-stu-id="1a60a-172">**Response**</span></span>

<span data-ttu-id="1a60a-173">Datová část odpovědi je strukturovaná takto:</span><span class="sxs-lookup"><span data-stu-id="1a60a-173">The response payload is structured as follows:</span></span>

<span data-ttu-id="1a60a-174">Kód odpovědi: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="1a60a-174">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="1a60a-175">Příklad datové části odpovědi:</span><span class="sxs-lookup"><span data-stu-id="1a60a-175">Response payload example:</span></span>

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

<span data-ttu-id="1a60a-176">**Glosář**</span><span class="sxs-lookup"><span data-stu-id="1a60a-176">**Glossary**</span></span>

<span data-ttu-id="1a60a-177">Tato tabulka definuje klíčové prvky v odpovědi:</span><span class="sxs-lookup"><span data-stu-id="1a60a-177">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="1a60a-178">Parametr</span><span class="sxs-lookup"><span data-stu-id="1a60a-178">Parameter</span></span>    |    <span data-ttu-id="1a60a-179">Popis</span><span class="sxs-lookup"><span data-stu-id="1a60a-179">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="1a60a-180">ID sestavy</span><span class="sxs-lookup"><span data-stu-id="1a60a-180">ReportId</span></span>     |    <span data-ttu-id="1a60a-181">Univerzálně jedinečný identifikátor (UUID) aktualizované sestavy</span><span class="sxs-lookup"><span data-stu-id="1a60a-181">Universally unique identifier (UUID) of the report being updated</span></span>     |
|    <span data-ttu-id="1a60a-182">ReportName</span><span class="sxs-lookup"><span data-stu-id="1a60a-182">ReportName</span></span>     |    <span data-ttu-id="1a60a-183">Název předaný sestavě v datové části požadavku</span><span class="sxs-lookup"><span data-stu-id="1a60a-183">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="1a60a-184">Description</span><span class="sxs-lookup"><span data-stu-id="1a60a-184">Description</span></span>     |    <span data-ttu-id="1a60a-185">Popis předáný sestavě v datové části požadavku</span><span class="sxs-lookup"><span data-stu-id="1a60a-185">Description given to the report in the request payload</span></span>     |
|    <span data-ttu-id="1a60a-186">ID dotazu</span><span class="sxs-lookup"><span data-stu-id="1a60a-186">QueryId</span></span>     |    <span data-ttu-id="1a60a-187">ID dotazu předané v době vytvoření sestavy</span><span class="sxs-lookup"><span data-stu-id="1a60a-187">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="1a60a-188">Dotaz</span><span class="sxs-lookup"><span data-stu-id="1a60a-188">Query</span></span>     |    <span data-ttu-id="1a60a-189">Text dotazu, který se provede pro tuto sestavu</span><span class="sxs-lookup"><span data-stu-id="1a60a-189">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="1a60a-190">Uživatel</span><span class="sxs-lookup"><span data-stu-id="1a60a-190">User</span></span>     |    <span data-ttu-id="1a60a-191">ID uživatele použité k vytvoření sestavy</span><span class="sxs-lookup"><span data-stu-id="1a60a-191">User ID used to create the report</span></span>     |
|    <span data-ttu-id="1a60a-192">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="1a60a-192">CreatedTime</span></span>     |    <span data-ttu-id="1a60a-193">Čas vytvoření sestavy</span><span class="sxs-lookup"><span data-stu-id="1a60a-193">Time the report was created.</span></span> <span data-ttu-id="1a60a-194">Formát času je rrrr-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="1a60a-194">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="1a60a-195">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="1a60a-195">ModifiedTime</span></span>     |    <span data-ttu-id="1a60a-196">Čas poslední změny sestavy</span><span class="sxs-lookup"><span data-stu-id="1a60a-196">Time the report was last modified.</span></span> <span data-ttu-id="1a60a-197">Formát času je rrrr-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="1a60a-197">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="1a60a-198">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="1a60a-198">ExecuteNow</span></span>     |    <span data-ttu-id="1a60a-199">Příznak ExecuteNow nastavený v době vytvoření sestavy</span><span class="sxs-lookup"><span data-stu-id="1a60a-199">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="1a60a-200">StartTime</span><span class="sxs-lookup"><span data-stu-id="1a60a-200">StartTime</span></span>     |    <span data-ttu-id="1a60a-201">Čas zahájení provádění sestavy</span><span class="sxs-lookup"><span data-stu-id="1a60a-201">Time the report execution will begin.</span></span> <span data-ttu-id="1a60a-202">Formát času je rrrr-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="1a60a-202">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="1a60a-203">Stav sestavy</span><span class="sxs-lookup"><span data-stu-id="1a60a-203">ReportStatus</span></span>     |    <span data-ttu-id="1a60a-204">Stav spuštění sestavy</span><span class="sxs-lookup"><span data-stu-id="1a60a-204">Status of the report execution.</span></span> <span data-ttu-id="1a60a-205">Možné hodnoty jsou Pozastaveno, Aktivní a Neaktivní.</span><span class="sxs-lookup"><span data-stu-id="1a60a-205">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="1a60a-206">OpakováníInterval</span><span class="sxs-lookup"><span data-stu-id="1a60a-206">RecurrenceInterval</span></span>     |    <span data-ttu-id="1a60a-207">Interval opakování v datové části požadavku</span><span class="sxs-lookup"><span data-stu-id="1a60a-207">Recurrence interval provided in the request payload</span></span>     |
|    <span data-ttu-id="1a60a-208">Počet opakování</span><span class="sxs-lookup"><span data-stu-id="1a60a-208">RecurrenceCount</span></span>     |    <span data-ttu-id="1a60a-209">Počet opakování v datové části požadavku</span><span class="sxs-lookup"><span data-stu-id="1a60a-209">Recurrence count provided in the request payload</span></span>     |
|    <span data-ttu-id="1a60a-210">CallbackUrl (Url zpětného volání)</span><span class="sxs-lookup"><span data-stu-id="1a60a-210">CallbackUrl</span></span>     |    <span data-ttu-id="1a60a-211">Adresa URL zpětného volání zadaná v požadavku</span><span class="sxs-lookup"><span data-stu-id="1a60a-211">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="1a60a-212">Metoda zpětného volání</span><span class="sxs-lookup"><span data-stu-id="1a60a-212">CallbackMethod</span></span>    |    <span data-ttu-id="1a60a-213">Metoda zpětného volání poskytnutá v požadavku</span><span class="sxs-lookup"><span data-stu-id="1a60a-213">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="1a60a-214">Formát</span><span class="sxs-lookup"><span data-stu-id="1a60a-214">Format</span></span>     |    <span data-ttu-id="1a60a-215">Formát souborů sestav</span><span class="sxs-lookup"><span data-stu-id="1a60a-215">Format of the report files</span></span>     |
|    <span data-ttu-id="1a60a-216">TotalCount</span><span class="sxs-lookup"><span data-stu-id="1a60a-216">TotalCount</span></span>     |    <span data-ttu-id="1a60a-217">Počet datových sad v poli Hodnota</span><span class="sxs-lookup"><span data-stu-id="1a60a-217">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="1a60a-218">Zpráva</span><span class="sxs-lookup"><span data-stu-id="1a60a-218">Message</span></span>     |    <span data-ttu-id="1a60a-219">Stavová zpráva z spuštění rozhraní API</span><span class="sxs-lookup"><span data-stu-id="1a60a-219">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="1a60a-220">Statuscode</span><span class="sxs-lookup"><span data-stu-id="1a60a-220">StatusCode</span></span>     |    <span data-ttu-id="1a60a-221">Kód výsledku.</span><span class="sxs-lookup"><span data-stu-id="1a60a-221">Result Code.</span></span> <span data-ttu-id="1a60a-222">Možné hodnoty jsou 200, 400, 401, 403, 500.</span><span class="sxs-lookup"><span data-stu-id="1a60a-222">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |