---
title: Použití analýzy partnerského centra pro Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se zobrazovat obchodní data pomocí aplikace Datacenter Center Analytics pro Power BI (pro přímé partnery v CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 96fe57f6e89928a69051c2e201c444882500b844
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855025"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Zobrazení obchodních dat pomocí aplikace Datacenter Center Analytics pro Microsoft Power BI



**Příslušné role**: globální správce | Správce správy uživatelů | Prodejní agent | Agent správce

## <a name="view-your-business-data"></a>Zobrazení obchodních dat

Získejte vizuální reprezentaci vašich obchodních dat pomocí aplikace Datacenter Center Analytics pro Power BI, včetně těchto:

- Růst zákaznické základny, předplatných a licencí

- Využití produktů Office 365, Microsoft Dynamics a Microsoft Azure

- Denní spotřeba jednotek pro každý měřený prostředek v každém předplatném Azure za posledních 60 dní

- Odhadované náklady (na základě karty s nejnovějšími sazbami)

- Možnost exportovat datové sady a vytvářet vlastní sestavy, včetně jednotlivých zákazníků.

### <a name="about-the-partner-center-analytics-app-preview-release"></a>Informace o verzi Preview partnerského centra pro aplikaci Analytics

- Tato aplikace je určena pouze pro přímé partnery v programu Cloud Solution Provider. Jiní partneři v CSP (například nepřímo prodejci) se nebudou moci přihlásit.

- Všechny odhadované náklady jsou platby před zdaněním a fakturaci a nejsou právně závazné. Odhadované náklady se mají použít jenom pro data Insights.

- Informace o zákaznících jsou založené na předplatných. Zákazníci, u kterých jste nedávno vytvořili účty pro, ale kteří ještě nemají předplatné, nejsou zahrnuti do počtu.

- Odhadované náklady vycházejí z karty nejnovějších sazeb, která vychází z cen CSP.

- Dny jsou dny kalendáře.

### <a name="business-insights-report"></a>Sestava Business Insights

- **Tenanti zákazníků:** Počet různých tenantů Azure AD zákazníků, kteří si zakoupili předplatná

- **Nové (posledních 30 dnů):** Noví zákazníci kupující alespoň jedno předplatné za posledních 30 dnů

- **Četnost změn (posledních 30 dnů):** Zákazníci bez jakýchkoli aktivních předplatných, předplatných s odkladem nebo zakázaných předplatných

- **Nové (posledních 24 hodin):** Noví zákazníci kupující alespoň jedno předplatné za posledních 24 hodin

- **Odhadované měsíční náklady za posledních 12** měsíců: Trend odhadované částky faktury před zdaněním agregované měsíčně za období posledních 12 měsíců

- **Odhadované náklady podle produktu za posledních 12** měsíců: Prodané produkty seřazené podle odhadované částky faktury před zdaněním agregované za období posledních 12 měsíců. Tento stav označuje hlavní produkty, které mají největší výnosy.

- **Zákazníci za posledních 12 měsíců:** Trend nových zákazníků po měsících a zákazníků se četností změn agregovaný měsíčně za období posledních 12 měsíců

- **Odhadované náklady podle zákazníků za posledních 12** měsíců: Zákazníci seřazení podle odhadované částky faktury před zdaněním agregované za období posledních 12 měsíců. Tento stav indikuje, že nejvíce výnosů mají zákazníci s nejvyššími tržby.

- **Počet zákazníků podle produktu:** Prodané produkty seřazené podle přidružených zákazníků. Tento stav označuje nejprodávané produkty většině zákazníků.

### <a name="subscription-insights-report"></a>Sestava Přehledy předplatného

- **Stav předplatného:**

- Aktivní: Předplatná patřící do "aktivní" nebo "v odkladu"

  - Pozastaveno: Předplatná patřící do stavu Zakázáno

  - Zrušit zřízení: Předplatná patřící do stavu "není zřízeno" nebo "vypršela jeho platnost".

- **Stav vypršení platnosti:**

  - Platnost vypršela: Předplatná, jejichž platnost už vypršela (u kterých vypršelo koncové datum předplatného)

  - Vypršení platnosti po 30 dnech: předplatná, jejichž platnost vyprší po 30 dnech (kde koncové datum předplatného je po následujících 30 dnech)

  - Vypršení platnosti během 30 dnů: předplatná, jejichž platnost vyprší během následujících 30 dnů (kde datum ukončení předplatného spadá do rozmezí dnešních a dalších 30 dnů)

- **Celkový počet předplatných**: předplatná ve stavu "aktivní", "ve lhůtě" nebo "zakázáno"

- **Novinka (posledních 30 dnů)**: nové předplatné zakoupené zákazníky během posledních 30 dnů

- **Novinka (posledních 24 hodin)**: nové předplatné zakoupené zákazníky během posledních 24 hodin

- **Platnost vyprší za 30 dní**: předplatná, jejichž platnost vyprší během následujících 30 dnů

- Změny **(posledních 30 dnů)**: předplatná, která byla během posledních 30 dnů zrušena nebo pozastavena (zakázána)

- **Distribuce podle typů předplatného**:% distribuce celkových předplatných podle licencí a typu předplatného založeného na použití

- **Počet aktivních předplatných podle produktu**: produkty prodávané seřazené podle aktivního počtu předplatných

- **Předplatná za posledních 12 měsíců**: trend za měsíc měsíčně nových předplatných a všech předplatných, které jsou v období posledních 12 měsíců agregované měsíčně.

- **Podrobnosti o předplatném zákazníka**: podrobné zobrazení zákazníků, předplatných a nabídek

### <a name="license-insights-report"></a>Sestava o licenci License Insights:

- **Celkem licencí**: celkový počet licencí agregovaných napříč všemi předplatnými na základě licencí

- **Novinka (posledních 30 dnů)**: Přidání licence během posledních 30 dnů

- Změny **(posledních 30 dnů)**: snížení počtu licencí během posledních 30 dnů

- **Novinka (posledních 24 hodin)**: Přidání licence během posledních 24 hodin

- **Licence v posledních 90 dnech**: Měsíční trend přidaných licencí a jejich snížení na měsíc za období posledních 90 dnů

- **Počet aktivních licencí podle produktu**: produkty prodávané seřazené podle počtu aktivních licencí

- **Počet aktivních licencí podle zákazníka**: zákazníci seřazené podle počtu aktivních licencí

- Podrobnosti o události zákaznické licence za **posledních 90** dnů: Podrobné zobrazení událostí zákazníků, předplatných a odběrů, včetně data události, názvu události, množství a změny množství.

### <a name="licenses-usage-report"></a>Sestava využití licencí:

- **Licence přiřazené podle produktu:** Prodané produkty seřazené podle počtu přiřazení licencí

- **Licence, které se používají podle produktu:** Prodané produkty seřazené podle počtu využití licencí

- **Distribuce přiřazených licencí ze strany** zákazníků: % rozdělení celkového počtu zákazníků v kbelíkůch po 20 % rozsahu podle % přiřazení licence

- **Distribuce licencí, které se používají** pro zákazníky: % distribuce celkového počtu zákazníků rozdělených do kbelíků o 20% rozsahu podle % využití licencí

- **Licence přiřazené zákazníkem:** Podrobné zobrazení prodaných licencí a licencí přiřazených zákazníky a produkty

- **Licence, které používá zákazník:** Podrobné zobrazení prodaných licencí a licencí, které používají zákazníci a produkty

### <a name="azure-insights-report"></a>Sestava Azure Insights:

- Zákazníci se založenými na využití za **posledních 12** měsíců: Trend měsíčních trendů nových zákazníků založených na využití a zákazníků založených na churnedu využití agregovaných měsíčně za období posledních 12 měsíců

- Předplatná založená na využití za **posledních 12** měsíců: Trend nových předplatných založených na využití a předplatných založených na četnosti změn agregovaných měsíčně za období posledních 12 měsíců

- **Odhadované náklady** na využití podle zákazníka za posledních 60 dnů: Zákazníci na základě využití seřazení podle odhadované částky faktury před zdaněním agregované za období posledních 60 dnů. Tento stav znamená, že zákazníci s nejvyšším využitím mají největší výnosy.

- Odhadované náklady na využití podle kategorií za posledních **60** dnů: Kategorie měřičů předplatných založených na využití seřazené podle odhadované částky faktury před zdaněním agregované za období posledních 60 dnů.

- **Odhadované náklady** na využití podle předplatného za posledních 60 dnů: Předplatná založená na využití podle odhadované částky faktury před zdaněním agregované za období posledních 60 dnů.

- **Odhadované náklady na využití na zákazníky podle rozpočtu útraty**: zákazníci, kteří se seřadili podle procenta jejich aktuálního využití, překračuje prahovou hodnotu (100%).

### <a name="azure-resource-usage-report"></a>Sestava využití prostředků Azure:

- **Využití prostředků Azure podle dne pro vybrané období**: denní jednotky spotřeby pro každý měřený prostředek v každém předplatném na základě využití pro vybrané období během posledních 60 dnů.

- **Odhadované náklady na využití prostředků Azure pro vybrané období**: Odhadované náklady na základě karty s nejnovějšími sazbami pro každý měřený prostředek v každém předplatném na základě využití pro vybrané období během posledních 60 dnů. 

## <a name="next-steps"></a>Další kroky

- [Přehled služby partner Center Analytics pro aplikaci Power BI](power-bi-app-for-direct-partners.md)

- [Instalace a vyzkoušení aplikace Analýzy v Partnerském centru pro Microsoft Power BI](power-bi-app-for-direct-partners-install.md)
