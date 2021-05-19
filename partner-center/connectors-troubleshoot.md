---
title: Řešení potíží s konektory referenčních odkazů spolusoudců
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si odpovědi na běžné dotazy týkající se používání konektorů pro spolu prodej. Přečtěte si tyto nejčastější dotazy k řešení potíží s konektory spoluproduování.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 49a2b6e5461dacbe87c34b36805a5c240c2e5fd1
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148342"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>Řešení potíží s konektory referenčních doporučení ke spoluprodání

**Platí pro:** Dynamics 365 CRM | Salesforce CRM

**Odpovídající role:** Správce referenčních | Správce systému nebo úpravce systému v CRM

 ## <a name="questions-and-answers-about-pre-requisites"></a>Dotazy a odpovědi týkající se požadavků

1. Můžete pro své prostředí použít zkušební řešení konektorů referenčních seznamu spoluprodáva?

Pokud jste v testovacím/pracovním prostředí, můžete zvolit zkušební řešení. Placená verze konektorů je k dispozici v AppSource na 15 USD za měsíc. Při placených připojeních budete za den do 10 tisíc volání rozhraní API. Konektory jsou obálky nad rozhraními API Partnerské centrum referenčních seznamech. Pokaždé, když se  řešení  konektoru spustí pro událost vytvoření nebo aktualizace pro příležitosti na Partnerské centrum nebo na straně CRM, je provedeno volání rozhraní API.

2. Jakou roli potřebujete k vytváření oddílů v prostředí CRM?

Uživatelé, kteří jsou správci systému nebo úpravci systému, mohou použít změny pro všechny. Všichni uživatelé aplikace ale mohou systém přizpůsobit a dokonce sdílet některá vlastní nastavení s ostatními. 

3. Potřebují prodejci partnerů zvláštní role, aby na Partnerské centrum?
 
Prodejcům partnerů musí být přiřazena role Správce referenčních seznamu. Další informace najdete v tématu [Přehled oprávnění.](create-user-accounts-and-set-permissions.md)

4. Jaká pole je potřeba v prostředí CRM nastavit jako první? 

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

Postupujte podle tohoto kroku řešení potíží:

- Pomocí přihlašovacích Partnerské centrum se jednou přihlaste k prostředí toku (flow.microsoft.com).


3. Co dělat, když se při aktivaci toku Partnerské centrum CRM na Power Automate platformě zobrazí následující chyba?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Chybová zpráva vyžadující aktualizace":::

Postupujte podle těchto kroků pro řešení potíží:

- Nejprve aktivujte následující dva podřízené toky před aktivací Partnerské centrum toku CRM.
      - Partnerské centrum na CRM – pomocná funkce (Insider Preview)
      - Partnerské centrum CRM (Insider Preview) od Microsoftu – Aktualizace referenčních doporučení ke spoluprodání

4. Co byste měli dělat, když se vám při pokusu o úpravu toku ne podařilo přidat připojení k toku?

Připojení k toku přidáte, když je tok spuštěný, a ke každému toku se přidávají samostatně.  Pokud se dialogové okno pro přidání připojení neotevře automaticky při úpravách toku, můžete upravit jednotlivé kroky a dílčí kroky toků jednotlivě.

- Vyberte každý tok a upravte je jednotlivě.
- Rozbalení všech kroků v toku 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Kroky, které potřebují připojení":::

- Vyberte kroky, ve kterých se zobrazí ikona upozornění s žádostí o přidružení připojení a přidání připojení. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Úprava toku krok za krokem":::


5. Co byste měli dělat, když se toky řešení konektorů referenčních odkazů spoluprodáky nezapnout?

A. V Power Automate budete muset toky upravit v následujícím pořadí a aktualizovat je tak, aby se používají správná připojení:

- Partnerské centrum registrace webhooku (Insider Preview)
- Vytvoření společného prodejního odkazu – Salesforce do partnerského centra (Insider Preview)
- Aktualizace referenčních seznamů Microsoftu v partnerském centru pro spoluprodej na Salesforce (Insider Preview)
- Partnerské centrum do Salesforce (Insider Preview)
- Salesforce do partnerského centra (Insider Preview)
- Možnost Salesforce v partnerském centru (Insider Preview)
- Řešení Salesforce Microsoftu do partnerského centra (Insider Preview)

 B. U každého toku vyberte možnost **Spustit pouze uživatele** . Vyberte **použít připojení** místo **přidaných uživatelem pouze pro spuštění**.  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Postup aktivace toku":::


C. Níže uvedené toky aktivujte:

 - Aktualizace referenčních seznamů Microsoftu v partnerském centru pro spoluprodej na Salesforce (Insider Preview)

