---
title: Přesun zákazníků z aktuálních nabídek Azure do plánu Azure
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak zprostředkovatelé CSP Partnerské centrum k přesunu zákazníků ze stávajících nabídek Azure CSP do služeb Azure v rámci plánu Azure.
author: mowree
ms.author: mowrim
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/16/2020
ms.openlocfilehash: 770df3cff40b8cc51eab16fb95d0bd43967a5a69
ms.sourcegitcommit: 3ac88f7925bfe1df90e267ee5c1ee4d752ac92d4
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/29/2021
ms.locfileid: "113013263"
---
# <a name="transition-customers-to-azure-plan-from-existing-csp-azure-offers"></a>Přechod zákazníků na plán Azure ze stávajících nabídek Azure CSP

**Platí pro:** Partnerské centrum 

**Odpovídající role:** Agent pro správu | Správce fakturace | Globální správce | Agent helpdesku | Sales agent | Správce správy uživatelů

Tento článek vysvětluje, jak zprostředkovatelé CSP Partnerské centrum k přesunu zákazníků z existujících nabídek Azure CSP do služeb Azure v rámci plánu Azure. Nepřímí poskytovatelé a partneři s přímým vyúčtováním mohou přejít na nové komerční prostředí dostupné v programu Microsoft Cloud Service Provider Program (CSP) pro Azure. (Nepřímí prodejci budou muset pracovat se svými nepřímými poskytovateli.) Zákazníci budou mít zjednodušený způsob nákupu cloudových služeb, ať už nákup od partnerů, prodejců Microsoftu nebo přímo na webu.

Možnost přechodu je pouze pro zákazníky, kteří přechádují na nové obchodní prostředí Pro Azure a kteří podepsali Smlouva se zákazníkem Microsoftu. Není pro jiné nabídky v CSP, jako je Office 365 nebo Dynamics 365.

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>Převod stávajících nabídek CSP na plán Azure

V novém komerčním prostředí v programu CSP můžete zákazníka přecházet ze stávajících nabídek Azure CSP na služby Azure v rámci plánu Azure z Partnerské centrum. Aby to bylo nutné, partner a zákazník musí mít na meziprodejní vztah prostřednictvím Partnerské centrum a zákazník musí smlouvu Smlouva se zákazníkem Microsoftu.

### <a name="select-transition-to-azure-plan"></a>Výběr přechodu na plán Azure

1. Vyberte plán Azure pro vašeho zákazníka.

2. Vyberte **Převod fakturace na plán Azure.**

   :::image type="content" source="images/azure/transition1.png" alt-text="Snímek obrazovky zobrazující informace o sestavě předplatných na základě využití s možností výběru s názvem: Převod fakturace předplatného Azure na plán Azure":::

3. Vyberte **Pokračovat**.

   :::image type="content" source="images/azure/transition2.png" alt-text="Dialogové okno s názvem Přechod do plánu Azure s důsledky pro přečtení informací o přechodu a dvou možnostech, které je třeba vybrat: Pokračovat nebo Zrušit.":::

   Váš zákazník bude přeován na plán Azure.

   **Pracovní postup přechodu automatizuje** požadované kroky:

   - Nákup plánů Azure
   - Jeden plán na zákazníka ve scénářích s přímým CSP  
   - Jeden plán na prodejce  

   Partner například zakoupil dvě nové Microsoft Azure a do nákupu zahrnul dvě odlišné por. V takovém případě pracovní postup přechodu zakoupí dva plány Azure (jeden na prodejce) a automaticky namapuje příslušná předplatná Azure v rámci plánů Azure.  

   **Mapování předplatného Azure na plán Azure**

   Po zakoupení plánů Azure bude náš systém mapovat stávající předplatná Azure na plány Azure. Průběh můžete zobrazit v Azure Portal i v Partnerském centru.

4. Vraťte se na stránku Partnerské centrum **předplatných** zákazníka a aktualizujte limit rozpočtu pomocí místní měny.

   :::image type="content" source="images/azure/transition3.png" alt-text="Částečné zobrazení stránky Partnerské centrum s limity rozpočtu nastavenými v místní měně pro fakturační období.":::

   >[!NOTE]
   >Rozpočet, který jste nastavili Partnerské centrum, se do tohoto Azure Portal. Měli byste také nastavit rozpočet a upozornění v Azure Portal.

   Po přechodu na plán Azure už pro tohoto zákazníka nemůžete kupovat předplatná Azure. Předplatná vytvoříte v rámci plánu Azure v Azure Portal.

   >[!NOTE]
   > Všechna předplatná Azure zakoupená prostřednictvím RBAC v rámci plánu Azure se budou účtovat v místní měně. Nebudou se používat sazby FX.

### <a name="track-your-transition-details"></a>Sledování podrobností o přechodu

Průběh přechodu můžete sledovat Azure Portal i v Partnerské centrum.

:::image type="content" source="images/azure/details1.png" alt-text="Snímek obrazovky zobrazující tabulku se seznamem podrobností o přechodu na předplatné – zahrnuje ID předplatného, datum přechodu a stav převodu":::

### <a name="billing-impact-to-partners"></a>Dopad fakturace na partnery

Pokud zákazníka přecházíte z existující nabídky Azure CSP, bude to mít následující dopad na fakturaci:

- Na vaší stávající faktuře ZA CSP se vám bude účtovat veškeré využití až do okamžiku ukončení původního předplatného Azure CSP.

- Pokud jste měli přístupová práva správce ke stávajícímu předplatnému CSP, budete mít přístup i po migraci tohoto předplatného.

Pokud chcete převést přímé smlouvy Enterprise na registrace CSP a serveru a cloudu na služby Azure, přečtěte si o získání vlastnictví fakturace [předplatných Azure pro Smlouva s partnerem Microsoftu](/azure/billing/mpa-request-ownership)

### <a name="audit-log"></a>Protokol auditu

Pokud chcete odsouhlasit fakturaci, zobrazte historii předplatných Microsoft Azure (0145P) na **stránce Předplatná.**

Předplatné Microsoft Azure (0145P) se skládá ze dvou částí:

1. Předplatné Commerce
2. Předplatné Azure (nárok)

Po dokončení přechodu se předplatné Azure přesune v rámci nového plánu Azure a komerční předplatné se pozastaví, aby se nehlásilo žádné další využití.  

>[!NOTE]
>Když Microsoft Azure předplatné (0145P) zakoupené v CSP, má předplatné pro komerční prostředí i předplatné Azure (nárok) stejnou hodnotu. Hodnoty se liší pouze v případě změn vlastnictví fakturace nebo převodů.

### <a name="transition-issues"></a>Problémy s přechodem

Během přechodů neočekáváme žádné problémy. Pokud k tomu dojde, budeme vás aktualizovat v samotném pracovním postupu přechodu. S využitím Azure se nic nesnídá.  

## <a name="next-steps"></a>Další kroky

- [Správa předplatných a prostředků v rámci plánu Azure](azure-plan-manage.md)

- [Kredit získaný partnerem – přehled](partner-earned-credit.md)
