---
title: Potvrzení souhlasu zákazníka se Smlouvou se zákazníkem Microsoftu
description: Partneři poskytovatele Cloud Solution Provider (CSP) musí před objednáním služeb Microsoft pro zákazníky potvrdit přijetí smlouvy se zákazníkem Microsoftu.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 05/05/2020
ms.openlocfilehash: 423cf1aab281ad8e77e03aa386b43360e1b99b3c
ms.sourcegitcommit: 6b03ff400d1350db9696f9b457fcfe710310c5d3
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/03/2020
ms.locfileid: "96570565"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement-in-the-csp-partner-program"></a>Potvrzení souhlasu zákazníka s zákaznickou smlouvou Microsoftu v partnerském programu CSP

**Platí pro**

- Partnerské centrum
- Centrum pro správu Microsoft 365

**Příslušné role**

- Agent správce
- Agent prodeje

Od 1. října 2019 společnost Microsoft do programu CSP představila **smlouvu o zákaznících Microsoftu** , aby nahradila smlouvu Microsoft Cloud. Přečtěte si další [pokyny](indirect-reseller-tasks-in-partner-center.md) pro nepřímé prodejce. Aby bylo možné zajistit migraci partnerů na novou smlouvu, obě dohody v programu CSP existovaly do 31. ledna 2020. Od 1. února 2020 smlouva o zákaznících Microsoftu nahradila smlouvu Microsoft Cloud.

Zákazníci mají dvě možnosti, jak přijmout zákaznickou smlouvu Microsoftu. 

**Možnost 1**: ověření partnerského serveru pro přijetí u zákazníka – partner může potvrdit přijetí zákazníkovi pomocí rozhraní API pro partnerské centrum a sady SDK nebo prostřednictvím řídicího panelu partnerského centra.

**Možnost 2**: přímé přijetí zákazníkem – partner může pozvat zákazníka přes adresu URL, aby si tuto smlouvu zkontroloval a přijal v centru pro správu Microsoft 365.

## <a name="access-microsoft-customer-agreement-template"></a>Přístup k šabloně zákaznických smluv Microsoftu

