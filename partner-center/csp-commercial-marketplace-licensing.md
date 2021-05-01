---
title: Správa licencování v nabídkách Marketplace
ms.topic: how-to
ms.date: 04/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se, jak nastavit a spravovat licencování pro vaše nabídky ISV komerčního tržiště.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3b2281696a2fe69253cd033eb2a7eef7fb3046f3
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284885"
---
# <a name="manage-licensing-in-marketplace-offers"></a>Správa licencování v nabídkách Marketplace

**Příslušné role**

- Globální správce
- Správce účtu

Tento článek vás provede procesem nastavení nabídky v partnerském centru, jejím zpřístupněním v Microsoft AppSource a následnou správou licencí pro tuto nabídku.  

>[!IMPORTANT]
>Možnosti v tomto článku jsou momentálně v Public Preview.

## <a name="before-you-begin"></a>Než začnete

Před zahájením tohoto procesu byste se měli seznámit s informacemi uvedenými níže.

### <a name="review-the-azure-marketplace-documentation"></a>Přečtěte si dokumentaci k Azure Marketplace

Níže uvedené články obsahují informace, které byste měli znát, než budete pokračovat. 

- [Vytvoření nabídky Dynamics 365 for Customer Engagement a PowerApps](https://docs.microsoft.com/azure/marketplace/dynamics-365-customer-engage-offer-setup)
- [Vytvoření účtu obchodního tržiště v partnerském centru](https://docs.microsoft.com/azure/marketplace/create-account)

### <a name="create-your-offer-id"></a>Vytvoření ID nabídky

V níže uvedených postupech budete vyzváni k zadání ID nabídky. Pořiďte si čas, který vám umožní začít s vhodným ID nabídky. Pamatujte na tyto body:

- Toto ID je viditelné pro zákazníky na webové adrese pro nabídku webu Marketplace a šablony Azure Resource Manager, pokud jsou k dispozici.
- ID nabídky v kombinaci s ID vydavatele musí být kratší než 40 znaků.
- Použijte při tom jenom malá písmena a číslice. ID nabídky může zahrnovat pomlčky a podtržítka, ale ne mezery. Pokud je například ID vydavatele testpublisherid a zadáte test-nabídka-1, bude webová adresa nabídky https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1 .
- Toto ID se po výběru **vytvořit** nedá změnit.

### <a name="create-your-offer-alias"></a>Vytvoření aliasu nabídky

Alias nabídky je název, který se používá pro nabídku v partnerském centru. Budete také potřebovat příslušný alias nabídky, který bude postupovat podle níže uvedených pokynů:

- Tento název se na webu Marketplace nepoužívá a liší se od názvu nabídky a dalších hodnot, které se zákazníkům zobrazují.
- Po výběru vytvořit se tento název nedá změnit.

## <a name="create-your-offer"></a>Vytvoření nabídky

Prvním krokem v licenčním procesu je vytvoření komerční nabídky na webu Marketplace. 

1. Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard/).
2. V levé navigační nabídce vyberte **komerční Marketplace/přehled**.
3. V horní části stránky přehled vyberte možnost **Nová nabídka** a potom vyberte **Dynamics 365 pro customer Engagement & PowerApps**.
4. Zadejte **ID nabídky** a **alias nabídky** , který jste vytvořili dříve.
5. Vyberte **vytvořit** pro vygenerování nabídky a pokračování.
6. Vyberte možnosti licencování.

    - Pokud chcete pro vaši nabídku povolit správu licencí, vyberte **Povolit správu licencí aplikací prostřednictvím Microsoftu**. Jedná se o jednorázové nastavení a po publikování vaší nabídky ho nemůžete změnit.

    - Zákazníkům taky můžete povolit, aby se základní funkce vaší aplikace spouštěli bez licence, a po zakoupení licence mohli používat prémiové funkce. Pokud to chcete provést, vyberte možnost **Povolit zákazníkům instalaci aplikace i v případě, že licence nejsou přiřazeny**.

    - Pokud nechcete, aby vaše nabídka měla povolenou správu licencí, vyberte **získat hned (zdarma)**, **bezplatnou zkušební verzi** nebo **kontaktujte mě**.

## <a name="create-your-plan"></a>Vytvoření plánu

V těchto krocích budete definovat plán nebo plány, které chcete pro vaši nabídku povolit.

1. V levém navigačním panelu vyberte **plán přehled** a pak vyberte **vytvořit nový plán**.
2. Zadejte **ID plánu** a **název plánu** a pak vyberte **vytvořit**.
3. Na stránce **seznam plánů** zadejte svůj **Popis plánu**.
4. Pokud chcete popis Uložit a dokončit později, vyberte **Uložit koncept**.

5. Až budete hotovi, vyberte **zkontrolovat a publikovat**. Informace o plánu se teď budou zobrazovat na appsource.microsoft.com v části Seznam nabídek (oddíl plány).

6. Po vytvoření všech plánů této nabídky budete muset zkopírovat ID služby každého plánu. V horní části stránky se seznamem plánů vyberte **plán – přehled** . Zkopírujte ID služby pro každý plán do bezpečného umístění.

## <a name="add-service-ids-to-your-solution"></a>Přidání ID služeb do řešení

Dalším krokem je aktualizace řešení přidáním ID služby pro každý plán, který jste právě zkopírovali. Pokyny k tomuto problému najdete v tématu [Vytvoření balíčku AppSource pro vaše řešení](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).

## <a name="upload-your-package-and-publish-your-offer"></a>Nahrání balíčku a publikování vaší nabídky

1. V levém navigačním podokně vyberte **komerční web Marketplace** a pak vyberte **Technická konfigurace**.
2. V části **základní licenční model** vyberte **uživatel**.
3. V části **balíček CRM** zadejte adresu URL umístění balíčku.
4. Další karty v levém navigačním podokně použijte k zadání jakýchkoli dalších požadovaných informací. Až budete hotovi, vyberte **zkontrolovat a publikovat**.

Po publikování této nabídky si probereme a ověříte vaše informace. Pokud s tímto procesem dojde k nějakým potížím, budeme vás informovat. Po vyřešení všech problémů se zobrazí oznámení, že vaše nabídka bude k dispozici v AppSource. V tomto okamžiku ji můžete nastavit jako živou.

## <a name="make-your-offer-live-in-partner-center"></a>Zajištění živé nabídky v partnerském centru

Následující postup vás provede procesem zajištění živé nabídky v AppSource. Další informace o tomto procesu najdete v tématu [Úvod do možností výpisu](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).

>[!NOTE]
>Po publikování vaší nabídky bude trvat 4-6 hodin, než budete moct zasílat.

1. Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard/).
2. V levé navigační nabídce vyberte **komerční Marketplace/přehled**.
3. Na stránce **Přehled** Najděte nabídku, kterou hledáte. Nabídky připravené k publikování budou mít stav **Preview**. Vyberte nabídku.
4. Na stránce **Přehled nabídky** vyberte možnost **Přejít na aktivní**.
Nabídka bude živá během 4-6 hodin.
5. Pokud chcete zobrazit seznam nabídek na AppSource, vyberte odkaz **AppSource** v dolní části stránky s **přehledem nabídky** .

    - **Pro nabídky s povolenými licencemi**: Pokud vaše nabídka vyžaduje kontrolu licencí, uživatelé budou moct zadat zájemce jenom tak, že kliknou na **kontaktovat**, abyste s nimi mohli komunikovat.

    - **U nabídek s povolenými licencemi s možností bezplatné instalace**: Pokud vaše nabídka nevyžaduje kontrolu licencí, uživatelům s oprávněními správce se zobrazí tlačítko **získat nyní** , aby se **mi kontaktovalo**. Uživatelé, kteří chtějí vyzkoušet možnost bezplatné instalace, by měli kliknout na **získat hned**, což jim umožní nainstalovat nabídku do centra pro správu Power Platform. Pokud mají uživatelé nějaké dotazy nebo pokud chtějí upgradovat na placený plán, můžou pořád použít **kontakt** .

