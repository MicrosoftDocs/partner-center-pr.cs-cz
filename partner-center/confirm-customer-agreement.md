---
title: Jak potvrdit, že zákazník přijal Smlouva se zákazníkem Microsoftu programu CSP
description: Cloud Solution Provider (CSP) musí před objednání zákazníků potvrdit souhlas zákazníka s Smlouva se zákazníkem Microsoftu před služby Microsoft zákazníka.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: 9deebf3d9aab2d4dc7953da67a7eb17078b3d30c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277007"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a>Jak potvrdit, že zákazník přijal Smlouva se zákazníkem Microsoftu programu CSP

**Odpovídající role:** Agent pro správu | Agent prodeje


Zákazníci mají dvě možnosti, jak přijmou Smlouva se zákazníkem Microsoftu.

**Možnost 1:** Ověření souhlasu partnera se zákazníkem – Partner může potvrdit přijetí u zákazníka pomocí Partnerské centrum API nebo sady SDK nebo prostřednictvím řídicího panelu Partnerské centrum serveru.

**Možnost 2:** Přímé přijetí zákazníkem – Partner může pozvat zákazníka prostřednictvím adresy URL a zkontrolovat a přijmout smlouvu v centru Microsoft 365 pro správu.

## <a name="access-microsoft-customer-agreement-template"></a>Šablona Smlouva se zákazníkem Microsoftu přístupu

