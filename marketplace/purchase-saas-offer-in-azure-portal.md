---
title: Jak zakoupit nabídku SaaS v Azure Portal
description: Naučte se najít a koupit nabídku SaaS v Azure Portal.
author: mingshen-ms
ms.author: mingshen
ms.reviewer: dannyevers
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: how-to
ms.date: 06/04/2021
ms.openlocfilehash: 8dba9f95607a4172e6d5d0bc2ec148a25b599cd1
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431454"
---
# <a name="purchase-a-saas-offer-in-azure-portal"></a>Nákup nabídky SaaS v Azure Portal

Tento článek popisuje různé možnosti a požadavky pro hledání, zkoušení a nákup nabídky SaaS (software jako služba) z Azure Portal.

## <a name="saas-offers-discovery-in-azure-portal"></a>SaaS nabízí zjišťování v Azure Portal

Až budete v Azure Portal, existuje několik způsobů, jak zúžit hledání na SaaS nabídek.

### <a name="narrowing-your-search"></a>Zúžení hledání

Na domovské stránce vyberte v části **služby Azure** možnost **+ vytvořit prostředek** nebo **tržiště**. Nebo použijte klávesovou zkratku **G + N** kdekoli na platformě.

- Zužte výsledky do SaaS nabídek pomocí filtru **typu nabídky** a pak vyberte **SaaS**.
- K vyhledání konkrétní nabídky SaaS použijte globální panel hledání v horní navigační oblasti.

Vyberte si banner v horní části domovské stránky **webu Marketplace** a najděte [soukromou SaaS nabídku](/marketplace/private-offers) . Ne všechny nabídky nebo plány jsou k dispozici ve všech geografických oblastech a některé mohou být zobrazeny pouze pro určité klienty.

Filtrované zobrazení zobrazuje všechny dostupné nabídky SaaS reprezentované názvem. Vyberte jednu pro zobrazení stránky s podrobnostmi o produktu. Který zahrnuje následující části:

- Přehled – Podrobnosti o službě, marketingových a studijních materiálech
- Plány a ceny – Každá nabídka bude zahrnovat aspoň jeden plán s různými fakturačními podmínkami a cenami.
- Informace o využití a podpora – zahrnuje ID vydavatele, ID nabídky a ID plánu.
- Hodnocení a přezkoumání konkrétní nabídky SaaS

## <a name="available-billing-models-plansskus-for-saas-offers"></a>Dostupné modely fakturace (plány/SKU) pro nabídky SaaS

Každá nabídka SaaS bude mít jeden nebo více plánů. K každé nabídce je přiřazený cenový model: paušální sazba nebo na uživatele. Každá cena plánu je opakovaný poplatek, který může být nulových dolarů (všechny uvedené ceny jsou například pouze pro účely a nejsou určené k tomu, aby odrážely skutečné náklady). Tento poplatek je buď paušální sazba, nebo cena na uživatele. Dostupné typy plánů:

- **Měsíční plány** – opakovaný měsíční poplatek; měsíční poplatek za paušální nebo na uživatele, který se hradí při měsíčním opakování. Po ukončení platnosti se plán automaticky obnoví.
- **Roční plány** – periodický roční poplatek; roční poplatek za paušální nebo na uživatele, který je vyplácen při ročním opakování. Po ukončení platnosti se plán automaticky obnoví.
- **Vlastní** měřiče – spolu s opakovanými poplatky, plán paušálních sazeb může také zahrnovat volitelné vlastní měřené dimenze pro překročení využití, které není zahrnuté do paušální sazby. Každá dimenze představuje Fakturovatelné jednotky. Jedná se o proměnlivou cenu, která se mění podle využití měřených jednotek, například: šířky pásma, lístků nebo zpracovaných e-mailů. Za měsíc se vám bude účtovat podle vaší spotřeby těchto dimenzí. Poznámka: spotřeba za nadlimitní využití začíná jenom v případě, že jste použili všechny měřené jednotky zahrnuté do paušální sazby.
- **Bezplatná zkušební verze** – v některých případech plán zahrnuje zkušební období jednoho měsíce, během kterého můžete software používat zdarma.  Po skončení zkušebního období se vám bude účtovat podle vašeho plánu. Nabídky zkušební verze nejsou kompatibilní s vlastními měřiči.

Tyto cenové modely jsou k dispozici pro veřejné i privátní plány.

## <a name="saas-purchase-experience"></a>Možnosti nákupu SaaS

1. Na stránce produkt vyberte plán, který vyhovuje vašim potřebám, a pokračujte **nastavením + přihlášení k odběru** .
2. V rámci procesu nákupu budete přesměrováni na kartu **základy** a budete muset:
    1. Definujte, které *předplatné* byste chtěli použít k fakturaci. U předplatného Azure, které použijete, by měla být pro ni definovaná platná metoda nákupu. Měli byste mít správnou úroveň oprávnění nebo skupinu prostředků v rámci tohoto předplatného se správnou úrovní oprávnění. Také země fakturace by měla být země, kde je nabídka dostupná k nákupu. Předplatná Azure bez platného způsobu platby (například předplatné MSDN) se dají použít jenom k nákupu bezplatných plánů.
    1. Vyberte nebo vytvořte *skupinu prostředků* *, do které bude prostředek SaaS patřit.
    1. Zadejte *název* předplatného SaaS, abyste ho snadno identifikovali později. Po zakoupení nemůžete název změnit.
    1. V části **plán** se zobrazí plán, který jste vybrali na stránce s podrobnostmi o produktu (PDP). Pokud jste v PDP nevytvořili aktivní výběr, zobrazí se výchozí plán. Výběr můžete změnit výběrem odkazu **změnit plán** . Vyberte odpovídající fakturační období a pak zvolte jiný plán. Plán může být po nákupu možné změnit, pokud ho Vydavatel podporuje. Nebudete ale moct změnit období z měsíčního na roční nebo z roční na měsíčně.
    1. V případech, kdy je cenový model *na uživatele*, možná budete muset zadat počet *uživatelů*. Cena, kterou vidíte, se změní na základě předplatného, plánu a termínu, který jste vybrali.
