---
title: Vyzkoušejte rozhraní API pro dotazy na sestavy
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Toto rozhraní API použijte k otestování dotazu a ověření výsledků v Partnerské centrum přehledech.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 13ad6fe385a4d31390b6806d863da3f647105b2c
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376451"
---
# <a name="try-report-queries-api"></a><span data-ttu-id="68dcd-103">Vyzkoušejte rozhraní API pro dotazy na sestavy</span><span class="sxs-lookup"><span data-stu-id="68dcd-103">Try report queries API</span></span>

<span data-ttu-id="68dcd-104">Toto rozhraní API spustí příkaz dotazu sestavy.</span><span class="sxs-lookup"><span data-stu-id="68dcd-104">This API executes a Report query statement.</span></span> <span data-ttu-id="68dcd-105">Rozhraní API vrátí pouze 100 záznamů, které jako partner můžete použít k ověření, jestli jsou data podle očekávání.</span><span class="sxs-lookup"><span data-stu-id="68dcd-105">The API returns only 100 records that you as a partner can use to verify if the data is as you expected.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="68dcd-106">Toto rozhraní API má časový limit spuštění dotazu 100 sekund.</span><span class="sxs-lookup"><span data-stu-id="68dcd-106">This API has a query execution timeout of 100 seconds.</span></span> <span data-ttu-id="68dcd-107">Pokud si všimnete, že rozhraní API trvá déle než 100 sekund, je vysoce pravděpodobné, že dotaz je syntakticky správný, jinak byste obdrželi jiný kód chyby než 200.</span><span class="sxs-lookup"><span data-stu-id="68dcd-107">If you notice the API is taking more than 100 seconds, it is highly likely that the query is syntactically correct or else you would have received an error code other than 200.</span></span> <span data-ttu-id="68dcd-108">Pokud je syntaxe dotazu správná, skutečné generování sestavy se předá.</span><span class="sxs-lookup"><span data-stu-id="68dcd-108">The actual report generation will pass if the query syntax is correct.</span></span>

<span data-ttu-id="68dcd-109">**Syntaxe požadavku**</span><span class="sxs-lookup"><span data-stu-id="68dcd-109">**Request syntax**</span></span>

|    <span data-ttu-id="68dcd-110">Metoda</span><span class="sxs-lookup"><span data-stu-id="68dcd-110">Method</span></span>    |    <span data-ttu-id="68dcd-111">Identifikátor URI žádosti</span><span class="sxs-lookup"><span data-stu-id="68dcd-111">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="68dcd-112">GET</span><span class="sxs-lookup"><span data-stu-id="68dcd-112">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?<exportQuery={query text}|queryId={queryId}>`    |
|        |        |

<span data-ttu-id="68dcd-113">**Hlavička požadavku**</span><span class="sxs-lookup"><span data-stu-id="68dcd-113">**Request header**</span></span>

|    <span data-ttu-id="68dcd-114">Hlavička</span><span class="sxs-lookup"><span data-stu-id="68dcd-114">Header</span></span>    |    <span data-ttu-id="68dcd-115">Typ</span><span class="sxs-lookup"><span data-stu-id="68dcd-115">Type</span></span>    |    <span data-ttu-id="68dcd-116">Description</span><span class="sxs-lookup"><span data-stu-id="68dcd-116">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="68dcd-117">Autorizace</span><span class="sxs-lookup"><span data-stu-id="68dcd-117">Authorization</span></span>    |    <span data-ttu-id="68dcd-118">řetězec</span><span class="sxs-lookup"><span data-stu-id="68dcd-118">string</span></span>    |    <span data-ttu-id="68dcd-119">Povinná hodnota.</span><span class="sxs-lookup"><span data-stu-id="68dcd-119">Required.</span></span> <span data-ttu-id="68dcd-120">Přístupový Azure Active Directory (AAD) ve formuláři`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="68dcd-120">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="68dcd-121">Typ obsahu</span><span class="sxs-lookup"><span data-stu-id="68dcd-121">Content-Type</span></span>    |    <span data-ttu-id="68dcd-122">řetězec</span><span class="sxs-lookup"><span data-stu-id="68dcd-122">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="68dcd-123">**Parametr cesty**</span><span class="sxs-lookup"><span data-stu-id="68dcd-123">**Path parameter**</span></span>

