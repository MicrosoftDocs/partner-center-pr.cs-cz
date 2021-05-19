---
title: Správa licencování v nabídek marketplace
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak nastavit a spravovat licencování nabídek komerčního marketplace isv.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c128b99b034564bcaa100ca975253f8b1bad7a42
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147951"
---
# <a name="manage-licensing-in-marketplace-offers"></a>Správa licencování v nabídek marketplace

**Odpovídající role:** Globální správce | Správce účtu

Tento článek vás provede procesem nastavení nabídky v Partnerské centrum, zpřístupnění v Microsoft AppSource a následně správy licencí pro tuto nabídku.  

>[!IMPORTANT]
>Možnosti v tomto článku jsou aktuálně v Public Preview.

## <a name="before-you-begin"></a>Než začnete

### <a name="commercial-marketplace-basics"></a>Základy komerčního marketplace

Než s tímto procesem začnete, měli byste se seznámit se základy komerčního marketplace. Články v následující tabulce vám pomůžou začít. 

| Téma  | Článek  |
|-------|--------|
|Plány komerčního marketplace | [Plány a ceny nabídek komerčního marketplace](/azure/marketplace/plans-pricing)    |
|Nabídky komerčního marketplace  | [Výpis typů](/azure/marketplace/determine-your-listing-type)    |
|Účty komerčního marketplace |  [Vytvoření účtu komerčního marketplace v Partnerské centrum](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a>Určení ID vaší nabídky

V následujících postupech budete vyzváni k zadání ID nabídky. Chvíli si vymyslete vhodné ID nabídky s vezměte v paměti následující body:

- Toto ID se zákazníkům zobrazí na webové adrese nabídky marketplace a v Azure Resource Manager šablony, pokud jsou k dispozici.
- ID nabídky v kombinaci s ID vydavatele musí být dlouhé pod 40 znaky.
- Použijte při tom jenom malá písmena a číslice. ID nabídky může zahrnovat pomlčky a podtržítka, ale ne mezery. Pokud je například vaším vydavatelem ID `testpublisherid` a zadáte `test-offer-1` , bude webová adresa nabídky `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` .
- Toto ID se po výběru **vytvořit** nedá změnit.

### <a name="determine-your-offer-alias"></a>Určení aliasu nabídky

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

V tomto postupu definujete plán nebo plány, které chcete pro svou nabídku povolit.

1. V levé navigační nabídce vyberte **Přehled plánu** a pak vyberte Vytvořit **nový plán.**
2. Zadejte **ID plánu a** **název plánu** a pak vyberte **Vytvořit.**
3. Na stránce **Výpis** plánu zadejte popis **plánu**.
4. Pokud chcete popis uložit a dokončit ho později, vyberte **Save draft (Uložit koncept).**

5. Až budete hotovi, vyberte Zkontrolovat a **publikovat**. Informace o plánu se teď zobrazí v části appsource.microsoft.com výpisu nabídek (oddíl plány).

6. Po vytvoření všech plánů pro tuto nabídku budete muset zkopírovat ID služby každého plánu. V **horní části** stránky Výpis plánu vyberte Přehled plánu. Zkopírujte ID služby pro každý plán do bezpečného umístění.

## <a name="add-service-ids-to-your-solution"></a>Přidání ID služeb do řešení

Dalším krokem je aktualizace řešení přidáním ID služeb pro každý plán, který jste právě zkopíroval. Pokyny najdete v tématu [Vytvoření balíčku AppSource pro vaše řešení.](/powerapps/developer/data-platform/create-package-app-appsource)

## <a name="upload-your-package-and-publish-your-offer"></a>Nahrání balíčku a publikování nabídky

1. V levém navigačním podokně vyberte **Komerční marketplace** a pak vyberte **Technická konfigurace**.
2. V **části Základní licenční model** vyberte **Uživatel.**
3. V **části Crm Package**(Balíček CRM) zadejte adresu URL umístění vašeho balíčku.
4. Pomocí ostatních karet v levém navigačním podokně zadejte další požadované informace. Až budete hotovi, vyberte Zkontrolovat a **publikovat.**

Po publikování nabídky si vaše informace ověříme a ověříme. Pokud s tímto procesem dojde k nějakým potížím, budeme vás informovat. Po vyřešení všech problémů se zobrazí oznámení, že vaše nabídka bude k dispozici v AppSource. V tomto okamžiku ji můžete nastavit jako živou.

## <a name="make-your-offer-live-in-partner-center"></a>Zajištění živé nabídky v partnerském centru

Následující postup vás provede procesem zajištění živé nabídky v AppSource. Další informace o tomto procesu najdete v tématu [Úvod do možností výpisu](/azure/marketplace/determine-your-listing-type).

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

## <a name="register-isv-connect-deal-in-deal-registration"></a>Registrace ISV Connect v registraci koupí

Než budete moct přiřadit licence k zákazníkovi, musíte každý prodej zaregistrovat v partnerském centru. Pokud to chcete udělat, podívejte [se na stránku Registrace dohod.](register-deals.md)

## <a name="invite-the-customer"></a>Pozvání zákazníka

Pomocí následujícího postupu pozvěte zákazníka, aby se této dohody účastnil.  

1. Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard/).
2. V levé navigační nabídce vyberte **Komerční marketplace/ Přehled.**
3. V levé navigační nabídce vyberte **Referenční odkazy** a pak vyberte **Registrace dohody.**
4. **Vyfiltrujte Odeslané** dohody, vyberte **kartu Probíhá** a pak vyberte požadovanou dohodu.
5. Na stránce přehledu pro tuto dohodu vyberte **Spravovat licence.**
6. V **okně Spravovat licence** vyberte zákazníka z rozevíracího seznamu **Podrobnosti** o zákazníkovi. Pokud vztah se zákazníkem ještě neexistuje, vyberte + Pozvat nového zákazníka k **udělení souhlasu**.
7. Zkopírujte odkaz, který se zobrazí.
8. Pošlete tento odkaz e-mailem správci fakturace nebo globálnímu správci zákazníka a nechat je použít tento odkaz pro přístup k admin.microsoft.com a přijetí a autorizaci navazování vztahu.

    >[!NOTE]
    >Vztah nebude navázán, dokud zákazník tento krok neprovádí.

## <a name="activate-manage-and-remove-your-licenses"></a>Aktivace, správa a odebrání licencí

Jakmile s vám zákazník autorizovaným vztahem začne přidávat plány z nabídky a přiřazovat licence k jednotlivým plánům.

1. V okně Spravovat licence pro tuto dohodu vyberte **+ Přidat plán**.
2. Vyplňte **pole Plány pro toto** řešení **a** Počet licencí a pak vyberte **Aktualizovat licence.** Licence budou k dispozici na admin.microsoft.com, aby je zákazníci spravují a přiřazují zaměstnancům.

    - Pokud chcete změnit počet licencí pro existující plán, zadejte nové číslo do pole **Počet** licencí a pak vyberte **Aktualizovat licence.**

    - Pokud chcete deaktivovat nebo odebrat licence pro dohodu,  vyberte ikonu odpadkového koše v poli Akce a pak vyberte **Aktualizovat licence.**

## <a name="next-steps"></a>Další kroky

[Zdroje informací o licencování](support-resources-licensing.md)