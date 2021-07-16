---
title: získat dotazy na sestavu API – Přehledy data
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Pomocí tohoto rozhraní API můžete získat všechny dostupné dotazy pro použití v rozhraní API pro sestavy.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 3bf140576a19439990405cfef23190045e0a98be
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376459"
---
# <a name="get-report-queries-api"></a><span data-ttu-id="5e456-103">Získat rozhraní API pro dotazy sestav</span><span class="sxs-lookup"><span data-stu-id="5e456-103">Get report queries API</span></span>

<span data-ttu-id="5e456-104">Rozhraní API pro dotazy Get Report získá všechny dotazy, které jsou k dispozici pro použití v sestavách.</span><span class="sxs-lookup"><span data-stu-id="5e456-104">The Get report queries API gets all the queries that are available for use in reports.</span></span> <span data-ttu-id="5e456-105">Ve výchozím nastavení získá všechny dotazy definované systémem a uživatelem.</span><span class="sxs-lookup"><span data-stu-id="5e456-105">It gets all the system and user-defined queries by default.</span></span>

<span data-ttu-id="5e456-106">**Syntaxe žádosti**</span><span class="sxs-lookup"><span data-stu-id="5e456-106">**Request syntax**</span></span>

|    <span data-ttu-id="5e456-107">Metoda</span><span class="sxs-lookup"><span data-stu-id="5e456-107">Method</span></span>    |    <span data-ttu-id="5e456-108">Identifikátor URI žádosti</span><span class="sxs-lookup"><span data-stu-id="5e456-108">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="5e456-109">GET</span><span class="sxs-lookup"><span data-stu-id="5e456-109">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
|        |        |

<span data-ttu-id="5e456-110">**Hlavička žádosti**</span><span class="sxs-lookup"><span data-stu-id="5e456-110">**Request header**</span></span>

