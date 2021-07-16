---
title: odstranit rozhraní API pro dotazy sestav – Přehledyá data
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Pomocí tohoto rozhraní API můžete odstranit dotaz definovaný uživatelem v centru pro partnery – přehled.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e608068613edad1fca277ba5886c9c4bc962ffd2
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376392"
---
# <a name="delete-report-queries-api"></a><span data-ttu-id="6a344-103">Odstranit rozhraní API pro dotazy sestav</span><span class="sxs-lookup"><span data-stu-id="6a344-103">Delete report queries API</span></span>

<span data-ttu-id="6a344-104">Toto rozhraní API odstraní uživatelsky definované dotazy.</span><span class="sxs-lookup"><span data-stu-id="6a344-104">This API deletes user-defined queries.</span></span>

<span data-ttu-id="6a344-105">**Syntaxe žádosti**</span><span class="sxs-lookup"><span data-stu-id="6a344-105">**Request syntax**</span></span>

|    <span data-ttu-id="6a344-106">Metoda</span><span class="sxs-lookup"><span data-stu-id="6a344-106">Method</span></span>    |    <span data-ttu-id="6a344-107">Identifikátor URI žádosti</span><span class="sxs-lookup"><span data-stu-id="6a344-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="6a344-108">DELETE</span><span class="sxs-lookup"><span data-stu-id="6a344-108">DELETE</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
|        |        |

<span data-ttu-id="6a344-109">**Hlavička žádosti**</span><span class="sxs-lookup"><span data-stu-id="6a344-109">**Request header**</span></span>

|    <span data-ttu-id="6a344-110">Hlavička</span><span class="sxs-lookup"><span data-stu-id="6a344-110">Header</span></span>    |    <span data-ttu-id="6a344-111">Typ</span><span class="sxs-lookup"><span data-stu-id="6a344-111">Type</span></span>    |    <span data-ttu-id="6a344-112">Description</span><span class="sxs-lookup"><span data-stu-id="6a344-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="6a344-113">Autorizace</span><span class="sxs-lookup"><span data-stu-id="6a344-113">Authorization</span></span>    |    <span data-ttu-id="6a344-114">řetězec</span><span class="sxs-lookup"><span data-stu-id="6a344-114">string</span></span>    |    <span data-ttu-id="6a344-115">Povinná hodnota.</span><span class="sxs-lookup"><span data-stu-id="6a344-115">Required.</span></span> <span data-ttu-id="6a344-116">přístupový token pro Azure Active Directory (AAD) ve formuláři`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="6a344-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="6a344-117">Typ obsahu</span><span class="sxs-lookup"><span data-stu-id="6a344-117">Content-Type</span></span>    |    <span data-ttu-id="6a344-118">řetězec</span><span class="sxs-lookup"><span data-stu-id="6a344-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="6a344-119">**Parametr cesty**</span><span class="sxs-lookup"><span data-stu-id="6a344-119">**Path parameter**</span></span>

|    <span data-ttu-id="6a344-120">Název parametru</span><span class="sxs-lookup"><span data-stu-id="6a344-120">Parameter Name</span></span>    |    <span data-ttu-id="6a344-121">Typ</span><span class="sxs-lookup"><span data-stu-id="6a344-121">Type</span></span>    |    <span data-ttu-id="6a344-122">Vyžadováno</span><span class="sxs-lookup"><span data-stu-id="6a344-122">Required</span></span>    |    <span data-ttu-id="6a344-123">Popis</span><span class="sxs-lookup"><span data-stu-id="6a344-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="6a344-124">queryId</span><span class="sxs-lookup"><span data-stu-id="6a344-124">queryId</span></span>     |    <span data-ttu-id="6a344-125">řetězec</span><span class="sxs-lookup"><span data-stu-id="6a344-125">string</span></span>     |    <span data-ttu-id="6a344-126">No</span><span class="sxs-lookup"><span data-stu-id="6a344-126">No</span></span>    |    <span data-ttu-id="6a344-127">Filtr pro získání podrobností o dotazech s ID uvedeným v argumentu</span><span class="sxs-lookup"><span data-stu-id="6a344-127">Filter to get details of only queries with the ID given in the argument</span></span>     |
|        |        |        |        |

<span data-ttu-id="6a344-128">**Parametr dotazu**</span><span class="sxs-lookup"><span data-stu-id="6a344-128">**Query parameter**</span></span>

<span data-ttu-id="6a344-129">Žádná</span><span class="sxs-lookup"><span data-stu-id="6a344-129">None</span></span>

<span data-ttu-id="6a344-130">**Datová část požadavku**</span><span class="sxs-lookup"><span data-stu-id="6a344-130">**Request payload**</span></span>

<span data-ttu-id="6a344-131">Žádná</span><span class="sxs-lookup"><span data-stu-id="6a344-131">None</span></span>

