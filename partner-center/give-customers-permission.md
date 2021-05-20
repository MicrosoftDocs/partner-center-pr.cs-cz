---
title: Nechte zákazníky, aby si kupili své vlastní služby v CSP.
description: Zjistěte, jak mohou partneři programu CSP nechat zákazníky nakupovat vlastní služby, jako jsou rezervace Azure, pro předplatné zakoupené pro ně v Partnerské centrum.
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9fabd6bd188c9d596128672d9fce3321db9b5432
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150756"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a>Udělit zákazníkům oprávnění Partnerské centrum k nákupu vlastních produktů nebo služeb

**Odpovídající role:** Agent pro správu | Agent prodeje

Tento článek ukazuje, jak může partner v Cloud Solution Provider (CSP) udělit zákazníkovi oprávnění k nákupu některých vlastních služeb nebo prostředků.

Partneři v programu CSP často používají Partnerské centrum a jeho komerční marketplace k nákupu řešení a služeb pro své zákazníky. Partneři pak umožňují některým zákazníkům tyto služby zřídit přímo z Azure Portal.

Tady je příklad. Řekněme, že si zakoupíte předplatné plánu Azure pro zákazníka v Partnerské centrum. Pak se rozhodnete přidat k předplatnému další prostředky nebo služby jménem zákazníka. V takovém případě můžete do předplatného zákazníka přidat rezervace Azure (například přidání rezervovaných instancí virtuálních počítačů). Pak můžete zákazníkovi umožnit, aby dále zř naspravovali prostředky rezervací Azure v Azure Portal.

Díky funkci **Oprávnění zákazníků** teď můžete zákazníkům poskytnout více samoobslužných možností s využitím prostředků Azure. Zapnutím oprávnění pro zákazníka umožníte zákazníkům koupit si vlastní prostředky (například nákup vlastních rezervací Azure).  

## <a name="overview-of-customer-permissions-in-partner-center"></a>Přehled oprávnění zákazníků v Partnerské centrum

Pokud chcete **zapnout** (nebo vypnout) oprávnění zákazníka, použijte stránku Zákaznický účet. V současné době tato funkce podporuje:

- **Rezervace Azure:** Zapnutí tohoto oprávnění umožní zákazníkovi zakoupit si vlastní rezervace Azure pro konkrétní předplatné Azure, které jste pro ně zakoupili.

Před zapnutím oprávnění zákazníka si všimněte těchto důležitých bodů:

- Ve výchozím nastavení jsou oprávnění zákazníka automaticky zakázána (vypnuta) v Partnerské centrum.

- Než budete moci zapnout (nebo vypnout) oprávnění pro zákazníka, musíte mít přiřazenou roli agenta správce v partnerském centru.

  Partneři, kteří mají přiřazenou roli obchodního agenta nebo agenta helpdesku, mají přístup jen pro čtení a nemůžou zapnout nebo vypnout oprávnění zákazníka.

- Můžete zapnout (Povolit) oprávnění pro libovolného zákazníka, kterého si zvolíte.

- Můžete zapnout (nebo vypnout) oprávnění pro zákazníky pomocí řídicího panelu nebo [rozhraní API partnerského](/partner-center/develop/manage-customers)centra.

- Až zapnete (povolíte) oprávnění pro konkrétního zákazníka, budete odpovědni za případné další nákupy provedené tímto zákazníkem. Pokud si zákazníci chtějí Exchange, zrušit nebo prodloužit nákup, které udělali (nebo chtějí změnit počáteční rozsah rezervace), nebudou moct dělat sami sebe. Musí vám požádat jako partnera, aby se mohli vyměňovat, zrušit a prodloužit nákupy nebo provádět pozdější změny v oboru rezervace.  

- Až zapnete oprávnění pro konkrétního zákazníka, **nebudete informováni** o jakýchkoli dalších nákupech provedených zákazníkem.

- Pozdější nákupy provedené zákazníkem se zobrazí v partnerském centru spolu s veškerými nákupy provedenými vámi. Tyto nákupy můžete najít na stránce **Historie objednávky** zákazníka, na stránce **rezervace** nebo v [**protokolu aktivit**](activity-logs.md).

