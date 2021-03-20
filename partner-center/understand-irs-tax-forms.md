---
title: Vysvětlení daňových formulářů IRS vydaných Microsoftem
description: Seznamte se s daňovými formuláři vydanými Microsoftem, včetně toho, kdo je obdrží a kdy jsou zpřístupněni.
ms.topic: article
author: mingshen-ms
ms.author: mingshen
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.localizationpriority: medium
ms.date: 09/30/2020
ms.openlocfilehash: 42c5d6f0d31e6509253fe44d5b97606fc688f177
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712813"
---
# <a name="understand-irs-tax-forms-issued-by-microsoft"></a>Vysvětlení daňových formulářů IRS vydaných Microsoftem

Každý rok může obdržet jednu nebo více daňových formulářů od společnosti Microsoft. To závisí na vašem umístění a objemu prodejů nebo plateb, které obdržíte. Společnost Microsoft je nutná k vystavení těchto formulářů a jejich podávání pomocí služby interního výnosu (finančního úřadu).

V tomto článku se dozvíte víc o těchto formulářích, včetně toho, kdo je obdrží a kdy jsou zpřístupněni.

## <a name="types-of-tax-forms"></a>Typy daňových formulářů

| Daňový formulář finančního úřadu | Description | Dostupnost |
|--------------|-------------|--------------|
|1099 – RŮZNÉ, 1099 AŽ K | Související s aktivitou prodeje a/nebo platbami, které jste provedli při účasti na tržištích společnosti Microsoft. | Tištěné formuláře budou postmarked do **31. ledna** a budou k dispozici v [partnerském centru](https://partner.microsoft.com/dashboard) (v **Nastavení účtu partnerského centra** pod položkou **Výběr a daňové > výběr a daňové profily**) ve stejnou dobu. |
|1042-S | V souvislosti s platbami, které jste provedli, se vztahují na USA srážková daň. | Tištěné formuláře budou postmarked do **15. března** nebo do 15. kopie. PDF budou k dispozici v partnerském centru (v **nastavení pro vývojáře partnerského centra** v části **Výběr a daňové > výběr a daňové profily**) ve stejnou dobu.  |

> [!NOTE]
> Adresa, kterou používáme u daňových formulářů finančního úřadu, přichází z adresy v daňovém profilu při [nastavování účtu výběr a daňového formuláře](set-up-your-payout-account.md). Pokud se vaše adresa změnila, ujistěte se, že jste adresu aktualizovali v **daňovém profilu**.

Daňové formuláře vám budou odesílány z následujících adres:

**Občané USA:**

| Obchodní skupina         | Právnická osoba          | Adresa                                          |
|------------------------|-----------------------|--------------------------------------------------|
| Windows, Office, Azure | Microsoft Corporation | One Microsoft Way<br>Redmond, WA 98052 USA       |
| Inzerce a reklama            | Microsoft Online Inc. | 6880 Sierra Center Parkway<br>Reno, NV 98511 USA |

**Občané od jiných společností než USA:**

| Obchodní skupina         | Právnická osoba          | Adresa                                          |
|------------------------|-----------------------|--------------------------------------------------|
| Windows, Office, Azure | Microsoft Ireland Operations je omezený (platba provedená společností Microsoft Corporation prostřednictvím programu Microsoft Ireland, který působí jako kvalifikovaný prostředník pro společnost Microsoft Corporation) | Jedno místo na Microsoftu<br>Jižní okres – obchodní Park<br>Leopardstown, Dublin 18, D18 P521, Irsko|
| Inzerce a reklama          | Microsoft Ireland Operations je omezený (platba provedená společností Microsoft Online Inc. prostřednictvím Microsoft Irska, která funguje jako agent jako výběr pro Microsoft Online Inc.) | Jedno místo na Microsoftu<br>Jižní okres& Business Park<br>Leopardstown, Dublin 18, D18 P521, Irsko |
| Inzerce a reklama            | Microsoft Online Inc. | 6880 Sierra Center Parkway<br>Reno, NV 98511 USA |

>[!NOTE]
> \* Občané následujících zemí, které mají nárok na reklamu, se hradí prostřednictvím Microsoft Ireland operací s omezením: Rakousko, Belgie, Bulharsko, Chorvatsko, Kypr, CZECHIA, Dánsko, Indie, Finsko, Francie, Německo, Řecko, Irsko, Irsko, Indie, Indie, Indie, Lotyšsko, Indie, Indie, Indie, Portugalsko, Rakousko, Španělsko, Švédsko, Švýcarsko, Slovinsko, Jižní Afrika, Španělsko, Švédsko, Švýcarsko, Spojené království

## <a name="for-developers-located-in-the-united-states"></a>Pro vývojáře nacházející se v USA

| Pokud jsem vývojář USA prodávající placené aplikace a...   | Měl by se zobrazit tento formulář: |
|------------------------|-----------------------|
| Byl **větší než 200 prodej aplikací** s celkovou kupní výší těchto prodejů **větším než $20 000 USD** v příslušném daňovém **roce (** nepočítá prodej v Brazílii a Číně prostřednictvím Microsoft Store ve Windows 10.)| **1099 – K:**<br/>Souborového: Microsoft Corporation<br/>Ein: \* \* \* \* \* 4442<br/><br/>**Důležité informace:** Formulář 1099-K obsahuje **celkové částky nákupu** , nikoli platby, které jste udělali za vás.| 
| Obdržel (a) jsem mi **aspoň $10 plateb** za (i) prodej aplikace provedený v Brazílii a číně prostřednictvím Microsoft Store ve Windows 10 nebo (II) Sales na webu Minecraftu Marketplace.<br/><br/>**OR**<br/><br/>Obdrželi jsme aspoň $600 plateb, které nesouvisí s prodejem aplikací od Microsoftu v příslušném daňovém roce (například motivačními platbami nebo platbami po soutěži nebo povýšení).| **1099 – RŮZNÉ:**<br/>Plátce: Microsoft Corporation<br/>Ein: \* \* \* \* \* 4442<br/><br/>**Důležité informace:** Některé obchodní entity nezískají 1099 – různé formuláře bez ohledu na platební částky obdržené od Microsoftu.  Další informace vám poskytne váš daňový Specialist.| 
| Žádná z výše uvedených neplatí.| Žádné |
| <br/><br/>**Pokud jsem vývojář USA prodávající reklamy v aplikacích a...** |<br/><br/>**Měl by se zobrazit tento formulář:** |
|V rámci služby ADS v aplikacích v rámci příslušného daňového roku jsem obdržel **alespoň $600 plateb** . | **1099 – RŮZNÉ:**<br/>Plátce: Microsoft Online Inc<br/>Ein: \* \* \* \* \* 0505<br/><br/>**Důležité informace:** Některé obchodní entity nezískají 1099 – různé formuláře bez ohledu na platební částky obdržené od Microsoftu.  Další informace vám poskytne váš daňový Specialist. |
| Do plateb z reklam v aplikacích v rámci příslušného daňového roku jsem dostal **méně než $600** . | Žádné |


## <a name="for-developers-located-outside-of-the-united-states"></a>Pro vývojáře nacházející se mimo USA


| **Otázka** | **Odpověď** |
|---|---|
| **Obdržel (a) jsem formu 1042-S od Microsoftu. K čemu slouží?** | Společnost Microsoft vám poskytla formulář nebo formuláře ve formátu 1042, protože jsme vám zaplaceni výnosy, které se považují za hlášení USA daňovým úřadům a měla by se vztahovat na srážkovou daň.  Pro tento požadavek vytváření sestav se používá formulář 1042-S. | 
| **Co mám dělat s formuláři?** | Obecně platí, že žádná konkrétní akce není na vaší straně nutná. Pokud chcete pro své místní daňové úřady požádat o jakoukoli formu daňového kreditu, může vám být užitečná forma 1042-S.  Další informace o tomto tématu vám poskytne vlastní Poradce pro daně. | 
| **Proč se při dokončování formuláře W8 vyvolala daň na moje platby?** | Daně se zamítne, pokud:<br/><br/>1. nedokončili jste oddíl daňové smlouvy v W8 správně nebo <br/>2. jste rezidenti v zemi, která nemá daňovou smlouvu s USA.<br/><br/>Partnerské centrum můžete kdykoli navštívit a odeslat aktualizovaný W8 formulář.<br/><br/> **Poznámka:** Ne všechny výnosy podléhají srážkám daně. | 
| **Odeslal (a) jsem aktualizovaný W8 formulář s platnými informacemi o smlouvě. Dá se Microsoft vrátit k dani, která byla odmítnutá?** | Po zablokování daně není možné ji znovu vyfinancovat. Řekněte svým daňovým poradcům, aby projednali, jestli pro tyto daně můžete uplatnit nárok na místní kredit, nebo jestli můžete požádat o refundaci v rámci finančního úřadu. | 
| **Jaké prodeje jsou hlášeny na formuláři 1042-S?** | Pouze prodeje provedené **pro kupující nacházející se ve USA, které byly klasifikovány jako podléhající srážkám daně** .  Všechny ostatní prodeje nejsou považovány za sestavy. | 
| **Proč se mi v jedné obálce dostaly tři kopie stejné formy 1042-S?** | Nařízení finančního úřadu vyžadují, aby byly k dispozici tři kopie formuláře:<br/><br/>– Jeden pro záznamy příjemců<br/>– One pro podání u USA federální daňové vratky (Pokud je k dispozici)<br/>– Jeden pro podání s návratovou daní stavu USA (Pokud je k dispozici) |

> [!NOTE]
> Pokud máte další otázky nebo obavy související s **daňovými formuláři finančního úřadu**, najdete [informace v části pomoc a podpora](https://partner.microsoft.com/dashboard/support/) na řídicím panelu partnerského centra. Společnost Microsoft nemůže odpovídat na otázky související s vašimi konkrétními daňovými okolnostmi. v případě těchto otázek prosím vyžádejte svůj daňový specialista na radu.

## <a name="next-steps"></a>Další kroky

- [Vyplácení na komerčním marketplace](marketplace-get-paid.md)
