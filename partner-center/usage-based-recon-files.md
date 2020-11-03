---
title: Soubory pro odsouhlasení podle využití
ms.topic: article
ms.date: 06/08/2020
description: Seznamte se se všemi položkami v souboru pro odsouhlasení na základě využití v partnerském centru. Obsahuje několik příkladů.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 04ad6a0c2c7a6330d2e1230f046ee78b2a7405c8
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/03/2020
ms.locfileid: "92526997"
---
# <a name="understand-usage-based-reconciliation-files-and-their-specific-fields-in-partner-center"></a>Pochopení souborů pro odsouhlasení podle využití a jejich konkrétních polí v partnerském centru

Platí pro:

- Partnerské centrum
- Partnerské centrum pro Microsoft Cloud pro státní správu USA

Pokud chcete své poplatky sjednotit na používání zákazníka, porovnejte **ResellerID** **, procustomers a** **ResellerBillableAccount** ze souboru pro odsouhlasení s **názvem zákazníka** a **ID předplatného** z partnerského centra.

## <a name="fields-in-usage-based-reconciliation-files"></a>Pole v souborech pro odsouhlasení na základě využití

Následující pole vysvětlují, které služby se použily, a rychlost.

| Sloupec | Popis | Ukázkové hodnoty |
| ------ | ----------- | ------------ |
| PartnerId | Identifikátor partnera ve formátu identifikátoru GUID | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | Název partnera. | *Contoso, Ltd.* |
| PartnerBillableAccountId | Identifikátor partnerského účtu. | *1010578050* |
| CustomerCompanyName | Název organizace zákazníka, jak je uvedeno v partnerském centru. *Velmi důležité pro sjednocení faktury s informacemi o systému.* | *Test zákazníka* |
| MpnId | Identifikátor MPN partnera CSP. | *4390934* |
| ResellerMpnId | Identifikátor MPN prodejce záznamu pro předplatné.  |
| InvoiceNumber | Číslo faktury, kde se zobrazí zadaná transakce. | *D020001IVK* |
| ChargeStartDate | Počáteční datum fakturačního cyklu, s výjimkou, kdy se prezentují data dříve neúčtovaných dat o latentních použitích (z předchozího cyklu vyúčtování). Čas je vždy začátek dne, tj. 0:00. | *2/1/2019 0:00* |
| ChargeEndDate | Koncové datum fakturačního cyklu, s výjimkou, kdy prezentují data dříve neúčtovaných dat latentního použití (z předchozího cyklu vyúčtování). Čas je vždy koncem dne, 23:59. | *2/28/2019 23:59* |
| SubscriptionId | Jedinečný identifikátor předplatného na platformě fakturace Microsoftu Může být užitečné k identifikaci předplatného při kontaktování podpory. Nepoužívá se pro odsouhlasení. *To není stejné jako **ID předplatného** v konzole pro správu partnerů.* | *usCBMgAAAAAAAAIA* |
| SubscriptionName | Přezdívka pro nabídku služby | *Microsoft Azure* |
| SubscriptionDescription | Odvětví nabídky služeb. | *Microsoft Azure* |
| OrderID | Jedinečný identifikátor pro objednávku na platformě fakturace Microsoftu. Může být užitečné k identifikaci předplatného při kontaktování podpory. Nepoužívá se pro odsouhlasení. | *566890604832738111* |
| ServiceName | Název příslušné služby Azure. | *VIRTUÁLNÍ POČÍTAČE* |
| ServiceType | Konkrétní typ služby Azure. | *Service Bus – jednotlivec nebo balíček* , *databáze SQL Azure – Business nebo Web Edition* |
| ResourceGuid | Specifický jedinečný identifikátor pro všechna data služby a cenovou strukturu. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| ResourceName | Název prostředku Azure. | *Přenos dat v (GB)* *přenos odchozích dat (GB)* |
| Region (Oblast) | Oblast, na kterou se vztahuje použití Primárně se používá k přiřazování sazeb přenosům dat, protože tarify se liší podle oblasti. | *Asie a Tichomoří* , *evropa* , *Latinská Amerika* *Severní Amerika* |
| Skladová jednotka (SKU) | Jedinečný identifikátor Microsoft pro nabídku | *7UD – 00001* |
| DetailLineItemId | Identifikátor a množství, které itemize různé sazby za službu nebo prostředek v daném fakturačním období. U cen vrstvených za Azure může existovat jedna sazba za určité množství fakturovaných jednotek a potom po tomto množství jinou sazbu. | *1* |
| ConsumedQuantity | Množství spotřebované služby (například hodiny nebo GB) během období generování sestav. Zahrnuje také veškeré nefakturované využití z předchozích období generování sestav. | *11* |
| IncludedQuantity | Jednotky zahrnuté jako součást nabídky Obvykle není přítomna ve zprostředkovateli CSP. | *0* |
| OverageQuantity | Jednotky nezahrnuté jako součást nabídky Tyto účty musí být placené partnerem. Rovná se **ConsumedQuantity** mínus **IncludedQuantity** . | *11* |
| ListPrice | Cenová nabídka v účinnosti v počátečním datu předplatného | *$0,0808* |
| PretaxCharges | Rovná se **ListPrist** vynásobený **OverageQuantity** , zaokrouhlený na nejbližší cent. | *$0,085* |
| TaxAmount | Účtuje se částka daně. V závislosti na daňových pravidlech na trhu a konkrétních okolnostech. | *$0,08* |
| PostTaxTotal | Celkem po dani, pokud je daň platná. | *$0,93* |
| Měna | Typ měny. Každá fakturační entita má pouze jednu měnu. Ověřte, že odpovídá vaší první faktuře a potom po všech hlavních aktualizacích fakturačních platforem. | *EUR* |
| PretaxEffectiveRate | Pretax cena za jednotku. Rovná se **PretaxCharges** dělený **OverageQuantity** , zaokrouhlený na nejbližší cent. | *$0,08* |
| PostTaxEffectiveRate | Účtujte daňovou cenu na jednotku. Rovná se **PostTaxTotal** dělený **OverageQuantity** , zaokrouhlený na nejbližší cent. Nebo se rovná **PretaxEffectiveRate** plus daňová sazba za jednotku a zaokrouhluje se na nejbližší cent. | *$0,08* |
| ChargeType | [Typ poplatků](recon-file-charge-types.md) nebo úprav. | Viz [typy poplatků](recon-file-charge-types.md). |
| CustomerId | Jedinečný identifikátor Microsoft pro zákazníka ve formátu GUID. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Název domény zákazníka. Toto pole může být prázdné až do druhého fakturačního cyklu. | *example.onmicrosoft.com* |
| BillingCycleType | Frekvence fakturace času.| **Měsíčně**  |
| Jednotka | Jednotka **názvu** prostředku. | *GB* nebo *hodiny* |
| CustomerBillableAccount | Jedinečný identifikátor účtu na fakturační platformě Microsoftu | *1280018095* |
| UsageDate | Datum nasazení služby | *2/1/2019 0:00* |
| MeteredRegion | Určuje umístění datového centra v rámci oblasti (pro služby, kde je tato hodnota platná a naplněná). | *Východní Asie* , *jižní východní Asie* , *Severní Evropa* , *západní Evropa* , *střed USA – sever* střed USA – jih *South Central US* |
| MeteredService | Identifikuje jednotlivá použití služby Azure, pokud není konkrétně identifikovaná ve sloupci **ServiceName** . Například přenosy dat jsou hlášeny jako *Microsoft Azure-všechny služby* ve sloupci **ServiceName** . | *AccessControl* , *CDN* , *COMPUTE* , *Database* , *ServiceBus* , *Storage* |
| MeteredServiceType | Podnadpis pro pole **MeteredService** , které poskytuje další vysvětlení využití služeb Azure. | *ZAHRANIČNÍCH* |
| Project | Název pro instanci služby definovaný zákazníkem | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | Počet Azure Service Bus připojení, která byla zřízena a využita v daném dni. | *1,000000 připojení/30 dní* (Pokud jste samostatně zřízené připojení během 30denní měsíce), *25 připojení/30 dní – využito: 1,000000* (Pokud jste měli k dispozici 25 sad připojení Service Bus a v tomto dni jste využili 1) |
