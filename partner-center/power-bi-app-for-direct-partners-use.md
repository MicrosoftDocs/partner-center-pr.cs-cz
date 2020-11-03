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
ms.openlocfilehash: 248527fdbc536c552f7b2d00f208838b4ef19085
ms.sourcegitcommit: 0a6b1e6d845391539f54213efff00af4d23f028c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/14/2020
ms.locfileid: "92527000"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Zobrazení obchodních dat pomocí aplikace Datacenter Center Analytics pro Microsoft Power BI

**Platí pro**

- Partnerské centrum

**Příslušné role**

- Globální správce
- Správce uživatelů
- Agent prodeje
- Agent správce

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

### <a name="business-insights-report"></a>Sestava obchodních přehledů

- **Klienti zákazníka** : počet různých TENANTŮ Azure AD pro zákazníky, kteří si zakoupili předplatná

- **Novinka (posledních 30 dnů)** : noví zákazníci, kteří si nakupují aspoň jedno předplatné za posledních 30 dní

- Změny **(posledních 30 dnů)** : zákazníci bez všech předplatných "aktivní", "v odkladu" nebo "zakázáno".

- **Novinka (posledních 24 hodin)** : noví zákazníci nakupují aspoň jedno předplatné za posledních 24 hodin

- **Odhadované měsíční náklady za posledních 12 měsíců** : Měsíční trend odhadované částky za měsíc v měsíci, který je v období posledních 12 měsíců agregovaný měsíčně.

- **Odhadované náklady podle produktu za posledních 12 měsíců** : produkty prodávané podle odhadované částky pro fakturační dolary, které jsou shrnuty v období posledních 12 měsíců. Tento stav označuje nejdůležitější produkty, které přináší většinu výnosů.

- **Zákazníci za posledních 12 měsíců** : trend za měsíc měsíčně nových zákazníků a změny, které se zákazníkům v období posledních 12 měsíců agreguje měsíčně

- **Odhadované náklady podle zákazníka za posledních 12 měsíců** : zákazníci setříděni podle odhadované částky předběžného daňového dolaru shrnuté v období posledních 12 měsíců. Tento stav označuje nejdůležitější zákazníky, kteří přinášejí většinu výnosů.

- **Počet zákazníků podle produktu** : produktů prodávaných seřazené podle přidružených zákazníků. Tento stav označuje nejdůležitější produkty prodávané většině zákazníků.

### <a name="subscription-insights-report"></a>Sestava přehledů předplatných

- **Stav předplatného** :

- Aktivní: předplatná, která patří do stavu "aktivní" nebo "ve lhůtě".

  - Pozastaveno: odběry patřící do stavu zakázáno

  - Nezřízeno: odběry patřící do stavu "de-provisioned" nebo "vypršela platnost"

- **Stav vypršení platnosti** :

  - Vypršela platnost předplatných, jejichž platnost již vypršela (kde koncové datum předplatného je v minulosti).

  - Vypršení platnosti po 30 dnech: předplatná, jejichž platnost vyprší po 30 dnech (kde koncové datum předplatného je po následujících 30 dnech)

  - Vypršení platnosti během 30 dnů: předplatná, jejichž platnost vyprší během následujících 30 dnů (kde datum ukončení předplatného spadá do rozmezí dnešních a dalších 30 dnů)

- **Celkový počet předplatných** : předplatná ve stavu "aktivní", "ve lhůtě" nebo "zakázáno"

- **Novinka (posledních 30 dnů)** : nové předplatné zakoupené zákazníky během posledních 30 dnů

- **Novinka (posledních 24 hodin)** : nové předplatné zakoupené zákazníky během posledních 24 hodin

- **Platnost vyprší za 30 dní** : předplatná, jejichž platnost vyprší během následujících 30 dnů

- Změny **(posledních 30 dnů)** : předplatná, která byla během posledních 30 dnů zrušena nebo pozastavena (zakázána)

- **Distribuce podle typů předplatného** :% distribuce celkových předplatných podle licencí a typu předplatného založeného na použití

- **Počet aktivních předplatných podle produktu** : produkty prodávané seřazené podle aktivního počtu předplatných

- **Předplatná za posledních 12 měsíců** : trend za měsíc měsíčně nových předplatných a všech předplatných, které jsou v období posledních 12 měsíců agregované měsíčně.

