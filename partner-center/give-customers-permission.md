---
title: Umožněte zákazníkům koupit si vlastní služby ve zprostředkovateli CSP.
description: Přečtěte si, jak partneři programu CSP můžou dovolit zákazníkům koupit vlastní služby, jako jsou rezervace Azure, pro předplatné zakoupené v partnerském centru.
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 19f86ec5353abc21e14a3a8ac2ef17dd17924cfe
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/22/2020
ms.locfileid: "92527364"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a>Poskytněte zákazníkům oprávnění v partnerském centru, aby si mohli koupit svoje vlastní produkty nebo služby.

**Platí pro**

- Partnerské centrum
- Partneři v programu CSP

**Příslušné role**

- Agent správce
- Agent prodeje

Tento článek ukazuje, jak může partner v programu Cloud Solution Provider (CSP) udělit zákazníkovi oprávnění k nákupu některých vlastních služeb nebo prostředků.

Partneři v programu CSP často používají Partnerské centrum a jeho komerční tržiště k nákupu řešení a služeb pro své zákazníky. Partneři pak zákazníkům umožní zřídit tyto služby přímo z Azure Portal.

Tady je příklad. Řekněme, že si koupíte předplatné plánu Azure pro zákazníka v partnerském centru. Pak se rozhodnete přidat další prostředky nebo služby k tomuto předplatnému jménem zákazníka. V takovém případě můžete přidat rezervace Azure do předplatného zákazníka (například přidat rezervované instance virtuálních počítačů). Potom můžete zákazníkům dovolit, aby se prostředky rezervace Azure v Azure Portal dále zřizovat sami.

Díky funkci **oprávnění zákazníka** zákazníkům poskytujete větší možnosti samoobslužných služeb s prostředky Azure. Když zapnete oprávnění pro zákazníka, umožníte zákazníkům koupit si vlastní prostředky (třeba koupit své vlastní rezervace Azure).  

## <a name="overview-of-customer-permissions-in-partner-center"></a>Přehled oprávnění zákazníka v partnerském centru

Na stránce **účet** zákazníka můžete zapnout (nebo vypnout) oprávnění pro zákazníky. V současné době tato funkce podporuje:

- **Rezervace Azure:** Zapnutím tohoto oprávnění umožníte zákazníkovi zakoupit si své vlastní rezervace Azure pro konkrétní předplatné Azure, které jste si zakoupili.

Než zapnete zákaznická oprávnění, vezměte v vědomí tyto důležité body:

