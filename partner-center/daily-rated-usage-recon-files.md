---
title: Denní hodnocení souborů pro odsouhlasení využití
ms.topic: article
ms.date: 06/12/2020
description: Naučte se číst soubory pro odsouhlasení s denním hodnocením využití v partnerském centru. Obsahuje popisy pro konkrétní pole v souboru rekognoskaci.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8b45ef4767e4bde28befd35c5294ed19149bf034
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/14/2020
ms.locfileid: "92527712"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>Naučte se číst soubory pro odsouhlasení s denním hodnocením využití v partnerském centru.

**Platí pro**

- Partnerské centrum
- Partnerské centrum pro Microsoft Cloud pro státní správu USA

**Příslušné role**

- Agent správce
- Správce fakturace
- Agent prodeje
- Agent helpdesku

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
| SubscriptionDescription | Název nabídky služby zakoupené zákazníkem, jak je definováno v ceníku. (Tento sloupec je identickým polem pro **offername** ). |
| SubscriptionId | Jedinečný identifikátor předplatného na platformě fakturace Microsoftu Nepoužívá se pro odsouhlasení. *Tento identifikátor není stejný jako **ID předplatného** v konzole pro správu partnerů.* |
| ChargeStartDate | Počáteční datum fakturačního cyklu (kromě případů, kdy se prezentují data dříve nenabitých latentních dat z předchozího fakturačního cyklu). Čas je vždy začátek dne, tj. 0:00. |
| ChargeEndDate | Koncové datum fakturačního cyklu (kromě případů, kdy se prezentují data dříve nenabitých dat o latentních používaní z předchozího fakturačního cyklu). Čas je vždy koncem dne, 23:59. |
| UsageDate | Datum použití služby |
| MeterType | Typ měřiče. |
| MeterCategory | Služba nejvyšší úrovně, které se využití týká. |
| MeterId | Identifikátor používaného měřiče. |
| MeterSubCategory | Typ služby Azure, který může mít vliv na sazbu. |
| MeterName | Měrná jednotka spotřebovaného měřiče. |
| MeterRegion | Tento sloupec určuje umístění datového centra v oblasti pro služby, kde se MeterRegion vztahuje a naplní. |
| Jednotka | Jednotka **názvu** prostředku. |
| ResourceLocation | Datové centrum, ve kterém je měřidlo spuštěno. |
| ConsumedService | Služba platformy Azure, kterou jste použili. |
| ResourceGroup | Představuje kontejner, který obsahuje související prostředky pro řešení Azure. |
| ResourceURI | Identifikátor URI používaného prostředku |
| ChargeType | Typ poplatku nebo úpravy.  |
| Jednotková cena | Cena za licenci, jak je publikována v ceníku v době nákupu. Ujistěte se, že tato cena odpovídá informacím uloženým v systému fakturace během odsouhlasení. |
| Množství | Počet licencí. Ujistěte se, že tato cena odpovídá informacím uloženým v systému fakturace během odsouhlasení. |
| Jednotkách UnitType | Typ jednotky, na kterou se měřič účtuje.  |
| BillingPreTaxTotal | Celková fakturovaná částka před zdaněním<br/> _**BillingPreTaxTotal** = Floor (([ @EffectiveUnitPrice ] *[ @Quantity ]* [ @PCToBCExchangeRate ]); 2)_ |
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
| EntitlementDescription | Představuje název ID předplatného Azure. |
| PartnerEarnedCreditPercentage | Zobrazí PartnerEarnedCredit pro položku řádku. Získaný kredit bude buď 0, nebo 15 procent. |

>[!NOTE]
>Denní hodnocené využití obvykle trvá 24 hodin, než se zobrazí v partnerském centru nebo bude k dispozici prostřednictvím rozhraní API.


