---
title: Zakoupení nabídky SaaS v Azure Portal
description: Zjistěte, jak najít a zakoupit nabídku SaaS v Azure Portal.
author: mingshen-ms
ms.author: mingshen
ms.reviewer: dannyevers
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: how-to
ms.date: 06/04/2021
ms.openlocfilehash: b73a9acb7b9cf9eee1151de1f8e45f6fd6ef256f
ms.sourcegitcommit: 8511fec63961d8c77a4d1eea3e3f1d37cdea46c6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/19/2021
ms.locfileid: "112373490"
---
# <a name="purchase-a-saas-offer-in-azure-portal"></a>Nákup nabídky SaaS v Azure Portal

Tento článek vysvětluje různé možnosti a požadavky pro vyhledávání, pokusy a nákup nabídky saaS (software jako služba) od Azure Portal.

## <a name="saas-offers-discovery-in-azure-portal"></a>SaaS nabízí zjišťování v Azure Portal

Jakmile budete v Azure Portal, existuje několik způsobů, jak hledání zúžit tak, aby se soustředil na nabídky SaaS.

### <a name="narrowing-your-search"></a>Zúžení hledání

Na domovské stránce v části **Služby Azure** vyberte + **Vytvořit prostředek** nebo **Marketplace**. Nebo použijte klávesovou **zkratku G + N** kdekoli na platformě.

- Zužte výsledky na nabídky SaaS pomocí **filtru Typ nabídky** a pak vyberte **SaaS.**
- Pomocí globální vyhledávání v horní navigační oblasti vyhledejte konkrétní nabídku SaaS.

Najděte [privátní nabídku SaaS](/marketplace/private-offers) výběrem banneru v horní části domovské **stránky Marketplace.** Ne všechny nabídky nebo plány jsou k dispozici ve všech geografických lokalitách a některé se můžou zobrazit pouze pro určité tenanty.

Filtrované zobrazení zobrazuje každou dostupnou nabídku SaaS reprezentované názvem. Výběrem jedné zobrazíte stránku s podrobnostmi o produktu. To zahrnuje následující části:

- Přehled – podrobnosti o službě, marketingu a výukových materiálech
- Plány a ceny – každá nabídka bude obsahovat alespoň jeden plán s různými fakturačními podmínkami a cenami.
- Informace o využití a podpora – zahrnuje ID vydavatele, ID nabídky a ID plánu.
- Hodnocení a recenze konkrétní nabídky SaaS

## <a name="available-billing-models-plansskus-for-saas-offers"></a>Dostupné fakturační modely (plány/SKU) pro nabídky SaaS

Každá nabídka SaaS bude mít jeden nebo více plánů. Ke každé nabídce je přidružený cenový model: ploché sazby nebo cena za uživatele. Každá cena plánu se účtuje opakovaně, což může být nula dolarů (všechny uvedené ceny jsou jenom pro účely příkladu a nemají odrážet skutečné náklady). Tento poplatek je buď plochý, nebo cena za uživatele. Dostupné typy plánů:

- **Měsíční plány** – pravidelné měsíční poplatky; plochý měsíční poplatek nebo měsíční poplatek za uživatele, který se platí v měsíčním opakování. Po ukončení období se plán automaticky obnoví.
- **Roční plány** – opakovaný roční poplatek; plochý roční poplatek nebo roční poplatek za uživatele, který se platí ročním opakováním. Po ukončení období se plán automaticky obnoví.
- **Vlastní měřiče** – společně s opakovanými poplatky může plán s plochými sazbami také zahrnovat volitelné vlastní měřené dimenze pro nadplatná využití, která nejsou zahrnutá v ploché sazbě. Každá dimenze představuje fakturovatelné jednotky. Jedná se o proměnlivé náklady, které se mění v závislosti na využití měřené jednotky, jako je šířka pásma, lístky nebo zpracování e-mailu. Budou se vám účtovat poplatky podle spotřeby těchto dimenzí v měsíčních intervalech. Upozorňujeme, že spotřeba nad využití začíná jenom v případě, že jste použili všechny měřené jednotky zahrnuté v ploché sazbě.
- **Bezplatná** zkušební verze – v některých případech zahrnuje plán zkušební období jednoho měsíce, během kterého můžete software používat zdarma.  Po uplynutí zkušební doby se vám budou účtovat poplatky podle vašeho plánu. Zkušební nabídky nejsou kompatibilní s vlastními měřiči.

