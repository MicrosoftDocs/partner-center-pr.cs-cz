---
title: Přesun zákazníků z aktuálních nabídek Azure do plánu Azure
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si, jak partneři CSP můžou pomocí partnerského centra přesunout zákazníky ze stávajících nabídek CSP Azure do služeb Azure v rámci plánu Azure.
author: mowree
ms.author: mowrim
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/16/2020
ms.openlocfilehash: 4e22386dc8bddd9662a0d80020a5c90c464e9d39
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534807"
---
# <a name="transition-customers-to-azure-plan-from-existing-csp-azure-offers"></a>Přechod zákazníků do plánu Azure ze stávajících nabídek Azure CSP

**Příslušné role**

- Agent správce
- Správce fakturace
- Globální správce
- Agent helpdesku
- Agent prodeje
- Správce správy uživatelů

V tomto článku se dozvíte, jak můžou partneři CSP používat Partnerské centrum k přesunu zákazníků ze stávajících nabídek CSP Azure do služeb Azure v rámci plánu Azure. Nepřímá poskytovatelé a Přímí partneři s přímým přístupem můžou přejít na nové prostředí pro obchod, které je dostupné v programu poskytovatele Microsoft Cloudch služeb (CSP) pro Azure. (Nepřímí prodejci budou muset pracovat prostřednictvím jejich nepřímých zprostředkovatelů.) Zákazníci budou mít k dispozici zjednodušený způsob nákupu cloudových služeb, ať už se jedná o nákupy od partnerů, od prodejců Microsoftu nebo přímo na webu.

Možnost přechodu je určena jenom pro zákazníky, kteří přecházejí na nové prostředí pro obchod s Azure a kteří podepsali smlouvu o zákaznících Microsoftu. Nejedná se o jiné nabídky ve zprostředkovateli CSP, jako je například Office 365 nebo Dynamics 365.

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>Převod stávajících nabídek CSP na plán Azure

Zákazníky ze svých stávajících poskytovatelů CSP Azure můžete převést na služby Azure v rámci plánu Azure v rámci nového prostředí pro obchod v programu CSP z partnerského centra. Aby to bylo možné, musí mít partner a zákazník zavedeného vztahu prodejce prostřednictvím partnerského centra a zákazník musí mít podepsané smlouvy o zákaznících Microsoftu.

### <a name="select-transition-to-azure-plan"></a>Vybrat přechod do plánu Azure

1. Vyberte plán Azure pro zákazníka.

2. Vyberte **Převod fakturace do plánu Azure**.

   :::image type="content" source="images/azure/transition1.png" alt-text="Snímek obrazovky s informacemi o předplatných založených na využití s možností s možností volby s názvem: přechod předplatného Azure do plánu Azure":::

3. Vyberte **Pokračovat**.

   :::image type="content" source="images/azure/transition2.png" alt-text="Dialogové okno s názvem přechod do plánu Azure s důsledky pro přečtení o přechodu a dvou možnostech pro výběr, pokračování nebo zrušení.":::

   Váš zákazník se převede na plán Azure.

   **Pracovní postup přechodu automatizuje požadavky na tyto kroky**:

   - Nákup plánů Azure
   - Jeden plán na zákazníka ve scénářích přímého CSP  
   - Jeden plán na prodejce  

   Například partneři koupili dvě Microsoft Azure nabídky a zahrnuli do nákupu dvě jedinečné POR. V takovém případě bude pracovní postup přechodu nakoupit dva plány Azure (jeden na prodejce) a automaticky namapovat příslušné předplatné Azure v rámci plánů Azure.  

   **Mapování předplatného Azure na plán Azure**

   Po zakoupení plánů Azure provede náš systém mapování stávajících předplatných Azure na plány Azure. Průběh můžete zobrazit v Azure Portal i v partnerském centru.

4. Vraťte se na stránku **předplatná** partnerského centra zákazníka a aktualizujte svůj limit rozpočtu pomocí místní měny.

   :::image type="content" source="images/azure/transition3.png" alt-text="Částečné zobrazení stránky předplatná partnerského centra s limity rozpočtu nastavenými v místní měně pro fakturační období":::

   >[!NOTE]
   >Rozpočet, který jste nastavili v partnerském centru, se nepřenese do Azure Portal. Měli byste také nastavit rozpočet a výstrahu v Azure Portal.

   Když přejdete na plán Azure, nebudete už moct koupit předplatné Azure pro tohoto zákazníka. Předplatná můžete vytvořit v rámci plánu Azure v Azure Portal.

   >[!NOTE]
   > Všechna předplatná Azure zakoupená prostřednictvím služby RBAC v rámci plánu Azure se účtují a účtují v místní měně. Sazby za FX nebudou použity.

### <a name="track-your-transition-details"></a>Sledovat podrobnosti přechodu

Sledujte průběh přechodu v Azure Portal i v partnerském centru.

:::image type="content" source="images/azure/details1.png" alt-text="Snímek obrazovky s tabulkou se seznamem podrobností o přechodu na předplatné – zahrnuje předplatné I D, datum přechodu a stav přechodu.":::

### <a name="billing-impact-to-partners"></a>Dopad fakturace na partnery

Pokud převedete zákazníka ze stávající nabídky Azure CSP, budete mít následující dopady na fakturaci:

- Bude se vám účtovat stávající faktura CSP pro veškeré využití až do chvíle, kdy se původní předplatné služby CSP Azure ukončí.

- Pokud máte přístupová práva správce k existujícímu předplatnému CSP, budete mít k dispozici přístup i v případě, že je předplatné migrováno.

Pro přechod přímých smluv Enterprise na cloudové a cloudové registrace do služeb Azure si přečtěte téma [získání vlastnictví fakturace předplatných Azure pro partnery Microsoftu](/azure/billing/mpa-request-ownership) .

### <a name="audit-log"></a>Protokol auditu

Pokud chcete sjednotit fakturaci, zobrazte si historii předplatných "Microsoft Azure" (0145P) na stránce **předplatná** .

Předplatné "Microsoft Azure" (0145P) se skládá ze dvou částí:

1. Předplatné Commerce
2. Předplatné Azure (nárok)

Po dokončení přechodu se předplatné Azure přesune v části nový plán Azure a předplatné Commerce se pozastaví, aby se neoznámilo žádné další použití.  

>[!NOTE]
>Po zakoupení předplatného Microsoft Azure (0145P) ve zprostředkovateli CSP mají stejné hodnoty jak předplatné obchodu, tak i předplatné Azure (nárok). Pouze v případě změny vlastnictví fakturace nebo převodů se hodnoty liší.

### <a name="transition-issues"></a>Problémy s přechodem

Během přechodů nepředpokládáme žádné problémy. Pokud k tomu dojde, budeme v pracovním postupu přechodu aktualizovat sám sebe. Nehrozí žádné narušení využití Azure.  

## <a name="next-steps"></a>Další kroky

- [Správa předplatných a prostředků v rámci plánu Azure](azure-plan-manage.md)

- [Získaný kredit partnerů – přehled](partner-earned-credit.md)