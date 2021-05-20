---
title: Fakturace plánu Azure – & soubory rekognoskaci na faktuře
ms.topic: article
ms.date: 01/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se, jak získat přístup ke strukturám souborů faktur a odsouhlasení souvisejících s fakturací za plán Azure.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 757383ee264e58e7b4dc8ffefafe213cb49acb79
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149787"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Nové obchodní prostředí v CSP – Fakturace Azure 

**Příslušné role**: Agent správce | Správce fakturace | Globální správce

Tento článek vysvětluje, jak získat přístup ke struktuře souborů fakturace a odsouhlasení souvisejících s fakturací za plán Azure. Fakturace v rámci plánu Azure je zjednodušené fakturační prostředí s využitím zarovnaných a fakturačních období na základě kalendářního měsíce.

## <a name="summary-of-billing-essentials"></a>Shrnutí základních informací o fakturaci

- **Datum faktury**: soubor fakturace a odsouhlasení bude k dispozici v 8. bodě a řídicím panelu partnerského centra/rozhraní API.

- **Fakturační období faktury**: fakturační období faktury je zarovnané na kalendářní měsíc, například 10/1-10/31, 11/1-11/30.

- Poplatky **za období služby**: poplatky se budou zarovnávat do kalendářního měsíce. Pokud třeba účtováná partner přidá služby Azure prostřednictvím plánu Azure na 10/15 a zákazník začne využívat služby Azure na 10/15, bude vám účtovaný partner dostávat faktury nebo rekognoskaci na 11/8 za spotřebu zákazníka za období služby 10/15-10/31. Faktura za příští měsíc, která se vygeneruje v 12/8, obsahuje všechny poplatky za období služby 11/1-11/31.

- **Platební podmínka faktury**: NET 60 dní.

- **Měna faktury**: od 1. ledna 28 2021 partneři v oblasti EU/ESVO a UK, kteří noví zákazníci a stávající zákazníci s poskytovatelem CSP nakupují nové nabídky pro Commerce, jejichž klienti byli vytvořeni ještě dřív, než 11. května 2020, budou se fakturovat za tyto nákupy v měně partnera Location. Partneři, kteří se nacházejí mimo oblast EU/ESVO a UK, se budou dál účtovat v měně partnera umístění.

- **Pobídky pro partnery**: placené 45 dny od konce měsíce faktury.

## <a name="access-your-invoices-and-reconciliation-files"></a>Přístup k vašim fakturám a souborům pro odsouhlasení

Správce globálního správce nebo fakturace vaší společnosti obdrží e-mail, když je faktura připravena k zobrazení.

Přístup k souboru faktury a odsouhlasení:

1. Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard/) pro Partnerské centrum.

2. V nabídce Partnerské centrum vyberte **Fakturace.**

3. Vyberte kartu Opakující se **a** **Jednou a** měnu, kterou vás zajímá.

   :::image type="content" source="images/azure/billing3.png" alt-text="Fakturační":::

4. Vyberte **fakturu** nebo **soubor s vyrovnáním.**  

   Pokud chcete zobrazit historické faktury a soubory odsoudíte, rozbalte řádek Historie fakturace níže.

## <a name="understanding-usage-data"></a>Vysvětlení dat o využití 

1. Plán Azure je kontejner kořenové nebo nejvyšší úrovně pro použití. Veškeré využití se váže zpět na jeden plán Azure.

2. V rámci plánu bude jedno nebo více předplatných Azure. Jedná se o kontejnery používané pro správu a nasazení prostředků. 

3. Skupiny prostředků se v rámci předplatného přidávají do skupin prostředků. Každý prostředek je nasazený do jedné skupiny prostředků. 

4. Mezi příklady prostředků patří virtuální počítače a účty úložiště. 

5. Měřiče pro vysílání prostředků: Měřiče měří spotřebu prostředku a jeden prostředek může generovat využití pro více měřičů. Měřiče se identifikuje podle Id produktu, SKUId a ID dostupnosti. 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a>Hierarchie skupin prostředků předplatného a měření

**Účet Azure (tenant)**

- Předplatné A
    - ResourceGroup 1
        - Virtuální počítač (prostředek)
            - Výpočetní měření
        - Virtuální síť (prostředek)
            - Žádný měřič fakturace

    - Zdroj dat 2
        - Virtuální počítač (prostředek)
            - Měřič počítačů
        - SSD úrovně Premium spravovaný disk (prostředek)
            - Měřič kapacity úložiště
            - Měřič operací úložiště

- Předplatné B-kategorie prostředků 1 – Azure SQL (prostředek) – měřič DTU – VPN Gateway (prostředek) – měřič brány VPN

    - Zdroj dat 2
        - Virtual Network rozhraní (prostředek)
            - Žádný měřič fakturace

## <a name="read-the-invoice"></a>Přečtěte si fakturu

1. Faktura bude k dispozici později než osmý měsíc v měsíci.

2. Partneři mají 60 dní na platbu.

3. Fakturační období bude pokrývat určitý kalendářní měsíc, například 10/1-10/31.