>[!NOTE]
> Informace o cenách, které zákazník hradí, a o tom, jak zákazníkům pomáhat se správou jejich nákupů, najdete v tématu [pomáhat zákazníkům se správou rezervací, které kupuje](give-customers-permission.md#help-customers-manage-reservations-they-purchase).

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>Poskytněte zákazníkům oprávnění k nákupu svých rezervací Azure.

Rezervace Azure představují skvělý způsob, jak koupit služby Azure za zvýhodněnou sazbu. Další informace o výhodách rezervací Azure najdete v tématu [co jsou Azure reservations?](/azure/cost-management-billing/reservations/save-compute-costs-reservations)

Teď máte možnost koupit si za vaše zákazníky rezervace Azure, jak už jste to mohli udělat. Nebo můžete zákazníkům udělit oprávnění k nákupu svých rezervací Azure.

>[!NOTE]
> Jakmile zákazníkům dáte oprávnění k nákupu vlastních rezervací Azure, pomozte jim se spravovat rezervace, které zakoupí. Další informace najdete v tématu [Pomoc zákazníkům se spravování rezervací, které si kupují.](give-customers-permission.md#help-customers-manage-reservations-they-purchase)

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>Jak zákazníkům umožnit nákup vlastních rezervací Azure

1. Ověřte, že zákazník má stávající plán Azure nebo globální předplatné Azure, které jste zakoupili jeho jménem.

2. Ověřte, že má zákazník přiřazenou roli **Vlastník** pro toto předplatné.

3. Povolte oprávnění zákazníků (tuto **funkci** zapněte) a kupte si vlastní rezervace Azure.

Každý krok se zobrazí níže.

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>Ověření, že zákazník má stávající předplatné Azure

Než zákazníkům dáte oprávnění k nákupu vlastních rezervací Azure, musíte ověřit, že zákazník má stávající plán Azure nebo globální předplatné Azure. Pokud zákazník ve službě Azure Partnerské centrum, musíte pro ně koupit předplatné, než zapnete jeho oprávnění zákazníka.

- Pokud chcete zobrazit, jestli zákazník už má předplatné Azure, přihlaste se k řídicímu Partnerské centrum a pak vyberte **CSP** a pak **Zákazníci.** V seznamu vyberte konkrétního zákazníka. Pak vyberte **Předplatná** a vyhledejte předplatná založená na využití pro plán Azure nebo globální Azure.

- Pokud zákazník nemá stávající předplatné Azure, můžete si pro ně koupit předplatné. Viz [Zakoupení plánu Azure.](purchase-azure-plan.md)

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>Ověřte, že zákazníkovi byla v Azure přiřazena správná role.

Jakmile ověříte, že zákazník má stávající předplatné Azure, musíte také ověřit, jestli  mají klíč uživatelé přidružení k vašemu zákazníkovi přiřazenou správnou roli vlastníka pro toto předplatné Azure. Jedná se o přístup na základě role (RBAC), který zákazník potřebuje k nákupu rezervací Azure pro zakoupené předplatné Azure.

Někteří partneři už možná mají přiřazenou roli **Vlastník** zákazníkům, kteří chtějí aktivně spravovat a zřřovat své vlastní prostředky Azure. Pokud jste už ke správě předplatných, které jste si pro ně nakoupili, přiřadili stav **vlastníka** , můžete tento krok přeskočit.  

> [!IMPORTANT]
> Pokud se zákazníkovi nepřiřadila role **vlastníka** , dostanou v Azure Portal chybu, která jim brání v nákupu rezervací Azure.

Pokud chcete ověřit, že byl zákazníkovi přiřazená role **vlastníka** pro předplatné Azure:

1. Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.

2. Vyberte **CSP** a pak **zákazníky** a vyberte konkrétního zákazníka.

3. Vyberte **předplatná** pro daného zákazníka a vyhledejte konkrétní předplatné Azure.

4. Klikněte na tlačítko **Spravovat** vedle předplatného zákazníka. Tím se otevře [Azure Portal](https://portal.azure.com/).

5. Chcete-li přiřadit roli **vlastníka** konkrétnímu uživateli, postupujte podle těchto kroků [a přiřaďte uživatele jako správce](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator).

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>Zapnout nebo vypnout zákaznická oprávnění k nákupu vlastních rezervací Azure

Po ověření, že zákazník má stávající předplatné Azure a že se uživatelům přiřadí role **vlastníka** pro toto předplatné, jste připraveni zapnout (Povolit) oprávnění pro zákazníky. Pomocí těchto kroků můžete také vypnout (zakázat) oprávnění pro zákazníky. Můžete povolit nebo zakázat oprávnění zákazníka buď pomocí řídicího panelu nebo [rozhraní API partnerského](/partner-center/develop/manage-customers)centra.

Zapnutí (nebo vypnutí) oprávnění zákazníka v partnerském centru:

1. Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.

2. V levém navigačním panelu vyberte **CSP** a pak na **zákazníci**. Zobrazí se seznam zákazníků.

3. Vyberte konkrétní jméno zákazníka.

4. V nabídce zákazník vyberte **účet** . Zobrazí se stránka **účet** zákazníka.

5. V dolní **části stránky** vyhledejte oblast Oprávnění zákazníka.

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="Oprávnění zákazníka na stránce Účet." border="true":::

6. V **části Rezervace Azure** vyhledejte možnost Povolit **zákazníkovi nákup.**

7. Pokud chcete zapnout oprávnění zákazníka, přesuňte přepínač vedle této možnosti na **pozici On (Zap.).** Pokud chcete oprávnění zákazníka vypnout, přesuňte přepínač do **pozice Vypnuto.**

>[!NOTE]
> Další informace o tom, co se stane, když zapnete oprávnění zákazníka k nákupu vlastních rezervací Azure, najdete v tématu Přehled oprávnění zákazníků v [Partnerské centrum](give-customers-permission.md#overview-of-customer-permissions-in-partner-center).
>
>Když zapnete (nebo vypnete) oprávnění zákazníka, protokol aktivit zaznamená každou akci. (Tento protokol je přístupný, když vyberete ikonu ozubeného kola v horní části řídicího Partnerské centrum ozubeného kola). Když zapnete nebo vypnete oprávnění zákazníka, akce se v protokolu aktivit zobrazí jako Create **Customer Purchase Permissions** (Vytvořit oprávnění k nákupu zákazníka) nebo Delete Customer Purchase **Permissions** (Odstranit oprávnění k nákupu zákazníka).

## <a name="help-customers-manage-reservations-they-purchase"></a>Pomoc zákazníkům se spravují rezervace, které kupují

Jakmile zákazníkům dáte oprávnění k nákupu vlastních rezervací Azure, můžete jim pomoct lépe spravovat prostředky, které si kupují. Zákazníci mohou spravovat mnoho aspektů rezervací Azure přímo z [webu Azure Portal](https://portal.azure.com/). Bude potřebovat vaši pomoc se správou několika dalších aspektů rezervací Azure, které si koupí v rámci vašeho předplatného CSP.  

Pomozte zákazníkům lépe porozumět správě těchto aspektů rezervací Azure:

- Ceny, které zákazníci budou platit za rezervace Azure
- Jak mohou zákazníci optimalizovat využití rezervací Azure
- Co se stane, když zákazníci kupují rezervace se sdíleným rozsahem?
- Co se stane, když zákazníci chtějí změnit, zrušit a obnovit rezervaci nebo změnit její rozsah?

**Ceny, které zákazníci platí za své rezervace.** Zákazník bude kupovat rezervace Azure na základě předplatného, které jste pro ně dříve koupili ve fakturačním účtu partnera CSP. Cena zákazníka za všechny rezervace Azure, které zakoupí na základě tohoto předplatného, je nastavená také vámi. Tato cena se může lišit od webové přímé ceny, kterou zákazník uvidí v Azure Portal.

**Způsob, jakým zákazníci můžou optimalizovat použití rezervace.** Někteří zákazníci můžou využít více informací o tom, jak optimalizovat jejich používání rezervace nebo jak přiřadit počáteční rozsah rezervace během jejich nákupu. Pokud potřebujete další informace, požádejte zákazníky, aby si přečetli téma [Správa rezervací pro prostředky Azure](/azure/cost-management-billing/reservations/manage-reserved-vm-instance).

**Co se stane, když zákazník koupí rezervaci se sdíleným oborem?** Když si zákazníci nakupují rezervaci na základě předchozího předplatného CSP a přiřadíte k této rezervaci sdílený obor, budou všechny slevy, které zákazník udělil, použít na odpovídající použití u všech předplatných, které partner CSP zakoupil pro daného zákazníka.

**Co by měli zákazníci dělat, pokud chtějí vyměnit, zrušit nebo prodloužit nákup, které udělali, nebo změnit počáteční rozsah rezervace?** Zákazníci musí požádat svého partnera, aby jim pomohly změnit počáteční rozsah rezervace. K výměně, rušení nebo obnovení rezervace potřebují taky podporu partnera. Tyto úlohy nemohou provádět samy sebe s rezervace na základě předplatných, která jsou pro ně zakoupena partnerem CSP.

## <a name="next-steps"></a>Další kroky

- [Nákup rezervací Azure jménem vašich zákazníků](azure-reservations-buying.md)

- [Partnerské centrum – prodej rezervací Microsoftu](azure-reservations.md)

- [Správa rezervací Azure jménem vašich zákazníků](azure-reservations-manage.md)