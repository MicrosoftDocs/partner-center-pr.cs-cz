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
ms.openlocfilehash: c25d4ab3077c6a0f648c767472e8b7b60ef53a9c
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148019"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a>Faktura za produkty a předplatné z komerčního tržiště v partnerském centru


**Příslušné role**: globální správce | Správce fakturace

Jako partner v programu CSP můžete použít Partnerské centrum k nákupu SaaS produktů založených na licencích od vydavatelů ISV na komerčním webu Marketplace. Až to uděláte, můžete pro tyto typy nákupů získat přístup k faktuře. Fakturační období začíná první den v kalendářním měsíci a končí poslední den v kalendářním měsíci. Faktury jsou k dispozici v 8. den následujícího měsíce.

K fakturám máte přístup z [řídicího panelu](https://partner.microsoft.com/dashboard/) partnerského centra nebo přes [rozhraní API partnerského centra](/partner-center/develop/).

Partneři v programu CSP se účtují podle řešení ISV Commercial Marketplace zakoupeného pro zákazníka, když si tyto produkty koupí z partnerského centra nebo z Azure Portal (pomocí předchozího poskytovatele Azure koupeného v rámci CSP).

>[!NOTE]
>Pokud zákazníci používají svůj tenant Azure AD (nekoupený od partnera v programu CSP), můžou si taky koupit své vlastní řešení ISV SaaS přímo z ([Microsoft AppSource](https://appsource.microsoft.com/) nebo [Azure Marketplace](https://azuremarketplace.microsoft.com/)). Pokud tomu tak je, obdrží svou vlastní faktura přímo od společnosti Microsoft. Podobně platí, že pokud partner v programu CSP prodává předplatné Azure nebo nový plán Azure pro zákazníka a udělí zákazníkovi (nebo nepřímému prodejci) [přístup na základě role](/azure/role-based-access-control/built-in-roles) k tomuto tenantovi (přiřazení jakékoli role k zákazníkovi kromě **čtecího zařízení**), může si zákazník (nebo nepřímý prodejce) zakoupit také nabídky komerčního tržiště bez předchozího schválení nebo oznámení partnerovi CSP. V těchto případech Microsoft neoznamuje partnerům v programu CSP informace o nákupech provedených svými zákazníky. Microsoft ale nabízí volitelný [](/azure/azure-monitor/platform/alerts-activity-log) mechanismus Azure Monitor, který můžete použít k nastavení upozornění nebo oznámení o aktivitě v předplatném Azure.

## <a name="access-billing-information-for-commercial-marketplace-products"></a>Přístup k fakturačním údajům pro produkty komerčního marketplace

Globální správce nebo správce fakturace vaší společnosti obdrží e-mail, jakmile bude faktura připravená k zobrazení. Přístup k nejnovější faktuře a souboru s vyrovnáním pro nákupy produktů na komerčním marketplace:

1. Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard/) pro Partnerské centrum.

2. V nabídce Partnerské centrum vyberte **Fakturace.** 

    V horní části stránky Fakturace se zobrazí dvě karty: **Opakované** a Opakované **a opakované nákupy.** Každá karta umožňuje přístup k souborům faktur a odsouhlasení (odsouhlasení) pro různé produkty z marketplace:

    - **Opakovaná** karta: Zobrazuje soubory faktur a odsouhlasení pro předplatná související s Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, Power BI Pro a Microsoft Azure.

    - **Karta Opakované a opakované nákupy:** Zobrazuje soubory faktur a odsouhlasení pro plán Azure, rezervace Azure, produkty softwarového a komerčního marketplace.
  
3. Vyberte kartu **Opakované a opakované** nákupy. Pokud jste si zakoupili předplatná pro zákazníka v jiné měně, zobrazí se karta pro každou měnu. Na této stránce můžete udělat několik věcí:

    - Pokud chcete zobrazit nejnovější fakturu a soubor s vyrovnáním, vyberte **Faktura** nebo **Soubor s vyrovnáním.** (Pokud chcete, můžete také získat přístup k nejnovější faktuře a odsoudíte data souborů [pomocí Partnerské centrum API.](/partner-center/develop/)

    - Pokud chcete zobrazit dřívější soubory faktur a odsouových vyúčtování, rozbalte řádek **Historie fakturace** níže.

    - Pokud chcete kdykoli zkontrolovat odhadovaný zůstatek účtu nebo fakturu na základě nejnovější aktivity účtu, vyberte odkaz pod **nadpisem Odhady.**  

    >[!NOTE]
    > Když fakturu zveřejňujeme 8. den v měsíci, bude zahrnovat daně a všechny ostatní příslušné poplatky a kredity. To znamená, že konečná splatná částka se může lišit od toho, co vidíte během fakturačního období.

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

- **Stránka 2 (a všechny následné stránky) faktury:** Podrobnosti se účtují jak pro nákupy od Microsoftu, tak pro nákupy od jiných výrobců ISV (na základě licencí) z komerčního tržiště. Nákupy na základě licencí isv můžete identifikovat na řádku **Vydavatel** pod každým názvem produktu. Přidružený soubor s vyrovnáním nabízí další podrobnosti fakturace pro konkrétní poplatky za fakturu.

- **Poslední stránka faktury:** Pokud vám od isv účtovány produkty z marketplace založené na licencích, na této poslední stránce se zobrazí další podrobnosti o názvu a adrese vydavatele ISV.

### <a name="tips-on-reading-your-reconciliation-file"></a>Tipy ke čtení souboru s vyrovnáním

Soubor **sesouhlasení** opakovaných a opakovaných nákupů obsahuje několik sloupců s dalšími podrobnostmi, které se mapuje na poplatky na faktuře. Ve **sloupci PublisherName** se zobrazuje, jestli nákup pochází od Microsoftu nebo od vydavatele ISV třetí strany.

Některé poplatky v souboru s vyrovnáním se dají zobrazit s náklady ve výši 0 USD. Důvodem může být nabídka bezplatné zkušební verze (obvykle 30 nebo 60 dnů) od výrobce softwaru nebo nabídka s vlastní licencí.

V případě nabídek bezplatných zkušebních verzí isv:

- Bezplatné zkušební období pokrývá během této doby náklady na produkt SaaS založený na licencích tohoto výrobce softwaru. Nebudou se vám účtovat ani poplatky za přidružené využití infrastruktury Azure pro tento produkt SaaS.  Pokud ale používáte nabídku isv na základě využití, bezplatná zkušební verze nezahrnuje náklady na využití základní infrastruktury Azure. V takovém případě se poplatky za využití infrastruktury Azure zobrazí v samostatném souboru s vyrovnáním v Azure.

- Když pro zákazníka zakoupíte a nasadíte bezplatný produkt způsobilý k zkušební verzi od isv, je tento zákazník automaticky zaregistrovan v bezplatné zkušební verzi vydavatelem ISV. Bezplatné zkušební období končí automaticky po období definovaném vydavatelem ISV. Po uplynutí této doby se zákazníkovi budou účtovat poplatky. To znamená, že soubor s vyrovnáním může u produktu s nárokem na zkušební verzi zobrazit dva řádky: jeden, který sleduje zkušební období a jeden, který sleduje placenou nabídku (zobrazí náklady ve výši 0 USD až do konce zkušebního období). Po ukončení zkušební verze začne řádek zobrazující placenou nabídku zobrazovat poplatky. 

Další informace o tom, co jednotlivé sloupce představují, najdete v tématu [použití souborů odsouhlasení](use-the-reconciliation-files.md). Viz také [typy fakturace v partnerském centru](./billing-basics.md) .

## <a name="next-steps"></a>Další kroky

- [Správa produktů z komerčního tržiště pro zákazníky](csp-commercial-marketplace-manage.md)
- [Další informace o podpoře pro komerční produkty na webu Marketplace](csp-commercial-marketplace-support.md)