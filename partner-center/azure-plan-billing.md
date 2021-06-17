---
title: Fakturace plánu Azure – soubory & faktury
ms.topic: article
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak získat přístup k faktuře a struktuře souborů s vyrovnáním související s fakturací plánu Azure a porozumět jim.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 725050d370d1266205f979aa6317768d05ae5c4c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277177"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Nové obchodní prostředí v CSP – Fakturace Azure 

**Odpovídající role:** Agent pro správu | Správce fakturace | Globální správce

Tento článek vysvětluje, jak získat přístup k faktuře a struktuře souborů s vyrovnáním související s fakturací plánu Azure a porozumět jim. Fakturace v rámci plánu Azure je zjednodušené prostředí pro fakturaci s využitím jednotného fakturačního data a kalendářního fakturačního období podle měsíců.

## <a name="summary-of-billing-essentials"></a>Souhrn základních informací o fakturaci

- **Datum faktury:** Soubor faktury a odsouhlasení budou k dispozici Partnerské centrum řídicím panelu nebo rozhraní API do 8. dne (půlnoc v UTC).

- **Fakturační období faktury:** Fakturační období faktury je v souladu s kalendářním měsícem, například 10/1-10/31, 11.1.11/30.

- **Období služeb s poplatky:** Poplatky se budou v souladu s kalendářním měsícem. Pokud například fakturovaný partner přidá služby Azure prostřednictvím plánu Azure 15. 10. 2015 a zákazník začne 10. 15. 2015 spotřebovat služby Azure, pak fakturovaný partner obdrží fakturu a odsoustavu 11. 8. 2019 pro spotřebu zákazníkům pro období 10.10.15–31. 10. Faktura za následující měsíc, která se vygeneruje 12. 8. 2018, obsahuje všechny poplatky za období služeb od 11. 1. 2011.

- **Platební období faktury:** Net 60 dnů.

- Měna **faktury:** Od 28. ledna 2021 budou partneři v oblasti EU/EFTA a Velké Británie, kteří mají nové zákazníky a stávající zákazníky CSP, kteří poprvé kupují nové obchodní nabídky, jejichž tenanti byli vytvořeni před 11. květnem 2020, fakturovat za tyto nákupy v měně pro umístění partnera. Partneři, kteří se nacházejí mimo oblast EU/EFTA a Spojené království, se budou dál fakturovat v měně umístění partnera.

- **Pobídky pro partnery:** Placené 45 dnů od konce fakturačního měsíce.

## <a name="access-your-invoices-and-reconciliation-files"></a>Přístup k fakturám a souborům odsouhlasení

Jakmile bude faktura připravená k zobrazení, globální správce nebo správce fakturace vaší společnosti obdrží e-mail.

Přístup k faktuře a souboru s vyrovnáním:

1. Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard/) pro Partnerské centrum.

2. V nabídce Partnerské centrum vyberte **Fakturace.**

3. Vyberte kartu pro **Opakující** se a **Jednou a** měnu, kterou vás zajímá.

   :::image type="content" source="images/azure/billing3.png" alt-text="Fakturační.":::

4. Vyberte **fakturu** nebo **soubor s vyrovnáním.**  

   Pokud chcete zobrazit historické faktury a soubory odsoudíte, rozbalte řádek Historie fakturace níže.

## <a name="understanding-usage-data"></a>Vysvětlení dat o využití 

1. Plán Azure je kontejner kořenové nebo nejvyšší úrovně pro použití. Veškeré využití se váže zpět na jeden plán Azure.

2. V rámci plánu bude jedno nebo více předplatných Azure. Jedná se o kontejnery, které se používají pro správu a nasazení prostředků. 

3. Skupiny prostředků se v rámci předplatného přidávají do skupin prostředků. Každý prostředek se nasadí do jedné skupiny prostředků. 

4. Mezi příklady prostředků patří virtuální počítače a účty úložiště. 

5. Měřiče pro vysílání prostředků: Měřiče měří spotřebu prostředku a jeden prostředek může generovat využití pro více měřičů. Měřiče se identifikuje podle Id produktu, SKUId a ID dostupnosti. 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a>Hierarchie skupin prostředků předplatného a měření

**Účet Azure (tenant)**

- Předplatné A
    - ResourceGroup 1
        - Virtuální počítač (prostředek)
            - Měřič výpočetních prostředků
        - Virtuální síť (prostředek)
            - Bez fakturačního měřiče

    - ResourceGroup 2
        - Virtuální počítač (prostředek)
            - Měřič počítače
        - SSD úrovně Premium spravovaný disk (prostředek)
            - Měřič kapacity úložiště
            - Měřič operací úložiště

- Předplatné B -ResourceGroup 1 – Azure SQL (prostředek) – měřič DTU – VPN Gateway (prostředek) – měřič brány VPN

    - ResourceGroup 2
        - Virtual Network rozhraní (prostředek)
            - Bez fakturačního měřiče

## <a name="read-the-invoice"></a>Čtení faktury

1. Faktura bude k dispozici nejpozději do 8. dne každého měsíce.

2. Partneři mají na úhradu 60 dnů.

3. Fakturační období bude pokrývat daný kalendářní měsíc, například 31. 10. 10. 10.

4. Poplatky jsou bez vyrovnání (částka je bez "kreditu získaného partnerem za spravované služby").