3. Přejděte na **značky** karet – *značky* jsou uživatelsky definované páry klíč/hodnota, které se dají umístit přímo do prostředku nebo skupiny prostředků. Pomocí značek můžete později snadno najít prostředek SaaS. Azure v současné době podporuje až 50 značek na jeden prostředek a skupinu prostředků. Značky lze umístit na prostředek v době vytvoření nebo přidání do existujícího prostředku.
4. Pokračujte v **kontrole a přihlášení k odběru** a Projděte si podrobnosti o nabídce a plánu.
    1. Kontrola *podmínky použití*, *změn* a *zásad ochrany osobních údajů* vydavatele a také pro Azure Marketplace
    1. Může se zobrazit výzva, abyste přidali svoje kontaktní údaje.
    1. Projděte si podrobnosti o *základech* a *značkách*
5. Po potvrzení vyberte **Přihlásit se k odběru**.

## <a name="saas-subscription-and-configuration"></a>Předplatné a konfigurace SaaS

Když vyberete přihlásit se k odběru, zobrazí se zpráva "vaše předplatné SaaS probíhá". Tento proces může trvat několik minut, nezavírejte okno, dokud se nedokončí.

Po dokončení předplatného se zobrazí zpráva, že předplatné SaaS je dokončené, a Vy byste ho měli nakonfigurovat tak, aby se při nákupu mohli začít užívat. Obdržíte také e-mail požadující aktivaci nového předplatného. Pokud nejste ten, který bude konfigurovat účet SaaS, předejte tento e-mail příslušné osobě.

Abyste mohli dokončit proces a začít používat SaaS, budete muset začít konfigurovat předplatné. Kliknutím na tlačítko **konfigurovat účet nyní** budete přesměrováni na web vydavatele.

Stav předplatného můžete také ověřit tak, že vyberete ikonu zvonku v pravém horním rohu záhlaví.

Pokud proces konfigurace nedokončíte do *30 dnů*, toto předplatné SaaS se automaticky *odstraní*. Fakturace se spustí po konfiguraci vašeho účtu na webu vydavatele.

Chybové zprávy, se kterými se můžete setkat v průběhu procesu:

- Název plánu *vybraného plánu* nejde koupit na bezplatné předplatné.
  - Upgradujte svůj účet https://aka.ms/UpgradeFreeSub . Další podrobnosti najdete v tématu.

- Nákup se nezdařil, protože se nám nepovedlo najít platnou platební kartu ani způsob platby, který je přidružený k vašemu předplatnému Azure.
  - Použijte pro toto předplatné jiné předplatné Azure nebo add\update aktuální platební kartu nebo způsob platby a zkuste to znovu.

- *Název plánu zvoleného plánu* nabídky *název* nabídky Vydavatel nabídky není k  dispozici pro nákup podle pravidel nastavených správcem IT.
  - Obraťte se na správce IT.

- *Název plánu vybraného* plánu nabídky *vybraný* *vydavatelem nabídky není k* dispozici pro nákup z důvodu nastavení privátního tržiště, které provádí správce IT vašeho tenanta.
  - Obraťte se na správce IT.

- Nákup se nezdařil, protože požadovaný fakturační termín je prázdný nebo neplatný.
  - Zkuste si koupit jiný plán nebo fakturační období.

- Nákup se nezdařil, protože se nám nepovedlo ověřit vaše přihlášení k právní smlouvě.
  - Opakujte. Pokud s tím budou dál problémy, zkuste si koupit v rámci jiného předplatného Azure nebo kontaktujte podporu.

- Nákup nabídky *hodnotami OfferId* vydavatelem *PublisherId* se nezdařil. Tato nabídka není momentálně k dispozici k nákupu.
  - Zkuste to později. Pokud se tato chybová zpráva zobrazuje po hodinové zprávě, obraťte se prosím na podporu.  

- Nákup plánu *planID* nabídky *hodnotami OfferId* od vydavatele *PublisherId* se nezdařil. Tento plán není v současné době k dispozici k nákupu.
  - Zkuste to později. Pokud se tato chybová zpráva zobrazuje po hodinové zprávě, obraťte se prosím na podporu. 

- *E-mailová adresa* klienta s ID objektu *objectID* nemá autorizaci k provedení akce *DeploymentValidationAction* , která se nachází v oboru *zdrojů. DeploymentScope* nebo obor je neplatný.  
  - Tato zpráva se zobrazí, pokud nemáte příslušná oprávnění k předplatnému nebo skupině prostředků Azure.  
    Pokud byl přístup udělen nedávno, aktualizujte své přihlašovací údaje.  
    Pokud chcete nasadit prostředky do skupiny prostředků, musíte mít alespoň přístup přispěvatele. Zkontrolujte stav přístupu v **části Skupiny prostředků** a pak **Access Control**. To ukazuje, kdo je vlastník, kterého můžete požádat, abyste byli přiřazeni jako Přispěvatel.

- Předplatné použité pro tento nákup neumožňuje nákupy na Marketplace.  
  - Použijte jiné předplatné nebo požádejte správce, aby změnil definici tohoto předplatného a zkuste to znovu.

## <a name="next-steps"></a>Další kroky

- Pokud jste už na marketplace zakoupili nabídku, přejděte do části Fakturace a [fakturace.](/marketplace/billing-invoicing)
- Můžete si také zobrazit další informace o [možnostech privátních](/marketplace/private-offers) plánů.
