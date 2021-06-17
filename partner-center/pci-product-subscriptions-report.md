---
title: Sestava předplatných služby partner Center Insights
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Podívejte se, co dobře děláte, a kde můžete vylepšit cloudová předplatná, která obchodujete nebo spravujete pro vaše zákazníky.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bf2663122ca95e8d610c8be792a26682ae1718bf
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276310"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>Sestava předplatných produktů dostupná na řídicím panelu přehledy partnerského centra

**Příslušné role**: globální správce | Agent správce | Prohlížeč sestav | Prohlížeč sestav Executive

Sestava odběry produktů představuje analýzy cloudových předplatných, které jste prodali nebo které spravujete pro vaše zákazníky. Jedná se o konkrétní produktovou zprávu, která zahrnuje výkon předplatných přidružených ke cloudovým produktům, jako je například Office 365, Azure, Dynamics a další.

Následující části můžete zobrazit v sestavě odběry produktů.

- Souhrn
- Geografické rozšiřování předplatných
- Trend přidání a změn předplatných
- Distribuce předplatného podle umístění partnera, prodejní kanál, SKU, typ připojení partnera, segment
- Trend podle stavů předplatného
- Trend produktů

 > [!NOTE]
 > Tato sestava je k dispozici na řídicím panelu Insights. Pokud chcete zobrazit tuto sestavu, musíte mít přiřazenou konkrétní roli v partnerském centru, jako je například globální správce, správce účtu, Prohlížeč sestav nebo správce sestav v nástroji Executive. Další informace najdete v tématu globální správce vaší společnosti. konkrétní typy dat v této sestavě mohou být také k dispozici pouze uživatelům s oprávněními správce sestav nástroje Executive.

## <a name="summary"></a>Souhrn

V části Souhrn najdete zobrazení snímků klíčových ukazatelů výkonu (KPI) souvisejících s předplatným, která se prodávají nebo spravují pro vaše zákazníky.  

:::image type="content" source="images/pci/pci-sub-report-summary-1.png" alt-text="Souhrn sestavy předplatných.":::

Další informace o jednotlivých částech souhrnu najdete níže:

- Předplatná:
  - Aktuální počet předplatných cloudových produktů, které jste prodali nebo spravovali vámi.
  - Procentuální nárůst nebo odmítnutí předplatných během vybraného rozsahu kalendářních dat.
  - Mikrograf prezentuje trend počtu předplatných předplatných v průběhu vybraného rozsahu dat měsíčně.

- Aktivní předplatná:
  - Aktuální počet odběrů cloudových produktů s aktivním využitím měřený na základě telemetrie produktů Tím se vyloučí všechna zkušební předplatná v případě předplatných Azure.
  - Procentuální nárůst nebo odmítnutí aktivních předplatných za vybrané časové období
  - Mikrograf prezentuje trend aktivních předplatných za měsíc v průběhu vybraného období.

- Přidaná předplatná:
  - Celkový počet přidaných zákaznických předplatných (prodaných nebo spravovaných) během vybraného časového období. Nová předplatná s **aktivním** nebo **obnoveným** stavem se počítají jako přidaná předplatná.
  - Procentuální nárůst nebo odmítnutí předplatných přidaných za poslední celý měsíc v porovnání s prvním celým měsícem
  - Mikrograf prezentuje měsíční trend předplatných přidaných během vybraného časového období.

- Předplatné byly v provozu:
  - Celkový počet změn zákaznických předplatných v průběhu vybraného rozsahu kalendářních dat. Předplatná s  **odloženým nebo pozastaveným** stavem v daném měsíci se počítají jako zrušené předplatné.  
  - Procento předplatných, které bylo v průběhu vybraného období změněno.
  - Mikrograf prezentuje měsíční trend předplatných, která se ve vybraném časovém období převzala.

- Předplatná podle produktů: rozpis počtu aktuálních předplatných podle cloudových produktů.

## <a name="geographical-spread-of-subscriptions"></a>Geografické rozšiřování předplatných

Zobrazení **předplatná podle geografického** zobrazení zobrazuje geografickou distribuci celkových předplatných na trzích zákazníků. Celková částka předplatného zahrnuje prodané předplatné i aktivní předplatná.

