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
# <a name="pause-report-executions-api"></a>Pozastavit rozhraní API pro spouštění sestav

Při spuštění toto rozhraní API pozastaví naplánované provádění sestav.

**Syntaxe žádosti**

|    Metoda    |    Identifikátor URI žádosti    |
|    ----    |    ----    |
|    PUT    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/pause/{ReportID}`    |
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
|    reportId     |    řetězec    |    No    |    ID upravované sestavy     |
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

**Glosář**

Tato tabulka definuje klíčové prvky v odpovědi:

|    Parametr    |    Popis    |
|    ----    |    ----    |
|    ReportId     |    Univerzálně jedinečný identifikátor (UUID) pozastavené sestavy     |
|    ReportName     |    Název zadaný pro sestavu během vytváření     |
|    Description     |    Popis zadaný při vytváření sestavy     |
|    QueryId     |    ID dotazu předané v okamžiku vytvoření sestavy     |
|    Dotaz     |    Text dotazu, který se spustí pro tuto sestavu     |
|    Uživatel     |    ID uživatele, které se použilo k vytvoření sestavy     |
|    CreatedTime     |    Čas, kdy byla sestava vytvořena. Formát času je RRRR-MM-ddTHH: mm: ssZ     |
|    ModifiedTime     |    Čas poslední změny sestavy Formát času je RRRR-MM-ddTHH: mm: ssZ     |
|    ExecuteNow     |    Příznak ExecuteNow se nastavil v okamžiku vytvoření sestavy.     |
|    StartTime     |    Čas, kdy se spustí spuštění sestavy. Formát času je RRRR-MM-ddTHH: mm: ssZ     |
|    ReportStatus     |    Stav provádění sestavy Možné hodnoty jsou pozastavené, aktivní a neaktivní.     |
|    RecurrenceInterval     |    Interval opakování zadaný při vytváření sestavy     |
|    RecurrenceCount     |    Počet opakování poskytnutý během vytváření sestavy     |
|    CallbackUrl     |    Adresa URL zpětného volání poskytnutá v žádosti     |
|    CallbackMethod    |    Metoda zpětného volání poskytnutá v žádosti    |
|    Formát     |    Formát souborů sestav     |
|    TotalCount     |    Počet datových sad v poli hodnot     |
|    Zpráva     |    Stavová zpráva od spuštění rozhraní API     |
|    StatusCode     |    Kód výsledku. Možné hodnoty jsou 200, 400, 401, 403, 500     |
|        |        |
