---
title: získat rozhraní API pro sestavy – Přehledy dat
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Pomocí tohoto rozhraní API získáte všechny dostupné ID sestav ve službě partner Center Insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 174a2f60a36cb46b287b787b177dd32236cef4eb
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376458"
---
# <a name="get-report-api"></a>Získat rozhraní API pro sestavy

Toto rozhraní API získá všechny plánované sestavy.

**Syntaxe žádosti**

|    Metoda    |    Identifikátor URI žádosti    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport?reportId={Report ID}&reportName={Report Name}&queryId={Query ID}` |
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
|    reportId     |    řetězec    |    No    |    Filtr pro získání podrobností o pouze sestavách s reportId, které jsou uvedeny v tomto argumentu     |
|    reportName     |    řetězec    |    No    |    Filtr, který získá podrobné informace o pouze sestavách se sestavou, která je uvedena v tomto argumentu     |
|    queryId     |    řetězec    |    No    |    Filtr pro získání podrobností o pouze sestavách s queryId, které jsou uvedeny v tomto argumentu     |
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
      "ReportId": "string", 
      "ReportName": "string", 
      "Description": "string", 
      "QueryId": "string", 
      "Query": "string", 
      "User": "string", 
      "CreatedTime": "string", 
      "ModifiedTime": "string", 
      "executeNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      " RecurrenceCount": 0, 
      "CallbackUrl": "string",
      "CallbackMethod": null,
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0 
}
```

**Glosář**

Tato tabulka definuje klíčové prvky v odpovědi:

|    Parametr    |    Popis    |
|    ----    |    ----    |
|    ReportId     |    Jedinečný identifikátor UUID sestavy, která byla vytvořena     |
|    ReportName     |    Název zadaný pro sestavu v datové části požadavku     |
|    Description     |    Popis zadaný při vytvoření sestavy     |
|    QueryId     |    ID dotazu předané v okamžiku vytvoření sestavy     |
|    Dotaz     |    Text dotazu, který se spustí pro tuto sestavu     |
|    Uživatel     |    ID uživatele, které se použilo k vytvoření sestavy     |
|    CreatedTime     |    Čas, kdy byla sestava vytvořena. Formát času je RRRR-MM-ddTHH: mm: ssZ     |
|    ModifiedTime     |    Čas poslední změny sestavy Formát času je RRRR-MM-ddTHH: mm: ssZ     |
|    executeNow     |    Příznak ExecuteNow se nastavil v okamžiku vytvoření sestavy.    |
|    StartTime     |    Čas, kdy se spustí spuštění. Formát času je RRRR-MM-ddTHH: mm: ssZ     |
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