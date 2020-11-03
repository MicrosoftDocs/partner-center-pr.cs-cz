---
title: Nastavení rozpočtu Azure útraty pro zákazníky
ms.topic: how-to
ms.date: 06/03/2020
description: Naučte se, jak nastavit nebo odebrat měsíční rozpočty Azure útraty pro vaše zákazníky, a také zobrazit data o výdajích Azure a nastavit oznámení týkající se rozpočtu.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 982d4ed310415349acde3d260afce04eb0d55ac5
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2020
ms.locfileid: "92527134"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>Nastavení, kontrolu nebo odebrání měsíčních rozpočtů Azure útraty pro zákazníky v partnerském centru

Platí pro:

- Partnerské centrum
- Partnerské centrum pro Microsoft Cloud pro státní správu USA

Můžete [nastavit měsíční rozpočet Azure útraty pro vaše zákazníky](#set-azure-spending-budget) v partnerském centru. To pomáhá vašim zákazníkům spravovat útraty Azure. Tato možnost umožňuje porovnat náklady na Azure, které jsou v daném měsíci v rozpočtu. Pomáhá zákazníkům také rozpočtovat své výdaje na Azure, takže jejich měsíční vyúčtování není vyšší než jejich předvídání.

> [!NOTE]  
> Tato funkce není k dispozici v izolovaném prostoru nebo v produkčním účtu (TIP).

Po [nastavení rozpočtu útraty Azure pro zákazníky](#set-azure-spending-budget)můžete také zkontrolovat používání zákazníka následujícími způsoby. Tyto možnosti vám mohou nabídnout možnost vyznačovat nesprávně nakonfigurované služby nebo neobvyklé trendy, které mohou navrhovat podvod. Potom můžete s vašimi zákazníky spolupracovat a identifikovat hlavní příčinu a spravovat náklady. V případě potřeby můžete také [změnit rozpočet zákazníka](#set-azure-spending-budget) na vyšší částku.

- [Kontrolovat aktuální útratu Azure](#check-current-azure-spending)

- [Zapnout e-mailová oznámení v případě, že se útrata zákazníka blíží ke svému limitu rozpočtu](#notifications-for-budget-limits)

- [Zobrazit nákladové náklady podle služby pro odběry založené na využití](#itemized-costs-by-service)

[Rozpočet Azure útraty](#remove-azure-spending-budget) můžete také kdykoli odebrat pro zákazníky.

## <a name="azure-spending-data"></a>Data o výdajích Azure

Data o výdajích Azure jsou *odhadem* a *skutečné fakturační částky se můžou lišit* . Hodnota dat *nezohledňuje* daně, kredity, úpravy nebo jiné poplatky, které mohou platit.

Data o výdajích se *aktualizují jednou denně* . Vaši zákazníci můžou dál používat (a budou se vám účtovat) služby a prostředky Azure, pokud nezměníte nastavení svého účtu v Azure Portal.

## <a name="set-azure-spending-budget"></a>Nastavení rozpočtu útraty Azure

Můžete *nastavit měsíční rozpočet Azure útraty* pro více zákazníků v partnerském centru:

1. Přihlaste se k [řídicímu panelu partnerského centra](https://partner.microsoft.com/dashboard/).

2. V nabídce vlevo v části **CSP** vyberte **útraty Azure** .

3. Na stránce **útraty Azure** v části **zákazníci s předplatnými Microsoft Azure** vyberte zákazníky, pro které chcete nastavit rozpočet.

4. Zadejte hodnotu pro **měsíční rozpočet** .

5. Chcete-li uložit změny, klikněte na tlačítko **použít** .

Můžete také *nastavit rozpočet pro jednotlivé zákazníky* v nastavení jejich předplatného:

1. Přihlaste se k řídicímu panelu partnerského centra.

2. V nabídce vlevo v části **CSP** vyberte **zákazníci** .

3. Na stránce **Customers (zákazníci** ) vyberte **název společnosti** zákazníka.

4. Na stránce **předplatná** zákazníka v části **předplatné na základě využití** vyberte **změnit rozpočet** .

5. Zadejte hodnotu pro rozpočet.

6. Chcete-li uložit změny, klikněte na tlačítko **použít** .

## <a name="remove-azure-spending-budget"></a>Odebrat rozpočet útraty Azure

*Měsíční rozpočet Azure útraty* můžete pro zákazníky v partnerském centru odebrat:

1. Přihlaste se k [řídicímu panelu partnerského centra](https://partner.microsoft.com/dashboard/).

2. V nabídce vlevo v části **CSP** vyberte **útraty Azure** .

3. Na stránce **útraty Azure** v části **zákazníci s předplatnými Microsoft Azure** vyberte zákazníky, jejichž rozpočet chcete odebrat.

4. Vyberte možnost **Odebrat rozpočet** .

## <a name="check-current-azure-spending"></a>Kontrolovat aktuální útratu Azure

*Aktuální výdaje na Azure a měsíční rozpočty můžete sledovat* kdykoli:

1. Přihlaste se k [řídicímu panelu partnerského centra](https://partner.microsoft.com/dashboard/).

2. V nabídce vlevo v části **CSP** vyberte **útraty Azure** .

3. Na stránce **útraty Azure** můžete v části **zákazníci s předplatnými Microsoft Azure** zobrazit přehled měsíčních rozpočtů zákazníků, aktuální odhady útraty a procento využití rozpočtu.

## <a name="notifications-for-budget-limits"></a>Oznámení pro limity rozpočtu

*E-mailová oznámení můžete zapnout* , když se Měsíční útrata vašeho zákazníka blíží jejich limitu. Když zapnete tuto možnost, budete upozorněni, když zákazníci použijí 80% nebo více jejich měsíčních rozpočtů. Tato možnost vám pomůže udržet si přehled o fakturaci Azure. Konfigurace e-mailových oznámení:

1. Přihlaste se do Partnerského centra.

2. V nabídce vlevo v části **CSP** vyberte **útraty Azure** .

3. Na stránce **útraty Azure** v části **e-mailová oznámení** přepněte nastavení **získat e-maily** na **zapnuto** .

4. Zvolením možnosti **změnit e-mailová** adresa zobrazíte e-mailovou adresu pro oznámení.

5. Pokud e-mailová adresa *není správná* , zadejte správnou e-mailovou adresu a klikněte na **aktualizovat** . Pokud je e-mailová adresa *správná* , klikněte na **tlačítko Storno** .

## <a name="itemized-costs-by-service"></a>Vynásobené náklady podle služby

*Podle služby můžete u předplatných založených na využití zobrazit náklady na zboží (a Odhadované využití)* :

1. Přihlaste se do Partnerského centra.

2. V nabídce vlevo v části **CSP** vyberte **zákazníci** .

3. Na stránce **Customers (zákazníci** ) vyberte **název společnosti** zákazníka.

4. Na stránce **předplatná** zákazníka v části **předplatná na základě využití** vyberte název **předplatného** .

5. Na stránce předplatného můžete zkontrolovat **náklady na zboží** podle služby a **Odhadované využití** aktuálního měsíce.