Tyto cenové modely jsou k dispozici pro veřejné i privátní plány.

## <a name="saas-purchase-experience"></a>Prostředí pro nákup SaaS

1. Na stránce produktu vyberte plán, který vyhovuje vašim potřebám, a pokračujte v **nastavení a odběru.**
2. V rámci procesu nákupu budete přesměrováni na kartu **Základy** a budete muset:
    1. *Definujte předplatné,* které chcete použít pro fakturaci. Předplatné Azure, které používáte, by mělo mít definovanou platnou metodu nákupu. V tomto předplatném byste měli mít správnou úroveň oprávnění nebo skupinu prostředků se správnou úrovní oprávnění. Země fakturace by také měla být zemí, kde je nabídka k dispozici k nákupu. Předplatná Azure bez platného způsobu platby (například předplatné MSDN) je možné použít pouze k nákupu bezplatných plánů.
    1. Zvolte nebo vytvořte **skupinu prostředků, do* které bude prostředek SaaS patřit.
    1. Zadejte Název *předplatného* SaaS, abyste ho později mohli snadno identifikovat. Po zakoupení nemůžete název změnit.
    1. V **části** Plán uvidíte plán, který jste vybrali, na stránce s podrobnou informací o produktu .PDP. Pokud jste v primárním záhonovém projektu ještě neudělali aktivní výběr, zobrazí se výchozí plán. Výběr můžete změnit výběrem odkazu **Změnit** plán. Vyberte příslušné fakturační období a pak zvolte jiný plán. Pokud to vydavatel podporuje, může být možné plán po nákupu změnit. Nebudete ale moct změnit období z měsíčního na roční nebo z ročního na měsíční.
    1. V případech, kdy je *cenový* model pro uživatele , může být nutné zadat počet *uživatelů*. Cena, kterou uvidíte, se změní v závislosti na předplatném, plánu a období, které jste vybrali.
3. Přejděte na **kartu Značky** – *Značky* jsou uživatelsky definované páry klíč-hodnota, které je možné umístit přímo na prostředek nebo skupinu prostředků. Později můžete pomocí značek snadno najít prostředek SaaS. Azure v současné době podporuje až 50 značek na prostředek a skupinu prostředků. Značky mohou být umístěny na prostředek v době vytváření nebo přidány do existujícího prostředku.
4. Pokračujte na **Zkontrolovat a přihlásit se k** odběru a prohlédněte si podrobnosti o nabídce a plánu.
    1. Zkontrolujte *Podmínky použití,* *dodatky* a zásady ochrany *osobních* údajů vydavatele a také Azure Marketplace
    1. Můžete být vyzváni k přidání kontaktních údajů.
    1. Kontrola *podrobností o základech* *a značkách*
5. Po potvrzení vyberte Přihlásit **k odběru.**

## <a name="saas-subscription-and-configuration"></a>Předplatné SaaS a konfigurace

Když vyberete přihlásit k odběru, zobrazí se zpráva "Vaše předplatné SaaS probíhá". Tento proces by měl trvat několik minut a nezabýt se oknem, dokud se nedokončí.

Po dokončení předplatného se zobrazí zpráva, že je vaše předplatné SaaS dokončené, a měli byste účet nakonfigurovat tak, aby se začal váš nákup využívat. Obdržíte také e-mail s žádostí o aktivaci nového předplatného. Pokud nejste ten, kdo nakonfiguruje účet SaaS, předáte tento e-mail příslušné osobě.

