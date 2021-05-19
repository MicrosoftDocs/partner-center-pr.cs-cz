---
title: Soubory s vyrovnáním na základě licencí
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si, jak číst soubory s vyrovnáním na základě licencí v Partnerské centrum. Tento článek vysvětluje význam jednotlivých polí v souboru s rekonsekcemi na základě licencí.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 041f0fadfea107027ae1d9796d235700e66e6834
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146574"
---
# <a name="understand-the-fields-in-partner-center-license-based-reconciliation-files"></a>Principy polí v Partnerské centrum s vyrovnáním na základě licencí

**Platí pro**: Partnerské centrum | Partnerské centrum pro Microsoft Cloud for US Government

**Odpovídající role:** Globální správce | Správce správy uživatelů | Správce fakturace | Agent pro správu

Pokud chcete odsouhlasit změny s  objednávkami zákazníka, porovnejte Syndication_Partner_Subscription_Number ze souboru s vyrovnáním s **ID** předplatného z Partnerské centrum.

## <a name="fields-in-license-based-reconciliation-files"></a>Pole v souborech s vyrovnáním na základě licencí

| Sloupec | Popis | Ukázková hodnota |
| ------ | ----------- | ------------ |
| ID partnera | Jedinečný identifikátor ve formátu GUID pro konkrétní fakturační entitu Nevyžaduje se pro sesouhlasení. Stejné ve všech řádcích. | *8ddd03642-test-test-46b58d356b4e* |
| CustomerId | Jedinečný identifikátor Microsoftu pro zákazníka ve formátu GUID | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| CustomerName | Název organizace zákazníka, jak je hlášeno v Partnerské centrum. *Velmi důležité pole pro odsoustavu faktury s informacemi o systému.* | *Test zákazníka A* |
| ID mpn | Identifikátor MPN partnera CSP. Podívejte [se, jak položky zařazovat podle partnera.](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner) | *4390934* |
| ResellerMpnId | Identifikátor MPN prodejce záznamu pro předplatné.  |
| OrderId | Jedinečný identifikátor pro objednávku na platformě fakturace Microsoftu. Může být užitečné k identifikaci objednávky při kontaktování podpory. Nepoužívá se pro odsouhlasení. | *566890604832738111* |
| SubscriptionId | Jedinečný identifikátor předplatného na platformě fakturace Microsoftu Může být užitečné k identifikaci předplatného při kontaktování podpory. Nepoužívá se pro odsouhlasení. *Tato hodnota se neshoduje s **ID předplatného** v konzole pro správu partnerů. Místo toho se prosím podívejte na **SyndicationPartnerSubscriptionNumber** .* | *usCBMgAAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | Jedinečný identifikátor předplatných. Zákazník může mít několik předplatných pro stejný plán. Tento sloupec je důležitý pro účely analýzy souborů pro odsouhlasení. Toto pole se mapuje na **ID předplatného** v konzole pro správu partnera. | *fb977ab5-test-test-test-24c8d9591708* |
| Hodnotami OfferId | Jedinečný identifikátor nabídky Standardní identifikátor nabídky, jak je definován v ceníku. *Tato hodnota neodpovídá **ID nabídky** z ceníku. Místo **toho si prohlédněte DurableOfferID.*** | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferId | Jedinečný identifikátor trvalé nabídky, jak je definován v ceníku. *Tato hodnota odpovídá **ID nabídky** z ceníku.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | Název nabídky služby zakoupené zákazníkem, jak je definováno v ceníku. | *systém Microsoft Office 365 (plán E3)* |
| Datum_zahájení_předplatného | Počáteční datum předplatného ve standardu UTC. Čas je vždy začátek dne, tj. 0:00. Toto pole je nastavené na den odeslané objednávky. Používá se s **SubscriptionEndDate** k určení, jestli se zákazník stále nachází v prvním roce předplatného nebo jestli se předplatné prodlouží na následující rok. | *2/1/2019 0:00* |
| Datum ukončení předplatného | Koncové datum předplatného ve standardu UTC. Čas je vždy začátek dne, tj. 0:00. Buď *12 měsíců plus **x** dní* po počátečním datu, aby bylo v souladu s fakturačním datem partnera, nebo *12* měsíců od data prodloužení . Při prodloužení se ceny aktualizují na aktuální ceník. Před automatickým prodlužováním platnosti může být nutná komunikace se zákazníkem. | *2/1/2019 0:00* |
| ChargeStartDate | Počáteční den poplatků. Čas je vždy začátek dne, tj. 0:00. Slouží k výpočtu denních poplatků (pro poplatky za *uplynulé* náklady), když zákazník změní číslo licence. | *2/1/2019 0:00* |
| ChargeEndDate | Koncový den poplatků Čas je vždy koncem dne, 23:59. Slouží k výpočtu denních poplatků (pro poplatky za *uplynulé* náklady), když zákazník změní číslo licence. | *2/28/2019 23:59* |
| ChargeType | [Typ poplatků](recon-file-charge-types.md) nebo úprav. | Viz [typy poplatků](recon-file-charge-types.md). |
| UnitPrice | Cena za licenci, jak je publikována v ceníku v době nákupu. Ujistěte se, že se shoduje s informacemi uloženými v systému fakturace během odsouhlasení. | *6,82* |
| Množství | Počet licencí. Ujistěte se, že se shoduje s informacemi uloženými v systému fakturace během odsouhlasení. | *2* |
| Částka | Celková cena za množství Slouží ke kontrole, zda výpočet množství odpovídá způsobu výpočtu této hodnoty pro zákazníky. | *13,32* |
| TotalOtherDiscount | Výše slevy uplatněné na tyto poplatky. Licence na produkty, které jsou součástí kompetence, MAPS nebo nových předplatných způsobilých k pobídce, budou v tomto sloupci také obsahovat výši slevy. | *2.32* |
| Mezisoučet | Celkem před zdaněním Zkontroluje, jestli mezisoučt odpovídá očekávanému součtu v případě slevy. | *11* |
| Daň | Poplatek za částku daně. Na základě daňových pravidel a konkrétních okolností vašeho trhu. | *0* |
| TotalForCustomer | Total after tax. Kontroluje, jestli se vám na faktuře účtují daně. | *11* |
| Měna | Typ měny. Každá fakturační entita má jenom jednu měnu. Zkontrolujte, jestli odpovídá vaší první faktuře. Po všech hlavních aktualizacích fakturační platformy to znovu zkontrolujte. | *EUR* |
| DomainName | Název domény zákazníka. Toto pole může být až do druhého fakturačního cyklu prázdné. *Nepoužívejte toto pole jako jedinečný identifikátor zákazníka. Zákazník nebo partner může aktualizovat vlastní nebo výchozí doménu prostřednictvím portálu Office 365.* | *example.onmicrosoft.com* |
| SubscriptionName | Přezdívka k předplatnému. Pokud není zadána žádná přezdívka, Partnerské centrum použije **offerName**. | *PROJEKT ONLINE* |
| SubscriptionDescription | Název nabídky služby zakoupené zákazníkem, jak je definováno v ceníku. (Toto je stejné pole jako **Nabídka**.) | *PROJECT ONLINE PREMIUM BEZ PROJEKTOVÉHO KLIENTA* |
| BillingCycleType | Četnost jednorázových faktur.| *měsíčně* |
