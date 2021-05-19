---
title: Denní hodnocení souborů pro odsouhlasení využití
ms.topic: article
ms.date: 06/12/2020
description: Naučte se číst soubory pro odsouhlasení s denním hodnocením využití v partnerském centru. Obsahuje popisy pro konkrétní pole v souboru rekognoskaci.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9b5daf91646324a9d4ace92d25736cfd0361ad6c
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147271"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>Naučte se číst soubory pro odsouhlasení s denním hodnocením využití v partnerském centru.

**Platí pro**: partnerské Centrum | Partnerské centrum pro Microsoft Cloud pro státní správu USA

**Příslušné role**: Agent správce | Správce fakturace | Prodejní agent | Agent helpdesku

Tento článek vysvětluje, jak číst každodenní soubory pro odsouhlasení s využitím.

>[!NOTE]
>Denní hodnocení využití obvykle trvá 24 hodin, než se zobrazí v partnerském centru nebo je k němu možné přistupovat prostřednictvím rozhraní API.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Pole v souborech pro odsouhlasení s denním hodnocením využití

| Sloupec | Popis |
| ------ | ----------- |
| PartnerId | Identifikátor partnera ve formátu identifikátoru GUID. |
| PartnerName | Název partnera. |
| CustomerId | Jedinečný identifikátor Microsoft pro zákazníka ve formátu GUID. |
| CustomerName | Název organizace zákazníka, jak je uveden v partnerském centru. *Tento sloupec je důležitý pro sjednocení faktury se systémovými informacemi.* |
| CustomerDomainName | Název domény zákazníka. |
| CustomerCountry | Země, kde se zákazník nachází. |
| MpnId | Identifikátor MPN partnera CSP. |
| Tier2MpnId | Identifikátor MPN prodejce záznamu pro předplatné. |
| InvoiceNumber | Číslo faktury, kde se zobrazí zadaná transakce. |
| ProductId | Identifikátor produktu. |
| SkuId | Identifikátor konkrétní SKU. |
| AvailabilityId | Identifikátor konkrétní dostupnosti skladové položky. V tomto sloupci se zobrazuje, jestli je SKU dostupná k nákupu v dané zemi, měně, oboru odvětví atd. |
| SkuName | Název konkrétní SKU |
| ProductName | Název produktu. |
| Název vydavatele | Název vydavatele |
| PublisherId | Identifikátor vydavatele ve formátu identifikátoru GUID |
| SubscriptionDescription | Název nabídky služby zakoupené zákazníkem, jak je definováno v ceníku. (Tento sloupec je identickým polem pro **offername**). |
| SubscriptionId | Jedinečný identifikátor předplatného na platformě fakturace Microsoftu Nepoužívá se pro odsouhlasení. *Tento identifikátor není stejný jako **ID předplatného** v konzole pro správu partnerů.* |
| ChargeStartDate | Počáteční datum fakturačního cyklu (s výjimkou případů, kdy se prezentují data dříve neúčtovaných latentních dat o využití z předchozího fakturačního cyklu). Čas je vždy začátek dne, tj. 0:00. |
| ChargeEndDate | Koncové datum fakturačního cyklu (s výjimkou případů, kdy se prezentují data dříve neúčtovaných latentních dat o využití z předchozího fakturačního cyklu). Čas je vždy konec dne, 23:59. |
| UsageDate | Datum využití služby |
| MeterType (Typ měřiče) | Typ měřiče. |
| MeterCategory | Služba nejvyšší úrovně, které se využití týká. |
| MeterId | Identifikátor použitého měřiče. |
| MeterSubCategory | Typ služby Azure, který může mít vliv na sazbu. |
| MeterName | Měrná jednotka spotřebovává měřič. |
| MeterRegion | Tento sloupec určuje umístění datového centra v rámci oblasti pro služby, ve kterých je oblast MeterRegion platná a naplněná. |
| Jednotka | Jednotka názvu **prostředku**. |
| ResourceLocation | Datové centrum, ve kterém je měřič spuštěný |
| ConsumedService | Služba platformy Azure, kterou jste použili. |
| ResourceGroup | Představuje kontejner, který obsahuje související prostředky pro řešení Azure. |
| Identifikátor URI prostředku | Identifikátor URI používaného prostředku. |
| ChargeType | Typ poplatku nebo úpravy.  |
| UnitPrice | Cena za licenci, jak je publikováno v ceníku v době nákupu. Ujistěte se, že tato cena odpovídá informacím uloženým ve vašem fakturačním systému během odsouhlasení. |
| Množství | Počet licencí. Ujistěte se, že tato cena odpovídá informacím uloženým v systému fakturace během odsouhlasení. |
| Jednotkách UnitType | Typ jednotky, na kterou se měřič účtuje.  |
| BillingPreTaxTotal | Celková fakturovaná částka před zdaněním<br/> _**BillingPreTaxTotal** = Floor (([ @EffectiveUnitPrice ]*[ @Quantity ]*[ @PCToBCExchangeRate ]); 2)_ |
| BillingCurrency | Měna v geografické oblasti zákazníka. |
| PricingPreTaxTotal | Ceny před přidáním daní. |
| PricingCurrency | Měna v ceníku. |
| ServiceInfo1 | Počet Service Bus připojení, která byla zřízena a použita v daném dni. |
| ServiceInfo2 | Starší verze pole, které zachycuje volitelná metadata specifická pro službu. |
| Značky | Představuje logickou organizaci prostředků Azure nastavených uživatelem. |
| AdditionalInfo | Další informace, které nejsou uvedené v jiných sloupcích. |
| EffectiveUnitPrice | Skutečná hodnota, která se účtuje za jednotku, včetně všech slev, získaného kreditu atd. |
| PCToBCExchangeRate | Směnný kurz, který se použije pro cenovou měnu a fakturační měnu |
| PCToBCExchangeRateDate | Datum, kdy se stanoví cenová měna pro fakturační měnu |
| EntitlementId | Představuje ID předplatného Azure. |
| Popis nároku | Představuje název ID předplatného Azure. |
| PartnerEarnedCreditPercentage | Zobrazí PartnerEarnedCredit pro položku řádku. Získaný kredit bude buď 0, nebo 15 procent. |
| CreditPercentage | Zobrazí kredit Azure Consumption. Získaný kredit bude buď 0, nebo 100 procent. |
| Typ kreditu | Typ kreditu Například **Uplatněný kredit Azure.** |
>[!NOTE]
>Zobrazení využití podle denního hodnocení obvykle trvá 24 hodin Partnerské centrum nebo se k němu přistupuje prostřednictvím rozhraní API.


