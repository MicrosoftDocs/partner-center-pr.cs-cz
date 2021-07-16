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
# <a name="get-report-queries-api"></a>Získat rozhraní API pro dotazy sestav

Rozhraní API pro dotazy Get Report získá všechny dotazy, které jsou k dispozici pro použití v sestavách. Ve výchozím nastavení získá všechny dotazy definované systémem a uživatelem.

**Syntaxe žádosti**

|    Metoda    |    Identifikátor URI žádosti    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
|        |        |

**Hlavička žádosti**

|    Hlavička    |    Typ    |    Description    |
|    ----    |    ----    |    ----    |
|    Autorizace    |    řetězec    |    Povinná hodnota. přístupový token pro Azure Active Directory (AAD) ve formuláři`Bearer <token>`    |
|    Typ obsahu    |    řetězec    |    `Application/JSON`    |
|        |        |        |

**Parametr cesty**

Žádná

**Parametr dotazu**

|    Název parametru    |    Typ    |    Vyžadováno    |    Popis    |
|    ----    |    ----    |    ----    |    ----    |
|    queryId     |    řetězec     |    No    |    Filtr pro získání podrobností o dotazech s ID uvedeným v argumentu     |
|    queryName     |    řetězec     |    No    |    Filtr, který získá podrobné informace o dotazech s názvem zadaným v argumentu     |
|    IncludeSystemQueries     |    boolean     |    No    |    Zahrnout předdefinované systémové dotazy do odpovědi     |
|    IncludeOnlySystemQueries     |    boolean     |    No    |    Zahrnout do odpovědi pouze systémové dotazy     |
|        |        |        |        |


**Datová část požadavku**

Žádná

**Glosář**

Žádná

**Response** (Odpověď)

Datová část odpovědi je strukturována takto:

Kód odpovědi: 200, 400, 401, 403, 404, 500

Příklad datové části odpovědi:

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

**Glosář**

Tato tabulka definuje klíčové prvky v odpovědi:

|    Parametr    |    Popis    |
|    ----    |    ----    |
|    QueryId     |    Jedinečný identifikátor UUID dotazu     |
|    Name     |    Název zadaný pro dotaz v době vytváření dotazu     |
|    Description     |    Popis zadaný při vytváření dotazu     |
|    Dotaz     |    Řetězec dotazu sestavy     |
|    Typ     |    Nastavte na Definovánouživatelem pro uživatelem vytvořené dotazy a systém pro předdefinované systémové dotazy.     |
|    Uživatel     |    ID uživatele, který vytvořil dotaz     |
|    CreatedTime     |    Čas vytvoření dotazu     |
|    TotalCount     |    Počet datových sad v poli hodnot     |
|    Zpráva     |    Stavová zpráva od spuštění rozhraní API     |
|    StatusCode     |    Kód výsledku. Možné hodnoty jsou 200, 400, 401, 403, 500     |
|        |        |