- Salesforce do partnerského centra (Insider Preview)

    
D. Aktivujte všechny zbývající toky.

E. V registraci Webhooku partnerského centra toku vyberte **Spustit**. Zadejte **adresu URL protokolu HTTP** z první akce v **partnerském centru do služby Salesforce** Flow. Vyberte všechny čtyři možnosti v části **události k registraci** a pro přepsání vyberte **Ano** .

## <a name="questions-and-answers-about-runmaintenance"></a>Otázky a odpovědi týkající se spuštění/údržby

1. Jak řešit chyby při automatizaci automatizace výkonu při automatizovaném zpracování?

Chcete-li zajistit, aby toky automatizovaného automatizace běžely, jak očekáváte, a chcete-li vyřešit chyby během provádění, přečtěte si téma [Oprava selhání toku](/power-automate/fix-flow-failures)

2. Co byste měli dělat, když vidíte odkazy, které nejsou synchronizované správně v partnerském centru nebo prostředí CRM?
 
Pokud chcete zjistit stav synchronizace referenčních seznamu, vyberte **Auditovat.** 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Synchronizace referenčních odkazů":::

Ujistěte se, že jsou splněné následující podmínky:

- ID řešení se poskytuje jako součást příležitosti.

- Vyžaduje se dvou písmeno kódu země.

- Pokud je pro příležitost vybrána pomoc od Microsoftu, jsou vyžadovány kontaktní údaje zákazníka.

3. Jak zajistit, aby se referenční seznam synchronizoval obousměrně?

Proveďte následující kroky:

- Prodejci partnerů musí zajistit, aby v části CRM **Partnerské centrum** možnost Synchronizovat s partnery.

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Ujistěte se, že jste povolili možnost Synchronizace.":::

- Prodejci musí při kvalifikaci zájemce poskytnout výnosy a datum ukončení.

- Pokud je ID CRM  uvedené  ve fázi vytvoření nebo aktualizace příležitosti ke spoluproduu, ale prodejní příležitost zájemce s tímto ID se v CRM nenaledí, bude aktualizace nebo vytvoření ignorována.

- Ujistěte se, že je v prostředí Salesforce nakonfigurované pole měny referenčního seznamu. 

4. Co dělat, když se konektor odpojí a nezmeškáte synchronizaci referenčních odkazů?

Tady je několik možností, které si můžete vyzkoušet:

- Zkontrolujte, jestli pro uživatele s rolí správce referenčních Partnerské centrum vypršela platnost uživatelského jména nebo hesla.

- Můžete přejít k nesynchronní příležitosti, provést dílčí aktualizaci a sledovat, jestli se referenční seznam synchronizoval.

- Pokud toky byly spuštěny a selhaly, vyberte tok a znovu odešlete neúspěšné spuštění.

5. Co dělat, když dojde k chybám odepření přístupu?

Ujistěte se, že existují příslušné role.

- Role Správce odkazů pro prodejce partnerského centra 
 
- Role správce systému nebo úpravce systému v instanci CRM

- Zajistěte, aby se uživatel účtu toku Power Automate přihlásil https://flow.microsoft.com alespoň jednou předem.

6. Pokud zjistíte, že při vytváření příležitosti společného prodeje chybí **kód země zákaznického účtu** , co byste měli dělat?

Do účtu zákazníka v aplikaci CRM budete muset přidat kód země o dvou písmenech.

7. Co byste měli dělat v případě, že se při vytváření příležitosti společného prodeje zobrazí chyba, že **se ID řešení vyžaduje** ?

Aby bylo možné vytvořit odkaz pro spoluprodej, potřebujete řešení připravené pro spoluprodejní účely Microsoftu. 

8. Co byste měli dělat v případě, že se v partnerském centru zobrazují příležitosti pro prodej, které nejsou synchronizované s CRM, i když nedochází k chybám toků?

Postupujte následovně:

- Po vytvoření nového společného prodeje v partnerském centru ověřte, jestli se má vyvolávat tok partnerského centra na Dynamics 365 (může se vyvolávat víckrát).

- Pokud se tok vyvolá, zkontroluje všechny vyvolané toky a určí běh toku, který by aktualizoval CRM. Můžete postupovat podle těchto akcí a ověřit, jestli aktualizace CRM aktualizovala nebo nastala nějaký problém.

- V partnerském centru pro kontrolu **nové koupě** zjistíte, jestli se naplní ID CRM.

- Ujistěte se, že obchod se nechtěně neuzavřel v partnerském centru jako **získaná** nebo **ztracená** .

## <a name="next-steps"></a>Další kroky

- [Správa potenciálních zákazníků](manage-leads.md)
 
- [Správa příležitostí ke spoluprodeji](manage-co-sell-opportunities.md)
