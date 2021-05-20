---
title: Fakturace plánu Azure – soubory & faktury
ms.topic: article
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak získat přístup k faktuře a struktuře souborů s vyrovnáním a porozumět jim související s fakturací plánu Azure.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 5ab086a4d15d16f094e33d19b81f1c93711916dc
ms.sourcegitcommit: e0444145d7720df948b9d02ae2469206db48dba5
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110201421"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Nové obchodní prostředí v CSP – Fakturace Azure 

**Odpovídající role:** Agent pro správu | Správce fakturace | Globální správce

Tento článek vysvětluje, jak získat přístup k faktuře a struktuře souborů s vyrovnáním související s fakturací plánu Azure a porozumět jim. Fakturace v rámci plánu Azure je zjednodušené prostředí pro fakturaci s využitím jednotného fakturačního data a kalendářního fakturačního období podle měsíců.

## <a name="summary-of-billing-essentials"></a>Souhrn základních informací o fakturaci

- **Datum faktury:** Soubor faktury a odsouhlasení budou k dispozici Partnerské centrum řídicím panelu nebo rozhraní API do 8. dne (půlnoc v UTC).

- **Fakturační období faktury:** Fakturační období faktury je v souladu s kalendářním měsícem, například 31. 10. 10. 11. 11. 2011.

- **Období služeb s poplatky:** Poplatky se budou v souladu s kalendářním měsícem. Pokud například fakturovaný partner přidá služby Azure prostřednictvím plánu Azure 15. 10. 2015 a zákazník začne 15. 10. 2015 spotřebovat služby Azure, pak fakturovaný partner obdrží fakturu a odsoustavu 8. 11. 10. 2011 pro spotřebu zákazníkům v 10./ 15. 10. 2011. Faktura za následující měsíc, která se vygeneruje 12. 8. 2018, obsahuje všechny poplatky za období služeb od 11. 1. do 31. 11. 2011.

- **Platební období faktury:** Net 60 dnů.

- Měna **faktury:** Od 28. ledna 2021 budou partneři v oblasti EU/EFTA a Spojeného království, kteří mají nové zákazníky a stávající zákazníky CSP, kteří poprvé kupují nové obchodní nabídky, jejichž tenanti byli vytvořeni před 11. květnem 2020, fakturovat za tyto nákupy v měně umístění partnera. Partneři, kteří se nacházejí mimo oblast EU/EFTA a Spojené království, se budou dál fakturovat v měně umístění partnera.

- **Pobídky pro partnery:** Placené 45 dnů od konce fakturačního měsíce.

## <a name="access-your-invoices-and-reconciliation-files"></a>Přístup k fakturám a souborům odsouhlasení

Globální správce nebo správce fakturace vaší společnosti obdrží e-mail, jakmile bude faktura připravená k zobrazení.

Přístup k faktuře a souboru s vyrovnáním:

1. Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard/) pro Partnerské centrum.

2. V nabídce partnerského centra vyberte **fakturace**.

3. Vyberte kartu pro **opakovanou** a **jednorázovou** a měnu, které vás zajímají.

   :::image type="content" source="images/azure/billing3.png" alt-text="fakturované":::

4. Vyberte soubor **faktury** nebo **souboru k odsouhlasení**.  

   Chcete-li zobrazit historické faktury a soubory rekognoskaci, rozbalte řádek historie fakturace níže.

## <a name="understanding-usage-data"></a>Seznámení s daty o využití 

1. Plán Azure je kořenový adresář nebo kontejner nejvyšší úrovně pro použití. Veškeré využití je vázané zpátky na jeden plán Azure.

2. V rámci plánu bude k dispozici jedno nebo několik předplatných Azure. Jedná se o kontejnery používané pro správu a nasazení prostředků. 

3. V rámci předplatného se skupiny prostředků přidávají do skupin prostředků. Všechny prostředky se nasazují do jedné skupiny prostředků. 

4. Mezi příklady prostředků patří virtuální počítače a účty úložiště. 

5. Měřiče emitování prostředků: měřiče měří spotřebu prostředku a jeden prostředek může vysílat využití pro více měřičů. Měřiče jsou označeny ProductId, SKUId a AvailabilityId. 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a>Hierarchie skupin prostředků předplatného a měření

**Účet Azure (tenant)**

- Předplatné A
    - Zdroj dat 1
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

4. Poplatky se netýkají úprav (částka je bez "kreditu získaného partnerem za spravované služby").

5. Další podrobnosti o fakturaci najdete v souboru s vyúčtováním faktur a souboru s denním hodnocením využití.

   :::image type="content" source="images/azure/invoice1.png" alt-text="Faktury":::

## <a name="read-the-invoice-reconciliation-file"></a>Přečtěte si soubor odsouhlasení faktury

1. Každá kombinace plánu a měření Azure může mít až dva fakturační řádky v souboru rekognoskaci.

