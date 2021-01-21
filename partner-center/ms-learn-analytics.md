---
title: Analýzy Microsoft Learn Datacenter v partnerském centru
ms.topic: article
ms.date: 08/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sledujte informace ve vaší společnosti využitím dat na jednotlivých školicích, dokončených modulech, dokončených výukových cestách a dalších.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 42c7af80ab49cee6e7043587207e553d2ffaa3ac
ms.sourcegitcommit: a7376c0ba8f4f3d01361bc227640311b486b3b6e
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/21/2020
ms.locfileid: "92527829"
---
# <a name="the-microsoft-learn-analytics-report-shows-the-status-of-learners-in-your-company"></a>Sestava Microsoft Learn Analytics zobrazuje stav učících ve vaší společnosti

**Příslušné role**
-   Globální správce
-   Správce partnera MPN

Sestava Microsoft Learn poskytuje informace o prodaných modulech ve vaší společnosti, včetně modulů, které dokončili, a studijních cest, na kterých jsou. V sestavě se zobrazí stav jednotlivých informací o jednotlivých uživatelích. Tato data může zobrazit globální správce a správce MPN pro vaši společnost.

## <a name="how-to-read-the-report"></a>Jak číst sestavu

### <a name="summary-charts"></a>Souhrnné grafy

Tyto grafy shrnují počet a měsíční kumulativní trendy pro vyškolené jednotlivce, dokončování modulů a studijní cesty.


**Počet vyškolených uživatelů**: počet všech jedinečných uživatelů, kteří během vybraného rozsahu dat dokončili aspoň jeden modul. 

**Minipanel trendu výukových jednotlivců**: Kumulativní počet měsíčně za měsíc v aktivních seznámcích 

**Počet dokončování modulu**: počet dokončování modulů v rámci společnosti partnera v podniku v průběhu vybraného období.
Pokud například "modul 1" dokončí 15 jednotlivců a "modul 2" byl dokončen stejnými 15 jednotlivci, bude počet dokončení modulu 30. Datum dokončení modulu by mělo být v rozsahu data vybrané.

**Zkrácený graf dokončování modulu trendu**: Kumulativní počet měsíců za měsíc dokončení modulu 

**Počet dokončení studijních cest**: počet doplňování studijních cest od těch, které se seznámíte se sestavami v podniku partnera v rámci vybraného rozsahu kalendářních dat.
Například pokud je Studijní cesta "cesta 1" dokončena o 20 jednotlivců a studijní cesta "cesta 2" byla dokončena stejnými 20 osobami, bude počet dokončení studijních kurzů 40. Datum dokončení cesty výuky by mělo spadat do vybraného rozsahu dat.

**Poučení o doplňováních výukových cest**: Kumulativní počet měsíců za měsíc pro dokončení studijních cest 

### <a name="trained-individuals-monthly-trend"></a>Měsíční trend školených jednotlivců

Tato data jsou trendem uživatelů vaší společnosti, kteří v daném měsíci dokončili modul v prvním čase. 

**Osa X** je měsíc pro vybraný časový filtr. 

**Osa Y** je počet aktivních uživatelů, kteří během daného měsíce zaregistrovali (při prvním dokončení modulu). Toto není kumulativní.

### <a name="module-completions-monthly-trend"></a>Měsíční trend dokončování modulu

Tato data jsou trendem modulů dokončených všemi uživateli vaší společnosti během daného měsíce. (nekumulativní) 

**Osa X** je měsíc pro vybraný časový filtr. 

**Osa Y** je počet dokončování modulu během daného měsíce. Toto není kumulativní.

### <a name="learning-path-completions-monthly-trend"></a>Měsíční trend dokončení studijních cest

Tato data jsou trendem studijních cest dokončených uživateli vaší společnosti během daného měsíce. (nekumulativní) 

**Osa X** je měsíc pro vybraný časový filtr. 

**Osa Y** je počet dokončení modulu v daném měsíci. Toto není kumulativní.

### <a name="learning-path-completion-tabs"></a>Karty doplňování cest výuky 

**Karta modul**

Tato karta obsahuje rozpis modulů dokončených ve vaší společnosti podle hlavních 5 názvů modulů. produkt, ke kterému je modul přidružen; a roli uživatele, která je pro modul relevantní.  

- Prstencový graf dokončení modulu: rozpis dokončování modulu (počet zobrazený v části Souhrn) podle názvů modulů.

Hodnota zobrazená uprostřed grafu představuje celkový počet dokončených modulů.