|    <span data-ttu-id="5e456-111">Hlavička</span><span class="sxs-lookup"><span data-stu-id="5e456-111">Header</span></span>    |    <span data-ttu-id="5e456-112">Typ</span><span class="sxs-lookup"><span data-stu-id="5e456-112">Type</span></span>    |    <span data-ttu-id="5e456-113">Description</span><span class="sxs-lookup"><span data-stu-id="5e456-113">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="5e456-114">Autorizace</span><span class="sxs-lookup"><span data-stu-id="5e456-114">Authorization</span></span>    |    <span data-ttu-id="5e456-115">řetězec</span><span class="sxs-lookup"><span data-stu-id="5e456-115">string</span></span>    |    <span data-ttu-id="5e456-116">Povinná hodnota.</span><span class="sxs-lookup"><span data-stu-id="5e456-116">Required.</span></span> <span data-ttu-id="5e456-117">přístupový token pro Azure Active Directory (AAD) ve formuláři`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="5e456-117">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="5e456-118">Typ obsahu</span><span class="sxs-lookup"><span data-stu-id="5e456-118">Content-Type</span></span>    |    <span data-ttu-id="5e456-119">řetězec</span><span class="sxs-lookup"><span data-stu-id="5e456-119">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="5e456-120">**Parametr cesty**</span><span class="sxs-lookup"><span data-stu-id="5e456-120">**Path parameter**</span></span>

<span data-ttu-id="5e456-121">Žádná</span><span class="sxs-lookup"><span data-stu-id="5e456-121">None</span></span>

<span data-ttu-id="5e456-122">**Parametr dotazu**</span><span class="sxs-lookup"><span data-stu-id="5e456-122">**Query parameter**</span></span>

|    <span data-ttu-id="5e456-123">Název parametru</span><span class="sxs-lookup"><span data-stu-id="5e456-123">Parameter Name</span></span>    |    <span data-ttu-id="5e456-124">Typ</span><span class="sxs-lookup"><span data-stu-id="5e456-124">Type</span></span>    |    <span data-ttu-id="5e456-125">Vyžadováno</span><span class="sxs-lookup"><span data-stu-id="5e456-125">Required</span></span>    |    <span data-ttu-id="5e456-126">Popis</span><span class="sxs-lookup"><span data-stu-id="5e456-126">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="5e456-127">queryId</span><span class="sxs-lookup"><span data-stu-id="5e456-127">queryId</span></span>     |    <span data-ttu-id="5e456-128">řetězec</span><span class="sxs-lookup"><span data-stu-id="5e456-128">string</span></span>     |    <span data-ttu-id="5e456-129">No</span><span class="sxs-lookup"><span data-stu-id="5e456-129">No</span></span>    |    <span data-ttu-id="5e456-130">Filtr pro získání podrobností o dotazech s ID uvedeným v argumentu</span><span class="sxs-lookup"><span data-stu-id="5e456-130">Filter to get details of only queries with the ID given in the argument</span></span>     |
|    <span data-ttu-id="5e456-131">queryName</span><span class="sxs-lookup"><span data-stu-id="5e456-131">queryName</span></span>     |    <span data-ttu-id="5e456-132">řetězec</span><span class="sxs-lookup"><span data-stu-id="5e456-132">string</span></span>     |    <span data-ttu-id="5e456-133">No</span><span class="sxs-lookup"><span data-stu-id="5e456-133">No</span></span>    |    <span data-ttu-id="5e456-134">Filtr, který získá podrobné informace o dotazech s názvem zadaným v argumentu</span><span class="sxs-lookup"><span data-stu-id="5e456-134">Filter to get details of only queries with the name given in the argument</span></span>     |
|    <span data-ttu-id="5e456-135">IncludeSystemQueries</span><span class="sxs-lookup"><span data-stu-id="5e456-135">IncludeSystemQueries</span></span>     |    <span data-ttu-id="5e456-136">boolean</span><span class="sxs-lookup"><span data-stu-id="5e456-136">boolean</span></span>     |    <span data-ttu-id="5e456-137">No</span><span class="sxs-lookup"><span data-stu-id="5e456-137">No</span></span>    |    <span data-ttu-id="5e456-138">Zahrnout předdefinované systémové dotazy do odpovědi</span><span class="sxs-lookup"><span data-stu-id="5e456-138">Include predefined system queries in the response</span></span>     |
|    <span data-ttu-id="5e456-139">IncludeOnlySystemQueries</span><span class="sxs-lookup"><span data-stu-id="5e456-139">IncludeOnlySystemQueries</span></span>     |    <span data-ttu-id="5e456-140">boolean</span><span class="sxs-lookup"><span data-stu-id="5e456-140">boolean</span></span>     |    <span data-ttu-id="5e456-141">No</span><span class="sxs-lookup"><span data-stu-id="5e456-141">No</span></span>    |    <span data-ttu-id="5e456-142">Zahrnout do odpovědi pouze systémové dotazy</span><span class="sxs-lookup"><span data-stu-id="5e456-142">Include only system queries in the response</span></span>     |
|        |        |        |        |


<span data-ttu-id="5e456-143">**Datová část požadavku**</span><span class="sxs-lookup"><span data-stu-id="5e456-143">**Request payload**</span></span>

<span data-ttu-id="5e456-144">Žádná</span><span class="sxs-lookup"><span data-stu-id="5e456-144">None</span></span>

<span data-ttu-id="5e456-145">**Glosář**</span><span class="sxs-lookup"><span data-stu-id="5e456-145">**Glossary**</span></span>

<span data-ttu-id="5e456-146">Žádná</span><span class="sxs-lookup"><span data-stu-id="5e456-146">None</span></span>

<span data-ttu-id="5e456-147">**Response** (Odpověď)</span><span class="sxs-lookup"><span data-stu-id="5e456-147">**Response**</span></span>

<span data-ttu-id="5e456-148">Datová část odpovědi je strukturována takto:</span><span class="sxs-lookup"><span data-stu-id="5e456-148">The response payload is structured as follows:</span></span>

<span data-ttu-id="5e456-149">Kód odpovědi: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="5e456-149">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="5e456-150">Příklad datové části odpovědi:</span><span class="sxs-lookup"><span data-stu-id="5e456-150">Response payload example:</span></span>

```json
{ 
  "Value": [ 
    { 
      "QueryId": "string", 
      "Name": "string", 
      "Description": "string", 
      "Query": "string", 
      "Type": "string", 
      "User": "string", 
      "CreatedTime": "string", 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="5e456-151">**Glosář**</span><span class="sxs-lookup"><span data-stu-id="5e456-151">**Glossary**</span></span>

<span data-ttu-id="5e456-152">Tato tabulka definuje klíčové prvky v odpovědi:</span><span class="sxs-lookup"><span data-stu-id="5e456-152">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="5e456-153">Parametr</span><span class="sxs-lookup"><span data-stu-id="5e456-153">Parameter</span></span>    |    <span data-ttu-id="5e456-154">Popis</span><span class="sxs-lookup"><span data-stu-id="5e456-154">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="5e456-155">QueryId</span><span class="sxs-lookup"><span data-stu-id="5e456-155">QueryId</span></span>     |    <span data-ttu-id="5e456-156">Jedinečný identifikátor UUID dotazu</span><span class="sxs-lookup"><span data-stu-id="5e456-156">Unique UUID of the query</span></span>     |
|    <span data-ttu-id="5e456-157">Name</span><span class="sxs-lookup"><span data-stu-id="5e456-157">Name</span></span>     |    <span data-ttu-id="5e456-158">Název zadaný pro dotaz v době vytváření dotazu</span><span class="sxs-lookup"><span data-stu-id="5e456-158">Name given to the query at the time of query creation</span></span>     |
|    <span data-ttu-id="5e456-159">Description</span><span class="sxs-lookup"><span data-stu-id="5e456-159">Description</span></span>     |    <span data-ttu-id="5e456-160">Popis zadaný při vytváření dotazu</span><span class="sxs-lookup"><span data-stu-id="5e456-160">Description given during creation of the query</span></span>     |
|    <span data-ttu-id="5e456-161">Dotaz</span><span class="sxs-lookup"><span data-stu-id="5e456-161">Query</span></span>     |    <span data-ttu-id="5e456-162">Řetězec dotazu sestavy</span><span class="sxs-lookup"><span data-stu-id="5e456-162">Report query string</span></span>     |
|    <span data-ttu-id="5e456-163">Typ</span><span class="sxs-lookup"><span data-stu-id="5e456-163">Type</span></span>     |    <span data-ttu-id="5e456-164">Nastavte na Definovánouživatelem pro uživatelem vytvořené dotazy a systém pro předdefinované systémové dotazy.</span><span class="sxs-lookup"><span data-stu-id="5e456-164">Set to userDefined for user created queries and system for predefined system queries</span></span>     |
|    <span data-ttu-id="5e456-165">Uživatel</span><span class="sxs-lookup"><span data-stu-id="5e456-165">User</span></span>     |    <span data-ttu-id="5e456-166">ID uživatele, který vytvořil dotaz</span><span class="sxs-lookup"><span data-stu-id="5e456-166">User ID who created the query</span></span>     |
|    <span data-ttu-id="5e456-167">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="5e456-167">CreatedTime</span></span>     |    <span data-ttu-id="5e456-168">Čas vytvoření dotazu</span><span class="sxs-lookup"><span data-stu-id="5e456-168">Time of creation of query</span></span>     |
|    <span data-ttu-id="5e456-169">TotalCount</span><span class="sxs-lookup"><span data-stu-id="5e456-169">TotalCount</span></span>     |    <span data-ttu-id="5e456-170">Počet datových sad v poli hodnot</span><span class="sxs-lookup"><span data-stu-id="5e456-170">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="5e456-171">Zpráva</span><span class="sxs-lookup"><span data-stu-id="5e456-171">Message</span></span>     |    <span data-ttu-id="5e456-172">Stavová zpráva od spuštění rozhraní API</span><span class="sxs-lookup"><span data-stu-id="5e456-172">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="5e456-173">StatusCode</span><span class="sxs-lookup"><span data-stu-id="5e456-173">StatusCode</span></span>     |    <span data-ttu-id="5e456-174">Kód výsledku.</span><span class="sxs-lookup"><span data-stu-id="5e456-174">Result Code.</span></span> <span data-ttu-id="5e456-175">Možné hodnoty jsou 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="5e456-175">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