2. Pokud je měřič kvalifikován pro jakýkoli typ slevy nebo kreditu (například vrstvené slevy nebo získaný kredit partnerských služeb) v celém kalendářním měsíci, bude soubor rekognoskaci obsahovat jenom jednu fakturační fakturu. Na sloupec **PriceAdjusmentDescription** se odkazuje na slevový nebo získaný kredit.

3. Pokud nejsou k dispozici žádné prostředky pro konkrétní měřič, který je kvalifikován pro zlevněný kredit nebo úvěr získaný pro partnery, bude soubor rekognoskaci obsahovat jenom jednu fakturační fakturu a skutečná Jednotková cena bude maloobchodní cena (což je jednotková cena).

4. Pokud měřič nebo všechny prostředky, které tento měřič vyvolaly, jsou určené pro kredity, které jsou pro **služby spravované** pro část měsíce, a soubor rekognoskaci bude obsahovat dva fakturační řádky. Jeden řádek bude představovat dny, ve kterých je měřený měřič, a druhý řádek bude představovat dny, které měřič nezpůsobil.

>[!NOTE]
>Můžete sjednotit využití Azure v jednorázovém souboru rekognoskaci nákupu. Provedete to tak, že přejdete na denní hodnocený soubor rekognoskaci využití a vyhledáte ID předplatného. Zobrazí se všechny náklady spojené s vaším ID plánu Azure. Vaše ID předplatného Azure se zobrazuje jako EntitlementID.

## <a name="read-the-daily-usage-file"></a>Přečtěte si soubor denního využití.

- Měřiče předplatného v rámci plánu Azure jsou ohodnocené a každý den se každoročně kumulovaná.

- **Získaný kredit partnerů pro spravované služby** je stanoven a použit každý den.

- Každý měřič předplatného bude mít řádek pro každý den v měsíci, kde byla spotřebována spotřeba.

- V následujícím příkladu:

  - Pro měření pro **služby spravované** z 7/1-7/3 se měří pro daný kredit. (Poznámka: efektivní Jednotková cena je maloobchodní cena nižší než partner získaný.

  - U služeb spravovaných z 7/4-7/7 se nezpůsobilo měření pro kredity, které jsou **pro služby spravované** . (Poznámka: efektivní Jednotková cena je maloobchodní cena).

  - Měřič kvalifikovaný pro **kredit získaný** partnerem pro služby spravované od 7/8 do 7/31 (všimněte si, že efektivní jednotková cena je maloobchodní cena menší než kredit získaný partnerem).

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a>Faktura v měně zákazníka

Služby Azure prostřednictvím plánu Azure se budou účtovat v USD a fakturují se v měně přiřazené zemi zákazníka. Pokud je fakturační měna mimo USD, použitá sazba devizové výměny (FX) se zobrazí na poslední stránce faktury. Směnné kurzy se určují měsíčně a použijí se na následující faktuře. Úplný seznam měn zemí najdete v nových obchodních nabídek pro země dostupnosti a [v matici měn zákazníků.](https://go.microsoft.com/fwlink/?linkid=2112354)

Microsoft se za převod řídí londýnské burzovní burzy. Používáme směnný kurz, který se rovná směnné sazbě zaznamenané k poslední sekundě posledního obchodního dne v měsíci na londýnské burze. Sazby FX se aktualizují a budou k dispozici den před prvním měsícem, pro který platí.

## <a name="azure-reservations"></a>Rezervace Azure


Pokud [nakupujete rezervace Azure](azure-reservations.md) prostřednictvím plánu Azure, můžete zvolit buď jednou, nebo měsíční fakturaci.


## <a name="azure-spending"></a>Útrata v Azure

Stávající prostředí útraty v Azure se aktualizuje tak, aby podporovalo fakturaci nového plánu Azure v Partnerské centrum. To umožňuje partnerům:

- Zobrazení, správa a příjem upozornění pro rozpočet nastavený na úrovni zákazníka 

- Zobrazení celkových odhadovaných výdajů v plánu Azure (rozdělené podle prostředků a úrovně měřiče)

Vzhledem k tomu, že fakturační model pro služby Azure prostřednictvím plánu Azure je spotřeba po platbě, aby se zabránilo vyšším fakturám, než se čekalo, mohou partneři použít měsíční rozpočet a sledovat procento využití. Rozpočet se může použít pro jednoho zákazníka nebo více zákazníků najednou. 

:::image type="content" source="images/azure/azurespend.png" alt-text="Útrata v Azure":::

## <a name="next-steps"></a>Další kroky

- Podívejte se, jak se počítá kredit získaný partnerem (PEC). Přihlaste se k Partnerské centrum [řídicího panelu a](https://partner.microsoft.com/dashboard/) vyhledejte ceník, který je k dispozici.

- Informace o [nákupu plánu Azure](purchase-azure-plan.md)

- Podívejte se na [ceník pro nové prostředí pro obchod v CSP](azure-plan-price-list.md) .