## <a name="register-isv-connect-deal-in-dealreg"></a>Registrace ISV Connect v DealReg

Dalším krokem je registrace vaší koupě. Postup najdete v tématu [registrace vašich obchodů](https://docs.microsoft.com/partner-center/register-deals).

## <a name="invite-the-customer"></a>Pozvat zákazníka

Následující postup slouží k pozvání zákazníka k účasti v této koupi.  

1. Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard/).
2. V levé navigační nabídce vyberte **komerční Marketplace/přehled**.
3. Filtr pro **odeslané** obchody vyberte kartu **probíhá** a pak vyberte obchod, kterou chcete.
4. Na stránce Přehled této práce vyberte **spravovat licence**.
5. V okně **spravovat licence** vyberte zákazníka v rozevíracím seznamu **Podrobnosti o zákazníkovi** . Pokud ještě neexistuje vztah zákazníka, vyberte **+ pozvat nového zákazníka k souhlasu**.
6. Zkopírujte zobrazený odkaz.
7. Tento odkaz odešlete e-mailem zákazníkovi nebo globálnímu správci fakturace zákazníka a požádejte ho, aby používali tento odkaz k přístupu k admin.microsoft.com a přijetí a autorizaci vztahu, který vytváříte.

    >[!NOTE]
    >Relace nebude navázána, dokud zákazník neprovede tento krok.

## <a name="activate-manage-and-remove-your-licenses"></a>Aktivace, Správa a odebírání licencí

Po navázání zákazníka můžete začít přidávat plány z nabídky a přiřazovat licence k jednotlivým plánům.

1. V okně Spravovat licence pro tento obchod vyberte **+ Přidat plán**.
2. Dokončete **plány pro toto řešení** a **počet licencí** a pak vyberte **aktualizovat licence**. Licence budou k dispozici na adrese admin.microsoft.com, aby si zákazníci mohli spravovat a přiřazovat k zaměstnancům.

    - Pokud chcete změnit počet licencí pro existující plán, zadejte nové číslo do pole **počet licencí** a pak vyberte **aktualizovat licence**.

    - Pokud chcete deaktivovat nebo odebrat licence pro určitý obchod, vyberte v poli **Akce** ikonu odpadkového koše a pak vyberte **aktualizovat licence**.