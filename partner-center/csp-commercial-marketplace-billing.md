---
title: Fakturace pro komerční produkty na webu Marketplace
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si, jak fakturace funguje pro produkty nebo předplatné ISV SaaS zakoupené pro zákazníky z komerčního tržiště v partnerském centru.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c03ab358b8fb6ab0f23ea5f42b9d35c6f6c2b80c
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/22/2020
ms.locfileid: "92527359"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a>Faktura za produkty a předplatné z komerčního tržiště v partnerském centru

**Platí pro**

- Partnerské centrum
- Partneři v programu CSP

**Příslušné role**

- Globální správce
- Správce fakturace

Jako partner v programu CSP můžete použít Partnerské centrum k nákupu SaaS produktů založených na licencích od vydavatelů ISV na komerčním webu Marketplace. Až to uděláte, můžete pro tyto typy nákupů získat přístup k faktuře. Fakturační období začíná první den v kalendářním měsíci a končí poslední den v kalendářním měsíci. Faktury jsou k dispozici v 8. den následujícího měsíce.

K fakturám máte přístup z [řídicího panelu](https://partner.microsoft.com/dashboard/) partnerského centra nebo přes [rozhraní API partnerského centra](/partner-center/develop/).

Partneři v programu CSP se účtují podle řešení ISV Commercial Marketplace zakoupeného pro zákazníka, když si tyto produkty koupí z partnerského centra nebo z Azure Portal (pomocí předchozího poskytovatele Azure koupeného v rámci CSP).

>[!NOTE]
>Pokud zákazníci používají svůj tenant Azure AD (nekoupený od partnera v programu CSP), můžou si taky koupit své vlastní řešení ISV SaaS přímo z ([Microsoft AppSource](https://appsource.microsoft.com/) nebo [Azure Marketplace](https://azuremarketplace.microsoft.com/)). Pokud tomu tak je, obdrží svou vlastní faktura přímo od společnosti Microsoft. Podobně platí, že pokud partner v programu CSP prodává předplatné Azure nebo nový plán Azure pro zákazníka a udělí zákazníkovi (nebo nepřímému prodejci) [přístup na základě role](/azure/role-based-access-control/built-in-roles) k tomuto tenantovi (přiřazení jakékoli role k zákazníkovi kromě **čtecího zařízení** ), může si zákazník (nebo nepřímý prodejce) zakoupit také nabídky komerčního tržiště bez předchozího schválení nebo oznámení partnerovi CSP. V těchto případech Microsoft neoznamuje partnerům v programu CSP informace o nákupech provedených svými zákazníky. Microsoft ale nabízí volitelný [Azure monitor](/azure/azure-monitor/platform/alerts-activity-log) mechanismus, který můžete použít k nastavení výstrah nebo oznámení o aktivitě v rámci předplatného Azure.

## <a name="access-billing-information-for-commercial-marketplace-products"></a>Přístup k informacím o fakturaci pro produkty z komerčního tržiště

Správce globálního správce nebo fakturace vaší společnosti obdrží e-mail, když je faktura připravena k zobrazení. Přístup k nejnovějšímu souboru faktury a odsouhlasení pro nákupy produktů z komerčního tržiště:

1. Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard/)partnerského centra.

2. V nabídce partnerského centra vyberte **fakturace** . 

    V horní části stránky fakturace se zobrazí dvě karty: **opakované** a **opakované a jednorázové nákupy** . Každá karta umožňuje přístup k souborům faktury a odsouhlasení (rekognoskaci) pro různé produkty na webu Marketplace:

    - Karta **perioda** : zobrazuje soubory faktury a odsouhlasení pro předplatné související s Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, Power BI Pro a Microsoft Azure.

    - Karta **opakovaná a jednorázová nákupy** : zobrazuje soubory faktury a odsouhlasení pro plán Azure, rezervace Azure, software a komerční produkty z webu Marketplace.
  
3. Vyberte kartu **opakované a jednorázové nákupy** . Pokud jste si zakoupili předplatné pro zákazníka v jiné měně, zobrazí se vám karta pro každou měnu. Můžete provést několik věcí fr: objekt OM této stránky:

    - Chcete-li zobrazit nejnovější soubor faktury a odsouhlasení, vyberte možnost soubor **faktury** nebo **odsouhlasení** . (Pokud jste chtěli, můžete také přistupovat k nejnovější faktuře a datům souborů rekognoskaci pomocí [rozhraní API partnerského centra](/partner-center/develop/).

    - Pokud chcete zobrazit dřívější faktury a soubory rekognoskaci, rozbalte níže uvedený řádek **historie fakturace** .

    - Pokud chcete na základě nejnovější aktivity účtu kontrolovat odhadované Saldo účtu nebo fakturovat, vyberte odkaz pod hlavičkou **odhady** .  

    >[!NOTE]
    > Když vyúčtujeme datum v 8. den v měsíci, bude se jednat o daně a další příslušné poplatky a kredity. To znamená, že poslední dlužná částka se může lišit od toho, co vidíte během fakturačního období.

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>Další informace o fakturách a rekognoskaci souborech pro produkty z komerčního tržiště

V této části najdete další informace o souborech faktury a odsouhlasení pro předplatná komerčního tržiště SaaS zakoupená pro zákazníky od třetích stran nezávislých vydavatelů.

Když v nabídce partnerského centra **vyberete možnost** **periodické a jednorázové nákupy** , získáte přístup k souborům faktur a odsouhlasení za poplatky související s nákupy od Microsoftu (First stran) a ISV (třetích stran). K těmto nákupům může přidružit:

- Předplatná SaaS (od vydavatelů Microsoftu nebo ISV)

- Plán Azure

- Rezervace Azure

- Jiný software založený na předplatném (od společnosti Microsoft nebo vydavatelů ISV)

Příklady těchto nákupů můžou zahrnovat software SUSE Linux (předplatné softwaru) nebo předplatné produktu Azure ISV SaaS.

>[!NOTE]
> Další informace o tom, jak číst faktury a soubory rekognoskaci, najdete v tématu [Přehled fakturace](billing.md).

### <a name="tips-on-reading-your-invoice"></a>Tipy pro čtení vaší faktury

Když si koupíte produkt SaaS založený na licenci od jiného vydavatele ISV, zobrazí se vám poplatky za licenční poplatky na faktuře. Platí to i v případě, že produkt SaaS ISV používá (nebo spotřebovává) základní prostředky infrastruktury Azure. Důvodem je skutečnost, že se poplatky za využití infrastruktury Azure na podnikovém produktu od zákazníka účtují přímo výrobci ISV. (Prodejci softwaru uvidí přidružené poplatky za využití Azure ve svém vlastním souboru pro odsouhlasení faktury za každodenní použití Azure.)

Vaše faktura bude obsahovat několik stránek:

- **Strana 1 faktury:** Obsahuje souhrnný přehled podrobností fakturace partnera programu CSP. Zahrnuje souhrn poplatků za fakturační období, číslo faktury, platební podmínku (NET 60 dní) a způsoby platby za službu, které se účtují podle drátu nebo pomocí kontroly.

- **Stránka 2 (a všechny následné stránky) faktury:** Podrobnosti se účtují jak pro nákupy od Microsoftu, tak pro nákupy od jiných výrobců ISV (na základě licencí) z komerčního tržiště. Nákupy na základě licencí ISV můžete identifikovat na řádku **vydavatele** pod každým názvem produktu. Přidružený soubor pro odsouhlasení nabízí další fakturační údaje za konkrétní poplatky za fakturu.

- **Poslední stránka faktury:** Pokud vám byly účtovány licence na webu Tržiště od nezávislého výrobce softwaru, zobrazí se na poslední stránce více podrobností o jménu a adrese vydavatele ISV.

### <a name="tips-on-reading-your-reconciliation-file"></a>Tipy pro čtení souboru odsouhlasení

Soubor pro odsouhlasení **opakujícího se a jednorázového nákupu** obsahuje několik sloupců s dalšími podrobnostmi, které se mapují na poplatky ve vaší faktuře. Sloupec **vydavatele** zobrazuje, zda je nákup od společnosti Microsoft nebo vydavatele ISV jiného výrobce.

Některé poplatky v souboru odsouhlasení se můžou zobrazit s náklady $0. Důvodem může být nabídka "bezplatné zkušební verze" ISV (obvykle 30 nebo 60 dní) nebo nabídka vlastní licence.

V případě bezplatného dodavatele softwaru pro bezplatné zkušební verze nabízí:

- Bezplatné zkušební období zahrnuje náklady na produkt SaaS založený na licenci ISV v této době. Nebudete se vám účtovat ani pro přidružené využití infrastruktury Azure tohoto produktu SaaS.  Pokud ale používáte nabídku ISV založenou na používání, bezplatná zkušební verze nezahrnuje náklady na základní využití infrastruktury Azure. V takovém případě se poplatky za využití infrastruktury Azure zobrazí v samostatném souboru pro odsouhlasení Azure.

- Když si koupíte a nasadíte produkt opravňující k bezplatné zkušební verzi nezávislého výrobce softwaru pro zákazníka, zákazník se automaticky zaregistruje v bezplatné zkušební verzi vydavatelem ISV. Bezplatné zkušební období skončí automaticky po období definovaném vydavatelem ISV. Po skončení období se bude účtovat zákazník. To znamená, že soubor pro odsouhlasení může zobrazit dva řádky pro produkt s nárokem na zkušební verzi: jeden, který sleduje zkušební období, a druhý, který sleduje placené nabídky (po skončení zkušebního období se zobrazí cena $0). Po skončení zkušebního období se v řádku zobrazujícím placenou nabídku začnou zobrazovat poplatky. 

Další informace o tom, co jednotlivé sloupce představují, najdete v tématu [použití souborů odsouhlasení](use-the-reconciliation-files.md). Viz také [typy fakturace v partnerském centru](billing-different-types.md) .

## <a name="next-steps"></a>Další kroky

- [Správa produktů z komerčního tržiště pro zákazníky](csp-commercial-marketplace-manage.md)
- [Další informace o podpoře pro komerční produkty na webu Marketplace](csp-commercial-marketplace-support.md)