<span data-ttu-id="6a344-132">**Glosář**</span><span class="sxs-lookup"><span data-stu-id="6a344-132">**Glossary**</span></span>

<span data-ttu-id="6a344-133">Žádná</span><span class="sxs-lookup"><span data-stu-id="6a344-133">None</span></span>

<span data-ttu-id="6a344-134">**Response** (Odpověď)</span><span class="sxs-lookup"><span data-stu-id="6a344-134">**Response**</span></span>

<span data-ttu-id="6a344-135">Datová část odpovědi je strukturována takto:</span><span class="sxs-lookup"><span data-stu-id="6a344-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="6a344-136">Kód odpovědi: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="6a344-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="6a344-137">Příklad datové části odpovědi:</span><span class="sxs-lookup"><span data-stu-id="6a344-137">Response payload example:</span></span>

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

<span data-ttu-id="6a344-138">**Glosář**</span><span class="sxs-lookup"><span data-stu-id="6a344-138">**Glossary**</span></span>

<span data-ttu-id="6a344-139">Tato tabulka definuje klíčové prvky v odpovědi:</span><span class="sxs-lookup"><span data-stu-id="6a344-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="6a344-140">Parametr</span><span class="sxs-lookup"><span data-stu-id="6a344-140">Parameter</span></span>    |    <span data-ttu-id="6a344-141">Popis</span><span class="sxs-lookup"><span data-stu-id="6a344-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="6a344-142">QueryId</span><span class="sxs-lookup"><span data-stu-id="6a344-142">QueryId</span></span>     |    <span data-ttu-id="6a344-143">Jedinečný identifikátor UUID pro dotaz, který byl odstraněn</span><span class="sxs-lookup"><span data-stu-id="6a344-143">Unique UUID of the query that was deleted</span></span>    |
|    <span data-ttu-id="6a344-144">Name</span><span class="sxs-lookup"><span data-stu-id="6a344-144">Name</span></span>     |    <span data-ttu-id="6a344-145">Název dotazu, který byl odstraněn</span><span class="sxs-lookup"><span data-stu-id="6a344-145">Name of the query that was deleted</span></span>    |
|    <span data-ttu-id="6a344-146">Description</span><span class="sxs-lookup"><span data-stu-id="6a344-146">Description</span></span>     |    <span data-ttu-id="6a344-147">Popis odstraněného dotazu</span><span class="sxs-lookup"><span data-stu-id="6a344-147">Description of the deleted query</span></span>     |
|    <span data-ttu-id="6a344-148">Dotaz</span><span class="sxs-lookup"><span data-stu-id="6a344-148">Query</span></span>     |    <span data-ttu-id="6a344-149">Řetězec dotazu na sestavu pro odstraněný dotaz</span><span class="sxs-lookup"><span data-stu-id="6a344-149">Report query string of the deleted query</span></span>    |
|    <span data-ttu-id="6a344-150">Typ</span><span class="sxs-lookup"><span data-stu-id="6a344-150">Type</span></span>     |    <span data-ttu-id="6a344-151">Nastavit na Definovánouživatelem pro uživatelem vytvořené dotazy</span><span class="sxs-lookup"><span data-stu-id="6a344-151">Set to userDefined for user created queries</span></span>     |
|    <span data-ttu-id="6a344-152">Uživatel</span><span class="sxs-lookup"><span data-stu-id="6a344-152">User</span></span>     |    <span data-ttu-id="6a344-153">ID uživatele, který vytvořil dotaz</span><span class="sxs-lookup"><span data-stu-id="6a344-153">User ID who created the query</span></span>     |
|    <span data-ttu-id="6a344-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="6a344-154">CreatedTime</span></span>     |    <span data-ttu-id="6a344-155">Čas vytvoření dotazu</span><span class="sxs-lookup"><span data-stu-id="6a344-155">Time of creation of query</span></span>     |
|    <span data-ttu-id="6a344-156">TotalCount</span><span class="sxs-lookup"><span data-stu-id="6a344-156">TotalCount</span></span>     |    <span data-ttu-id="6a344-157">Počet datových sad v poli hodnot</span><span class="sxs-lookup"><span data-stu-id="6a344-157">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="6a344-158">Zpráva</span><span class="sxs-lookup"><span data-stu-id="6a344-158">Message</span></span>     |    <span data-ttu-id="6a344-159">Stavová zpráva od spuštění rozhraní API</span><span class="sxs-lookup"><span data-stu-id="6a344-159">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="6a344-160">StatusCode</span><span class="sxs-lookup"><span data-stu-id="6a344-160">StatusCode</span></span>     |    <span data-ttu-id="6a344-161">Kód výsledku.</span><span class="sxs-lookup"><span data-stu-id="6a344-161">Result Code.</span></span> <span data-ttu-id="6a344-162">Možné hodnoty jsou 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="6a344-162">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