Nejnovější verzi šablony zákaznických smluv od Microsoftu si můžete stáhnout [ručně.](https://aka.ms/customeragreement) Smlouva o zákaznících Microsoftu je specifická pro danou zemi. Při požadavku na šablonu smlouvy o zákaznících Microsoftu nezapomeňte vybrat správnou zemi na základě umístění zákazníka.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>Možnost 1: potvrzení přijetí zákazníkem v partnerském centru

Partneři můžou potvrdit přijetí smlouvy o zákaznících Microsoftu v partnerském centru pro zákazníky, kteří mají nové a stávající zákazníky. Prodejci nemohou jménem svých zákazníků ověřit platnost a při dokončení ověření identity musí spolupracovat s jejich nepřímým zprostředkovatelem.

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

Pomocí následujících kroků můžete načíst potvrzení, že stávající zákazník přijal smlouvu o zákaznících Microsoftu. K tomu musíte být agentem správce nebo agentem pro prodej.

1. Vyberte **zákazníci** a pak vyhledejte a vyberte zákazníka, kterého chcete zobrazit.

2. Vyberte **informace o účtu**.

3. V části **Smlouva o zákaznících Microsoftu** se zobrazí potvrzení, jestli ho zákazník zadal nebo neposkytl.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Potvrzení přijetí zákazníkovi pomocí rozhraní API pro partnerské centrum a sady SDK

Pomocí rozhraní API a sady SDK partnerského centra můžete potvrdit přijetí smlouvy o zákaznících Microsoftu v rámci zákazníka. Podrobnosti o rozhraní API nebo sadě SDK najdete v tématu:

- [Získat metadata smlouvy pro zákaznickou smlouvu Microsoftu](/partner-center/develop/get-customer-agreement-metadata)

- [Potvrzení souhlasu zákazníka s zákaznickou smlouvou Microsoftu](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Získání potvrzení o přijetí smlouvy Microsoft Customer Agreement od zákazníka](/partner-center/develop/get-confirmation-of-customer-agreement)

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

3. V části **smlouva se zákazníkem** vyberte první možnost. **Zákazník se vyzve k přijetí smlouvy o zákaznících Microsoftu v centru pro správu Microsoft 365**. Vyplňte všechna další povinná pole na stránce.

4. Vyberte **Další: Zkontrolujte** a pokračujte postupem vytvoření tenanta zákazníka. 

>[!NOTE] 
>Noví zákazníci si nemůžou koupit nový nákup, dokud nepřijmou zákaznickou smlouvu Microsoftu.  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Vytvořit nového zákazníka":::

5. Až se dostanete na obrazovku pro **potvrzení** v pracovním postupu nový zákazník, uložte přihlašovací údaje zákazníka. Tyto přihlašovací údaje budete muset později poskytnout zákazníkovi.

6. Mimo partnerské Centrum vytvořte a odešlete e-mail, který vyzývá zákazníka, aby přijal zákaznickou smlouvu Microsoftu v centru pro správu Microsoft 365. Nezapomeňte zahrnout tyto položky do e-mailu:

   - Odkaz na tuto [adresu URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (vyžaduje se přihlášení)

   - Přihlašovací údaje zákazníka, které jste uložili v kroku 5.

7. Zákazník pak obdrží pozvánku e-mailu od partnera a vybere [adresu URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).

8. Zákazník se přihlásí do centra pro správu Microsoft 365 pomocí přihlašovacích údajů zákazníka dříve přijatých od partnera.

9. Zákazník pak toto políčko zkontroluje, aby přijal zákaznickou smlouvu od Microsoftu.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Pozvání nového zákazníka ke kontrole a přijetí vztahu prodejce a smlouvy o zákaznících Microsoftu 

Pomocí následujícího postupu můžete pozvat nového zákazníka ke kontrole a přijetí vztahu prodejce a smlouvy o zákaznících Microsoftu. 

1. Na kartě **zákazníci** v partnerském centru vyberte odkaz **požádat o vztah prodejce** . 

2. Automaticky se vytvoří šablona e-mailu, včetně textu a parametrizované adresy URL, která zákazníka přesměruje na centrum pro správu Microsoft 365.

3. Můžete přizpůsobit automaticky vygenerovanou šablonu e-mailu a pak vybrat **Kopírovat do schránky** nebo **otevřít v e-mailu**.

4. Tato e-mailová šablona slouží k pozvání zákazníka k přijetí žádosti o **vztah prodejce** a **smlouvy o zákaznících Microsoftu**. (Poznámka: v pozvánce k e-mailu zajistěte, aby partner zahrnoval taky adresu URL, která se automaticky zadala, a také přihlašovací údaje zákazníka, které se nedávno vytvořily.)

   :::image type="content" source="images/mca/createrelationship.png" alt-text="Vytvoření relace":::

5. Zákazník obdrží pozvánku prostřednictvím e-mailu a klikne na parametrizovanou adresu URL. 

6. Zákazník používá k přihlášení do centra pro správu Microsoft 365 přihlašovací údaje poskytnuté partnerem v rámci e-mailu.

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
>V některých scénářích nemusí zákazníci být schopni zákaznickou smlouvu od Microsoftu přijmout přímo. Další informace o těchto situacích najdete v tématu [dva scénáře, kdy potřebujete ověřit jménem svého zákazníka](attest-acceptance-customer-agreement.md).

### <a name="historical-timeline-details"></a>Podrobnosti historické časové osy

| Datum | RTM | Podrobnosti |
|------------|------------|--------------------------------|
|Srpen 01, 2019| Dostupná verze Preview v izolovaném prostoru| Partneři můžou potvrdit přijetí zákaznických smluv Microsoftu pomocí řídicího panelu partnerského centra v prostředí sandboxu CSP. Partneři s přístupem k prostředí izolovaného prostoru (CSP) ve verzi Preview se změnami zkušeností uživatelů. O změnách v tomto tématu se můžou dozvědět partneři bez přístupu k izolovanému prostoru.|
|Září 03, 2019|Rozhraní API Preview je dostupné v izolovaném prostoru (sandbox).|Partner může potvrdit přijetí zákaznických smluv Microsoftu pomocí rozhraní API partnerského centra v prostředí cloudového izolovaného prostoru (sandbox). Partneři rozhraní API můžou tuto příležitost využít k zobrazení náhledu změn rozhraní API a k podpoře nové smlouvy začít pracovat na integraci rozhraní API.|
|20. září 2019|Sada .NET SDK Preview je dostupná v izolovaném prostoru (sandbox).|Partner může potvrdit přijetí smlouvy o zákaznících Microsoftu pomocí partnerského centra .NET SDK v prostředí cloudového izolovaného prostoru (sandbox). Partneři rozhraní API můžou tuto příležitost využít k zobrazení náhledu změn sady .NET SDK a k podpoře nové smlouvy začít pracovat na integraci rozhraní API.|
|Říjen 01, 2019|Zákaznické smlouvy Microsoftu dostupné v produkčním prostředí|Společnost Microsoft se zavede na základě smlouvy o zákaznících Microsoftu k programu CSP, aby nahradila smlouvu Microsoft Cloud. Partneři můžou potvrdit přijetí zákaznických smluv Microsoftu pomocí řídicího panelu partnerského centra a rozhraní API v produkčním prostředí. Smlouva Microsoft Cloud zůstane podporovaná v rámci partnerského programu CSP. Nicméně partneři mají na začátku migrace na zákaznickou smlouvu Microsoftu. Nové nákupy a počty licencí u stávajících předplatných budou vyžadovat, aby se na základě souhlasu s zákaznickou smlouvou Microsoftu nebo Microsoft Cloud smlouvou. Některé nové nabídky (například nový plán Azure) budou vyžadovat potvrzení smlouvy o zákaznících Microsoftu.|
|31. ledna 2020|Microsoft Cloud smlouva se odebrala z produkčního prostředí.|Microsoft Cloud smlouva již není v partnerském programu CSP přijata. Nové nákupy a počty licencí u stávajících předplatných budou vyžadovat, aby partner poskytoval potvrzení smlouvy o zákaznících Microsoftu. Tento požadavek se vztahuje na nové zákazníky a stávající zákazníky, kteří mohli smlouvu Microsoft Cloud dřív přijali.|
|3. února 2020|Partner má teď možnost pozvat zákazníka přes adresu URL, aby si ho zkontroloval a přijal v centru pro správu ověřovaného Microsoft 365. | Zákazník může přijmout smlouvu o zákaznících Microsoftu v centru pro správu Microsoft 365. Přímé přijetí smlouvy zákazníka v centru pro správu Microsoft 365 potvrdí schválení podmínek. 