Abyste tento proces dokončili a začali používat SaaS, musíte začít konfigurovat své předplatné. Výběrem **tlačítka Konfigurovat účet** se přesměrujete na web vydavatele.

Stav předplatného můžete zkontrolovat také výběrem ikony zvonku v pravém horním rohu záhlaví.

Pokud proces konfigurace do *30* dnů dokončíte, toto předplatné SaaS se automaticky *odstraní.* Fakturace se spustí po nakonfigurování vašeho účtu na webu vydavatele.

Chybové zprávy, se které se můžou během tohoto procesu zobrazit:

- Název plánu *vybraného plánu není možné* zakoupit v bezplatném předplatném.
  - Další podrobnosti najdete v tématu https://aka.ms/UpgradeFreeSub Upgrade účtu.

- Nákup selhal, protože jsme nenašli platnou platební kartu ani způsob platby přidružený k vašemu předplatnému Azure.
  - Použijte jiné předplatné Azure nebo pro toto předplatné přidejte nebo aktualizujte aktuální platební kartu nebo způsob platby a zkuste to znovu.

- Název *plánu vybraného z* názvu nabídky  podle vydavatele nabídky není k dispozici k nákupu podle pravidel nastavených správcem IT. 
  - Obraťte se na správce IT.

- Název *plánu vybraného*  z plánu  nabídky vybraného vydavatelem nabídky není k dispozici k nákupu z důvodu nastavení privátního marketplace provedeného správcem IT vašeho tenanta.
  - Obraťte se na správce IT.

- Nákup selhal, protože požadovaný fakturační období je prázdné nebo neplatné.
  - Zkuste si koupit jiný plán nebo fakturační období.

- Nákup selhal, protože jsme nemohli ověřit vaše podepisování právní smlouvy.
  - Opakovat. Pokud chyba přetrvává, zkuste nákup provést pomocí jiného předplatného Azure nebo se obraťte na podporu.

- Nákup offer *offerID* podle id *vydavatele* selhal. Tato nabídka momentálně není k dispozici pro nákup.
  - Zkuste to později. Pokud se vám po hodině stále zobrazí tato chybová zpráva, kontaktujte podporu.  

- Nákup *planID nabídky* *offerID* podle id *vydavatele* selhal. Tento plán momentálně není k dispozici pro nákup.
  - Zkuste to později. Pokud se vám po hodině stále zobrazí tato chybová zpráva, kontaktujte podporu. 

- *E-mailová adresa klienta* s ID objektu *ObjectID* nemá oprávnění k provedení akce *DeploymentValidationAction* v oboru *ResourceGroup. DeploymentScope* nebo obor je neplatný.  
  - Tato zpráva se zobrazí, pokud nemáte příslušná oprávnění k předplatnému nebo skupině prostředků Azure.  
    Pokud byl přístup udělen nedávno, aktualizujte své přihlašovací údaje.  
    Pokud chcete nasadit prostředky do skupiny prostředků, musíte mít alespoň přístup přispěvatele. Zkontrolujte stav přístupu v **části Skupiny prostředků** a pak **Access Control**. To ukazuje, kdo je vlastník, kterého můžete požádat, abyste byli přiřazeni jako Přispěvatel.

- Předplatné použité pro tento nákup neumožňuje nákupy na Marketplace.  
  - Použijte jiné předplatné nebo požádejte správce, aby změnil definici tohoto předplatného a zkuste to znovu.

## <a name="next-steps"></a>Další kroky

- Pokud nabídku prodáváte prostřednictvím Microsoftu, přejděte na článek Přidání cílové skupiny pro verzi [Preview pro vaši nabídku SaaS.](/azure/marketplace/create-new-saas-offer-preview)
- Jinak přejděte na [stránku Jak prodávat nabídku SaaS.](/azure/marketplace/create-new-saas-offer-marketing)