- **Podrobnosti o předplatném zákazníka** : podrobné zobrazení zákazníků, předplatných a nabídek

### <a name="license-insights-report"></a>Sestava o licenci License Insights:

- **Celkem licencí** : celkový počet licencí agregovaných napříč všemi předplatnými na základě licencí

- **Novinka (posledních 30 dnů)** : Přidání licence během posledních 30 dnů

- Změny **(posledních 30 dnů)** : snížení počtu licencí během posledních 30 dnů

- **Novinka (posledních 24 hodin)** : Přidání licence během posledních 24 hodin

- **Licence v posledních 90 dnech** : Měsíční trend přidaných licencí a jejich snížení na měsíc za období posledních 90 dnů

- **Počet aktivních licencí podle produktu** : produkty prodávané seřazené podle počtu aktivních licencí

- **Počet aktivních licencí podle zákazníka** : zákazníci seřazené podle počtu aktivních licencí

- **Podrobnosti o licenční události zákazníka v posledních 90 dnech** : podrobné zobrazení událostí zákazníků, předplatných a předplatných včetně data události, názvu události, množství a změny v množství.

### <a name="licenses-usage-report"></a>Sestava využití licencí:

- **Licence přiřazené produktem** : prodávané produkty seřazené podle počtu přiřazení licencí

- **Licence používané produktem** : produkty prodávané seřazené podle počtu využití licencí

- **Zákaznická distribuce přiřazených licencí** :% rozdělení celkových zákazníků v intervalech, které jsou v intervalech 20% v rozsahu podle přiřazení licencí%

- **Zákaznická distribuce licencí, které se používají** :% rozdělení celkových zákazníků v intervalech po 20% rozsahu podle využití licencí%

- **Licence přiřazené zákazníkem** : podrobné zobrazení prodaných licencí a licencí přiřazených zákazníky a produkty

- **Licence používané zákazníkem** : podrobné zobrazení prodaných licencí a licencí používaných zákazníky a produkty

### <a name="azure-insights-report"></a>Sestava Azure Insights:

- **Zákazníci na základě využití za posledních 12 měsíců** : Měsíční trend nových zákazníků založených na používání a změny v rámci využívání, které jsou v průběhu posledních 12 měsíců shrnuté měsíčně.

- **Předplatná založená na využití za posledních 12 měsíců** : Měsíční trend nových předplatných založených na využití a změny předplatných na základě využití, které jsou v období posledních 12 měsíců shrnuté po měsících.

- **Odhadované náklady na využití od zákazníka za posledních 60 dní** : zákazníci na základě využití setříděni podle odhadované částky za použití předběžného daňového dolaru v období posledních 60 dnů. Tento stav indikuje zákazníky s nejvyšším využitím, který přináší nejvíc výnosů.

- **Odhadované náklady na využití podle kategorie za posledních 60 dní** : kategorie měřičů předplatných založených na použití seřazené podle odhadované částky předběžného daňového dolaru v období posledních 60 dnů.

- **Odhadované náklady na využití podle předplatného v posledních 60 dnech** : předplatná na základě využití odhadovaná částka za fakturační dolary, která se agreguje za období posledních 60 dnů.

- **Odhadované náklady na využití na zákazníky podle rozpočtu útraty** : zákazníci, kteří se seřadili podle procenta jejich aktuálního využití, překračuje prahovou hodnotu (100%).

### <a name="azure-resource-usage-report"></a>Sestava využití prostředků Azure:

- **Využití prostředků Azure podle dne pro vybrané období** : denní jednotky spotřeby pro každý měřený prostředek v každém předplatném na základě využití pro vybrané období během posledních 60 dnů.

- **Odhadované náklady na využití prostředků Azure pro vybrané období** : Odhadované náklady na základě karty s nejnovějšími sazbami pro každý měřený prostředek v každém předplatném na základě využití pro vybrané období během posledních 60 dnů. 

## <a name="next-steps"></a>Další kroky

- [Přehled služby partner Center Analytics pro aplikaci Power BI](power-bi-app-for-direct-partners.md)

- [Instalace a vyzkoušení aplikace Analýzy v Partnerském centru pro Microsoft Power BI](power-bi-app-for-direct-partners-install.md)