<span data-ttu-id="68dcd-124">Žádná</span><span class="sxs-lookup"><span data-stu-id="68dcd-124">None</span></span>

<span data-ttu-id="68dcd-125">**Parametr dotazu**</span><span class="sxs-lookup"><span data-stu-id="68dcd-125">**Query parameter**</span></span>

|    <span data-ttu-id="68dcd-126">Název parametru</span><span class="sxs-lookup"><span data-stu-id="68dcd-126">Parameter Name</span></span>    |    <span data-ttu-id="68dcd-127">Typ</span><span class="sxs-lookup"><span data-stu-id="68dcd-127">Type</span></span>    |    <span data-ttu-id="68dcd-128">Vyžadováno</span><span class="sxs-lookup"><span data-stu-id="68dcd-128">Required</span></span>    |    <span data-ttu-id="68dcd-129">Popis</span><span class="sxs-lookup"><span data-stu-id="68dcd-129">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="68dcd-130">exportQuery</span><span class="sxs-lookup"><span data-stu-id="68dcd-130">exportQuery</span></span>     |    <span data-ttu-id="68dcd-131">řetězec</span><span class="sxs-lookup"><span data-stu-id="68dcd-131">string</span></span>    |    <span data-ttu-id="68dcd-132">No</span><span class="sxs-lookup"><span data-stu-id="68dcd-132">No</span></span>    |    <span data-ttu-id="68dcd-133">Řetězec dotazu sestavy, který je potřeba spustit</span><span class="sxs-lookup"><span data-stu-id="68dcd-133">Report query string that needs to be executed</span></span>     |
|    <span data-ttu-id="68dcd-134">ID dotazu</span><span class="sxs-lookup"><span data-stu-id="68dcd-134">queryId</span></span>     |    <span data-ttu-id="68dcd-135">řetězec</span><span class="sxs-lookup"><span data-stu-id="68dcd-135">string</span></span>    |    <span data-ttu-id="68dcd-136">No</span><span class="sxs-lookup"><span data-stu-id="68dcd-136">No</span></span>    |    <span data-ttu-id="68dcd-137">Platné ID existujícího dotazu.</span><span class="sxs-lookup"><span data-stu-id="68dcd-137">A valid existing query ID.</span></span> <span data-ttu-id="68dcd-138">Vzájemné vylučování s řetězcem dotazu zadaným v parametru exportQuery</span><span class="sxs-lookup"><span data-stu-id="68dcd-138">Mutually exclusive with query string specified in exportQuery parameter</span></span>    |
|    <span data-ttu-id="68dcd-139">startTime</span><span class="sxs-lookup"><span data-stu-id="68dcd-139">startTime</span></span>     |    <span data-ttu-id="68dcd-140">řetězec</span><span class="sxs-lookup"><span data-stu-id="68dcd-140">string</span></span>    |    <span data-ttu-id="68dcd-141">No</span><span class="sxs-lookup"><span data-stu-id="68dcd-141">No</span></span>    |    <span data-ttu-id="68dcd-142">Čas zahájení, od kterého chceme data.</span><span class="sxs-lookup"><span data-stu-id="68dcd-142">Start time from which we want the data.</span></span> <span data-ttu-id="68dcd-143">Přepisuje časové rozpětí zadané v dotazu.</span><span class="sxs-lookup"><span data-stu-id="68dcd-143">It overrides timespan specified in the query</span></span>    |
|    <span data-ttu-id="68dcd-144">endTime</span><span class="sxs-lookup"><span data-stu-id="68dcd-144">endTime</span></span>     |    <span data-ttu-id="68dcd-145">řetězec</span><span class="sxs-lookup"><span data-stu-id="68dcd-145">string</span></span>    |    <span data-ttu-id="68dcd-146">No</span><span class="sxs-lookup"><span data-stu-id="68dcd-146">No</span></span>    |    <span data-ttu-id="68dcd-147">Čas ukončení, do kterého chceme data.</span><span class="sxs-lookup"><span data-stu-id="68dcd-147">End time till which we want the data.</span></span> <span data-ttu-id="68dcd-148">Přepisuje časové rozpětí zadané v dotazu.</span><span class="sxs-lookup"><span data-stu-id="68dcd-148">It overrides timespan specified in the query</span></span>    |
|        |        |        |        |

