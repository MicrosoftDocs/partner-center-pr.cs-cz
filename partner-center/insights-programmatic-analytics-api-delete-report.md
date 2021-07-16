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
# <a name="delete-report-api"></a>Rozhraní API pro odstranění sestavy

Při spuštění toto rozhraní API odstraní všechny záznamy o spuštění sestavy a sestavy.

**Syntaxe požadavku**

|    Metoda    |    Identifikátor URI žádosti    |
|    ----    |    ----    |
|    DELETE    |    ` https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

**Hlavička požadavku**

|    Hlavička    |    Typ    |    Description    |
|    ----    |    ----    |    ----    |
|    Autorizace    |    řetězec    |    Povinná hodnota. Přístupový Azure Active Directory (AAD) ve formuláři`Bearer <token>`    |
|    Typ obsahu    |    řetězec    |    `Application/JSON`    |
|        |        |        |

**Parametr cesty**

|    Název parametru    |    Typ    |    Vyžadováno    |    Popis    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId     |    řetězec    |    No    |    ID odstraněné sestavy    |
|        |        |        |        |

**Parametr dotazu**

Žádná

**Žádost o datovou část**

Žádná

**Glosář**

Žádná

**Response** (Odpověď)

Datová část odpovědi je strukturovaná takto:

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
|    ID sestavy     |    Univerzálně jedinečný identifikátor (UUID) odstraněné sestavy     |
|    ReportName     |    Název přidán sestavě během vytváření     |
|    Description     |    Popis při vytváření sestavy     |
|    ID dotazu     |    ID dotazu předané v době vytvoření sestavy     |
|    Dotaz     |    Text dotazu, který se provede pro tuto sestavu     |
|    Uživatel     |    ID uživatele použité k vytvoření sestavy     |
|    CreatedTime     |    Čas vytvoření sestavy Formát času je rrrr-MM-ddTHH:mm:ssZ.     |
|    ModifiedTime     |    Čas poslední změny sestavy Formát času je rrrr-MM-ddTHH:mm:ssZ.     |
|    ExecuteNow     |    Příznak ExecuteNow nastavený v době vytvoření sestavy     |
|    StartTime     |    Čas zahájení provádění sestavy Formát času je rrrr-MM-ddTHH:mm:ssZ.     |
|    Stav sestavy     |    Stav spuštění sestavy Možné hodnoty jsou Pozastaveno, Aktivní a Neaktivní.     |
|    OpakováníInterval     |    Interval opakování poskytovaný během vytváření sestavy     |
|    Počet opakování     |    Počet opakování při vytváření sestavy     |
|    CallbackUrl (Url zpětného volání)     |    Adresa URL zpětného volání zadaná v požadavku     |
|    Metoda zpětného volání    |    Metoda zpětného volání poskytnutá v požadavku    |
|    Formát     |    Formát souborů sestav     |
|    TotalCount     |    Počet datových sad v poli Hodnota     |
|    Zpráva     |    Stavová zpráva z spuštění rozhraní API     |
|    Statuscode     |    Kód výsledku. Možné hodnoty jsou 200, 400, 401, 403, 500.     |
|        |        |