4. Poplatky jsou očištěné od úprav (množství je netto "získaným partnerským kreditem pro spravované služby").

5. Další informace o fakturaci najdete v souboru rekognoskaci faktury a v souboru denního hodnocení využití.

   :::image type="content" source="images/azure/invoice1.png" alt-text="faktur":::

## <a name="read-the-invoice-reconciliation-file"></a>Přečtěte si soubor odsouhlasení faktury

1. Každá kombinace plánu a měření Azure může mít až dva fakturační řádky v souboru rekognoskaci.

2. Pokud je měřič kvalifikován pro jakýkoli typ slevy nebo kreditu (například vrstvené slevy nebo získaný kredit partnerských služeb) v celém kalendářním měsíci, bude soubor rekognoskaci obsahovat jenom jednu fakturační fakturu. Na sloupec **PriceAdjusmentDescription** se odkazuje na slevový nebo získaný kredit.

3. Pokud nejsou k dispozici žádné prostředky pro konkrétní měřič, který je kvalifikován pro zlevněný kredit nebo úvěr získaný pro partnery, bude soubor rekognoskaci obsahovat jenom jednu fakturační fakturu a skutečná Jednotková cena bude maloobchodní cena (což je jednotková cena).

4. Pokud měřič nebo všechny prostředky, které tento měřič vyvolaly, jsou určené pro kredity, které jsou pro **služby spravované** pro část měsíce, a soubor rekognoskaci bude obsahovat dva fakturační řádky. Jeden řádek bude představovat dny, ve kterých je měřený měřič, a druhý řádek bude představovat dny, které měřič nezpůsobil.

## <a name="read-the-daily-usage-file"></a>Přečtěte si soubor denního využití.

- Měřiče předplatného v rámci plánu Azure jsou ohodnocené a každý den se každoročně kumulovaná.

- **Získaný kredit partnerů pro spravované služby** je stanoven a použit každý den.

- Každý měřič předplatného bude mít řádek pro každý den v měsíci, kde byla spotřebována spotřeba.

- V následujícím příkladu:

  - Pro měření pro **služby spravované** z 7/1-7/3 se měří pro daný kredit. (Poznámka: efektivní Jednotková cena je maloobchodní cena nižší než partner získaný.

  - U služeb spravovaných z 7/4-7/7 se nezpůsobilo měření pro kredity, které jsou **pro služby spravované** . (Poznámka: efektivní Jednotková cena je maloobchodní cena).

  - Pro měřený **kredit pro služby spravované** z 7/8-7/31 se měří na měřič. (Poznámka: efektivní Jednotková cena je cenově dosažená za maloobchodní cenu, která je nižší než partnerský.

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a>Faktura v měně zákazníka

Ceny služeb Azure v rámci plánu Azure budou platit v USD a budou se fakturovat v přiřazené měně země zákazníka. Pokud fakturační měna není USD, zobrazí se na poslední stránce faktury použitá sazba za cizí Exchange (FX). Sazby za FX se určují měsíčně a platí pro následující fakturu. Úplný seznam měn za země najdete v části [Nová obchodní oddělení nabídky dostupnost země a měna zákazníka](https://go.microsoft.com/fwlink/?linkid=2112354).

Microsoft dodržuje při konverzi burzovní sklad s Londýn. Používáme směnný kurz, který se rovná směnnému kurzu zaznamenanému za poslední sekundu posledního pracovního dne v měsíci na burze cenných papírů v Londýně. Sazby za FX budou aktualizovány a k dispozici v den před prvním dnem v měsíci, pro které se vztahují.

## <a name="azure-reservations"></a>Rezervace Azure


Při nákupu [rezervací Azure](azure-reservations.md) prostřednictvím plánu Azure si můžete vybrat buď jednorázovou, nebo měsíční fakturaci.


## <a name="azure-spending"></a>Útrata v Azure

Stávající prostředí Azure útraty se aktualizuje tak, aby podporovalo nové účtování plánu Azure v partnerském centru. To umožňuje partnerům:

- Zobrazení, Správa a příjem výstrah pro rozpočtovou sadu na úrovni zákazníka 

- Zobrazení celkového odhadu útraty v plánu Azure (rozdělené podle prostředků a úrovně měřiče)

Vzhledem k tomu, že model fakturace pro služby Azure prostřednictvím plánu Azure je spotřeba po platbě, aby se předešlo většímu množství, než je očekávané, můžou partneři použít měsíční rozpočet a sledovat procento využití. Rozpočet lze použít na jednoho zákazníka nebo více zákazníků najednou. 

:::image type="content" source="images/azure/azurespend.png" alt-text="Útrata v Azure":::

## <a name="next-steps"></a>Další kroky

- Podívejte se, jak se počítá partner získaný kredit (PEC). Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard/) partnerského centra a vyhledejte dostupný ceník.

- Další informace o [nákupu plánu Azure](purchase-azure-plan.md)

- Podívejte se na [ceník pro nové prostředí pro obchod v CSP](azure-plan-price-list.md) .
