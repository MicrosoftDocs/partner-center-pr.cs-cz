---
title: Řešení potíží s konektory pro souběžné vyprodejní reference
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si odpovědi na běžné dotazy týkající se používání vzájemně prodávaných konektorů. Přečtěte si tyto Nejčastější dotazy týkající se řešení potíží s konektory pro spoluprodej.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 988a696a8a0a0abb4d37e3915c76f905ec5b35b0
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/14/2020
ms.locfileid: "92527682"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>Řešení potíží s konektory pro souběžné vyprodejní reference

**Platí pro:**

- Partnerské centrum
- Dynamics 365 CRM
- Salesforce CRM

**Příslušné role**

- Správce odkazů
- Správce systému nebo úpravce systému v CRM

 ## <a name="questions-and-answers-about-pre-requisites"></a>Otázky a odpovědi týkající se požadavků

1. Můžete pro svoje prostředí použít řešení konektorů pro zkušební verzi předprodejního prostředí?

Pokud jste v testovacím nebo přípravném prostředí, můžete se rozhodnout pro zkušební řešení. Placená verze konektorů je k dispozici v AppSource ve výši US 15 měsíčně. U placeného připojení budete získávat 10 000 volání rozhraní API za den. Konektory jsou obálkami nad rozhraní API pro odkazy partnerského centra. Pokaždé, když jsou řešení konektoru spuštěna pro událost **Vytvoření** nebo **aktualizace** v příležitostech na straně partnerského centra nebo na straně CRM, bude provedeno volání rozhraní API.

2. Jaké role potřebujete k vytváření oddílů v prostředí CRM?

Uživatelé, kteří jsou systémový správce nebo úpravce systému, mohou použít změny pro všechny. Všichni uživatelé aplikace ale můžou přizpůsobit systém a dokonce sdílet některá vlastní nastavení s ostatními. 

3. Potřebují prodejci v partnerském centru pracovat s dalšími rolemi?
 
Prodejcům partnera musí být přiřazena role Správce odkazů. Další informace najdete v následujícím článku [Přehled oprávnění) (Create-User-Accounts-and-set-Permissions).

4. Jaká pole je třeba nejprve nastavit v prostředí CRM? 

• Ujistěte se, že je vaše měna vhodná pro vaše umístění a že je ve vašem prostředí CRM přesně. • Váš prodejní tým by měl být uveden v prostředí CRM jako uživatelé aplikace CRM.

5. Jaké jsou požadavky nutné k vytvoření prostředí Power Automate pro automatizaci?

Pokud chcete používat prostředí Power Automate, potřebujete:

- Vyžaduje se licence Power Automate.
- Vyžaduje se minimálně 1 GB úložiště.

6.  Potřebujete předplatné Dynamics 365, abyste mohli používat řešení konektorů Salesforce?

Řešení konektoru Salesforce je typu Dynamics flow, který podporuje synchronizaci s ostatními systémy CRM. Řešení nevyžaduje, abyste měli instanci Dynamics 365 nebo předplatné. Při instalaci řešení Salesforce se může zobrazit rozevírací seznam s existujícím prostředím CD ve vaší společnosti. Je nutné vybrat toto prostředí. Pokud se navíc zobrazí chyba "nepovedlo se nám najít organizaci Dynamics 365 spojenou s přihlášeným uživatelem", budete muset vytvořit nové prostředí pro konektor.

## <a name="questions-and-answers-about-configuration"></a>Otázky a odpovědi týkající se konfigurace

1. Co byste měli dělat v případě, že při aktivaci toků na platformě Power Automate čelíte následující chybě?

Chyba: požadavek na Azure Resource Manager se nezdařil s chybou: {"Error": {"Code": "WorkflowTriggerNotFound", "Message": "pracovní postup" e14d00f1-1fdf-4b1b-aaac-54a5064093d3 "Trigger" Manual "nebylo možné najít."}} ". 

Postupujte podle těchto kroků pro řešení potíží:

- Odstraňte připojení k DISKům CD a pak znovu vytvořte připojení k těmto DISKům.
- Zapnutí a vypnutí podřízeného toku 
- Odstraňte řešení a pak ho znovu nainstalujte. 

2.  Co byste měli dělat v případě, že při přidávání konektoru partnerského centra na platformě Power automatu máte na výběrovou chybu "přihlásit"?

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Chybová zpráva vyžadující přihlášení":::

Postupujte podle tohoto kroku pro řešení potíží:

- Pomocí přihlašovacích údajů partnerského centra se přihlaste do prostředí flow (flow.microsoft.com).


3. Co byste měli dělat, když při aktivaci partnerského centra do služby CRM na platformě Power Automate dojde k následující chybě?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Chybová zpráva vyžadující přihlášení":::

Postupujte podle těchto kroků pro řešení potíží:

- Před aktivací partnerského centra na Flow CRM aktivujte nejprve následující dva podřízené toky.
      - Partnerské centrum na CRM – pomocníka (Insider Preview)
      - Partnerské centrum pro spoluprodejní aktualizace pro Microsoft CRM (Insider Preview)

4. Co byste měli dělat, když při pokusu o úpravu toku nemůžete přidat připojení k toku?

Do toku přidáte připojení, zatímco tok běží a přidáte do každého toku samostatně.  Pokud se dialogové okno pro přidání připojení při úpravě toku automaticky neotevře, můžete upravit každý z kroků a dílčích kroků jednotlivých toků.

- Vyberte jednotlivé toky a upravte je jednotlivě.
- Rozbalení všech kroků v toku 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Chybová zpráva vyžadující přihlášení":::

- Vyberte postup, ve kterém se zobrazí výstražná ikona s výzvou k přidružení připojení a přidání připojení. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Chybová zpráva vyžadující přihlášení":::


5. Co byste měli dělat v případě, že se nezapne toky řešení konektorů pro spoluprodejní odkazy?

A. V Power automatu budete muset toky upravit v následujícím pořadí a aktualizovat je, aby používaly správná připojení:

- Registrace Webhooku partnerského centra (Insider Preview)
- Vytvoření společného prodejního odkazu – Salesforce do partnerského centra (Insider Preview)
- Aktualizace referenčních seznamů Microsoftu v partnerském centru pro spoluprodej na Salesforce (Insider Preview)
- Partnerské centrum do Salesforce (Insider Preview)
- Salesforce do partnerského centra (Insider Preview)
- Možnost Salesforce v partnerském centru (Insider Preview)
- Řešení Salesforce Microsoftu do partnerského centra (Insider Preview)

 B. U každého toku vyberte možnost **Spustit pouze uživatele** . Vyberte **použít připojení** místo **přidaných uživatelem pouze pro spuštění** .  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Chybová zpráva vyžadující přihlášení":::


C. Níže uvedené toky aktivujte:

 - Aktualizace referenčních seznamů Microsoftu v partnerském centru pro spoluprodej na Salesforce (Insider Preview)

- Salesforce do partnerského centra (Insider Preview)

    
D. Aktivujte všechny zbývající toky.

E. V registraci Webhooku partnerského centra toku vyberte **Spustit** . Zadejte **adresu URL protokolu HTTP** z první akce v **partnerském centru do služby Salesforce** Flow. Vyberte všechny čtyři možnosti v části **události k registraci** a pro přepsání vyberte **Ano** .

## <a name="questions-and-answers-about-runmaintenance"></a>Otázky a odpovědi týkající se spuštění/údržby

1. Jak řešit problémy v případě selhání při automatizovaném provádění toku napájení?

Chcete-li zajistit, aby toky automatizovaného automatizace běžely, jak očekáváte, a chcete-li vyřešit chyby během provádění, přečtěte si téma [Oprava selhání toku](/power-automate/fix-flow-failures)

2. Co byste měli dělat, když vidíte odkazy, které nejsou synchronizované správně v partnerském centru nebo prostředí CRM?
 
Pokud chcete zjistit stav synchronizace referenčních odkazů, vyberte **audit** . 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Chybová zpráva vyžadující přihlášení":::

Ujistěte se, že jsou splněné následující podmínky:

- ID řešení se poskytuje jako součást příležitosti.

- Je požadováno dva kódy země.

- Když je pro příležitost vybraná možnost Microsoft, kontaktní informace zákazníka se vyžadují.

3. Jak zajistit, aby se odkaz synchronizovaly v obousměrném směru?

Proveďte následující kroky:

- Prodejci partnerů musí zajistit, aby v části CRM povolili možnost **synchronizovat s partnerským centrem** .

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Chybová zpráva vyžadující přihlášení" v partnerském centru.

## <a name="next-steps"></a>Další kroky

- [Správa potenciálních zákazníků](manage-leads.md)
 
- [Správa příležitostí ke spoluprodeji](manage-co-sell-opportunities.md)