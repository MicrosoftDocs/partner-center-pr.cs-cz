---
title: Daně a poplatky za místní službu PSTN
description: Jako partner Office 365, který slouží Microsoft 365m hlasovým produktům, se mohou vztahovat regionální daně, poplatky nebo zákonné požadavky na služby PSTN.
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 85eefb49cf62c4bcfa5533683abd8ddb0e854463
ms.sourcegitcommit: 09eabb559aae25518caf3f2a59ef16a3e123c207
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/23/2021
ms.locfileid: "112490066"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>Regionální daně, předpisy pro služby PTSN (Public Switched Telephone Network)

**Příslušné role**: globální správce | Správce uživatelů | Agent správce

Služby veřejné komutované telefonní sítě (PSTN) v některých jurisdikcích mohou podléhat zvláštním daňovým a zákonným požadavkům, které mohou ovlivnit pořadí a fakturace partnerských serverů. V USA, včetně Portoriko, služeb PSTN, které zahrnují zvukové konference, volání plánů a komunikační kredity, se vztahují speciální daňové a zákonné požadavky. V USA a Portoriko jsou služby Microsoft cenami PSTN jako daně včetně.  Jedinečné daně a předpisy v PSTN budou mít vliv na partnery Office 365, kteří se Microsoft 365 hlasové produkty.  Pokud partner uvede cenu služby PSTN společnosti Microsoft, může být zodpovědná za výpočet a přesměrování daní a poplatků v síti PSTN.

## <a name="partner-recommendations"></a>Doporučení partnerů

Zapojte se do svého daňového a právního poradce a pochopte zodpovědnost vaší organizace ohledně předpisů, daní a poplatků za veřejné telefonní služby a dalších potenciálních závazků.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Prezentace faktury a soubor pro odsouhlasení s partnerským serverem

Faktury poskytovatele Cloud Solution Provider (CSP) a soubory odsouhlasení CSP v USA, Portoriko a Kanadě, které zahrnují službu Skype pro firmy pro veřejné telefonní služby a Microsoft 365 hlasové služby, budou poskytovat samostatné položky řádku pro součásti veřejné sítě a jiné než veřejné telefonní služby.

Ve fakturách CSP se navíc zobrazí následující poznámka pod čarou:

* Zobrazená cena je poplatek za službu audio Conferencing a službu pro plánování volání.  Jakékoli použitelné transakční daně se účtují výhradně na zobrazené množství, s výjimkou prodejů provedených v rámci USA.  V USA je zobrazená cena DPH včetně poplatků za volání plánu a služeb zvukové konference a poplatků za daně a poplatky, které se musí účtovat.  Služby zvukového konferenčního a služeb pro naplánování se účtují podle afilace společnosti Microsoft autorizované k jejich poskytování.  Podrobnosti najdete v [multilicenčním programu společnosti Microsoft](https://go.microsoft.com/fwlink/?LinkId=690247).

## <a name="reconciliation-file-example"></a>Příklad souboru pro odsouhlasení

Office 365 Enterprise E5 prezentuje soubor pro odsouhlasení jako dvě řádkové položky se stejnými názvy a stejnými ID, ale každá položka řádku má jedinečnou jednotkovou cenu (například: $28,40 a $2,00). Tím se oddělí komponenta konferenčních konferencí Skypu pro firmy v rámci nabídky Office 365, takže můžete správně použít daně.

**Příklady odsouhlasení partnerů #1 (výběr sloupců):**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Poplatek za cyklus   |28.40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Poplatek za cyklus   |2,00   |

**Příklad odsouhlasení partnerů #2**

Microsoft 365 Business hlas dostupný v Kanadě má další komponenty zdanitelné na veřejné síti, které jsou konsolidovány na faktuře CSP (podobně jako u Office 365 E5, jsou uvedeny dvě řádkové položky, jeden pro součásti PSTN a druhý pro jiné součásti než PSTN).  Soubor pro odsouhlasení CSP pro Microsoft 365 Business hlas zobrazí všechny komponenty s zdanitelným odkazem na síť PSTN jednotlivě (jednotlivé komponenty veřejné sítě PSTN nebudou konsolidovány v .CSV nebo nástroji rozhraní API).  Souhrn podrobností objednávky a fakturované částky pro zákazníky nalezené v souboru pro odsouhlasení budou odpovídat faktuře CSP.

## <a name="additional-resources"></a>Další materiály
Další podrobnosti najdete na webu [Microsoft 365 pro partnery](https://www.microsoft.com/microsoft-365/partners/) .

