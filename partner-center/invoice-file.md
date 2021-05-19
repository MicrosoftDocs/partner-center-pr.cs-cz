---
title: Principy Partnerské centrum faktur
ms.topic: article
ms.date: 05/18/2020
description: Porozuměli jste polím v souboru faktury pro Partnerské centrum fakturaci. Zahrnutá jsou pole a definice pro všechna pole faktury a pole s časovými poplatky.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5cb60c775bd8de38b8d7ca69c4dd97cf11b919fd
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146608"
---
# <a name="understand-partner-center-billing-invoice-fields"></a>Principy Partnerské centrum fakturační faktury

**Odpovídající role:** Globální správce | Správce správy uživatelů | Správce fakturace | Agent helpdesku

Pomocí následujících tabulek můžete porozumět polím v Partnerské centrum faktur.

## <a name="invoice-file-fields"></a>Pole souboru faktury

V souborech faktury se zobrazí následující pole.

| Pole | Definice |
| ----- | ---------- |
| US FEIN | Vaše identifikační číslo federálního zaměstnavatele (FEIN). Toto je vaše USA číslo daňového identifikačního čísla. |
| Číslo zákazníka | Číslo zákazníka. |
| Příjemce faktury | Adresa, na kterou posíláme fakturu. Název a adresu společnosti můžete změnit ve svém Partnerské centrum profilu. |
| Poplatky na základě licencí | Ploché měsíční nebo roční poplatky za zakoupené licence na základě využití, které se účtují předem. Toto číslo je součtem všech  poplatků ve sloupci Mezisoučty (sloupec **T)** v souboru s vyrovnáním na základě licencí. |
| Poplatky na základě využití | Vaše využití Azure. To zahrnuje nové služby nebo aplikace povolené a používané během fakturačního období. Toto číslo je součet všech poplatků ve sloupci **PretaxCharges** (sloupec **Z**) v souboru odsouhlasení založeném na využití. |
| Slevy | Sleva, kterou zákazník obdrží z normální ceny předplatného. Toto číslo se zobrazuje jako *paušální množství*, nikoli jako cena za jednotku nebo licenci. |
| Kredity | Kredity nebo úpravy pro změny předplatných (například zvýšení nebo snížení licence). |
| Mezisoučet | Celkem před zdaněním a poplatky a kredity bez daně. |
| Daň | Celková daň za vaše aktuální poplatky, jak je uvedeno v části **podrobností** počínaje stránkou 2 vaší faktury. Toto číslo je součet všech poplatků ve sloupci **TaxAmount** (sloupec **AA**) ve vašem souboru odsouhlasení založeném na využití a sloupec **daně** (sloupec **U**) v souboru odsouhlasení na základě licence. |
| Další kredity | Kredity výhradně pro daň. |
| Aktuální poplatky za celkem | Částka splatná v fakturační měně pro fakturační období Tyto poplatky jsou splatné podle data splatnosti platby. |
| Pokyny pro platbu | Popis způsobu platby faktury na základě vaší oblasti. *Při platbě vždycky nezapomeňte zahrnout číslo vaší faktury.* |
| Číslo faktury | Číslo vaší faktury |
| Fakturační období | Měsíční období zavedené na datum faktury. Toto je doba, po kterou jsou spotřebované služby založené na využívání, a služby založené na licencích jsou odsouhlaseny pro jakékoli úpravy kreditu nebo změny počtu licencí. |
| Datum faktury | Datum fakturace nebo datum výročí, kdy se vaše faktura generuje každý měsíc. |
| Platební podmínky | Platební období. U 1krát zakoupených nákupů to bude vždy 60 dnů. |
| Datum splatnosti platby | Datum, do kterého musí být vaše platba přijata. |
| Po zákazníka | Vaše nákupní číslo objednávky. |
| Služby zákazníkům | Adresa webu, na které máte přístup ke službě zákazníkům. |
| Příjemce služby | Adresa, na které se služba používá. (Toto je oficiální adresa společnosti přidružená k prověřování společnosti.) |

## <a name="one-time-charges-fields"></a>Pole s časovými poplatky

Následující pole se vztahují pouze na **poplatky za Partnerské centrum:**

| Pole | Definice |
| ----- | ---------- |
| Datum | Datum nákupu |
| Description | Název produktu. |
| Množství | Počet zakoupených produktů (například rezervací). |
| Jednotková cena | Cena za produkt (například rezervace). |
| Slevy | Všechny příslušné slevy. |
| Částka před zdaněním | Mezisoučt nákupů před daněmi |
| Dph | Daňová částka. |
| Celkem | Celková částka, která se má zaplatit |
