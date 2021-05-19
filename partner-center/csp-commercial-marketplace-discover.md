---
title: Seznam nabídek – komerční tržiště
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si, jak můžou partneři CSP používat Partnerské centrum k zobrazení nebo hledání na webu Marketplace pro nabídky SaaS nebo ceny od nezávislých výrobců softwaru (ISV).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ab30f8391df58155c8511dc628b1fefd94c8d768
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147968"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a>Objevte nabídky a ceny v partnerském centru komerční Marketplace

**Příslušné role**: globální správce | Agent správce

Pokud se nezávislí dodavatelé softwaru (ISV) rozhodli publikovat nabídku na komerčním webu Marketplace, můžou se také rozhodnout, jestli chtějí nabídku zpřístupnit v programu CSP. Pokud se rozhodne prodávat nabídku prostřednictvím programu CSP, měla by partnerům CSP zobrazit nabídku v oblasti tržiště partnerského centra.

Pokud se nabídka ISV nezobrazuje podle očekávání v partnerském centru, může to být z těchto důvodů:

- ISV rozhodl neprodávat nabídku prostřednictvím programu CSP. Některé produkty ISV například mohou být k dispozici v jiných oblastech komerčního tržiště (například v [Microsoft AppSource](https://appsource.microsoft.com/) a [Azure Marketplace](https://azuremarketplace.microsoft.com/)), ale nemusí se zobrazovat pro partnery v programu CSP v tržišti partnerského centra.

- ISV se rozhodla, že nabídku zpřístupní jenom pro zvolený počet partnerů CSP. Další informace o exkluzivních nabídkách najdete v části dále v tomto tématu nápovědy.

- Typ nabídky nemůže být transakční prostřednictvím partnerského centra nebo Azure Portal (například kontejnery nebo některé nabídky založené na používání).

- Fakturační země přidružených zákazníků nemusí být pro tuto nabídku ISV podporována.

## <a name="view-marketplace-offers-in-partner-center"></a>Zobrazit nabídky Marketplace v partnerském centru

Zobrazení dostupných komerčních nabídek pro Marketplace v programu CSP:

1. Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra a pak v levé navigační nabídce vyberte **CSP** .

2. Vyberte **prodávat** a potom na **Marketplace**. Ve výchozím nastavení se zobrazí produkty všech typů a kategorií.

3. Vyberte filtr podle typu nebo kategorie. Pomocí **vyhledávání** můžete také vyhledat konkrétní klíčová slova, názvy nabídek nebo názvy vydavatelů ISV.

4. V seznamu vyberte konkrétní nabídku produktů. Tím se zobrazí karta Přehled produktu, kde najdete další informace o nabídce. Mezi informace na této kartě můžou zahrnovat: 

    - Popis produktu nebo nabídky

    - Další informace o vydavateli ISV

    - Odkazy na dokumentaci nebo marketingové materiály nahrané vydavatelem ISV

    - Další možné kontakty isv pro zákaznickou podporu, techniku nebo kontakt pro program CSP

5. Pokud chcete zobrazit další informace o dostupných plánech, skladových cenách nebo plánech nabídky, vyberte kartu **Plány a** ceny. Na této kartě se zobrazí:

    - Trhy, na kterých máte tuto nabídku k dispozici

    - Seznam skladových položek nebo plánů dostupných pro nabídku

    - Ceny pro jednotlivé dostupné SKU nebo plány

## <a name="view-marketplace-offers-via-partner-center-apis"></a>Zobrazení nabídek marketplace prostřednictvím Partnerské centrum API

Partneři programu CSP mohou také pomocí rozhraní API vrátit seznam oprávněných nabídek. Způsobilé nabídky budou pouze nabídky SaaS ISV, které partner může prodávat prostřednictvím Partnerské centrum Marketplace. Pokud partneři používají rozhraní API k identifikaci nabídek v katalogu, přečtěte si pokyny k získání seznamu nabídek [pro trh.](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>Zobrazení nejnovějších cen nabídek Marketplace v Partnerské centrum

Nejnovější podrobnosti o cenách přidružené k nabídce najdete podle těchto kroků:

1. Přihlaste se Partnerské centrum [řídicího](https://partner.microsoft.com/dashboard)panelu a pak v levé navigační nabídce vyberte **CSP.**

2. Vyberte **Sell (Prodej)** a pak **Pricing and offers (Ceny a nabídky).**

3. Posuňte se dolů do **části Marketplace,** vyberte umístění a stáhněte si **ceny za Marketplace.** Tím se vygeneruje tabulka s nejnovějšími údaji o cenách pro SaaS, nabídkami na základě licencí a měřené nabídky dostupné od vydavatelů ISV. Tady se můžou objevit i některé ceny za aplikace Azure. Tyto informace se aktualizují každý den, takže si je můžete podle potřeby podívat na aktuální ceny.

4. Pokud produkt ISV obsahuje bezplatné zkušební období, zobrazí se v tabulce dva řádky pro daný produkt:

    - V jednom řádku se zobrazuje cena bezplatné zkušební verze nula. To znamená, že je k dispozici bezplatné zkušební období.

    - V druhém řádku se zobrazí cena a podmínky, které se použijí po skončení bezplatné zkušební doby.

Jako partner programu CSP můžete mít nárok na další pobídky spojené s některými komerčními nabídkami na webu Marketplace. Další informace o dalších motivech najdete v tématu [Příručka k motivaci CSP](https://aka.ms/partnerincentives) (vyžaduje přihlášení CSP).

## <a name="learn-about-marketplace-exclusive-offers"></a>Další informace o exkluzivních nabídkách Marketplace

Prodejci softwaru mají možnost zpřístupnit své nabídky pouze konkrétním partnerům v programu CSP. To se označuje jako exkluzivní nabídka. Všichni partneři v programu CSP můžou dál prohlížet všechny nabídky ISV v partnerském centru pro komerční tržišti, včetně nabídek označených jako exkluzivní.

Pokud nabídka není označená jako exkluzivní, můžou si tuto nabídku koupit všichni partneři (za předpokladu, **že se fakturační** země vybraného zákazníka shodují s dostupností země nabídky ISV).

U jakékoli nabídky označené jako exkluzivní budou ale moci zakoupit tuto nabídku pouze partneři vybraní ISV.

> [!NOTE]
> Pokud se zobrazí nabídka označená jako exkluzivní, kterou byste chtěli prodávat zákazníkům, kontaktujte nezávislého výrobce softwaru a požádejte ho o oprávnění k prodeji exkluzivní nabídky. Když si zobrazíte podrobnosti exkluzivní nabídky, může se zobrazit odkaz **ISV** , který můžete vybrat.

Pokud se chcete dozvědět víc o prostředí ISV na komerčním webu Marketplace, přečtěte si téma [poskytovatelé Cloud Solution Provider](/azure/marketplace/cloud-solution-providers).

Další informace o zkušenostech s CSP na webu Marketplace najdete v tématu [Přehled komerčního tržiště](csp-commercial-marketplace-overview.md).

## <a name="next-steps"></a>Další kroky

- [Nákup nabídek pro komerční web Marketplace](csp-commercial-marketplace-purchase.md)