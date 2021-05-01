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
ms.openlocfilehash: 939654202a370f6d9ba15d9e62a11be44884b613
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284209"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="ac790-104">Řešení potíží s konektory pro souběžné vyprodejní reference</span><span class="sxs-lookup"><span data-stu-id="ac790-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="ac790-105">**Platí pro**</span><span class="sxs-lookup"><span data-stu-id="ac790-105">**Applies to**</span></span>

- <span data-ttu-id="ac790-106">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="ac790-106">Dynamics 365 CRM</span></span>
- <span data-ttu-id="ac790-107">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="ac790-107">Salesforce CRM</span></span>

<span data-ttu-id="ac790-108">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="ac790-108">**Appropriate roles**</span></span>

- <span data-ttu-id="ac790-109">Správce odkazů</span><span class="sxs-lookup"><span data-stu-id="ac790-109">Referrals admin</span></span>
- <span data-ttu-id="ac790-110">Správce systému nebo úpravce systému v CRM</span><span class="sxs-lookup"><span data-stu-id="ac790-110">System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="ac790-111">Otázky a odpovědi týkající se požadavků</span><span class="sxs-lookup"><span data-stu-id="ac790-111">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="ac790-112">Můžete pro svoje prostředí použít řešení konektorů pro zkušební verzi předprodejního prostředí?</span><span class="sxs-lookup"><span data-stu-id="ac790-112">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="ac790-113">Pokud jste v testovacím nebo přípravném prostředí, můžete se rozhodnout pro zkušební řešení.</span><span class="sxs-lookup"><span data-stu-id="ac790-113">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="ac790-114">Placená verze konektorů je k dispozici v AppSource ve výši US 15 měsíčně.</span><span class="sxs-lookup"><span data-stu-id="ac790-114">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="ac790-115">U placeného připojení budete získávat 10 000 volání rozhraní API za den.</span><span class="sxs-lookup"><span data-stu-id="ac790-115">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="ac790-116">Konektory jsou obálkami nad rozhraní API pro odkazy partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="ac790-116">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="ac790-117">Pokaždé, když jsou řešení konektoru spuštěna pro událost **Vytvoření** nebo **aktualizace** v příležitostech na straně partnerského centra nebo na straně CRM, bude provedeno volání rozhraní API.</span><span class="sxs-lookup"><span data-stu-id="ac790-117">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="ac790-118">Jaké role potřebujete k vytváření oddílů v prostředí CRM?</span><span class="sxs-lookup"><span data-stu-id="ac790-118">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="ac790-119">Uživatelé, kteří jsou systémový správce nebo úpravce systému, mohou použít změny pro všechny.</span><span class="sxs-lookup"><span data-stu-id="ac790-119">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="ac790-120">Všichni uživatelé aplikace ale můžou přizpůsobit systém a dokonce sdílet některá vlastní nastavení s ostatními.</span><span class="sxs-lookup"><span data-stu-id="ac790-120">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="ac790-121">Potřebují prodejci v partnerském centru pracovat s dalšími rolemi?</span><span class="sxs-lookup"><span data-stu-id="ac790-121">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="ac790-122">Prodejcům partnera musí být přiřazena role Správce odkazů.</span><span class="sxs-lookup"><span data-stu-id="ac790-122">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="ac790-123">Další informace najdete v tématu [Přehled oprávnění](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="ac790-123">For more information, see [Permissions overview](create-user-accounts-and-set-permissions.md).</span></span>

4. <span data-ttu-id="ac790-124">Jaká pole je třeba nejprve nastavit v prostředí CRM?</span><span class="sxs-lookup"><span data-stu-id="ac790-124">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="ac790-125">• Ujistěte se, že je vaše měna vhodná pro vaše umístění a že je ve vašem prostředí CRM přesně.</span><span class="sxs-lookup"><span data-stu-id="ac790-125">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="ac790-126">• Váš prodejní tým by měl být uveden v prostředí CRM jako uživatelé aplikace CRM.</span><span class="sxs-lookup"><span data-stu-id="ac790-126">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="ac790-127">Jaké jsou požadavky nutné k vytvoření prostředí Power Automate pro automatizaci?</span><span class="sxs-lookup"><span data-stu-id="ac790-127">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="ac790-128">Pokud chcete používat prostředí Power Automate, potřebujete:</span><span class="sxs-lookup"><span data-stu-id="ac790-128">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="ac790-129">Vyžaduje se licence Power Automate.</span><span class="sxs-lookup"><span data-stu-id="ac790-129">A Power Automate license is required.</span></span>
- <span data-ttu-id="ac790-130">Vyžaduje se minimálně 1 GB úložiště.</span><span class="sxs-lookup"><span data-stu-id="ac790-130">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="ac790-131">Potřebujete předplatné Dynamics 365, abyste mohli používat řešení konektorů Salesforce?</span><span class="sxs-lookup"><span data-stu-id="ac790-131">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="ac790-132">Řešení konektoru Salesforce je typu Dynamics flow, který podporuje synchronizaci s ostatními systémy CRM.</span><span class="sxs-lookup"><span data-stu-id="ac790-132">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="ac790-133">Řešení nevyžaduje, abyste měli instanci Dynamics 365 nebo předplatné.</span><span class="sxs-lookup"><span data-stu-id="ac790-133">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="ac790-134">Při instalaci řešení Salesforce se může zobrazit rozevírací seznam s existujícím prostředím CD ve vaší společnosti.</span><span class="sxs-lookup"><span data-stu-id="ac790-134">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="ac790-135">Je nutné vybrat toto prostředí.</span><span class="sxs-lookup"><span data-stu-id="ac790-135">You need to select that environment.</span></span> <span data-ttu-id="ac790-136">Pokud se navíc zobrazí chyba "nepovedlo se nám najít organizaci Dynamics 365 spojenou s přihlášeným uživatelem", budete muset vytvořit nové prostředí pro konektor.</span><span class="sxs-lookup"><span data-stu-id="ac790-136">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="ac790-137">Otázky a odpovědi týkající se konfigurace</span><span class="sxs-lookup"><span data-stu-id="ac790-137">Questions and answers about configuration</span></span>

1. <span data-ttu-id="ac790-138">Co byste měli dělat v případě, že při aktivaci toků na platformě Power Automate čelíte následující chybě?</span><span class="sxs-lookup"><span data-stu-id="ac790-138">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="ac790-139">Chyba: požadavek na Azure Resource Manager se nezdařil s chybou: {"Error": {"Code": "WorkflowTriggerNotFound", "Message": "pracovní postup" e14d00f1-1fdf-4b1b-aaac-54a5064093d3 "Trigger" Manual "nebylo možné najít."}} ".</span><span class="sxs-lookup"><span data-stu-id="ac790-139">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="ac790-140">Postupujte podle těchto kroků pro řešení potíží:</span><span class="sxs-lookup"><span data-stu-id="ac790-140">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="ac790-141">Odstraňte připojení k DISKům CD a pak znovu vytvořte připojení k těmto DISKům.</span><span class="sxs-lookup"><span data-stu-id="ac790-141">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="ac790-142">Zapnutí a vypnutí podřízeného toku</span><span class="sxs-lookup"><span data-stu-id="ac790-142">Turn the child flow off and on</span></span> 
- <span data-ttu-id="ac790-143">Odstraňte řešení a pak ho znovu nainstalujte.</span><span class="sxs-lookup"><span data-stu-id="ac790-143">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="ac790-144">Co byste měli dělat v případě, že při přidávání konektoru partnerského centra na platformě Power automatu máte na výběrovou chybu "přihlásit"?</span><span class="sxs-lookup"><span data-stu-id="ac790-144">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Chybová zpráva vyžadující přihlášení":::

<span data-ttu-id="ac790-146">Postupujte podle tohoto kroku pro řešení potíží:</span><span class="sxs-lookup"><span data-stu-id="ac790-146">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="ac790-147">Pomocí přihlašovacích údajů partnerského centra se přihlaste do prostředí flow (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="ac790-147">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="ac790-148">Co byste měli dělat, když při aktivaci partnerského centra do služby CRM na platformě Power Automate dojde k následující chybě?</span><span class="sxs-lookup"><span data-stu-id="ac790-148">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Chybová zpráva vyžadující aktualizace":::

<span data-ttu-id="ac790-150">Postupujte podle těchto kroků pro řešení potíží:</span><span class="sxs-lookup"><span data-stu-id="ac790-150">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="ac790-151">Před aktivací partnerského centra na Flow CRM aktivujte nejprve následující dva podřízené toky.</span><span class="sxs-lookup"><span data-stu-id="ac790-151">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="ac790-152">Partnerské centrum na CRM – pomocníka (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="ac790-152">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="ac790-153">Partnerské centrum pro spoluprodejní aktualizace pro Microsoft CRM (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="ac790-153">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="ac790-154">Co byste měli dělat, když při pokusu o úpravu toku nemůžete přidat připojení k toku?</span><span class="sxs-lookup"><span data-stu-id="ac790-154">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="ac790-155">Do toku přidáte připojení, zatímco tok běží a přidáte do každého toku samostatně.</span><span class="sxs-lookup"><span data-stu-id="ac790-155">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="ac790-156">Pokud se dialogové okno pro přidání připojení při úpravě toku automaticky neotevře, můžete upravit každý z kroků a dílčích kroků jednotlivých toků.</span><span class="sxs-lookup"><span data-stu-id="ac790-156">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="ac790-157">Vyberte jednotlivé toky a upravte je jednotlivě.</span><span class="sxs-lookup"><span data-stu-id="ac790-157">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="ac790-158">Rozbalení všech kroků v toku</span><span class="sxs-lookup"><span data-stu-id="ac790-158">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Postup, který vyžaduje připojení":::

- <span data-ttu-id="ac790-160">Vyberte postup, ve kterém se zobrazí výstražná ikona s výzvou k přidružení připojení a přidání připojení.</span><span class="sxs-lookup"><span data-stu-id="ac790-160">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Upravit tok krok za krokem":::


5. <span data-ttu-id="ac790-162">Co byste měli dělat v případě, že se nezapne toky řešení konektorů pro spoluprodejní odkazy?</span><span class="sxs-lookup"><span data-stu-id="ac790-162">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="ac790-163">A.</span><span class="sxs-lookup"><span data-stu-id="ac790-163">A.</span></span> <span data-ttu-id="ac790-164">V Power automatu budete muset toky upravit v následujícím pořadí a aktualizovat je, aby používaly správná připojení:</span><span class="sxs-lookup"><span data-stu-id="ac790-164">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="ac790-165">Registrace Webhooku partnerského centra (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="ac790-165">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="ac790-166">Vytvoření společného prodejního odkazu – Salesforce do partnerského centra (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="ac790-166">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="ac790-167">Aktualizace referenčních seznamů Microsoftu v partnerském centru pro spoluprodej na Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="ac790-167">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="ac790-168">Partnerské centrum do Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="ac790-168">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="ac790-169">Salesforce do partnerského centra (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="ac790-169">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="ac790-170">Možnost Salesforce v partnerském centru (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="ac790-170">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="ac790-171">Řešení Salesforce Microsoftu do partnerského centra (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="ac790-171">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="ac790-172">B.</span><span class="sxs-lookup"><span data-stu-id="ac790-172">B.</span></span> <span data-ttu-id="ac790-173">U každého toku vyberte možnost **Spustit pouze uživatele** .</span><span class="sxs-lookup"><span data-stu-id="ac790-173">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="ac790-174">Vyberte **použít připojení** místo **přidaných uživatelem pouze pro spuštění**.</span><span class="sxs-lookup"><span data-stu-id="ac790-174">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Postup aktivace toku":::


<span data-ttu-id="ac790-176">C.</span><span class="sxs-lookup"><span data-stu-id="ac790-176">C.</span></span> <span data-ttu-id="ac790-177">Níže uvedené toky aktivujte:</span><span class="sxs-lookup"><span data-stu-id="ac790-177">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="ac790-178">Aktualizace referenčních seznamů Microsoftu v partnerském centru pro spoluprodej na Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="ac790-178">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="ac790-179">Salesforce do partnerského centra (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="ac790-179">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="ac790-180">D.</span><span class="sxs-lookup"><span data-stu-id="ac790-180">D.</span></span> <span data-ttu-id="ac790-181">Aktivujte všechny zbývající toky.</span><span class="sxs-lookup"><span data-stu-id="ac790-181">Activate all the remaining flows.</span></span>

<span data-ttu-id="ac790-182">E.</span><span class="sxs-lookup"><span data-stu-id="ac790-182">E.</span></span> <span data-ttu-id="ac790-183">V registraci Webhooku partnerského centra toku vyberte **Spustit**.</span><span class="sxs-lookup"><span data-stu-id="ac790-183">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="ac790-184">Zadejte **adresu URL protokolu HTTP** z první akce v **partnerském centru do služby Salesforce** Flow.</span><span class="sxs-lookup"><span data-stu-id="ac790-184">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="ac790-185">Vyberte všechny čtyři možnosti v části **události k registraci** a pro přepsání vyberte **Ano** .</span><span class="sxs-lookup"><span data-stu-id="ac790-185">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="ac790-186">Otázky a odpovědi týkající se spuštění/údržby</span><span class="sxs-lookup"><span data-stu-id="ac790-186">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="ac790-187">Jak řešit chyby při automatizaci automatizace výkonu při automatizovaném zpracování?</span><span class="sxs-lookup"><span data-stu-id="ac790-187">How do you troubleshoot failures during Power Automate flow execution?</span></span>

<span data-ttu-id="ac790-188">Chcete-li zajistit, aby toky automatizovaného automatizace běžely, jak očekáváte, a chcete-li vyřešit chyby během provádění, přečtěte si téma [Oprava selhání toku](/power-automate/fix-flow-failures)</span><span class="sxs-lookup"><span data-stu-id="ac790-188">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="ac790-189">Co byste měli dělat, když vidíte odkazy, které nejsou synchronizované správně v partnerském centru nebo prostředí CRM?</span><span class="sxs-lookup"><span data-stu-id="ac790-189">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="ac790-190">Pokud chcete zjistit stav synchronizace referenčních odkazů, vyberte **audit**.</span><span class="sxs-lookup"><span data-stu-id="ac790-190">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Postup synchronizace odkazů":::

<span data-ttu-id="ac790-192">Ujistěte se, že jsou splněné následující podmínky:</span><span class="sxs-lookup"><span data-stu-id="ac790-192">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="ac790-193">ID řešení se poskytuje jako součást příležitosti.</span><span class="sxs-lookup"><span data-stu-id="ac790-193">Solution ID is provided as part of the opportunity.</span></span>

- <span data-ttu-id="ac790-194">Je požadováno dva kódy země.</span><span class="sxs-lookup"><span data-stu-id="ac790-194">Two letter country code is required.</span></span>

- <span data-ttu-id="ac790-195">Když je pro příležitost vybraná možnost Microsoft, kontaktní informace zákazníka se vyžadují.</span><span class="sxs-lookup"><span data-stu-id="ac790-195">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="ac790-196">Jak zajistit, aby se odkaz synchronizovaly v obousměrném směru?</span><span class="sxs-lookup"><span data-stu-id="ac790-196">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="ac790-197">Proveďte následující kroky:</span><span class="sxs-lookup"><span data-stu-id="ac790-197">Do the following steps:</span></span>

- <span data-ttu-id="ac790-198">Prodejci partnerů musí zajistit, aby v části CRM povolili možnost **synchronizovat s partnerským centrem** .</span><span class="sxs-lookup"><span data-stu-id="ac790-198">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Ujistěte se, že jste povolili synchronizaci.":::

- <span data-ttu-id="ac790-200">Prodejci musí zadat datum a čas uzavření při kvalifikaci potenciálního zákazníka.</span><span class="sxs-lookup"><span data-stu-id="ac790-200">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="ac790-201">Pokud je ID CRM k dispozici v fázi **Vytvoření** nebo **aktualizace** v rámci společného prodeje, ale v CRM se nenalezne příležitost s tímto ID, aktualizace nebo vytvoření se budou ignorovat.</span><span class="sxs-lookup"><span data-stu-id="ac790-201">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="ac790-202">Ujistěte se, že je v prostředí Salesforce nakonfigurované pole Měna reference.</span><span class="sxs-lookup"><span data-stu-id="ac790-202">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="ac790-203">Co byste měli dělat v případě, že se konektor odpojí a Vy jste nedostali synchronizaci referenčních informací?</span><span class="sxs-lookup"><span data-stu-id="ac790-203">What should you do if the connector gets disconnected and you miss a referral synchronization.?</span></span>

<span data-ttu-id="ac790-204">Níže jsou uvedené některé z možností, které můžete vyzkoušet:</span><span class="sxs-lookup"><span data-stu-id="ac790-204">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="ac790-205">Ověřte, jestli vypršela platnost uživatelského jména nebo hesla pro uživatele partnerského centra s rolemi Správce odkazů.</span><span class="sxs-lookup"><span data-stu-id="ac790-205">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="ac790-206">Můžete přejít na nesynchronizovanou příležitost, udělat dílčí aktualizaci a sledovat, zda se odkaz synchronizoval.</span><span class="sxs-lookup"><span data-stu-id="ac790-206">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="ac790-207">Pokud jsou toky spuštěné a selhaly, vyberte tok a znovu odešlete spuštění, které selhalo.</span><span class="sxs-lookup"><span data-stu-id="ac790-207">If the flows have run and failed, then select the flow and re-submit the run that has failed.</span></span>

5. <span data-ttu-id="ac790-208">Co byste měli dělat, když získáte chyby při odepření přístupu?</span><span class="sxs-lookup"><span data-stu-id="ac790-208">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="ac790-209">Ujistěte se, že existují vhodné role.</span><span class="sxs-lookup"><span data-stu-id="ac790-209">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="ac790-210">Role Správce odkazů pro prodejce partnerského centra</span><span class="sxs-lookup"><span data-stu-id="ac790-210">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="ac790-211">Role správce systému nebo úpravce systému v instanci CRM</span><span class="sxs-lookup"><span data-stu-id="ac790-211">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="ac790-212">Zajistěte, aby se uživatel účtu toku Power Automate přihlásil https://flow.microsoft.com alespoň jednou předem.</span><span class="sxs-lookup"><span data-stu-id="ac790-212">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="ac790-213">Pokud zjistíte, že při vytváření příležitosti společného prodeje chybí **kód země zákaznického účtu** , co byste měli dělat?</span><span class="sxs-lookup"><span data-stu-id="ac790-213">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="ac790-214">Do účtu zákazníka v aplikaci CRM budete muset přidat kód země o dvou písmenech.</span><span class="sxs-lookup"><span data-stu-id="ac790-214">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="ac790-215">Co byste měli dělat v případě, že se při vytváření příležitosti společného prodeje zobrazí chyba, že **se ID řešení vyžaduje** ?</span><span class="sxs-lookup"><span data-stu-id="ac790-215">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="ac790-216">Aby bylo možné vytvořit odkaz pro spoluprodej, potřebujete řešení připravené pro spoluprodejní účely Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="ac790-216">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="ac790-217">Co byste měli dělat v případě, že se v partnerském centru zobrazují příležitosti pro prodej, které nejsou synchronizované s CRM, i když nedochází k chybám toků?</span><span class="sxs-lookup"><span data-stu-id="ac790-217">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors?</span></span>

<span data-ttu-id="ac790-218">Postupujte následovně:</span><span class="sxs-lookup"><span data-stu-id="ac790-218">Do the following:</span></span>

- <span data-ttu-id="ac790-219">Po vytvoření nového společného prodeje v partnerském centru ověřte, jestli se má vyvolávat tok partnerského centra na Dynamics 365 (může se vyvolávat víckrát).</span><span class="sxs-lookup"><span data-stu-id="ac790-219">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="ac790-220">Pokud se tok vyvolá, zkontroluje všechny vyvolané toky a určí běh toku, který by aktualizoval CRM.</span><span class="sxs-lookup"><span data-stu-id="ac790-220">If the flow gets invoked, check all invoked flows, and identify the flow run which that would update the CRM.</span></span> <span data-ttu-id="ac790-221">Můžete postupovat podle těchto akcí a ověřit, jestli aktualizace CRM aktualizovala nebo nastala nějaký problém.</span><span class="sxs-lookup"><span data-stu-id="ac790-221">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="ac790-222">V partnerském centru pro kontrolu **nové koupě** zjistíte, jestli se naplní ID CRM.</span><span class="sxs-lookup"><span data-stu-id="ac790-222">Check **New deal** in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="ac790-223">Ujistěte se, že obchod se nechtěně neuzavřel v partnerském centru jako **získaná** nebo **ztracená** .</span><span class="sxs-lookup"><span data-stu-id="ac790-223">Make sure that the deal is not accidentally closed as **Won** or **Lost** in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ac790-224">Další kroky</span><span class="sxs-lookup"><span data-stu-id="ac790-224">Next steps</span></span>

- [<span data-ttu-id="ac790-225">Správa potenciálních zákazníků</span><span class="sxs-lookup"><span data-stu-id="ac790-225">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="ac790-226">Správa příležitostí ke spoluprodeji</span><span class="sxs-lookup"><span data-stu-id="ac790-226">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
