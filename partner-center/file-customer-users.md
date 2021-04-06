---
title: Pole pro soubor. CSV pro import několika uživatelů pro účet zákazníka
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Pokud chcete přidat více uživatelů k účtu zákazníka, vytvořte soubor hodnot oddělených čárkami (. csv) s příslušnými poli.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8ba08d97f1d360eae5af1941ed36753addd24939
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441417"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>Přidání více uživatelů na účet zákazníka vytvořením souboru. csv

**Příslušné role**

- Globální správce

Přidejte více uživatelů na účet zákazníka najednou, a to tak, že do partnerského centra nahrajete datový soubor ve formátu textový soubor s oddělovači (. csv). Ukázkový datový soubor si můžete stáhnout z partnerského centra a pak ho upravit pro vaše použití, nebo můžete vytvořit nový datový soubor pomocí datového modelu definovaného níže.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>Požadavky na datové soubory

Chcete-li přidat více uživatelů k účtu zákazníka pomocí procesu hromadného nahrávání, je nutné splnit následující požadavky:

- Musíte mít oprávnění globálního správce k účtu zákazníka;
- Každý uživatel musí mít jedinečnou e-mailovou adresu, která se připojí k e-mailovým doménám zákazníka;
- Můžete nahrávat až 100 záznamů najednou. Pokud potřebujete přidat více než 100 uživatelů, vytvořte a nahrajte další datové soubory.
- Všichni uživatelé musí být ve stejném geografickém **umístění**.
- Zadejte pouze data popsaná níže. Nadbytečné údaje způsobí selhání nahrávání.

V datovém souboru zadejte následující data:

| **Název sloupce** | **Popis**  | **Omezení**  |
|:-------- |:------  |:----- |
| Jméno  | Křestní jméno uživatele (volitelné pole)  | 50 – limit znaků  |
| Příjmení  | Poslední jméno uživatele (volitelné pole)  | 50 – limit znaků  |
| Zobrazované jméno    | Název zobrazený v partnerském centru (povinné pole)                            | 50 – limit znaků                         |
| E-mail   | Obchodní e-mailová adresa uživatele na zákaznické firmě (povinné pole)           | Každý uživatel musí mít jedinečnou e-mailovou adresu. |
| Aktualizace stavu   | Slouží k označení, zda byl záznam nového uživatele úspěšně vytvořen. | \*\*Ponechat prázdné\*\*                        |

## <a name="next-steps"></a>Další kroky

- [Postup přidání více uživatelů pro zákazníka](adding-multiple-users-to-a-customer-account.md)