- Ve výchozím nastavení jsou oprávnění zákazníka v partnerském centru automaticky zakázána (vypnuta).

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
> Když zákazníkům udělíte oprávnění k nákupu vlastních rezervací Azure, pomůžou jim spravovat všechny rezervace, které si nakupují. Další informace najdete v tématu [pomáhat zákazníkům se správou rezervací, které kupuje](give-customers-permission.md#help-customers-manage-reservations-they-purchase).

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>Umožnění zákazníkům koupit vlastní rezervace Azure

1. Ověřte, že zákazník má stávající plán Azure nebo globální předplatné Azure, které jste si zakoupili za vás.

2. Ověřte, že byl zákazníkovi přiřazená role **vlastníka** pro toto předplatné.

3. Povolit zákaznická oprávnění **(zapnout tuto funkci)** a koupit své vlastní rezervace Azure

Každý krok se zobrazí níže.

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>Ověřte, že zákazník má stávající předplatné Azure.

Předtím, než zákazníkům udělíte oprávnění k nákupu vlastních rezervací Azure, musíte ověřit, jestli má zákazník existující předplatné Azure nebo globální předplatné Azure. Pokud zákazník v partnerském centru nezobrazuje žádné aktuální předplatné Azure, musíte si pro ně koupit předplatné, než zapnete jeho oprávnění zákazníka.

- Pokud chcete zjistit, jestli už zákazník má předplatné Azure, přihlaste se k řídicímu panelu partnerského centra a pak vyberte **CSP** následovaný **zákazníky** . Vyberte ze seznamu konkrétního zákazníka. Pak vyberte **předplatná** a vyhledejte všechny odběry založené na používání pro plán Azure nebo globální Azure.

- Pokud zákazník nemá stávající předplatné Azure, můžete si pro ně koupit předplatné. Viz [Nákup plánu Azure](purchase-azure-plan.md).

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>Ověřte, že byl zákazníkovi přiřazená správná role v Azure.

Až ověříte, že zákazník má stávající předplatné Azure, musíte taky ověřit, jestli se klíčovým uživatelům přidruženým k vašemu zákazníkovi přiřadila správná role **vlastníka** pro toto předplatné Azure. Toto je přístup založený na rolích (RBAC), který zákazník potřebuje k nákupu rezervací Azure pro předplatné Azure, které jste zakoupili.

Někteří partneři už mohli mít přiřazenou roli **vlastníka** , aby mohli aktivně spravovat a zřizovat svoje vlastní prostředky Azure. Pokud jste už ke správě předplatných, které jste si pro ně nakoupili, přiřadili stav **vlastníka** , můžete tento krok přeskočit.  

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

2. V levém navigačním panelu vyberte **CSP** a pak na **zákazníci** . Zobrazí se seznam zákazníků.

3. Vyberte konkrétní jméno zákazníka.

4. V nabídce zákazník vyberte **účet** . Zobrazí se stránka **účet** zákazníka.

5. V dolní části stránky Najděte oblast **oprávnění zákazníka** .

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="Oprávnění zákazníka na stránce účtu." border="true":::

6. V části **rezervace Azure** Najděte možnost **Allow Customer koupit** .

7. Pokud chcete zapnout zákaznická oprávnění, přesuňte přepínač vedle této možnosti na místo **na** pozici. Pokud chcete vypnout oprávnění zákazníka, přesuňte přepínač na **volnou** pozici.

>[!NOTE]
> Další informace o tom, co se stane, když zapnete oprávnění zákazníka k nákupu vlastních rezervací Azure, najdete v tématu [Přehled oprávnění zákazníka v partnerském centru](give-customers-permission.md#overview-of-customer-permissions-in-partner-center).
>
>Když zapnete (nebo vypnete) oprávnění pro zákazníky, zaznamenává protokol aktivit každou akci. (Tento protokol je dostupný, když vyberete ikonu ozubeného kolečka v horní části řídicího panelu partnerského centra). Když zapnete nebo vypnete oprávnění zákazníka, akce se zobrazí jako buď **vytvořit nákupní oprávnění zákazníka** , nebo **odstranit oprávnění k nákupu zákazníka** v protokolu aktivit.

## <a name="help-customers-manage-reservations-they-purchase"></a>Pomáhat zákazníkům se správou rezervací, které kupují

Jakmile zákazníkům udělíte oprávnění k nákupu svých rezervací Azure, můžete jim usnadnit správu všech zakoupených prostředků. Zákazníci můžou spravovat mnoho aspektů rezervací Azure přímo z [Azure Portal](https://portal.azure.com/). Budou potřebovat vaši technickou správu, která vám nakupují několik dalších aspektů rezervací Azure, které si zakoupí v rámci vašeho předplatného CSP.  

Pomáhat zákazníkům pochopit Další informace o správě těchto aspektů rezervací Azure:

- Zákazníci ceny budou platit za rezervace Azure
- Jak můžou zákazníci optimalizovat použití rezervací Azure
- Co se stane, když si zákazníci nakupují rezervace se sdíleným oborem?
- Co se stane, když zákazníci chtějí změnit, zrušit a obnovit rezervaci nebo změnit její obor?

**Zákazníci ceny budou platit za své rezervace.** Vaše zákazníci si zakoupí rezervace Azure na základě předplatného, které jste pro ně dříve koupili ve fakturačním účtu partnera CSP. Cena zákazníka za všechny rezervace Azure, které zakoupí na základě tohoto předplatného, je nastavená také vámi. Tato cena se může lišit od webové přímé ceny, kterou zákazník uvidí v Azure Portal.

**Způsob, jakým zákazníci můžou optimalizovat použití rezervace.** Někteří zákazníci můžou využít více informací o tom, jak optimalizovat jejich používání rezervace nebo jak přiřadit počáteční rozsah rezervace během jejich nákupu. Pokud potřebujete další informace, požádejte zákazníky, aby si přečetli téma [Správa rezervací pro prostředky Azure](/azure/cost-management-billing/reservations/manage-reserved-vm-instance).

**Co se stane, když zákazník koupí rezervaci se sdíleným oborem?** Když si zákazníci nakupují rezervaci na základě předchozího předplatného CSP a přiřadíte k této rezervaci sdílený obor, budou všechny slevy, které zákazník udělil, použít na odpovídající použití u všech předplatných, které partner CSP zakoupil pro daného zákazníka.

**Co by měli zákazníci dělat, pokud chtějí vyměnit, zrušit nebo prodloužit nákup, které udělali, nebo změnit počáteční rozsah rezervace?** Zákazníci musí požádat svého partnera, aby jim pomohly změnit počáteční rozsah rezervace. K výměně, rušení nebo obnovení rezervace potřebují taky podporu partnera. Tyto úlohy nemohou provádět samy sebe s rezervace na základě předplatných, která jsou pro ně zakoupena partnerem CSP.

## <a name="next-steps"></a>Další kroky

- [Nákup rezervací Azure jménem vašich zákazníků](azure-reservations-buying.md)

- [Partnerské centrum – prodej rezervací Microsoftu](azure-reservations.md)

- [Správa rezervací Azure jménem vašich zákazníků](azure-reservations-manage.md)