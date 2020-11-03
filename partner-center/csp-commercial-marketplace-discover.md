---
title: Seznam nabídek – komerční tržiště
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si, jak můžou partneři CSP používat Partnerské centrum k zobrazení nebo hledání na webu Marketplace pro nabídky SaaS nebo ceny od nezávislých výrobců softwaru (ISV).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cb7b4ffdb4edf75e3e121e4ddea6b9de191ddbbf
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/22/2020
ms.locfileid: "92527358"
---
# <a name="discover-offers-and-pricing-in-the-partner-center-commercial-marketplace"></a>Seznamte se s nabídkami a cenami na komerčním tržišti partnerského centra

**Platí pro**

- Partnerské centrum
- Partneři v programu CSP

**Příslušné role**

- Globální správce
- Agent správce

Pokud se nezávislí dodavatelé softwaru (ISV) rozhodli publikovat nabídku na komerčním webu Marketplace, můžou se také rozhodnout, jestli chtějí nabídku zpřístupnit v programu CSP. Pokud se rozhodnete tuto nabídku prodávat prostřednictvím programu CSP, měla by partnerům CSP zobrazit nabídku v oblasti tržiště partnerského centra.

Pokud se nabídka ISV nezobrazuje v partnerském centru podle očekávání, může to být z těchto důvodů:

- ISV rozhodl neprodávat nabídku prostřednictvím programu CSP. Některé produkty ISV například mohou být k dispozici v jiných oblastech komerčního tržiště (například v [Microsoft AppSource](https://appsource.microsoft.com/) a [Azure Marketplace](https://azuremarketplace.microsoft.com/)), ale nemusí se zobrazovat pro zprostředkovatele CSP v tržišti partnerského centra.

- ISV se rozhodla, že nabídku zpřístupní jenom pro zvolený počet partnerů CSP. Další informace o exkluzivních nabídkách najdete v části dále v tomto tématu nápovědy.

- Typ nabídky nemůže být transakční prostřednictvím partnerského centra nebo Azure Portal (například kontejnery nebo některé nabídky založené na používání).

- Fakturační země přidružených zákazníků nemusí být pro tuto nabídku ISV podporována.

## <a name="view-marketplace-offers-in-partner-center"></a>Zobrazit nabídky Marketplace v partnerském centru

Zobrazení dostupných komerčních nabídek pro Marketplace v programu CSP: 

1. Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard)partnerského centra a v levé navigační nabídce vyberte **CSP** .

2. Vyberte **prodávat** a potom na **Marketplace** . Ve výchozím nastavení se zobrazí produkty všech typů a kategorií.

3. Vyberte filtr podle typu nebo kategorie. Pomocí **vyhledávání** můžete také vyhledat konkrétní klíčová slova, názvy nabídek nebo názvy vydavatelů ISV.

4. Vyberte ze seznamu konkrétní nabídku produktu. Tím přejdete na kartu Přehled produktu, kde můžete získat další informace o této nabídce. Informace na této kartě můžou zahrnovat: 

    - Popis produktu nebo nabídky

    - Další informace o vydavateli ISV

    - Odkazy na dokumentaci nebo marketingové materiály odeslané vydavatelem ISV

    - Další možné kontakty ISV pro zákaznickou podporu, inženýrství nebo kontaktní osoby pro program CSP

5. Pokud chcete zobrazit další informace o dostupných plánech, SKU nebo cenách nabídky, vyberte kartu **plány a ceny** . Na této kartě se zobrazí:

    - Trhy, na kterých je tato nabídka k dispozici

    - Seznam SKU nebo plánů dostupných pro nabídku

    - Ceny pro každou dostupnou SKU nebo plán

## <a name="view-marketplace-offers-via-partner-center-apis"></a>Zobrazení nabídek Marketplace prostřednictvím rozhraní API partnerského centra

Partneři programu CSP můžou také použít rozhraní API k vrácení seznamu oprávněných nabídek. Opravňující nabídky budou jenom SaaS prodejci softwaru, kteří jsou k dispozici pro partnery, kteří prodávají prostřednictvím tržiště partnerského centra. Partnerům, kteří používají rozhraní API k identifikaci nabídek v katalogu, najdete v pokynech k [získání seznamu nabídek pro trh](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market).

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>Zobrazit nejnovější ceny nabídky na webu Marketplace v partnerském centru

Pomocí těchto kroků získáte nejnovější informace o cenách spojené s nabídkou:

1. Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard)partnerského centra a v levé navigační nabídce vyberte **CSP** .

2. Vyberte **prodávat** a potom klikněte na **ceny a nabídky** .

3. Posuňte se dolů k části **Marketplace** , vyberte umístění a Stáhněte si **ceny na webu Marketplace** . Tím se vygeneruje tabulka s nejnovějšími údaji o cenách pro SaaS. nabídky založené na licencích, které jsou k dispozici od vydavatelů ISV. Tady se můžou objevit i některé ceny za aplikace Azure. Tyto informace se aktualizují každý den, takže si je můžete podle potřeby podívat na aktuální ceny.

4. Pokud produkt ISV obsahuje bezplatné zkušební období, zobrazí se v tabulce dva řádky pro daný produkt:

    - V jednom řádku se zobrazuje cena bezplatné zkušební verze nula. To znamená, že je k dispozici bezplatné zkušební období.

    - V druhém řádku se zobrazí cena a podmínky, které se použijí po skončení bezplatné zkušební doby.

Jako partner programu CSP můžete mít nárok na další pobídky spojené s některými komerčními nabídkami na webu Marketplace. Další informace o dalších motivech najdete v tématu [Příručka k motivaci CSP](https://aka.ms/partnerincentives) (vyžaduje přihlášení CSP).

## <a name="learn-about-marketplace-exclusive-offers"></a>Další informace o exkluzivních nabídkách Marketplace

Prodejci softwaru mají možnost zpřístupnit své nabídky pouze konkrétním partnerům v programu CSP. To se označuje jako exkluzivní nabídka. Všichni partneři v programu CSP můžou pořád Zobrazit všechny nabídky ISV v partnerském centru pro komerční obchod, včetně nabídek označených jako exkluzivní.

Pokud nabídka není označená jako exkluzivní, můžou si tuto nabídku koupit všichni partneři (za předpokladu, **že se fakturační** země vybraného zákazníka shodují s dostupností země nabídky ISV).

U jakékoli nabídky označené jako exkluzivní budou ale moci zakoupit tuto nabídku pouze partneři vybraní ISV.

> [!NOTE]
> Pokud se zobrazí nabídka označená jako exkluzivní, kterou byste chtěli prodávat zákazníkům, kontaktujte nezávislého výrobce softwaru a požádejte ho o oprávnění k prodeji exkluzivní nabídky. Když si zobrazíte podrobnosti exkluzivní nabídky, může se zobrazit odkaz **ISV** , který můžete vybrat.

Pokud se chcete dozvědět víc o prostředí ISV na komerčním webu Marketplace, přečtěte si téma [poskytovatelé Cloud Solution Provider](/azure/marketplace/cloud-solution-providers).

Další informace o zkušenostech s CSP na webu Marketplace najdete v tématu [Přehled komerčního tržiště](csp-commercial-marketplace-overview.md).

## <a name="next-steps"></a>Další kroky

- [Nákup nabídek pro komerční web Marketplace](csp-commercial-marketplace-purchase.md)