5. Další podrobnosti o fakturaci najdete v souboru s vyúčtováním faktur a souboru s denním hodnocením využití.

   :::image type="content" source="images/azure/invoice1.png" alt-text="Faktury.":::

## <a name="read-the-invoice-reconciliation-file"></a>Čtení souboru s vyrovnáním faktur

1. Každá kombinace plánu a měřiče Azure může mít v souboru s vyúčtováním až dva fakturační řádky.

2. Pokud je měřič kvalifikovaný pro jakýkoli typ slevy nebo kreditu (například vrstvené slevy nebo kredit získaný partnerem za spravované služby) v průběhu celého kalendářního měsíce, bude soubor s vyúčtováním obsahovat pouze jeden řádek fakturace. Sloupec **PriceAdjusmentDescription bude** odkazovat na slevu nebo získaný kredit.

3. Pokud pro konkrétní měřič neexistují žádné prostředky, které jsou kvalifikované pro slevový kredit nebo kredit získaný partnerem, bude soubor s předsoudky obsahovat pouze jednu fakturační řádek a efektivní jednotková cena bude maloobchodní cena (což je jednotková cena).

4. Pokud měřič nebo prostředky, které tento měřič  vypouštějí, jsou kvalifikované pro kredit získaný partnerem za služby spravované po část měsíce, bude soubor s vyúčtováním obsahovat dva fakturační řádky. Jeden řádek bude představovat dny, ve které je měřič kvalifikovaný, a druhý řádek bude představovat dny, ve které měřič nebyl kvalifikován.

>[!NOTE]
>Spotřebu Azure můžete odsouhlasit v souboru s vyrovnáním pro jeden nákup. Pokud to chcete udělat, přejděte do souboru s odsoustavou využití podle denního hodnocení a vyhledejte SVÉ ID předplatného. Zobrazí se všechny náklady spojené s vaším ID plánu Azure. Vaše ID předplatného Azure se zobrazí jako EntitlementID.

## <a name="read-the-daily-usage-file"></a>Čtení souboru s denním využitím

- Měřiče předplatného v rámci plánu Azure jsou hodnoceny a simulovány každý den.

- **Kredit získaný partnerem za spravované služby** se určuje a používá každý den.

- Každý měřič předplatného bude mít řádek pro každý den v měsíci, ve kterém došlo ke spotřebě.

- V následujícím příkladu:

  - Měřič kvalifikovaný pro **kredit získaný** partnerem pro služby spravované od 7/1 do 7/3 (všimněte si, že efektivní jednotková cena je maloobchodní cena menší než kredit získaný partnerem.

  - Měřič neměl nárok  na kredit získaný partnerem pro služby spravované od 7/4 do 7/7 (všimněte si, že efektivní jednotková cena je maloobchodní cena).

  - Měřič kvalifikovaný pro **kredit získaný** partnerem pro služby spravované od 7/8 do 7/31 (všimněte si, že efektivní jednotková cena je maloobchodní cena menší než kredit získaný partnerem).

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2.":::

## <a name="invoice-in-customer-currency"></a>Faktura v měně zákazníka

Služby Azure prostřednictvím plánu Azure se budou účtovat v USD a fakturují se v měně přiřazené zemi zákazníka. Pokud je fakturační měna mimo USD, použitá sazba devizové výměny (FX) se zobrazí na poslední stránce faktury. Směnné kurzy se určují měsíčně a použijí se na následující faktuře. Úplný seznam měn zemí najdete v nových obchodních nabídek pro země dostupnosti a [v matici měn zákazníků.](https://go.microsoft.com/fwlink/?linkid=2112354)

Microsoft pro převod dodržuje london stock exchange. Používáme směnný kurz, který se rovná směnné sazbě zaznamenané k poslední sekundě posledního obchodního dne v měsíci na londýnské burze. Sazby FX se aktualizují a budou k dispozici den před prvním měsícem, pro který platí.

## <a name="azure-reservations"></a>Rezervace Azure


Pokud [nakupujete rezervace Azure](azure-reservations.md) prostřednictvím plánu Azure, můžete zvolit buď jednou, nebo měsíční fakturaci.


## <a name="azure-spending"></a>Útrata v Azure

Stávající prostředí útraty Azure se aktualizuje tak, aby podporovalo fakturaci nového plánu Azure v Partnerské centrum. To umožňuje partnerům:

- Zobrazení, správa a příjem upozornění pro rozpočet nastavený na úrovni zákazníka 

- Zobrazení celkových odhadovaných výdajů v plánu Azure (rozdělené podle prostředků a úrovně měřiče)

Vzhledem k tomu, že fakturační model pro služby Azure prostřednictvím plánu Azure je spotřeba po platbě, aby se zabránilo vyšším fakturám, než se čekalo, mohou partneři použít měsíční rozpočet a sledovat procento využití. Rozpočet se může použít pro jednoho zákazníka nebo více zákazníků najednou. 

:::image type="content" source="images/azure/azurespend.png" alt-text="Útraty za Azure.":::

## <a name="next-steps"></a>Další kroky

- Podívejte se, jak se počítá kredit získaný partnerem (PEC). Přihlaste se k řídicímu Partnerské centrum [a](https://partner.microsoft.com/dashboard/) vyhledejte dostupný ceník.

- Informace o [nákupu plánu Azure](purchase-azure-plan.md)

- Podívejte se [na ceník nového komerčního prostředí v CSP.](azure-plan-price-list.md)
