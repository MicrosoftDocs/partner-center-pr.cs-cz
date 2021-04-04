---
title: Soubory s vyrovnáním na základě licencí
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si, jak číst soubory pro odsouhlasení na základě licencí v partnerském centru. Tento článek vysvětluje význam jednotlivých polí v souboru rekognoskaci založeném na licencích.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bc97156d23fa4ea1082a0ad4a931ff36375897a7
ms.sourcegitcommit: 6498c57e75aa097861523b206dc142f789deeb36
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/02/2021
ms.locfileid: "106178914"
---
# <a name="understand-the-fields-in-partner-center-license-based-reconciliation-files"></a>Pochopení polí v souborech pro odsouhlasení na základě licence partnerského centra

**Platí pro**

- Partnerské centrum pro oficiální Cloud Microsoftu

**Příslušné role**

- Globální správce
- Správce správy uživatelů
- Správce fakturace
- Agent správce

Pokud chcete sloučit změny s objednávkami zákazníka, porovnejte **Syndication_Partner_Subscription_Number** ze souboru pro odsouhlasení s **ID předplatného** z partnerského centra.

## <a name="fields-in-license-based-reconciliation-files"></a>Pole v souborech pro odsouhlasení na základě licencí

| Sloupec | Popis | Ukázková hodnota |
| ------ | ----------- | ------------ |
| PartnerId | Jedinečný identifikátor ve formátu identifikátoru GUID pro konkrétní entitu fakturace Není vyžadováno pro odsouhlasení. Stejné ve všech řádcích. | *8ddd03642-test-test-test-46b58d356b4e* |
| CustomerId | Jedinečný identifikátor Microsoft pro zákazníka ve formátu GUID. | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| CustomerName | Název organizace zákazníka, jak je uvedeno v partnerském centru. *Velmi důležité pole pro sjednocení faktury s informacemi o systému* | *Test zákazníka A* |
| MpnId | Identifikátor MPN partnera CSP. Podívejte [se, jak itemize partner](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| ResellerMpnId | Identifikátor MPN prodejce záznamu pro předplatné.  |
| OrderId | Jedinečný identifikátor pro objednávku na platformě fakturace Microsoftu. Může být užitečné k identifikaci objednávky při kontaktování podpory. Nepoužívá se pro odsouhlasení. | *566890604832738111* |
| SubscriptionId | Jedinečný identifikátor předplatného na platformě fakturace Microsoftu Může být užitečné k identifikaci předplatného při kontaktování podpory. Nepoužívá se pro odsouhlasení. *Tato hodnota se neshoduje s **ID předplatného** v konzole pro správu partnerů. Místo toho se prosím podívejte na **SyndicationPartnerSubscriptionNumber** .* | *usCBMgAAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | Jedinečný identifikátor předplatných. Zákazník může mít několik předplatných pro stejný plán. Tento sloupec je důležitý pro účely analýzy souborů pro odsouhlasení. Toto pole se mapuje na **ID předplatného** v konzole pro správu partnera. | *fb977ab5-test-test-test-24c8d9591708* |
| Hodnotami OfferId | Jedinečný identifikátor nabídky Identifikátor standardní nabídky, jak je definován v ceníku. *Tato hodnota neodpovídá **ID nabídky** ze ceníku. Místo toho se podívejte na **DurableOfferID** .* | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferId | Jedinečný identifikátor odolné nabídky, jak je definován v ceníku. *Tato hodnota odpovídá **ID nabídky** ze ceníku.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | Název nabídky služby zakoupené zákazníkem, jak je definováno v ceníku. | *Systém Microsoft Office 365 (plán E3)* |
| SubscriptionStartDate | Počáteční datum odběru Čas je vždy začátek dne, tj. 0:00. Toto pole je nastaveno na den po odeslání objednávky. Používá se s **SubscriptionEndDate** k určení: Pokud je zákazník stále v prvním roce předplatného nebo pokud se předplatné obnovilo na následující rok. | *2/1/2019 0:00* |
| SubscriptionEndDate | Datum ukončení předplatného Čas je vždy začátek dne, tj. 0:00. Buď *12 měsíců plus **x** dní od počátečního data* v souladu s datem fakturace partnera nebo *12 měsíců od data obnovení*. Při obnovení se ceny aktualizují na aktuální ceník. V případě automatizovaného obnovení může být nutné provést zákaznickou komunikaci. | *2/1/2019 0:00* |
| ChargeStartDate | Počáteční den poplatků. Čas je vždy začátek dne, tj. 0:00. Slouží k výpočtu denních poplatků (pro poplatky za *uplynulé* náklady), když zákazník změní číslo licence. | *2/1/2019 0:00* |
| ChargeEndDate | Koncový den poplatků Čas je vždy koncem dne, 23:59. Slouží k výpočtu denních poplatků (pro poplatky za *uplynulé* náklady), když zákazník změní číslo licence. | *2/28/2019 23:59* |
| ChargeType | [Typ poplatků](recon-file-charge-types.md) nebo úprav. | Viz [typy poplatků](recon-file-charge-types.md). |
| UnitPrice | Cena za licenci, jak je publikována v ceníku v době nákupu. Ujistěte se, že se shoduje s informacemi uloženými v systému fakturace během odsouhlasení. | *6,82* |
| Množství | Počet licencí. Ujistěte se, že se shoduje s informacemi uloženými v systému fakturace během odsouhlasení. | *2* |
| Částka | Celková cena za množství Slouží ke kontrole, zda výpočet množství odpovídá způsobu výpočtu této hodnoty pro zákazníky. | *13,32* |
| TotalOtherDiscount | Množství slevy použité pro tyto poplatky. Licence k produktům, které jsou součástí kompetence nebo map, nebo nových předplatných, která mají nárok na motivaci, budou v tomto sloupci také obsahovat částku slevy. | *2,32* |
| Mezisoučet | Celkem před zdaněním Zkontroluje, jestli váš Mezisoučet odpovídá očekávanému součtu v případě slevy. | *11* |
| Daň | Poplatek za daň V závislosti na daňových pravidlech na trhu a konkrétních okolnostech. | *0* |
| TotalForCustomer | Celkem po dani Kontroluje, jestli se na faktuře účtují daň. | *11* |
| Měna | Typ měny. Každá fakturační entita má pouze jednu měnu. Ověřte, jestli se shoduje s vaší první fakturou. Znovu se vraťte po všech hlavních aktualizacích fakturačních platforem. | *EUR* |
| DomainName | Název domény zákazníka. Toto pole může být prázdné až do druhého fakturačního cyklu. *Nepoužívejte toto pole jako jedinečný identifikátor pro zákazníka. Zákazník nebo partner může aktualizovat individuální nebo výchozí doménu prostřednictvím portálu Office 365.* | *example.onmicrosoft.com* |
| SubscriptionName | Přezdívka předplatného Pokud není zadaná Přezdívka, Partnerské centrum použije **nabídku offername**. | *PROJEKT ONLINE* |
| SubscriptionDescription | Název nabídky služby zakoupené zákazníkem, jak je definováno v ceníku. (Toto je stejné pole jako **Nabídka**.) | *PROJECT ONLINE PREMIUM BEZ PROJEKTOVÉHO KLIENTA* |
| BillingCycleType | Četnost jednorázových faktur.| *Měsíčně* |