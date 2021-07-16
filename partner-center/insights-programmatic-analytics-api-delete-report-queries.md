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
# <a name="delete-report-queries-api"></a>Odstranit rozhraní API pro dotazy sestav

Toto rozhraní API odstraní uživatelsky definované dotazy.

**Syntaxe žádosti**

|    Metoda    |    Identifikátor URI žádosti    |
|    ----    |    ----    |
|    DELETE    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
|        |        |

**Hlavička žádosti**

|    Hlavička    |    Typ    |    Description    |
|    ----    |    ----    |    ----    |
|    Autorizace    |    řetězec    |    Povinná hodnota. přístupový token pro Azure Active Directory (AAD) ve formuláři`Bearer <token>`    |
|    Typ obsahu    |    řetězec    |    `Application/JSON`    |
|        |        |        |

**Parametr cesty**

|    Název parametru    |    Typ    |    Vyžadováno    |    Popis    |
|    ----    |    ----    |    ----    |    ----    |
|    queryId     |    řetězec     |    No    |    Filtr pro získání podrobností o dotazech s ID uvedeným v argumentu     |
|        |        |        |        |

**Parametr dotazu**

Žádná

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
|    QueryId     |    Jedinečný identifikátor UUID pro dotaz, který byl odstraněn    |
|    Name     |    Název dotazu, který byl odstraněn    |
|    Description     |    Popis odstraněného dotazu     |
|    Dotaz     |    Řetězec dotazu na sestavu pro odstraněný dotaz    |
|    Typ     |    Nastavit na Definovánouživatelem pro uživatelem vytvořené dotazy     |
|    Uživatel     |    ID uživatele, který vytvořil dotaz     |
|    CreatedTime     |    Čas vytvoření dotazu     |
|    TotalCount     |    Počet datových sad v poli hodnot     |
|    Zpráva     |    Stavová zpráva od spuštění rozhraní API     |
|    StatusCode     |    Kód výsledku. Možné hodnoty jsou 200, 400, 401, 403, 500     |
|        |        |
