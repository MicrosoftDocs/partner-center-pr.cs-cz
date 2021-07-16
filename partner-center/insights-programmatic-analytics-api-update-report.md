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
# <a name="update-report-api"></a>Aktualizace rozhraní API pro sestavy

Toto rozhraní API vám pomůže upravit parametr sestavy.

**Syntaxe požadavku**

|    Metoda    |    Identifikátor URI žádosti    |
|    ----    |    ----    |
|    PUT    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
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
|    reportId     |    řetězec    |    No    |    ID upravované sestavy     |
|        |        |        |        |

**Parametr dotazu**

Žádná

**Žádost o datovou část**

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

**Glosář**

Tato tabulka obsahuje seznam klíčových definic elementů v odpovědi.

|    Parametr    |    Povinné    |    Popis    |    Povolené hodnoty    |
|    ----    |    ----    |    ----    |    ----    |
|    ReportName     |    Yes     |    Název, který se má k sestavě přiřadit     |    Řetězec     |
|    Popis     |    No     |    Popis vytvořené sestavy     |    Řetězec     |
|    StartTime     |    Yes    |    Časové razítko, po kterém začne generování sestavy     |    Řetězec     |
|    OpakováníInterval     |    No     |    Frekvence generování sestavy v hodinách Minimální hodnota je 4     |    Integer     |
|    Počet opakování     |    No     |    Čísla sestav, které se budou generovat Výchozí hodnota je neurčitý.     |    Integer     |
|    Formát     |    No    |    Formát exportovaného souboru. Výchozí hodnota je CSV.     |    CSV/TSV     |
|    CallbackURL     |    No     |    Adresa URL zpětného volání https, která se má volat při generování sestav     |    Řetězec     |
|    Metoda zpětného volání    |    No    |    Metoda HTTP, která se má použít pro zpětné volání    |    GET/POST    |
|        |        |        |        |


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
|    ID sestavy     |    Univerzálně jedinečný identifikátor (UUID) aktualizované sestavy     |
|    ReportName     |    Název předaný sestavě v datové části požadavku     |
|    Description     |    Popis předáný sestavě v datové části požadavku     |
|    ID dotazu     |    ID dotazu předané v době vytvoření sestavy     |
|    Dotaz     |    Text dotazu, který se provede pro tuto sestavu     |
|    Uživatel     |    ID uživatele použité k vytvoření sestavy     |
|    CreatedTime     |    Čas vytvoření sestavy Formát času je rrrr-MM-ddTHH:mm:ssZ.     |
|    ModifiedTime     |    Čas poslední změny sestavy Formát času je rrrr-MM-ddTHH:mm:ssZ.     |
|    ExecuteNow     |    Příznak ExecuteNow nastavený v době vytvoření sestavy    |
|    StartTime     |    Čas zahájení provádění sestavy Formát času je rrrr-MM-ddTHH:mm:ssZ.     |
|    Stav sestavy     |    Stav spuštění sestavy Možné hodnoty jsou Pozastaveno, Aktivní a Neaktivní.     |
|    OpakováníInterval     |    Interval opakování v datové části požadavku     |
|    Počet opakování     |    Počet opakování v datové části požadavku     |
|    CallbackUrl (Url zpětného volání)     |    Adresa URL zpětného volání zadaná v požadavku     |
|    Metoda zpětného volání    |    Metoda zpětného volání poskytnutá v požadavku    |
|    Formát     |    Formát souborů sestav     |
|    TotalCount     |    Počet datových sad v poli Hodnota     |
|    Zpráva     |    Stavová zpráva z spuštění rozhraní API     |
|    Statuscode     |    Kód výsledku. Možné hodnoty jsou 200, 400, 401, 403, 500.     |
|        |        |