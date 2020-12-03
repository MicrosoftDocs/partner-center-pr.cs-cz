---
title: Vysvětlení fakturačních faktur partnerských Center
ms.topic: article
ms.date: 05/18/2020
description: Seznamte se s poli v souboru faktury pro fakturaci partnerského centra. Zahrnuje pole a definice pro všechna pole faktury a pole jednorázového poplatku.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3e9eb392279c0a09b5e30395b38ab7030bfa87d4
ms.sourcegitcommit: 147813ba322653c989df5afe0b3bf0c252523a92
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/03/2020
ms.locfileid: "96556289"
---
# <a name="understand-partner-center-billing-invoice-fields"></a>Vysvětlení polí fakturační fakturace partnerského centra

**Příslušné role**

- Globální správce
- Správce uživatelů
- Správce fakturace
- Agent helpdesku

Následující tabulky vám pomohou pochopit pole v souborech faktury v partnerském centru.

## <a name="invoice-file-fields"></a>Pole souboru faktury

Následující pole se zobrazí v souborech faktury.

| Pole | Definice |
| ----- | ---------- |
| US FEIN | Vaše identifikační číslo federální zaměstnavatele (FEIN). Toto je vaše USA federální daňové identifikační číslo. |
| Číslo zákazníka | Vaše číslo zákazníka. |
| Příjemce faktury | Adresa, na kterou posíláme vaši fakturu. V fakturačním profilu partnerského centra můžete změnit název společnosti nebo adresu. |
| Poplatky na základě licencí | Paušální měsíční nebo roční poplatek za vaše zakoupené licence na základě využití se účtují předem za službu. Toto číslo je součet všech poplatků ve sloupci **Mezisoučet** (sloupec **T**) v souboru odsouhlasení na základě licence. |
| Poplatky na základě využití | Využití Azure. To zahrnuje nové služby nebo aplikace povolené a používané během fakturačního období. Toto číslo je součet všech poplatků ve sloupci **PretaxCharges** (sloupec **Z**) v souboru odsouhlasení založeném na využití. |
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
| Platební podmínky | Platební podmínky. Pro jednorázové nákupy bude vždycky 60 dní. |
| Datum splatnosti platby | Datum, kdy se platba musí přijmout. |
| Zákazník | Vaše objednávka čísla nákupu. |
| Služby zákazníkům | Adresa webu, kde můžete získat přístup ke službám zákazníkům. |
| Příjemce služby | Adresa, na které se služba používá (Jedná se o platnou adresu společnosti přidruženou k dozvíte ČSFD společnosti.) |

## <a name="one-time-charges-fields"></a>Pole jednorázových poplatků

Následující pole se vztahují jenom na **jednorázové poplatky** v partnerském centru:

| Pole | Definice |
| ----- | ---------- |
| Datum | Datum nákupu |
| Popis | Název produktu |
| Množství | Počet zakoupených produktů (například rezervací). |
| Jednotková cena | Cena za produkt (například rezervace). |
| Slevy | Jakékoli použitelné slevy. |
| Částka před zdaněním | Dílčí součet nákupů před zdaněním. |
| DPH | Daňová částka. |
| Celkem | Celková částka, která se má zaplatit |
