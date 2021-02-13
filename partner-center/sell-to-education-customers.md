---
title: Jak prodávat nabídky zákazníkům pro vzdělávání
description: Naučte se, jak vytvořit zákazníka pro vzdělávání a prodávat nabídky v partnerském centru. Zahrnuje potvrzení stavu ověření pro zákazníka ve vzdělávání.
ms.topic: how-to
ms.date: 12/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: alikhaki
ms.author: alikhaki
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a101c3d29b947950179ca0ae446f049ccf785bb8
ms.sourcegitcommit: 64b43ad8fb7bb56628450bea06b9cd2606c36b03
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/12/2021
ms.locfileid: "100281311"
---
# <a name="how-to-sell-offers-to-education-customers-and-how-to-create-an-education-customer-in-partner-center"></a>Jak prodávat nabídky zákazníkům pro vzdělávání a jak vytvořit zákazníka vzdělávání v partnerském centru


**Příslušné role**

- Globální správce
- Agent správce
- Agent prodeje

## <a name="create-an-education-customer"></a>Vytvoření zákazníka v oblasti vzdělávání

Tento článek vysvětluje, jak vytvořit zákazníka vzdělávání v partnerském centru a prodávat vzdělávací produkty. Obsahuje také informace o tom, jak zobrazit stav ověřování a v případě potřeby znovu odeslat žádost o ověření. Nabídky vzdělávání jsou momentálně **dostupné jenom pro služby založené na licencích** , jako je Microsoft 365, Dynamics, Intune atd. Není k dispozici pro jiné typy (odběry softwaru, trvalé softwarové nebo produkty Azure).

> [!IMPORTANT]
> Společnost Microsoft ověří každého nově vytvořeného tenanta zákazníka, aby zajistil, že jsou kvalifikováni pro nabídky vzdělávání.  Nezapomeňte přesně a úplně zadat požadované informace, abyste zabránili prodlevám v procesu ověřování.

1. Přihlaste se do Partnerského centra.

2. Vyberte **zákazníci** a pak vyberte **Přidat zákazníka**. Z rozevíracího seznamu **speciální kvalifikace** vyberte **vzdělávání** .  Podle potřeby vyplňte zbývající informace o účtu.  Mezi klíčová pole, která pomáhají procesu ověřování, patří:

   - **Název společnosti**: Zadejte platný název entity – vyžadováno pro ověření.
   - **Země/oblast a řádky adres**: zadejte úplnou poštovní adresu entity – požadováno pro ověření.
   - **E-mailová adresa**: Zadejte e-maily vlastněné entitou – ne bezplatný nebo on.Microsoft.com e-mail – vyžaduje se pro ověření.
   - **Kontaktní údaje zákazníka**: tyto podrobnosti se budou používat jako součást procesu ověřování.
   - **Primární název domény**: používá se k vytvoření účtu zákazníka a e-mailových adres.  Vyberte název podobný názvu společnosti bez mezer nebo speciálních znaků.  Tento název nelze později změnit.

3. Až budete hotovi, vyberte **zkontrolovat**.

   :::image type="content" source="images/eduaccountinfo.png" alt-text="Účet zákazníka pro vzdělávání":::

4. Po potvrzení **Revize** obdržíte stav informování, pokud jsou odeslané informace platné.  

    :::image type="content" source="images/edu/create-review.png" alt-text="Vzdělávání zákaznického účtu na revizi"lightbox="images/edu/create-review-expanded.png":::

### <a name="confirm-your-education-customers-verification-status"></a>Potvrďte stav ověření zákazníka ve vzdělávání.

Na stránce **účet** zákazníka se podívejte na **stav speciální kvalifikace**.
Příklady stavu:

- Pokud zákazník prošel ověřením: vzdělávání

   :::image type="content" source="images/edupassedvetting.png" alt-text="Ověření vzdělávání bylo úspěšné.":::

- Pokud zákazník neuspěl při ověřování: nejedná se o zákazníka vzdělávání.

   :::image type="content" source="images/edu/fail-reason.png" alt-text="Ověření vzdělávání nebylo úspěšné." lightbox="images/edu/fail-reason-expanded.png":::

- Pokud zákazník není označený jako zákazník pro vzdělávání: žádné

   :::image type="content" source="images/edu/account-one.png" alt-text="Zákazník pro vzdělávání není označený jako" lightbox="images/edu/account-one-expanded.png":::

- Pokud zákazník přezkoumáte jako zákazník pro vzdělávání: Projděte si

    :::image type="content" source="images/edu/in-review.png" alt-text="Zákazník pro vzdělávání je právě přezkoumáván." lightbox="images/edu/in-review-expanded.png":::

## <a name="correct-the-customer-account-info-and-resubmit-for-verification"></a>Opravte informace o účtu zákazníka a znovu odešlete pro ověření.

Pokud zákazník neprojde počátečním ověřením, můžete si teď opravit informace a znovu ho odeslat.

### <a name="correct-the-customer-account-information"></a>Oprava informací o účtu zákazníka

Chcete-li aktualizovat informace o zákazníkovi, je nutné mít oprávnění globálního správce. Informace na portálu Office 365 aktualizujete, protože tato data nejde aktualizovat z portálu partnerského centra.

1. Na stránce **účet** se zobrazí informace o tom, že kvalifikace zákazníka se považuje za zákazníka, který není zákazníkem pro vzdělávání.

2. Aktualizujte prohlížeč, aby se stránka obnovila. K dispozici bude tlačítko **Update** a **zvláštní stav kvalifikace** je nastaven na **možnost žádné**.

3. Vyberte **Aktualizovat**. Na stránce **Správa služby** vyberte možnost **Office 365**.

4. Budete přesměrováni do centra pro správu Office 365 na nové kartě prohlížeče. Možná budete požádáni, abyste se přihlásili pomocí svých přihlašovacích údajů.

5. Vyberte **Nastavení**.

6. V horní části obrazovky vyberte kartu **Profil organizace** a potom **informace o organizaci**. Nyní můžete aktualizovat podrobnosti o zákazníkovi.

7. V dolní části bočního panelu vyberte **Uložit změny** .  

### <a name="resubmit-for-verification"></a>Znovu spustit pro ověření

1. Přejděte na kartu partnerského centra a na stránku **účet** zákazníka. Aktualizujte prohlížeč a ověřte, že se stránka společnosti aktualizovala na nové informace. Kliknutím na tlačítko **aktualizovat** vyžádáte opětovné ověření vzdělávání.

2. Pokud jsou aktualizované podrobnosti o zákaznících nárok na nabídky vzdělávání, budou se vám na **vzdělávání** zobrazovat **zvláštní kvalifikace** . Pokud se stále nezobrazuje **Zákazník pro vzdělávání**, obraťte se na podporu pro ruční ověřování.

## <a name="next-steps"></a>Další kroky

- [Prodej specializovaným odvětvím](get-special-pricing-for-offers.md)

- [Přidání nového zákazníka](add-a-new-customer.md)

- [Prodej Minecraftu: předplatná pro vzdělávací edice pro zákazníky v oblasti vzdělávání](minecraft-subscriptions.md)
