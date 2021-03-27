---
title: Jak ověřit, že zákazník přijal do programu CSP zákaznickou smlouvu Microsoftu
description: Partneři poskytovatele Cloud Solution Provider (CSP) musí před objednáním služeb Microsoft pro zákazníky potvrdit přijetí smlouvy se zákazníkem Microsoftu.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: ebb52a3a8223d3b1101e3a8e78728fcc167e25e3
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633774"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a>Jak ověřit, že zákazník přijal do programu CSP zákaznickou smlouvu Microsoftu

**Příslušné role**

- Agent správce
- Agent prodeje


Zákazníci mají dvě možnosti, jak přijmou zákaznickou smlouvu Microsoftu.

**Možnost 1**: ověření partnerského serveru pro přijetí u zákazníka – partner může potvrdit přijetí zákazníkovi pomocí rozhraní API pro partnerské centrum a sady SDK nebo prostřednictvím řídicího panelu partnerského centra.

**Možnost 2**: přímé přijetí zákazníkem – partner může pozvat zákazníka přes adresu URL, aby si tuto smlouvu zkontroloval a přijal v centru pro správu Microsoft 365.

## <a name="access-microsoft-customer-agreement-template"></a>Přístup k šabloně zákaznických smluv Microsoftu

Nejnovější verzi šablony zákaznických smluv od Microsoftu si můžete stáhnout [ručně.](https://aka.ms/customeragreement) Smlouva o zákaznících Microsoftu je specifická pro danou zemi. Při požadavku na šablonu smlouvy o zákaznících Microsoftu nezapomeňte vybrat správnou zemi na základě umístění zákazníka.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>Možnost 1: potvrzení přijetí zákazníkem v partnerském centru

Partneři s přímým účtováním můžou potvrdit přijetí smlouvy o zákaznících Microsoftu v partnerském centru pro zákazníky, kteří mají nové a stávající zákazníky. Nepřímí prodejci nemůžou v zastoupení svých zákazníků ověřit platnost a při provádění ověření identity musí spolupracovat s jejich nepřímým zprostředkovatelem.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Potvrďte přijetí zákazníkovi pro nové zákazníky

Při vytváření nového tenanta zákazníka v partnerském centru použijte následující postup k potvrzení souhlasu zákazníka s zákaznickou smlouvou Microsoftu. K provedení těchto kroků musíte být agentem správce nebo prodejní agent.

1. Vyberte **zákazníci** a pak **Nový zákazník**.

2. V části **informace o účtu** zadejte informace pro společnost a její primární kontakt.

3. V části **smlouva Microsoft** zaškrtněte políčko s potvrzením, že zákazník přijal zákaznickou smlouvu Microsoftu.

4. V části **Datum přijetí smlouvy** zadejte příslušné datum. Tuto hodnotu nelze nastavit na budoucí datum.

5. Ujistěte se, že se zobrazují správné kontaktní informace uživatele. Pokud je nesprávná, vyberte **aktualizovat** a zadejte přesné informace pro osobu, která smlouvu přijala.

6. Kliknutím na tlačítko **Další** pokračujte v vytváření tenanta zákazníka.

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Nový zákazník":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Potvrďte přijetí zákazníky u stávajících zákazníků

K tomu musíte být agentem správce nebo agent pro prodej:

1. Vyberte **Zákazníci**. Vyhledejte a vyberte zákazníka.

2. Vyberte **informace o účtu**.

3. V části **Zákaznická smlouva Microsoftu** vyberte **aktualizovat**.

4. Zadejte **jméno**, **příjmení**, **e-mailovou adresu** a **telefonní číslo** (nepovinné) osoby, která smlouvu přijala. V části **Datum přijetí smlouvy** zadejte příslušné datum. Tuto hodnotu nelze nastavit na budoucí datum.

5. Vyberte **Uložit** a pokračovat.

   :::image type="content" source="images/mcua2-update2.png" alt-text="Stávající zákazník":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Načíst potvrzení přijetí u zákazníka

Pokud chcete načíst potvrzení, že stávající zákazník přijal smlouvu o zákaznících Microsoftu, postupujte podle následujících kroků. K tomu musíte být agentem správce nebo agentem pro prodej.

1. Vyberte **zákazníci** a pak vyhledejte a vyberte zákazníka, kterého chcete zobrazit.

2. Vyberte **informace o účtu**.

3. V části **Smlouva o zákaznících Microsoftu** se zobrazí potvrzení, jestli ho zákazník zadal nebo neposkytl.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Potvrzení přijetí zákazníkovi pomocí rozhraní API pro partnerské centrum a sady SDK

Pomocí rozhraní API a sady SDK partnerského centra můžete potvrdit přijetí smlouvy o zákaznících Microsoftu v rámci zákazníka. Podrobnosti o rozhraní API nebo sadě SDK najdete v tématu:

- [Získání metadat smluv pro Smlouvu se zákazníkem Microsoftu](/partner-center/develop/get-customer-agreement-metadata)

- [Potvrzení přijetí Smlouvy se zákazníkem Microsoftu ze strany zákazníka](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Získání potvrzení přijetí Smlouvy se zákazníkem Microsoftu ze strany zákazníka](/partner-center/develop/get-confirmation-of-customer-agreement)

- [Získat odkaz ke stažení pro šablonu zákaznických smluv Microsoftu](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>Možnost 2: přijetí zákazníkem v centru pro správu Microsoft 365

Partneři můžou pozvat nové a stávající zákazníky přes adresu URL, aby si tuto smlouvu zkontrolovali a přijali v rámci centra pro správu Microsoft 365. V následujících částech se dozvíte, jak:

- Vytvořte nového zákazníka a pozvěte zákazníka, aby smlouvu zkontroloval a přijal.

- Pozvěte nového zákazníka, aby zkontroloval a přijal vztah prodejce a smlouvu.

- Pozvání stávajícího zákazníka ke kontrole a přijetí smlouvy.

>[!NOTE]
> Pomocí [rozhraní API a sady SDK pro partnery](/partner-center/develop/get-direct-sign-status-of-customer-agreement) můžete získat stav přímého přijetí smlouvy o zákaznících Microsoftu od zákazníka.  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Vytvoření nového zákazníka a pozvání zákazníka ke kontrole a přijetí smlouvy

Pomocí následujících kroků můžete vytvořit nového zákazníka v partnerském centru a pak je pozvat k revizi a přijetí smlouvy o zákaznících Microsoftu v rámci centra pro správu Microsoft 365.

1. Na kartě **zákazníci** v partnerském centru vyberte **Přidat zákazníka**.

2. V části **informace o účtu** zadejte informace o novém zákazníkovi ve všech povinných polích, včetně názvu společnosti zákazníka a primárního kontaktu.

3. V části **smlouva se zákazníkem** vyberte **Zákazník se žádost o přijetí smlouvy o zákaznících Microsoftu v centru pro správu Microsoft 365**. Vyplňte všechna další povinná pole na stránce.

4. Vyberte **Další: Zkontrolujte** a pokračujte postupem vytvoření tenanta zákazníka. 

>[!NOTE] 
>Noví zákazníci si nemůžou koupit nákup, dokud nepřijmou zákaznickou smlouvu Microsoftu.  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Vytvořit nového zákazníka":::

5. Až se dostanete na obrazovku pro **potvrzení** v pracovním postupu nový zákazník, uložte přihlašovací údaje zákazníka. Tyto přihlašovací údaje budete muset později poskytnout zákazníkovi.

6. Mimo partnerské Centrum vytvořte a odešlete e-mail, který vyzývá zákazníka, aby přijal zákaznickou smlouvu Microsoftu v centru pro správu Microsoft 365. Nezapomeňte zahrnout tyto položky do e-mailu:

   - Odkaz na tuto [adresu URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (vyžaduje se přihlášení)

   - Přihlašovací údaje zákazníka, které jste uložili v kroku 5.

7. Zákazník pak obdrží pozvánku e-mailu od partnera a vybere [adresu URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).

8. Zákazník se přihlásí do centra pro správu Microsoft 365 pomocí zadaných přihlašovacích údajů zákazníka.

9. Zákazník zkontroluje pole, aby přijal zákaznickou smlouvu od Microsoftu.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Pozvání nového zákazníka ke kontrole a přijetí vztahu prodejce a smlouvy o zákaznících Microsoftu 

Pomocí následujícího postupu můžete pozvat nového zákazníka ke kontrole a přijetí vztahu prodejce a smlouvy o zákaznících Microsoftu. 

1. Na kartě **zákazníci** v partnerském centru vyberte odkaz **požádat o vztah prodejce** . 

2. Automaticky se vytvoří šablona e-mailu, včetně textu a parametrizované adresy URL, která zákazníka přesměruje na centrum pro správu Microsoft 365.

3. Můžete přizpůsobit automaticky vygenerovanou šablonu e-mailu a pak vybrat **Kopírovat do schránky** nebo **otevřít v e-mailu**.

4. Tato e-mailová šablona slouží k pozvání zákazníka k přijetí žádosti o **vztah prodejce** a **smlouvy o zákaznících Microsoftu**. (Poznámka: v pozvánce k e-mailu zajistěte, aby partner zahrnoval taky adresu URL, která se automaticky zadala, a také přihlašovací údaje zákazníka, které se nedávno vytvořily.)

   :::image type="content" source="images/mca/createrelationship.png" alt-text="Vytvoření relace":::

5. Zákazník obdrží pozvánku prostřednictvím e-mailu a klikne na parametrizovanou adresu URL. 

6. Zákazník používá přihlašovací údaje, které poskytnete v e-mailu pro přihlášení do centra pro správu Microsoft 365.

7. Zákazník zkontroluje pole, aby přijal **vztah prodejce** a **Zákaznickou smlouvu od Microsoftu**. 

8. V rámci stejné adresy URL je zákazník schopný zobrazit konsolidovaný seznam různých partnerů, se kterými pracují. Pokud si chcete zobrazit podrobnosti, můžete vybrat partnera.

   :::image type="content" source="images/mca/accept.jpg" alt-text="Přijetí smlouvy":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Pozvání stávajícího zákazníka ke kontrole a přijetí smlouvy

Pomocí následujících kroků můžete pozvat stávajícího zákazníka, aby zkontroloval a přijal zákaznickou smlouvu Microsoftu. 

1. Vytvořte e-mail zákazníka s vloženou adresou URL, která vyzývá zákazníka, aby přijal zákaznickou smlouvu Microsoftu.

2. Váš zákazník obdrží pozvánku prostřednictvím e-mailu a klikne na [adresu URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement). 

3. Zákazník zadá své přihlašovací údaje do centra pro správu Microsoft 365.

4. Zákazník toto políčko přijme, aby přijal zákaznickou smlouvu od Microsoftu. 

5. V rámci stejné adresy URL může zákazník zobrazit konsolidovaný seznam různých partnerů, se kterými pracují. Pokud si chcete zobrazit podrobnosti, můžete vybrat partnera.

   :::image type="content" source="images/mca/customeraccept.png" alt-text="zákazníka":::

>[!NOTE]
>V některých scénářích nemusí zákazníci být schopni zákaznickou smlouvu od Microsoftu přijmout přímo. Pokud chcete získat další informace o těchto situacích, přečtěte si dva scénáře, kdy potřebujete ověřit jménem zákazníka níže.

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a>Dva scénáře, kdy potřebujete ověřit jménem zákazníka

Existují dva scénáře, kdy zákazníci nemusí být schopni přímo přijmout smlouvu o zákaznících Microsoftu v centru pro správu Microsoft 365.

**Scénář 1**: stávající zákazník si koupil některý z následujících stávajících partnerských vztahů: nabídky, předplatné softwaru nebo softwaru, rezervované instance nebo plán Azure. Zákazník se teď snaží vytvořit nový nákup (kromě automatického obnovování). Když zákazník klikne na adresu URL, obdrží zprávu "kontaktujte svého partnera a potvrďte přijetí smlouvy o zákaznících Microsoftu."  

**Řešení**: je nutné, abyste byli jménem zákazníka ověřeni.

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Snímek obrazovky se stránkou centra pro správu Microsoft 365 s výzvou, abyste se mohli obrátit na svého partnera a potvrdit přijetí smlouvy o zákaznících Microsoftu.":::

**Scénář 2**: stávající zákazník si koupil některou z následujících nabídek, předplatných softwaru a softwaru, rezervovaných instancí a plánu Azure. Zákazník se teď snaží vytvořit nový nákup s novým partnerem.

Když zákazník klikne na adresu URL, Microsoft 365 centrum pro správu, aby přijal nový partnerský vztah a smlouvu, obdrží zprávu "kontaktujte svého partnera a potvrďte přijetí smlouvy o zákaznících Microsoftu."  

**Řešení**: je nutné, abyste byli jménem zákazníka ověřeni.  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a>Potvrďte, že zákazník přijal smlouvu.

Pokud se pokusíte vytvořit novou objednávku pro existujícího zákazníka, kterého jste ještě nepotvrzuji, zobrazí se výzva k dokončení potvrzení. K tomu použijte následující postup.

1. Zadejte **jméno**, **příjmení**, **e-mailovou adresu** a **telefonní číslo** (nepovinné) uživatele, který smlouvu přijal.

2. V části **Datum přijetí smlouvy** zadejte příslušné datum. Tuto hodnotu nelze nastavit na budoucí datum.

3. Vyberte **Uložit a pokračovat**. 

## <a name="next-steps"></a>Další kroky

- [Ověření nebo aktualizace informací o profilu společnosti](update-your-partner-profile.md)
- [Smlouvy se zákazníkem Microsoftu (podle oblasti a jazyka)](Agreements.md)
