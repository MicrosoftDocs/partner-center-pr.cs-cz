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
# <a name="resume-report-executions-api"></a>Obnovit rozhraní API pro spouštění sestav

Po spuštění toto rozhraní API obnoví plánované provádění pozastavené sestavy.

**Syntaxe žádosti**

|    Metoda    |    Identifikátor URI žádosti    |
|    ----    |    ----    |
|    PUT    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/resume/{ReportID}`    |
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
|    ReportId     |    Univerzálně jedinečný identifikátor (UUID) obnovené sestavy     |
|    ReportName     |    Název zadaný pro sestavu během vytváření     |
|    Description     |    Popis zadaný při vytváření sestavy     |
|    QueryId     |    ID dotazu předané v okamžiku vytvoření sestavy     |
|    Dotaz     |    Text dotazu, který se spustí pro tuto sestavu     |
|    Uživatel     |    ID uživatele, které se použilo k vytvoření sestavy     |
|    CreatedTime     |    Čas, kdy byla sestava vytvořena. Formát času je RRRR-MM-ddTHH: mm: ssZ     |
|    ModifiedTime     |    Čas poslední změny sestavy Formát času je RRRR-MM-ddTHH: mm: ssZ     |
|    ExecuteNow     |    Příznak ExecuteNow se nastavil v okamžiku vytvoření sestavy.    |
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
