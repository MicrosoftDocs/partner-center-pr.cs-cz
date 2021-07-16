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
# <a name="try-report-queries-api"></a>Vyzkoušejte rozhraní API pro dotazy na sestavy

Toto rozhraní API spustí příkaz dotazu sestavy. Rozhraní API vrátí pouze 100 záznamů, které jako partner můžete použít k ověření, jestli jsou data podle očekávání.

> [!IMPORTANT]
> Toto rozhraní API má časový limit spuštění dotazu 100 sekund. Pokud si všimnete, že rozhraní API trvá déle než 100 sekund, je vysoce pravděpodobné, že dotaz je syntakticky správný, jinak byste obdrželi jiný kód chyby než 200. Pokud je syntaxe dotazu správná, skutečné generování sestavy se předá.

**Syntaxe požadavku**

|    Metoda    |    Identifikátor URI žádosti    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?<exportQuery={query text}|queryId={queryId}>`    |
|        |        |

**Hlavička požadavku**

|    Hlavička    |    Typ    |    Description    |
|    ----    |    ----    |    ----    |
|    Autorizace    |    řetězec    |    Povinná hodnota. Přístupový Azure Active Directory (AAD) ve formuláři`Bearer <token>`    |
|    Typ obsahu    |    řetězec    |    `Application/JSON`    |
|        |        |        |

**Parametr cesty**

Žádná

**Parametr dotazu**

|    Název parametru    |    Typ    |    Vyžadováno    |    Popis    |
|    ----    |    ----    |    ----    |    ----    |
|    exportQuery     |    řetězec    |    No    |    Řetězec dotazu sestavy, který je potřeba spustit     |
|    ID dotazu     |    řetězec    |    No    |    Platné ID existujícího dotazu. Vzájemné vylučování s řetězcem dotazu zadaným v parametru exportQuery    |
|    startTime     |    řetězec    |    No    |    Čas zahájení, od kterého chceme data. Přepisuje časové rozpětí zadané v dotazu.    |
|    endTime     |    řetězec    |    No    |    Čas ukončení, do kterého chceme data. Přepisuje časové rozpětí zadané v dotazu.    |
|        |        |        |        |

**Žádost o datovou část**

Žádná

**Glosář**

Žádná

**Response** (Odpověď)

Datová část odpovědi je strukturovaná takto:

Kód odpovědi: 200, 400, 401, 403, 404, 500

Příklad datové části odpovědi:

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

**Glosář**

Tato tabulka definuje klíčové prvky v odpovědi:

|    Parametr    |    Popis    |
|    ----    |    ----    |
|    TotalCount     |    Počet datových sad v poli Hodnota     |
|    Zpráva     |    Stavová zpráva z spuštění rozhraní API     |
|    Statuscode     |    Kód výsledku. Možné hodnoty jsou 200, 400, 401, 403, 500.     |
|        |        |