V tabulce **počet zemí/oblastí** je uvedena celková země/oblasti, ve kterých máte předplatná, a částku za zemi celkových a aktivních předplatných.

Můžete vyhledat a vybrat zemi v mřížce pro přiblížení do umístění v mapě. Stisknutím možnosti **Domů** na mapě se vraťte k původnímu zobrazení. Pokud chcete zobrazit všechna předplatná a aktivní předplatná podle země, najeďte myší na mapu. Obě pole v mřížce lze seřadit.

:::image type="content" source="images/pci/pci-sub-report-sub-by-geography-2.png" alt-text="předplatná podle geografického umístění":::

## <a name="subscription-addschurns"></a>Přidání a změny předplatného

Toto zobrazení představuje trend předplatných. Ty jsou rozdělené do různých kategorií (nové, existující, změny) pro vybraný rozsah dat. Osa X představuje měsíce vybraného rozsahu kalendářních dat. Osa Y představuje počet předplatných. Ovlivněné odběry jsou reprezentovány na záporném měřítku osy Y. 

Skládaný sloupcový graf prezentuje rozpis nových, stávajících a změněných předplatných v daném měsíci. Můžete znovu sestavit sloupcový graf, rozdělený dolů s konkrétními položkami zásobníku. Provedete to tak, že vyberete tyto konkrétní položky v legendě. K přiblížení konkrétního období můžete použít také posuvník v horní části grafu.

:::image type="content" source="images/pci/pci-sub-report-sub-adds-churns-3.png" alt-text="předplatné přináší změny a změny.":::

## <a name="subscription-distribution"></a>Distribuce předplatného

Toto zobrazení představuje rozpis vašich aktuálních předplatných podle umístění MPN, zákaznických segmentů, prodejních kanálů/cenového modelu Azure a typu přidělení (například partnera DPOR, DAP a dalších). Vyberte příslušné karty pro zobrazení rozpisu podle těchto kategorií. Chcete-li vytvořit výsečový graf s rozpisem konkrétních kategorií položek, vyberte tyto kategorie položek v legendě.

:::image type="content" source="images/pci/pci-sub-report-distribution-4.png" alt-text="distribuce předplatného.":::

## <a name="subscription-state-distribution"></a>Distribuce stavu předplatného

Toto zobrazení ukazuje distribuci aktuálních zákaznických předplatných podle stavu nebo stavu předplatného. To zahrnuje následující stavy předplatného: **aktivní**, **zakázané**, **zrušení zřízení**, **otevřené**, **v období odkladu**, **uzavřené** a **jiné**.

:::image type="content" source="images/pci/pci-sub-report-sub-states-5.png" alt-text="distribuce stavu předplatného":::

## <a name="products-trend"></a>Trend produktů

Toto zobrazení ukazuje sloupcový graf a dva výsečové grafy. Pruhový graf prezentuje měsíční trend předplatných rozdělených podle komerčních produktů, jako je Azure, Office, Dynamics atd.

V těchto dvou výsečových grafech se zobrazuje rozpis aktuálních zákaznických předplatných. První výsečový graf rozdělí odběry podle produktů. Druhý výsečový graf rozdělí předplatná podle skladů nebo plánů. Když vyberete produkt v výsečovém grafu rozpis **podle produktů** , zobrazí se v sousedním výsečovém grafu rozpis předplatných těchto produktů pomocí SKU.

:::image type="content" source="images/pci/pci-sub-report-prods-trend-6.png" alt-text="trend produktů.":::

> [!NOTE]
 > Počet předplatných rozepsaný podle SKU nemusí vždy odpovídat celkovému počtu předplatných pro daný produkt. Tato situace může nastat, pokud zákazník zakoupil více SKU v rámci stejného předplatného produktu.

## <a name="next-steps"></a>Další kroky

- Další sestavy najdete v tématu [Přehled služby partner Center](partner-center-insights.md).

>[!NOTE] 
> Nezpracovaných dat v této sestavě si můžete stáhnout z oddílu stažení sestav na řídicím panelu Insights. [Další informace](pci-download-reports.md) 
