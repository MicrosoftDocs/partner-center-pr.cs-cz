---
title: Daně a poplatky za místní službu PSTN
description: Jako partner Office 365, který slouží Microsoft 365m hlasovým produktům, se mohou vztahovat regionální daně, poplatky nebo zákonné požadavky na služby PSTN.
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5817e5bb010cee0ab280c83408167f28915a6237
ms.sourcegitcommit: 9b36128fdbd24e4bfe4597b1e6104bd560583c5c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/15/2020
ms.locfileid: "92527238"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>Regionální daně, předpisy pro služby PTSN (Public Switched Telephone Network)

**Platí pro**

- Partnerské centrum
- Partneři Office 365 s podporou Microsoft 365ch hlasových produktů

**Příslušné role**
-    Globální správce
-    Správce uživatelů
-    Agent správce

Služby veřejné komutované telefonní sítě (PSTN) v některých jurisdikcích mohou podléhat zvláštním daňovým a zákonným požadavkům, které mohou ovlivnit pořadí a fakturace partnerských serverů. V USA, včetně Portoriko, služeb PSTN, které zahrnují zvukové konference, volání plánů a komunikační kredity, se vztahují speciální daňové a zákonné požadavky. V USA a Portoriko jsou služby Microsoft cenami PSTN jako daně včetně.  Jedinečné daně a předpisy v PSTN budou mít vliv na partnery Office 365, kteří se Microsoft 365 hlasové produkty.  Pokud partner uvede cenu služby PSTN společnosti Microsoft, může být zodpovědná za výpočet a přesměrování daní a poplatků v síti PSTN.

## <a name="partner-recommendations"></a>Doporučení partnerů

Zapojte se do svého daňového a právního poradce a pochopte zodpovědnost vaší organizace ohledně předpisů, daní a poplatků za veřejné telefonní služby a dalších potenciálních závazků.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Prezentace faktury a soubor pro odsouhlasení s partnerským serverem

Soubory faktury CSP a odsouhlasení CSP v USA, Portoriko a Kanadě, které zahrnují službu Skype pro firmy a Microsoft 365 hlasové služby, poskytují samostatné položky řádku pro součásti veřejné sítě a jiné než PSTN.

Ve fakturách CSP se navíc zobrazí následující poznámka pod čarou:

* Zobrazená cena je poplatek za službu audio Conferencing a službu pro plánování volání.  Jakékoli použitelné transakční daně se účtují výhradně na zobrazené množství, s výjimkou prodejů provedených v rámci USA.  V USA je zobrazená cena DPH včetně poplatků za volání plánu a služeb zvukové konference a poplatků za daně a poplatky, které se musí účtovat.  Služby zvukového konferenčního a služeb pro naplánování se účtují podle afilace společnosti Microsoft autorizované k jejich poskytování.  Podrobnosti najdete v [multilicenčním programu společnosti Microsoft](https://go.microsoft.com/fwlink/?LinkId=690247).

## <a name="reconciliation-file-example"></a>Příklad souboru pro odsouhlasení

Office 365 Enterprise E5 prezentuje soubor pro odsouhlasení jako dvě řádkové položky se stejnými názvy a stejnými ID, ale každá položka řádku má jedinečnou jednotkovou cenu (například: $28,40 a $2,00). Tím se oddělí komponenta konferenčních konferencí Skypu pro firmy v rámci nabídky Office 365, takže můžete správně použít daně.

**Příklady odsouhlasení partnerů #1 (výběr sloupců):**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Poplatek za cyklus   |28,40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Poplatek za cyklus   |2,00   |

**Příklad odsouhlasení partnerů #2**

Microsoft 365 Business hlas dostupný v Kanadě má další komponenty zdanitelné na veřejné síti, které jsou konsolidovány na faktuře CSP (podobně jako u Office 365 E5, jsou uvedeny dvě řádkové položky, jeden pro součásti PSTN a druhý pro jiné součásti než PSTN).  Soubor pro odsouhlasení CSP pro Microsoft 365 Business hlas zobrazí všechny komponenty s zdanitelným odkazem na síť PSTN jednotlivě (jednotlivé komponenty veřejné sítě PSTN nebudou konsolidovány. Soubor CSV nebo nástroj rozhraní API).  Souhrn podrobností objednávky a fakturované částky pro zákazníky nalezené v souboru pro odsouhlasení budou odpovídat faktuře CSP.

## <a name="additional-resources"></a>Další zdroje
Další podrobnosti najdete na webu [Microsoft 365 pro partnery](https://www.microsoft.com/microsoft-365/partners/) .

