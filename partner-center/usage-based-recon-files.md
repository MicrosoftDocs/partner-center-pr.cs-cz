---
title: Soubory s vyrovnáním na základě využití
ms.topic: article
ms.date: 06/08/2020
description: Seznamte se se všemi položkami v souboru s vyrovnáním na základě využití v Partnerské centrum. Obsahuje několik příkladů.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6c486d4866b0a2a912801d2648a1822418687078
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431705"
---
# <a name="understand-usage-based-reconciliation-files-and-their-specific-fields-in-partner-center"></a>Pochopení souborů odsouhlasení na základě využití a jejich konkrétních polí v Partnerské centrum

**Odpovídající role:** Správce účtu | Správce fakturace

Pokud chcete poplatky odsouhlasit s využitím zákazníka, porovnejte hodnoty **ResellerID**, **ResellerName** a  **ResellerBillableAccount** ze souboru s vyrovnáním se jménem zákazníka a **ID** předplatného ze seznamu Partnerské centrum.

## <a name="fields-in-usage-based-reconciliation-files"></a>Pole v souborech s vyrovnáním na základě využití

V následujících polích jsou vysvětlené použité služby a sazba.

| Sloupec | Popis | Ukázkové hodnoty |
| ------ | ----------- | ------------ |
| ID partnera | Identifikátor partnera ve formátu GUID. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | Název partnera. | *Contoso, Ltd.* |
| PartnerBillableAccountId | Identifikátor partnerského účtu. | *1010578050* |
| CustomerCompanyName | Název organizace zákazníka, jak je hlášeno v Partnerské centrum. *To je velmi důležité pro odsoustavu faktury s informacemi o systému.* | *Testování zákazníka* |
| ID mpn | Microsoft Partner Network (MPN) partnera Cloud Solution Provider (CSP). | *4390934* |
| ResellerMpnId | Identifikátor MPN prodejce záznamu pro předplatné.  |
| InvoiceNumber | Číslo faktury, kde se zadaná transakce objeví. | *D020001IVK* |
| ChargeStartDate | Počáteční datum fakturačního cyklu, s výjimkou případů, kdy se prezentují data dříve nevyúčtovaných latentních dat o využití (z předchozího fakturačního cyklu). Čas je vždy začátek dne, tj. 0:00. | *2/1/2019 0:00* |
| ChargeEndDate | Koncové datum fakturačního cyklu, s výjimkou případů, kdy se prezentují data dříve nevyúčtovaných latentních dat o využití (z předchozího fakturačního cyklu). Čas je vždy konec dne, 23:59. | *2/28/2019 23:59* |
| SubscriptionId | Jedinečný identifikátor předplatného na fakturační platformě Microsoftu Může být užitečné identifikovat předplatné při kontaktování podpory. Nepouží se k odsouhlasení. *Toto není stejné jako **ID předplatného** v konzole pro správu partnera.* | *usCBMgAAAAAAAAIA* |
| SubscriptionName | Přezdívku pro nabídku služby. | *Microsoft Azure* |
| Popis předplatného | Obchodní činnost nabídky služby. | *Microsoft Azure* |
| OrderID | Jedinečný identifikátor objednávky na fakturační platformě Microsoftu Může být užitečné identifikovat předplatné při kontaktování podpory. Nepouží se k odsouhlasení. | *566890604832738111* |
| ServiceName | Název této služby Azure. | *VIRTUÁLNÍ POČÍTAČE* |
| ServiceType | Konkrétní typ služby Azure. | *Service Bus – individuální nebo balíček*, databáze SQL Azure – Business nebo Web *Edition* |
| ResourceGuid | Konkrétní jedinečný identifikátor pro všechna data služby a cenovou strukturu. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| ResourceName | Název prostředku Azure. | *Přenos dat v (GB)*, *přenos dat (GB)* |
| Oblast | Oblast, na kterou se využití vztahuje. Primárně slouží k přiřazování sazeb k přenosům dat, protože sazby se liší podle oblastí. | *Asie a Tichomoří*, *Evropa,* *Latinská Amerika*, *Severní Amerika* |
| Skladová jednotka (SKU) | Jedinečný identifikátor Microsoftu pro nabídku | *7UD-00001* |
| ID položky DetailLineItem | Identifikátor a množství pro položky různých sazeb pro službu nebo prostředek v daném fakturačním období. U cen v úrovních Azure může být jedna sazba až pro určité množství fakturovatelných jednotek a po tomto množství jiná sazba. | *1* |
| ConsumedQuantity | Množství spotřebované služby (například hodiny nebo GB) během období generování sestav. Zahrnuje také jakékoli nefaktované využití z předchozích období generování sestav. | *11* |
| IncludedQuantity | Jednotky zahrnuté jako součást nabídky. V CSP se obvykle nenacháduje. | *0* |
| OverageQuantity | Jednotky, které nejsou součástí nabídky. Za tyto účty musí platit partner. Rovná **se ConsumedQuantity** minus **IncludedQuantity**. | *11* |
| Listprice | Cena nabídky, která platí k počátečnímu datu předplatného. | *0,0808 USD* |
| PretaxCharges | Rovná se **ListPrist vynásobené** **hodnotou OverageQuantity** zaokrouhlené na nejbližší cent. | *0,085 USD* |
| TaxAmount (Částka daně) | Účtuje se částka daně. V závislosti na daňových pravidlech na trhu a konkrétních okolnostech. | *$0,08* |
| PostTaxTotal | Celkem po dani, pokud je daň platná. | *$0,93* |
| Měna | Typ měny. Každá fakturační entita má pouze jednu měnu. Ověřte, že odpovídá vaší první faktuře a potom po všech hlavních aktualizacích fakturačních platforem. | *EUR* |
| PretaxEffectiveRate | Pretax cena za jednotku. Rovná se **PretaxCharges** dělený **OverageQuantity**, zaokrouhlený na nejbližší cent. | *$0,08* |
| PostTaxEffectiveRate | Účtujte daňovou cenu na jednotku. Rovná se **PostTaxTotal** dělený **OverageQuantity**, zaokrouhlený na nejbližší cent. Nebo se rovná **PretaxEffectiveRate** plus daňová sazba za jednotku a zaokrouhluje se na nejbližší cent. | *$0,08* |
| ChargeType | [Typ poplatků](recon-file-charge-types.md) nebo úprav. | Viz [typy poplatků](recon-file-charge-types.md). |
| CustomerId | Jedinečný identifikátor Microsoft pro zákazníka ve formátu GUID. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Název domény zákazníka. Toto pole může být prázdné až do druhého fakturačního cyklu. | *example.onmicrosoft.com* |
| BillingCycleType | Frekvence fakturace času.| **měsíčně**  |
| Jednotka | Jednotka **názvu** prostředku. | *GB* nebo *hodiny* |
| CustomerBillableAccount | Jedinečný identifikátor účtu na fakturační platformě Microsoftu | *1280018095* |
| UsageDate | Datum nasazení služby | *2/1/2019 0:00* |
| MeteredRegion | Určuje umístění datového centra v rámci oblasti (pro služby, kde je tato hodnota platná a naplněná). | *Východní Asie*, *jižní východní Asie*, *Severní Evropa*, *západní Evropa*, *střed USA – sever* střed USA – jih  |
| MeteredService | Identifikuje jednotlivá použití služby Azure, pokud není konkrétně identifikovaná ve sloupci **ServiceName** . Například přenosy dat jsou hlášeny jako *Microsoft Azure-všechny služby* ve sloupci **ServiceName** . | *AccessControl*, *CDN*, *COMPUTE*, *Database*, *ServiceBus*, *Storage* |
| MeteredServiceType | Podnadpis pro pole **MeteredService** , které poskytuje další vysvětlení využití služeb Azure. | *ZAHRANIČNÍCH* |
| Project | Název pro instanci služby definovaný zákazníkem | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | Počet Azure Service Bus připojení, která byla zřízena a využita v daném dni. | *1,000000 připojení/30 dní* (Pokud jste samostatně zřízené připojení během 30denní měsíce), *25 připojení/30 dní – využito: 1,000000* (Pokud jste měli k dispozici 25 sad připojení Service Bus a v tomto dni jste využili 1) |

## <a name="next-steps"></a>Další kroky

- [Pochopení polí v souborech pro odsouhlasení na základě licence partnerského centra](license-based-recon-files.md)