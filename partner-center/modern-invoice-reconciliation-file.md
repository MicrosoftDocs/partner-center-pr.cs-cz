---
title: Pole souboru rekognoskaci pro jednorázové nákupy CSP
ms.topic: conceptual
ms.date: 01/29/2021
description: Přečtěte si o všech položkách v souboru pro odsouhlasení s jednorázovým nákupem CSP v partnerském centru, včetně ukázkových hodnot.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: 85946f44e1265ad5012faf9d782609904100c80e
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146251"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>Pole souboru pro odsouhlasení s jedním časovým nákupem CSP

**Příslušné role**: správce účtu | Fakturační Agent

## <a name="using-the-recon-file"></a>Použití souboru rekognoskaci
V následující tabulce jsou uvedeny popisy a ukázkové hodnoty pro pole v souboru odsouhlasení pro jednorázové nákupy CSP.

Další informace o souborech pro odsouhlasení najdete v tématu [použití souborů pro odsouhlasení](use-the-reconciliation-files.md).

| Sloupec | Popis | Ukázková hodnota |
| ------ | ----------- | ------------ |
| PartnerId | Jedinečný identifikátor ve formátu identifikátoru GUID pro konkrétní entitu fakturace Není vyžadováno pro odsouhlasení. Stejné ve všech řádcích. | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | Jedinečný identifikátor Microsoft pro zákazníka ve formátu GUID. | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | Název organizace zákazníka, jak je uveden v partnerském centru. Tento sloupec je důležitý pro sjednocení faktury se systémovými informacemi. | *Moderní DE2 zák Johnny* |
| CustomerDomainName | Název domény zákazníka. | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | Země, ve které se nachází váš zákazník. Podívejte se [na úplný seznam zemí](./regional-authorization-overview.md) pro vaši oblast.  | *DE* |
| InvoiceNumber | Číslo faktury přidružené k souboru s vyrovnáním.  | *G002297372* |
| ID mpn | Identifikátor MPN partnera CSP. Další informace najdete v tématu [o tom, jak položky zařazovat podle partnera.](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner) | *6034453* |
| ResellerMpnId | Identifikátor MPN prodejce záznamu pro předplatné. | *6048879* |
| OrderId | Jedinečný identifikátor objednávky na fakturační platformě Microsoftu Může být užitečné při identifikaci objednávky při kontaktování podpory. Nepouží se k odsouhlasení. | *0ET2qaZvJGfF9wgSKnWzR5JLm 10lOc1* |
| OrderDate | Datum ve standardu UTC, kdy byla objednávka umístěna. | *10/3/2020* |
| ProductId | Jedinečný identifikátor produktu. | *DZH318Z0BNZ5* |
| SkuId | Jedinečný identifikátor SKU | *006G* |
| AvailabilityId | Jedinečný identifikátor dostupnosti. | *DZH318Z08B80* |
| SkuName | Název SKU. | *Tabulky – LRS* |
| ProductName | Název produktu | *Tabulky* |
| ChargeType | [Typ poplatků](./recon-file-charge-types.md) nebo úprav. | *Nový* |
| UnitPrice | Cena za licenci, jak je publikována v ceníku v době nákupu. Ujistěte se, že se shoduje s informacemi uloženými v systému fakturace během odsouhlasení. | *0,045* |
| Množství | Počet licencí. Ujistěte se, že se shoduje s informacemi uloženými v systému fakturace během odsouhlasení. | *1* |
| Mezisoučet | Celkem před zdaněním Mezisoučet by měl být roven Fakturovatelné množství vynásobenému platnou jednotkovou cenou. | *0* |
| TaxTotal | Poplatek za daň Na základě daňových pravidel a konkrétních okolností vašeho trhu. | *0* |
| Celkem | Celková částka se rovná mezisoučtu plus částka daně. | *0* |
| Měna | Vaše faktura se vygeneruje v kontextu měny zákazníka. To znamená, že pokud jste partner, který provádí transakce se zákazníky z různých fakturovatelných měn, obdržíte fakturu za každý typ měny zákazníka.  | *EUR* |
| Popis vlastnosti PriceAdjustment | Důvody úprav jednotkové ceny Toto jsou hlavní důvody, ale nejen určení efektivní jednotkové ceny. | *["15,0% kredit získaný partnerem za spravované služby"]* |
| Název vydavatele | Vydavatel produktu.  | *Microsoft* |
| PublisherId | Jedinečný identifikátor, který Partnerské centrum používá k identifikaci vydavatele. | *NA* |
| Popis předplatného | Název nabídky služeb zakoupené zákazníkem, jak je definováno v ceníku. Tento sloupec je stejné pole jako OfferName. | *Plán Azure* |
| SubscriptionId | Jedinečný identifikátor předplatného na fakturační platformě Microsoftu Nepouží se k odsouhlasení. Všimněte si, že tento identifikátor není stejný jako ID předplatného v konzole pro správu partnera. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | Datum zahájení fakturačního období předplatného | *9/1/2020* |
| ChargeEndDate | Datum, kdy končí fakturační období předplatného. | *30. září 2020* |
| TermAndBillingCycle | Doba trvání závazku pokračovat v předplatném v době nákupu. | *Uložená data (GB/měsíc)* |
| EffectiveUnitPrice | Poměrná jednotková cena pro výpočet nákladů za fakturační cyklus. Efektivní jednotkovou cenu určují slevy, úpravy ve fakturačních dnech a další faktory. Další informace najdete v tématu [Výpočet efektivní jednotkové ceny.](./effective-unit-price-calculation.md)  | *0.03825* |
| Unittype | Typ jednotky, za kterou se měřič účtuje. | *1 GB/měsíc* |
| Alternativní ID | Alternativní ID odkazované řádkové položky objednávky. | *6dc5c039750a* |
| BillableQuantity | Celkové fakturované množství  | *0.005001* |
| FakturaceFrequency | Fakturační plán vybraný v době nákupu. | *NA*  |
| PricingCurrency | Měna v ceníku. | *USD* |
| PCToBCExchangeRate | Směnný kurz použitý pro ceníkovou měnu na fakturační měnu | *0.846202666* |
| PCToBCExchangeRateDate | Určuje se datum, kdy se určuje měna s cenami pro fakturační měnu. | *30. září 2020* |
| Popis měřiče | Popis měřiče.  | *Tabulky – uložená data LRS (GB/měsíc)* |
| ReservationOrderId | ID objednávky rezervace. | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | Popis kreditu | *Kredit Azure Consumption* |

>[!NOTE]
>Spotřebu Azure můžete odsouhlasit v souboru s vyrovnáním pro jeden nákup. Pokud to chcete udělat, přejděte do souboru s odsoustavou využití podle denního hodnocení a vyhledejte své ID předplatného. Zobrazí se všechny náklady spojené s vaším ID plánu Azure. Jako EntitlementID se zobrazí vaše ID předplatného Azure.

## <a name="next-steps"></a>Další kroky

- [Fakturace a daně](billing.md)