Nejnovější verzi této šablony si můžete Smlouva se zákazníkem Microsoftu stáhnout [tady.](https://aka.ms/customeragreement) Tento Smlouva se zákazníkem Microsoftu je specifický pro jednotlivé země. Při žádosti Smlouva se zákazníkem Microsoftu šablony aplikace nezapomeňte vybrat správnou zemi na základě polohy zákazníka.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>Možnost 1: Potvrzení přijetí zákazníkem v Partnerské centrum

Partneři s přímým vyúčtováním mohou potvrdit souhlas zákazníka s Smlouva se zákazníkem Microsoftu v Partnerské centrum pro nové i stávající zákazníky. Nepřímí prodejci nemohou provést ověření jménem svých zákazníků a potřebují spolupracovat se svým nepřímým poskytovatelem na dokončení ověření identity.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Potvrzení souhlasu zákazníka s novými zákazníky

Když vytvoříte nového tenanta zákazníka v Partnerské centrum, pomocí následujících kroků potvrďte souhlas zákazníka s Smlouva se zákazníkem Microsoftu. K provedení těchto kroků musíte být agentem pro správu nebo agentem Sales.

1. Vyberte **Customers (Zákazníci)** a pak **New customer (Nový zákazník).**

2. V **části Informace o** účtu zadejte informace o společnosti a jejím primárním kontaktu.

3. V **části Smlouva s Microsoftem** zaškrtněte políčko pro testování, že zákazník přijal Smlouva se zákazníkem Microsoftu.

4. V **části Datum přijetí smlouvy** zadejte příslušné datum. Tuto možnost nelze nastavit na budoucí datum.

5. Ujistěte se, že jsou zobrazené primární kontaktní informace uživatele správné. Pokud je nesprávný, vyberte **Aktualizovat a** zadejte přesné informace pro osobu, která smlouvu přijala.

6. Výběrem **možnosti** Další pokračujte ve vytváření tenanta zákazníka.

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Nový zákazník.":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Potvrzení přijetí u stávajících zákazníků zákazníkem

K tomu musíte být agentem pro správu nebo agentem Sales:

1. Vyberte **Zákazníci**. Vyhledejte a vyberte zákazníka.

2. Vyberte **Informace o účtu.**

3. V **Smlouva se zákazníkem Microsoftu** vyberte **Aktualizovat.**

4. Zadejte **jméno, příjmení,** **e-mailovou adresu** a telefonní číslo **(volitelné)** osoby, která smlouvu přijala.  V **části Datum přijetí smlouvy** zadejte příslušné datum. Tuto možnost nelze nastavit na budoucí datum.

5. Vyberte **Uložit a** pokračovat.

   :::image type="content" source="images/mcua2-update2.png" alt-text="Stávající zákazník.":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Načtení potvrzení přijetí zákazníkem

Pokud chcete načíst potvrzení, že stávající zákazník Smlouva se zákazníkem Microsoftu, použijte následující postup. K tomu musíte být agentem pro správu nebo agentem Sales.

1. Vyberte **Zákazníci** a pak vyhledejte a vyberte zákazníka, kterého chcete zobrazit.

2. Vyberte **Informace o účtu.**

3. V **části Smlouva se zákazníkem Microsoftu** zobrazte, jestli zákazník neposkytl nebo neposkytl potvrzení.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Potvrzení přijetí zákazníkem pomocí Partnerské centrum API nebo SDK

Pomocí rozhraní API Partnerské centrum SDK můžete potvrdit souhlas zákazníka s Smlouva se zákazníkem Microsoftu. Podrobnosti o rozhraní API nebo sadě SDK najdete zde:

- [Získání metadat smluv pro Smlouvu se zákazníkem Microsoftu](/partner-center/develop/get-customer-agreement-metadata)

- [Potvrzení přijetí Smlouvy se zákazníkem Microsoftu ze strany zákazníka](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Získání potvrzení přijetí Smlouvy se zákazníkem Microsoftu ze strany zákazníka](/partner-center/develop/get-confirmation-of-customer-agreement)

- [Získání odkazu ke stažení Smlouva se zákazníkem Microsoftu šablony](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>Možnost 2: Přijetí zákazníkem v Microsoft 365 admin Center

Partneři mohou prostřednictvím adresy URL pozvat nové a stávající zákazníky, aby smlouvu mohli zkontrolovat a přijmout v Microsoft 365 pro správu. V následujících několika částech si ukážeme, jak:

- Vytvořte nového zákazníka a požádejte ho, aby smlouvu zkontrolovat a přijmout.

- Pozvěte nového zákazníka, aby přezval a přijal vztah a smlouvu na prodejci.

- Pozvěte existujícího zákazníka, aby smlouvu zkontrolovat a přijmout.

>[!NOTE]
> Pomocí Partnerské centrum [API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) můžete získat stav přímého přijetí požadavku zákazníkem Smlouva se zákazníkem Microsoftu.  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Vytvoření nového zákazníka a pozvání zákazníka ke kontrola a přijetí smlouvy

Pomocí následujícího postupu vytvořte nového zákazníka v Partnerské centrum a pak ho pozvěte ke kontrola a přijetí tohoto Smlouva se zákazníkem Microsoftu v Microsoft 365 pro správu.

1. Na kartě **Zákazníci** v Partnerské centrum vyberte **Přidat zákazníka.**

2. V **části Informace o** účtu zadejte informace o novém zákazníkovi do všech požadovaných polí, včetně názvu společnosti zákazníka a primárního kontaktu.

3. V **části Customer Agreement**(Smlouva se zákazníkem) vyberte Customer (Zákazník) a přijměte Smlouva se zákazníkem Microsoftu v Microsoft 365 Admin **Center.** Vyplňte všechna další povinná pole na stránce.

4. Vyberte **Další: Projděte si** postup vytvoření tenanta zákazníka. 

>[!NOTE] 
>Noví zákazníci nemohou provést nákup, dokud nepřijme Smlouva se zákazníkem Microsoftu.  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Vytvořte nového zákazníka.":::

5. Když se v pracovním postupu nového zákazníka dostanete na obrazovku **Potvrzení,** uložte si přihlašovací údaje zákazníka. Tyto přihlašovací údaje budete muset zákazníkovi poskytnout později.

6. Mimo tuto Partnerské centrum vytvořte a odešlete e-mail, který pozve zákazníka, aby přijal Smlouva se zákazníkem Microsoftu v Microsoft 365 pro správu. Nezapomeňte do e-mailu zahrnout tyto položky:

   - Odkaz na tuto adresu [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (vyžaduje se přihlášení)

   - Přihlašovací údaje zákazníka, které jste si uložili v kroku 5.

7. Zákazník pak obdrží e-mailovou pozvánku od partnera a vybere adresu [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).

8. Zákazník se přihlásí k Microsoft 365 pro správu pomocí přihlašovacích údajů zákazníka, které jste poskytli.

9. Zákazník zaškrtnutím políčka přijme smlouvu se zákazníkem Microsoftu.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Požádejte nového zákazníka, aby zkontrolovat a přijmout vztah prodejce a Smlouva se zákazníkem Microsoftu 

Pomocí následujícího postupu pozvěte nového zákazníka, aby si prohlédněte a přijal vztah prodejce a Smlouva se zákazníkem Microsoftu. 

1. Na kartě **Zákazníci** v Partnerské centrum odkaz **Požádat o vztah prodejce.** 

2. Vygeneruje se automatická e-mailová šablona, včetně textu a parametrizované adresy URL, která přesměruje zákazníka do Microsoft 365 správce.

3. Můžete přizpůsobit automaticky vygenerované e-mailové šablony a pak vybrat **Zkopírovat do schránky** nebo **Otevřít v e-mailu.**

4. Pomocí této e-mailové šablony můžete zákazníka pozvat, aby přijal žádost o vztah **prodejce,** **a Smlouva se zákazníkem Microsoftu**. (Poznámka: V e-mailové pozvánce se ujistěte, že partner obsahuje také automaticky zadanou adresu URL a také nedávno vytvořené přihlašovací údaje zákazníka.)

   :::image type="content" source="images/mca/createrelationship.png" alt-text="vytvořte relaci.":::

5. Zákazník obdrží pozvánku e-mailem a klikne na parametrizovanou adresu URL. 

6. Zákazník se pomocí přihlašovacích údajů, které poskytnete v e-mailu, Microsoft 365 centru pro správu.

7. Zákazník zaškrtnutím políčka přijme vztah **prodejce a** **Smlouva se zákazníkem Microsoftu**. 

8. V rámci stejné adresy URL může zákazník zobrazit konsolidovaný seznam různých partnerů, se kterou pracuje. Mohou vybrat partnera a zobrazit podrobnosti.

   :::image type="content" source="images/mca/accept.jpg" alt-text="Přijměte smlouvu.":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Pozvání existujícího zákazníka ke kontrola a přijetí smlouvy

Pomocí následujícího postupu můžete pozvat stávajícího zákazníka, aby si tyto požadavky Smlouva se zákazníkem Microsoftu. 

1. Vytvořte e-mail zákazníka s vloženou adresou URL, která pozve zákazníka k přijetí Smlouva se zákazníkem Microsoftu.

2. Zákazník obdrží pozvánku e-mailem a klikne na adresu [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement). 

3. Zákazník zadá své přihlašovací údaje do Microsoft 365 admin Center.

4. Zákazník zaškrtnutím políčka přijme Smlouva se zákazníkem Microsoftu. 

5. V rámci stejné adresy URL může zákazník zobrazit konsolidovaný seznam různých partnerů, se které pracují. Mohou vybrat partnera a zobrazit podrobnosti.

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Zákazníka.":::

>[!NOTE]
>V některých scénářích zákazníci nemusí být schopni přímo přijmout Smlouva se zákazníkem Microsoftu. Další informace o těchto situacích najdete níže v části Dva scénáře, ve kterých potřebujete pro své zákazníky něco otestovat.

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a>Dva scénáře, kdy je potřeba to udělat jménem zákazníka

Existují dva scénáře, ve kterých zákazníci nemusí být schopni přímo přijmout Smlouva se zákazníkem Microsoftu v Microsoft 365 admin Center.

**Scénář 1:** Stávající zákazník zakoupil prostřednictvím existujícího partnerského vztahu jakoukoli z následujících možností: nabídky, předplatná softwaru nebo softwaru, rezervované instance nebo plán Azure. Zákazník se teď pokouší provést nový nákup (s výjimkou automatického prodlužování platnosti). Když zákazník klikne na adresu URL, zobrazí se zpráva "Kontaktujte svého partnera a potvrďte přijetí tohoto Smlouva se zákazníkem Microsoftu."  

**Pokud chcete** tento problém vyřešit: Musíte to protestovat jménem zákazníka.

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Snímek obrazovky Microsoft 365 stránce Centra pro správu s dotazem, jestli chcete kontaktovat svého partnera a potvrdit přijetí Smlouva se zákazníkem Microsoftu":::

**Scénář 2:** Stávající zákazník zakoupil jakoukoli z následujících nabídek, softwarových a softwarových předplatných, rezervovaných instancí a plánu Azure. Zákazník se teď pokouší provést nový nákup s novým partnerem.

Když zákazník klikne na adresu URL centra pro správu Microsoft 365 přijme nový partnerský vztah Microsoft 365 smlouvu, zobrazí se zpráva "Obraťte se na svého partnera a potvrďte souhlas s Smlouva se zákazníkem Microsoftu".  

**Pokud chcete** tento problém vyřešit: Musíte to protestovat jménem zákazníka.  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a>Potvrzení, že zákazník přijal smlouvu

Pokud se pokusíte vytvořit novou objednávku pro stávajícího zákazníka, u které jste to ještě nepotvrdili, zobrazí se výzva k dokončení potvrzení. Použijte k tomu následující postup.

1. Zadejte **jméno, příjmení,** **e-mailovou adresu** a telefonní číslo **(volitelné)** uživatele, který smlouvu přijal. 

2. V **části Datum přijetí smlouvy** zadejte příslušné datum. Tuto možnost nelze nastavit na budoucí datum.

3. Vyberte **Uložit a pokračovat**. 

## <a name="next-steps"></a>Další kroky

- [Ověření nebo aktualizace informací o profilu společnosti](update-your-partner-profile.md)
- [Smlouvy se zákazníkem Microsoftu (podle oblasti a jazyka)](Agreements.md)
