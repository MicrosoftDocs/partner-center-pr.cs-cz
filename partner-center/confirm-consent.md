---
title: Potvrzení přijetí Smlouvy se zákazníkem Microsoftu ze strany zákazníka
description: Zjistěte, jak potvrdit přijetí smlouvy o zákaznících Microsoftu v rámci zákazníka. To může být nutné k objednání produktů a služeb společnosti Microsoft pro zákazníky.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/02/2021
ms.openlocfilehash: ab2f5be77f6480b4a8b47bef0e0fd5096f7c1776
ms.sourcegitcommit: a7897284b79abb1ceeee79deb3a87b72d59900dc
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/04/2021
ms.locfileid: "102029912"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Potvrzení souhlasu zákazníka se Smlouvou se zákazníkem Microsoftu


**Příslušné role**

- Agent správce
- Agent prodeje

> [!NOTE]
> Prostředek smlouvy je aktuálně podporovaný partnerským centrem jenom ve veřejném cloudu Microsoftu. Neplatí pro:
> * Partnerské centrum provozovaný společností 21Vianet
> * Partnerské centrum pro Microsoft Cloud pro Německo
> * Partnerské centrum pro Microsoft Cloud for US Government


Jako partner musíte od zákazníka získat souhlas s zákaznickou smlouvou Microsoftu, abyste mohli objednat produkty a služby Microsoftu pro daného zákazníka. Aby lépe pomáhali partnerům plnit požadavky na dodržování předpisů, vyžádá si partneři, aby potvrdili přijetí poskytnutím následujících údajů týkajících se osoby, která smlouvu přijala:

- Jméno

- Příjmení

- E-mailová adresa

- Telefonní číslo (volitelné)

- Datum přijetí

Zákazníci s přímým přístupem a nepřímými poskytovateli musí potvrdit přijetí smlouvy o zákaznících Microsoftu při vyúčtování prostřednictvím partnerského centra nebo rozhraní API partnerského centra. Potvrzení je *povinné*.

>[!NOTE]
>Od 31. ledna 2020 musí všechny zákazníky, stávající a nové, podepsat nové smlouvy o zákaznících Microsoftu. Pokud se chcete dozvědět víc, přečtěte si téma potvrzení souhlasu zákazníka s zákaznickou [smlouvou Microsoftu](confirm-customer-agreement.md).

Pokud pro daného zákazníka není zadáno potvrzení:

- Pro tohoto zákazníka nebudete moct vytvořit nové objednávky.

- Pro tohoto zákazníka nebudete moct změnit počet licencí stávajících předplatných založených na licencích.

Potvrzení přijetí zákazníkovi se dá dělat prostřednictvím partnerského centra nebo rozhraní API partnerského centra. K tomu je možné využít rozhraní API partnerského centra, které najdete v následujících tématech:

- [Získat potvrzení souhlasu zákazníka](/partner-center/develop/get-confirmation-of-customer-consent)

- [Získat metadata smlouvy](/partner-center/develop/get-agreement-metadata)

- [Potvrzení souhlasu zákazníka](/partner-center/develop/confirm-customer-consent)

To platí pro produkční prostředí i pro prostředí izolovaného prostoru (sandbox).

## <a name="confirm-customer-acceptance-for-a-new-customer"></a>Potvrzení přijetí zákazníkovi pro nového zákazníka

Pomocí následujícího postupu potvrďte přijetí zákazníkovi při vytváření nového tenanta zákazníka v partnerském centru. K tomu musíte být agentem správce nebo agentem pro prodej.

1. Vyberte **zákazníci** a pak **Nový zákazník** a pak vyberte **informace o účtu**.

2. Zadejte informace o **společnosti** a **primárním kontaktu**.

   :::image type="content" source="images/mca/mca1.png" alt-text="Informace o společnosti":::

3. V části **Smlouva o zákaznících Microsoftu** vyberte zákazníka, který **přijal nejnovější zákaznickou smlouvu Microsoftu**.

4. V části **Datum přijetí smlouvy** zadejte příslušné datum. Tuto hodnotu nelze nastavit na budoucí datum.

5. Zadejte podrobnosti uživatele, který poskytl přijetí.

   :::image type="content" source="images/mca/MCA3.png" alt-text="Přidat datum přijetí":::

   Ve výchozím nastavení se zobrazí informace o primárním uživateli kontaktu. Pokud to není správné, vyberte **aktualizovat** a zadejte **jméno,** **příjmení**, **e-mailovou adresu** a **telefonní číslo* (nepovinné) osoby, která smlouvu přijala.

6. Kliknutím na tlačítko **Další** pokračujte podle zbývajících kroků a vytvořte tenanta zákazníka.

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Potvrzení přijetí zákazníkovi pro existujícího zákazníka

K tomu musíte být agentem správce nebo agentem pro prodej.

1. Vyberte **zákazníci** a pak vyhledejte a vyberte zákazníka, kterého chcete zobrazit.

2. Vyberte **informace o účtu**.

3. V části **Zákaznická smlouva Microsoftu** vyberte **aktualizovat**.

   :::image type="content" source="images/mca/mca4.png" alt-text="Aktualizace":::

4. Zadejte **jméno**, **příjmení**, **e-mailovou adresu** a **telefonní číslo** (nepovinné) uživatele, který smlouvu přijal.

5. V části **Datum přijetí smlouvy** zadejte příslušné datum. Tuto hodnotu nelze nastavit na budoucí datum.

6. Vyberte **Uložit a pokračovat**.

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Potvrdit přijetí zákazníkovi při vytváření nové objednávky pro existujícího zákazníka

Pokud se pokusíte vytvořit novou objednávku pro existujícího zákazníka, kterého jste ještě nepotvrzuji, zobrazí se výzva k dokončení potvrzení. K tomu použijte následující postup.

1. Zadejte **jméno**, **příjmení**, **e-mailovou adresu** a **telefonní číslo** (nepovinné) uživatele, který smlouvu přijal.

2. V části **Datum přijetí smlouvy** zadejte příslušné datum. Tuto hodnotu nelze nastavit na budoucí datum.

3. Vyberte **Uložit a pokračovat**.

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Načtení potvrzení přijetí zákazníkovi pro existujícího zákazníka

Potvrzení přijetí zákazníkovi můžete načíst pro existujícího zákazníka, který jste zadali dříve pomocí níže uvedeného postupu. K tomu musíte být agentem správce nebo agentem pro prodej.

1. Vyberte **zákazníci** a pak vyhledejte a vyberte zákazníka, kterého chcete zobrazit.

2. Vyberte **informace o účtu**.

3. V části **Smlouva o zákaznících Microsoftu** se zobrazí informace o tom, jestli se pro tohoto zákazníka zadalo potvrzení.

## <a name="next-steps"></a>Další kroky

- [Potvrzení souhlasu zákazníka s zákaznickou smlouvou Microsoftu v partnerském programu CSP](confirm-customer-agreement.md)

- [Potvrzení souhlasu smlouvy se zákazníkem Microsoftu jménem vašeho zákazníka](attest-acceptance-customer-agreement.md)