- Dokončování podle role: rozpis modulu dokončování rolí modulu. Pokud je modul přidružen k více rolím, pak jsou jednotlivé role přidány do počtu dokončení modulu.

Číslo zobrazené uprostřed grafu je počet jedinečných rolí pro dokončení modulu. 

- Dokončí produkt: rozpis modulu dokončuje produkt, na který je modul mapován. Pokud je modul přidružen k více produktům, pak jsou jednotlivé produkty přidány do počtu dokončení modulu.    

Číslo zobrazené uprostřed grafu je počet různých produktů pro dokončení modulu.  

**Karta cesta výuky**   

Tato karta obsahuje rozpis studijních tras dokončených ve vaší společnosti podle hlavních 5 názvů modulů; produkt, na který je mapována cesta výuky; a role, které se vztahují k této cestě výuky.  

- Prstenec dokončení studijních cest: rozpis dokončení studijních cest (počet zobrazený v části Souhrn) podle názvu.

- Dokončování podle role *: rozpis studijních cest, které role dokončuje. Pokud je modul přidružen k více rolím, pak jsou jednotlivé role přidány do počtu dokončení modulu.

- Dokončí produkt: rozpis výukových cest dokončí produkt, ke kterému je mapována cesta výuky. Pokud je modul přidružen k více produktům, pak jsou jednotlivé produkty přidány do počtu dokončení modulu.

### <a name="completions-by-learning-individuals"></a>Doplňování prostřednictvím vzdělávání jednotlivců

Zobrazuje seznam vyškolených uživatelů ve vaší společnosti a podrobnosti o jejich dokončených modulech a výukových cestách.

Microsoft Learn identifikuje informace o uživatelích s ID objektu uživatele. Na **kartě moduly** jsou všechny moduly setříděny podle dokončených modulů. Zobrazují se jim Microsoft Learn uživatelské jméno, ID objektu a počet modulů. Můžete hledat pomocí uživatelského jména. 

Na **kartě studijních cest** se zobrazí všechny přehledy seřazené podle studijních cest dokončených se zobrazeným zobrazovaným názvem, ID objektu a počtem modulů.

Získání podrobných informací o uživateli pomocí ID objektu uživatele: 

1. Přihlaste se do [Graph Exploreru](https://developer.microsoft.com/graph/graph-explorer ). (Musíte být globální správce tenanta Azure AD vaší společnosti.)

2. Zkopírujte ID objektu uživatele do [oblasti zvýrazněné](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f) v Graph Exploreru. 

## <a name="faq"></a>Nejčastější dotazy

1. Nedaří se mi mi zobrazit podrobnosti o studiu naší společnosti.

Tato sestava je k dispozici partnerům, kteří mají účet v partnerském centru. Pokud pořád jste v centru pro členství v partnerovi, nebudete moct zobrazit tuto sestavu.

2.  Kdo v naší firmě může zobrazit tuto sestavu? 

Sestavu může zobrazit globální správce a správce programu MPN.

3. Jak zajistím, aby všichni naši uživatelé přidružili své účty Microsoft Learn k účtu partnerského centra?

Po přidání nového uživatele globálním správcem musí uživatel přejít do svého **profilu** a přidružit svůj účet Microsoft Learn.

- V pravém rohu řídicího panelu vyberte ikonu **účtu** a pak vyberte **můj profil**. 

-  V rámci **učení** bude moci uživatel přidružit svůj účet Microsoft Learning a připojit své účet Microsoft k Partnerská Univerzita.

3. Můžu v této sestavě zobrazit všechny uživatele společnosti, kteří se k Microsoft Learn přihlásí pomocí účtu MSA?

V současné době nejlepším způsobem, jak to udělat, je přidat tyto uživatele do svého tenanta Azure AD a přidat je do partnerského centra, aby mohli přidružit svůj účet Microsoft Learn přes **můj profil** v partnerském centru. 

Pro uživatele, kteří používají jenom svůj účet MSA pro školení, bude mít tým Microsoft Learn v blízké budoucnosti možnost přidružit svůj pracovní e-mail ke svému Microsoft Learn profilu. 

## <a name="next-steps"></a>Další kroky

Další sestavy najdete v tématu [Přehled služby partner Center](partner-center-insights.md).

>[!NOTE] 
> Nezpracovaných dat v této sestavě si můžete stáhnout z oddílu stažení sestav na řídicím panelu Insights. [Další informace](pci-download-reports.md) 