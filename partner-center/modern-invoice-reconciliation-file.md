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
ms.openlocfilehash: 3264c793dfb2e8592cd059cd84d5bb08769abbcf
ms.sourcegitcommit: c8d1bcf54cdcdc3f827f9210c8abddab02a686fe
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/14/2021
ms.locfileid: "112073794"
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
| CustomerCountry | Země, kde se zákazník nachází. Podívejte se na úplný [seznam zemí](./regional-authorization-overview.md) pro vaši oblast.  | *DE* |
| InvoiceNumber | Číslo faktury přidružené k souboru odsouhlasení.  | *G002297372* |
| MpnId | Identifikátor MPN partnera CSP. Další informace najdete v tématu [How to itemize by partner](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *6034453* |
| ResellerMpnId | Identifikátor MPN prodejce záznamu pro předplatné. | *6048879* |
| OrderId | Jedinečný identifikátor pro objednávku na platformě fakturace Microsoftu. Může být užitečné k identifikaci objednávky při kontaktování podpory. Nepoužívá se pro odsouhlasení. | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | Datum v UTC, kdy bylo pořadí umístěno. | *10/3/2020* |
| ProductId | Jedinečný identifikátor produktu | *DZH318Z0BNZ5* |
| SkuId | Jedinečný identifikátor SKU | *006G* |
| AvailabilityId | Jedinečný identifikátor dostupnosti. | *DZH318Z08B80* |
| SkuName | Název SKU. | *Tabulky – LRS* |
| ProductName | Název produktu | *Tabulky* |
| ChargeType | [Typ poplatků](./recon-file-charge-types.md) nebo úprav. | *Nový* |
| UnitPrice | Cena za licenci, jak je publikována v ceníku v době nákupu. Ujistěte se, že se shoduje s informacemi uloženými v systému fakturace během odsouhlasení. | *0,045* |
| Množství | Počet licencí. Ujistěte se, že se shoduje s informacemi uloženými v systému fakturace během odsouhlasení. | *1* |
| Mezisoučet | Celkem před zdaněním Mezisoučet by měl být roven Fakturovatelné množství vynásobenému platnou jednotkovou cenou. | *0* |
| TaxTotal | Poplatek za daň V závislosti na daňových pravidlech na trhu a konkrétních okolnostech. | *0* |
| Celkem | Celková částka je rovna mezisoučtu plus daňová částka. | *0* |
| Měna | Vaše vyúčtování se vygeneruje v souvislosti s měnou zákazníka. To znamená, že pokud jste partnerem s podporou transakcí z různých fakturovatelných měn, obdržíte fakturu za každý typ měny zákazníka.  | *EUR* |
| PriceAdjustmentDescription | Důvody pro úpravy v ceně jednotky. Jedná se o hlavní důvody, ale ne omezené na určení efektivní jednotkové ceny. | *["15,0% kredit získaný pro partnery pro spravované služby"]* |
| Název vydavatele | Vydavatel produktu.  | *Microsoft* |
| PublisherId | Jedinečný identifikátor, který Partnerské centrum používá k identifikaci vydavatele. | *NA* |
| SubscriptionDescription | Název nabídky služby zakoupené zákazníkem, jak je definováno v ceníku. Tento sloupec je stejné pole jako OfferName. | *Plán Azure* |
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
| ReservationOrderId | ID objednávky rezervace | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | Popis kreditu | *Kredit Azure Consumption* |
| Datum_zahájení_předplatného | Datum nákupu předplatného | *5/1/2021* |
| Datum ukončení předplatného | Datum vypršení platnosti předplatného | *4/30/2022* |
| ID odkazu | Propojení se všemi transakcemi, ke kterým dochází během upgradů. | *025d68a6-1bd6-42ab-9636-15e8d776a30e* |
| ProductQualifiers | Identifikátor, který se má znát při nákupu doplňků nebo zkušebních verzí | *["Doplněk"]* |
| ID povýšení | Identifikátor, který se má použít k načtení informací o povýšení. | *78bcf906-b945-4210-8818-cfb93caf12a1* |

>[!NOTE]
>Spotřebu Azure můžete odsouhlasit v souboru s vyrovnáním pro jeden nákup. Pokud to chcete udělat, přejděte do souboru s odsoustavou využití podle denního hodnocení a vyhledejte SVÉ ID předplatného. Zobrazí se všechny náklady spojené s vaším ID plánu Azure. Vaše ID předplatného Azure se zobrazí jako EntitlementID.
>

## <a name="how-to-connect-the-base-subscription-with-the-upgraded-subscription"></a>Jak připojit základní předplatné k upgradovanému předplatnému?

K vyhledání odpovídajících ID odkazů a jejich použití k načtení všech přidružených transakcí byste měli použít ID předplatného základního produktu. V kombinaci s ID předplatného a ID odkazu můžete připojit všechny upgrady, ke kterým došlo v jedné události.

## <a name="next-steps"></a>Další kroky

- [Fakturace a daně](billing.md)