<span data-ttu-id="68dcd-149">**Žádost o datovou část**</span><span class="sxs-lookup"><span data-stu-id="68dcd-149">**Request payload**</span></span>

<span data-ttu-id="68dcd-150">Žádná</span><span class="sxs-lookup"><span data-stu-id="68dcd-150">None</span></span>

<span data-ttu-id="68dcd-151">**Glosář**</span><span class="sxs-lookup"><span data-stu-id="68dcd-151">**Glossary**</span></span>

<span data-ttu-id="68dcd-152">Žádná</span><span class="sxs-lookup"><span data-stu-id="68dcd-152">None</span></span>

<span data-ttu-id="68dcd-153">**Response** (Odpověď)</span><span class="sxs-lookup"><span data-stu-id="68dcd-153">**Response**</span></span>

<span data-ttu-id="68dcd-154">Datová část odpovědi je strukturovaná takto:</span><span class="sxs-lookup"><span data-stu-id="68dcd-154">The response payload is structured as follows:</span></span>

<span data-ttu-id="68dcd-155">Kód odpovědi: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="68dcd-155">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="68dcd-156">Příklad datové části odpovědi:</span><span class="sxs-lookup"><span data-stu-id="68dcd-156">Response payload example:</span></span>

```json
Top 100 rows of query execution 
{ 
  "Value": [ 
    { 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="68dcd-157">**Glosář**</span><span class="sxs-lookup"><span data-stu-id="68dcd-157">**Glossary**</span></span>

<span data-ttu-id="68dcd-158">Tato tabulka definuje klíčové prvky v odpovědi:</span><span class="sxs-lookup"><span data-stu-id="68dcd-158">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="68dcd-159">Parametr</span><span class="sxs-lookup"><span data-stu-id="68dcd-159">Parameter</span></span>    |    <span data-ttu-id="68dcd-160">Popis</span><span class="sxs-lookup"><span data-stu-id="68dcd-160">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="68dcd-161">TotalCount</span><span class="sxs-lookup"><span data-stu-id="68dcd-161">TotalCount</span></span>     |    <span data-ttu-id="68dcd-162">Počet datových sad v poli Hodnota</span><span class="sxs-lookup"><span data-stu-id="68dcd-162">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="68dcd-163">Zpráva</span><span class="sxs-lookup"><span data-stu-id="68dcd-163">Message</span></span>     |    <span data-ttu-id="68dcd-164">Stavová zpráva z spuštění rozhraní API</span><span class="sxs-lookup"><span data-stu-id="68dcd-164">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="68dcd-165">Statuscode</span><span class="sxs-lookup"><span data-stu-id="68dcd-165">StatusCode</span></span>     |    <span data-ttu-id="68dcd-166">Kód výsledku.</span><span class="sxs-lookup"><span data-stu-id="68dcd-166">Result Code.</span></span> <span data-ttu-id="68dcd-167">Možné hodnoty jsou 200, 400, 401, 403, 500.</span><span class="sxs-lookup"><span data-stu-id="68dcd-167">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
