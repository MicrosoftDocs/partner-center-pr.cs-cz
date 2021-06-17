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
ms.openlocfilehash: bb7a227624c548a29046b80d3bd5fa363a4aee2f
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276923"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="b35fd-104">Řešení potíží s konektory pro souběžné vyprodejní reference</span><span class="sxs-lookup"><span data-stu-id="b35fd-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="b35fd-105">**Platí pro**: Dynamics 365 CRM | Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="b35fd-105">**Applies to**: Dynamics 365 CRM | Salesforce CRM</span></span>

<span data-ttu-id="b35fd-106">**Příslušné role**: Správce odkazů | Správce systému nebo úpravce systému v CRM</span><span class="sxs-lookup"><span data-stu-id="b35fd-106">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="b35fd-107">Otázky a odpovědi týkající se požadavků</span><span class="sxs-lookup"><span data-stu-id="b35fd-107">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="b35fd-108">Můžete pro svoje prostředí použít řešení konektorů pro zkušební verzi předprodejního prostředí?</span><span class="sxs-lookup"><span data-stu-id="b35fd-108">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="b35fd-109">Pokud jste v testovacím nebo přípravném prostředí, můžete se rozhodnout pro zkušební řešení.</span><span class="sxs-lookup"><span data-stu-id="b35fd-109">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="b35fd-110">Placená verze konektorů je k dispozici v AppSource ve výši US 15 měsíčně.</span><span class="sxs-lookup"><span data-stu-id="b35fd-110">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="b35fd-111">U placeného připojení budete získávat 10 000 volání rozhraní API za den.</span><span class="sxs-lookup"><span data-stu-id="b35fd-111">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="b35fd-112">Konektory jsou obálkami nad rozhraní API pro odkazy partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="b35fd-112">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="b35fd-113">Pokaždé, když jsou řešení konektoru spuštěna pro událost **Vytvoření** nebo **aktualizace** v příležitostech na straně partnerského centra nebo na straně CRM, bude provedeno volání rozhraní API.</span><span class="sxs-lookup"><span data-stu-id="b35fd-113">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="b35fd-114">Jaké role potřebujete k vytváření oddílů v prostředí CRM?</span><span class="sxs-lookup"><span data-stu-id="b35fd-114">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="b35fd-115">Uživatelé, kteří jsou systémový správce nebo úpravce systému, mohou použít změny pro všechny.</span><span class="sxs-lookup"><span data-stu-id="b35fd-115">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="b35fd-116">Všichni uživatelé aplikace ale můžou přizpůsobit systém a dokonce sdílet některá vlastní nastavení s ostatními.</span><span class="sxs-lookup"><span data-stu-id="b35fd-116">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="b35fd-117">Potřebují prodejci v partnerském centru pracovat s dalšími rolemi?</span><span class="sxs-lookup"><span data-stu-id="b35fd-117">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="b35fd-118">Prodejcům partnera musí být přiřazena role Správce odkazů.</span><span class="sxs-lookup"><span data-stu-id="b35fd-118">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="b35fd-119">Další informace najdete v tématu [Přehled oprávnění](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="b35fd-119">For more information, see [Permissions overview](create-user-accounts-and-set-permissions.md).</span></span>

4. <span data-ttu-id="b35fd-120">Jaká pole je třeba nejprve nastavit v prostředí CRM?</span><span class="sxs-lookup"><span data-stu-id="b35fd-120">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="b35fd-121">• Ujistěte se, že je vaše měna vhodná pro vaše umístění a že je ve vašem prostředí CRM přesně.</span><span class="sxs-lookup"><span data-stu-id="b35fd-121">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="b35fd-122">• Váš prodejní tým by měl být uveden v prostředí CRM jako uživatelé aplikace CRM.</span><span class="sxs-lookup"><span data-stu-id="b35fd-122">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="b35fd-123">Jaké jsou požadavky nutné k vytvoření prostředí Power Automate pro automatizaci?</span><span class="sxs-lookup"><span data-stu-id="b35fd-123">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="b35fd-124">Pokud chcete používat prostředí Power Automate, potřebujete:</span><span class="sxs-lookup"><span data-stu-id="b35fd-124">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="b35fd-125">Vyžaduje se licence Power Automate.</span><span class="sxs-lookup"><span data-stu-id="b35fd-125">A Power Automate license is required.</span></span>
- <span data-ttu-id="b35fd-126">Vyžaduje se minimálně 1 GB úložiště.</span><span class="sxs-lookup"><span data-stu-id="b35fd-126">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="b35fd-127">Potřebujete předplatné Dynamics 365, abyste mohli používat řešení konektorů Salesforce?</span><span class="sxs-lookup"><span data-stu-id="b35fd-127">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="b35fd-128">Řešení konektoru Salesforce je typu Dynamics flow, který podporuje synchronizaci s ostatními systémy CRM.</span><span class="sxs-lookup"><span data-stu-id="b35fd-128">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="b35fd-129">Řešení nevyžaduje, abyste měli instanci Dynamics 365 nebo předplatné.</span><span class="sxs-lookup"><span data-stu-id="b35fd-129">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="b35fd-130">Při instalaci řešení Salesforce se může zobrazit rozevírací seznam s existujícím prostředím CD ve vaší společnosti.</span><span class="sxs-lookup"><span data-stu-id="b35fd-130">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="b35fd-131">Je nutné vybrat toto prostředí.</span><span class="sxs-lookup"><span data-stu-id="b35fd-131">You need to select that environment.</span></span> <span data-ttu-id="b35fd-132">Pokud se navíc zobrazí chyba "nepovedlo se nám najít organizaci Dynamics 365 spojenou s přihlášeným uživatelem", budete muset vytvořit nové prostředí pro konektor.</span><span class="sxs-lookup"><span data-stu-id="b35fd-132">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="b35fd-133">Otázky a odpovědi týkající se konfigurace</span><span class="sxs-lookup"><span data-stu-id="b35fd-133">Questions and answers about configuration</span></span>

1. <span data-ttu-id="b35fd-134">Co byste měli dělat v případě, že při aktivaci toků na platformě Power Automate čelíte následující chybě?</span><span class="sxs-lookup"><span data-stu-id="b35fd-134">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="b35fd-135">Chyba: požadavek na Azure Resource Manager se nezdařil s chybou: {"Error": {"Code": "WorkflowTriggerNotFound", "Message": "pracovní postup" e14d00f1-1fdf-4b1b-aaac-54a5064093d3 "Trigger" Manual "nebylo možné najít."}} ".</span><span class="sxs-lookup"><span data-stu-id="b35fd-135">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="b35fd-136">Postupujte podle těchto kroků pro řešení potíží:</span><span class="sxs-lookup"><span data-stu-id="b35fd-136">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="b35fd-137">Odstraňte připojení k DISKům CD a pak znovu vytvořte připojení k těmto DISKům.</span><span class="sxs-lookup"><span data-stu-id="b35fd-137">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="b35fd-138">Zapnutí a vypnutí podřízeného toku</span><span class="sxs-lookup"><span data-stu-id="b35fd-138">Turn the child flow off and on</span></span> 
- <span data-ttu-id="b35fd-139">Odstraňte řešení a pak ho znovu nainstalujte.</span><span class="sxs-lookup"><span data-stu-id="b35fd-139">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="b35fd-140">Co byste měli dělat v případě, že při přidávání konektoru partnerského centra na platformě Power automatu máte na výběrovou chybu "přihlásit"?</span><span class="sxs-lookup"><span data-stu-id="b35fd-140">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Chybová zpráva vyžadující přihlášení":::

<span data-ttu-id="b35fd-142">Postupujte podle tohoto kroku pro řešení potíží:</span><span class="sxs-lookup"><span data-stu-id="b35fd-142">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="b35fd-143">Pomocí přihlašovacích údajů partnerského centra se přihlaste do prostředí flow (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="b35fd-143">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="b35fd-144">Co byste měli dělat, když při aktivaci partnerského centra do služby CRM na platformě Power Automate dojde k následující chybě?</span><span class="sxs-lookup"><span data-stu-id="b35fd-144">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Chybová zpráva vyžadující aktualizace.":::

<span data-ttu-id="b35fd-146">Postupujte podle těchto kroků pro řešení potíží:</span><span class="sxs-lookup"><span data-stu-id="b35fd-146">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="b35fd-147">Před aktivací partnerského centra na Flow CRM aktivujte nejprve následující dva podřízené toky.</span><span class="sxs-lookup"><span data-stu-id="b35fd-147">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="b35fd-148">Partnerské centrum na CRM – pomocníka (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b35fd-148">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="b35fd-149">Partnerské centrum pro spoluprodejní aktualizace pro Microsoft CRM (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b35fd-149">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="b35fd-150">Co byste měli dělat, když při pokusu o úpravu toku nemůžete přidat připojení k toku?</span><span class="sxs-lookup"><span data-stu-id="b35fd-150">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="b35fd-151">Do toku přidáte připojení, zatímco tok běží a přidáte do každého toku samostatně.</span><span class="sxs-lookup"><span data-stu-id="b35fd-151">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="b35fd-152">Pokud se dialogové okno pro přidání připojení při úpravě toku automaticky neotevře, můžete upravit každý z kroků a dílčích kroků jednotlivých toků.</span><span class="sxs-lookup"><span data-stu-id="b35fd-152">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="b35fd-153">Vyberte jednotlivé toky a upravte je jednotlivě.</span><span class="sxs-lookup"><span data-stu-id="b35fd-153">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="b35fd-154">Rozbalení všech kroků v toku</span><span class="sxs-lookup"><span data-stu-id="b35fd-154">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Kroky, které vyžadují připojení.":::

- <span data-ttu-id="b35fd-156">Vyberte postup, ve kterém se zobrazí výstražná ikona s výzvou k přidružení připojení a přidání připojení.</span><span class="sxs-lookup"><span data-stu-id="b35fd-156">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Upravte tok krok za krokem.":::


5. <span data-ttu-id="b35fd-158">Co byste měli dělat v případě, že se nezapne toky řešení konektorů pro spoluprodejní odkazy?</span><span class="sxs-lookup"><span data-stu-id="b35fd-158">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="b35fd-159">A.</span><span class="sxs-lookup"><span data-stu-id="b35fd-159">A.</span></span> <span data-ttu-id="b35fd-160">V Power automatu budete muset toky upravit v následujícím pořadí a aktualizovat je, aby používaly správná připojení:</span><span class="sxs-lookup"><span data-stu-id="b35fd-160">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="b35fd-161">Registrace Webhooku partnerského centra (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b35fd-161">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="b35fd-162">Vytvoření společného prodejního odkazu – Salesforce do partnerského centra (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b35fd-162">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="b35fd-163">Aktualizace referenčních seznamů Microsoftu v partnerském centru pro spoluprodej na Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b35fd-163">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="b35fd-164">Partnerské centrum do Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b35fd-164">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="b35fd-165">Salesforce do partnerského centra (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b35fd-165">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="b35fd-166">Možnost Salesforce v partnerském centru (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b35fd-166">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="b35fd-167">Řešení Salesforce Microsoftu do partnerského centra (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b35fd-167">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="b35fd-168">B.</span><span class="sxs-lookup"><span data-stu-id="b35fd-168">B.</span></span> <span data-ttu-id="b35fd-169">U každého toku vyberte možnost **Spustit pouze uživatele** .</span><span class="sxs-lookup"><span data-stu-id="b35fd-169">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="b35fd-170">Vyberte **použít připojení** místo **přidaných uživatelem pouze pro spuštění**.</span><span class="sxs-lookup"><span data-stu-id="b35fd-170">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Aktivuje tok.":::


<span data-ttu-id="b35fd-172">C.</span><span class="sxs-lookup"><span data-stu-id="b35fd-172">C.</span></span> <span data-ttu-id="b35fd-173">Níže uvedené toky aktivujte:</span><span class="sxs-lookup"><span data-stu-id="b35fd-173">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="b35fd-174">Aktualizace referenčních seznamů Microsoftu v partnerském centru pro spoluprodej na Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b35fd-174">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="b35fd-175">Salesforce do partnerského centra (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="b35fd-175">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="b35fd-176">D.</span><span class="sxs-lookup"><span data-stu-id="b35fd-176">D.</span></span> <span data-ttu-id="b35fd-177">Aktivujte všechny zbývající toky.</span><span class="sxs-lookup"><span data-stu-id="b35fd-177">Activate all the remaining flows.</span></span>

<span data-ttu-id="b35fd-178">E.</span><span class="sxs-lookup"><span data-stu-id="b35fd-178">E.</span></span> <span data-ttu-id="b35fd-179">V registraci Webhooku partnerského centra toku vyberte **Spustit**.</span><span class="sxs-lookup"><span data-stu-id="b35fd-179">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="b35fd-180">Zadejte **adresu URL protokolu HTTP** z první akce v **partnerském centru do služby Salesforce** Flow.</span><span class="sxs-lookup"><span data-stu-id="b35fd-180">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="b35fd-181">Vyberte všechny čtyři možnosti v části **události k registraci** a pro přepsání vyberte **Ano** .</span><span class="sxs-lookup"><span data-stu-id="b35fd-181">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="b35fd-182">Otázky a odpovědi týkající se spuštění/údržby</span><span class="sxs-lookup"><span data-stu-id="b35fd-182">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="b35fd-183">Jak řešit chyby při automatizaci automatizace výkonu při automatizovaném zpracování?</span><span class="sxs-lookup"><span data-stu-id="b35fd-183">How do you troubleshoot failures during Power Automate flow execution?</span></span>

<span data-ttu-id="b35fd-184">Chcete-li zajistit, aby toky automatizovaného automatizace běžely, jak očekáváte, a chcete-li vyřešit chyby během provádění, přečtěte si téma [Oprava selhání toku](/power-automate/fix-flow-failures)</span><span class="sxs-lookup"><span data-stu-id="b35fd-184">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="b35fd-185">Co byste měli dělat, když vidíte odkazy, které nejsou synchronizované správně v partnerském centru nebo prostředí CRM?</span><span class="sxs-lookup"><span data-stu-id="b35fd-185">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="b35fd-186">Pokud chcete zjistit stav synchronizace referenčních odkazů, vyberte **audit**.</span><span class="sxs-lookup"><span data-stu-id="b35fd-186">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Jak synchronizovat odkazy.":::

<span data-ttu-id="b35fd-188">Ujistěte se, že jsou splněné následující podmínky:</span><span class="sxs-lookup"><span data-stu-id="b35fd-188">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="b35fd-189">ID řešení se poskytuje jako součást příležitosti.</span><span class="sxs-lookup"><span data-stu-id="b35fd-189">Solution ID is provided as part of the opportunity.</span></span>

- <span data-ttu-id="b35fd-190">Je požadováno dva kódy země.</span><span class="sxs-lookup"><span data-stu-id="b35fd-190">Two letter country code is required.</span></span>

- <span data-ttu-id="b35fd-191">Když je pro příležitost vybraná možnost Microsoft, kontaktní informace zákazníka se vyžadují.</span><span class="sxs-lookup"><span data-stu-id="b35fd-191">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="b35fd-192">Jak zajistit, aby se odkaz synchronizovaly v obousměrném směru?</span><span class="sxs-lookup"><span data-stu-id="b35fd-192">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="b35fd-193">Proveďte následující kroky:</span><span class="sxs-lookup"><span data-stu-id="b35fd-193">Do the following steps:</span></span>

- <span data-ttu-id="b35fd-194">Prodejci partnerů musí zajistit, aby v části CRM povolili možnost **synchronizovat s partnerským centrem** .</span><span class="sxs-lookup"><span data-stu-id="b35fd-194">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Ujistěte se, že jste povolili synchronizaci.":::

- <span data-ttu-id="b35fd-196">Prodejci musí zadat datum a čas uzavření při kvalifikaci potenciálního zákazníka.</span><span class="sxs-lookup"><span data-stu-id="b35fd-196">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="b35fd-197">Pokud je ID CRM k dispozici v fázi **Vytvoření** nebo **aktualizace** v rámci společného prodeje, ale v CRM se nenalezne příležitost s tímto ID, aktualizace nebo vytvoření se budou ignorovat.</span><span class="sxs-lookup"><span data-stu-id="b35fd-197">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="b35fd-198">Ujistěte se, že je v prostředí Salesforce nakonfigurované pole Měna reference.</span><span class="sxs-lookup"><span data-stu-id="b35fd-198">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="b35fd-199">Co byste měli dělat v případě, že se konektor odpojí a Vy jste nedostali synchronizaci referenčních informací?</span><span class="sxs-lookup"><span data-stu-id="b35fd-199">What should you do if the connector gets disconnected and you miss a referral synchronization.?</span></span>

<span data-ttu-id="b35fd-200">Níže jsou uvedené některé z možností, které můžete vyzkoušet:</span><span class="sxs-lookup"><span data-stu-id="b35fd-200">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="b35fd-201">Ověřte, jestli vypršela platnost uživatelského jména nebo hesla pro uživatele partnerského centra s rolemi Správce odkazů.</span><span class="sxs-lookup"><span data-stu-id="b35fd-201">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="b35fd-202">Můžete přejít na nesynchronizovanou příležitost, udělat dílčí aktualizaci a sledovat, zda se odkaz synchronizoval.</span><span class="sxs-lookup"><span data-stu-id="b35fd-202">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="b35fd-203">Pokud jsou toky spuštěné a selhaly, vyberte tok a znovu odešlete spuštění, které selhalo.</span><span class="sxs-lookup"><span data-stu-id="b35fd-203">If the flows have run and failed, then select the flow and re-submit the run that has failed.</span></span>

5. <span data-ttu-id="b35fd-204">Co byste měli dělat, když získáte chyby při odepření přístupu?</span><span class="sxs-lookup"><span data-stu-id="b35fd-204">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="b35fd-205">Ujistěte se, že existují vhodné role.</span><span class="sxs-lookup"><span data-stu-id="b35fd-205">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="b35fd-206">Role Správce odkazů pro prodejce partnerského centra</span><span class="sxs-lookup"><span data-stu-id="b35fd-206">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="b35fd-207">Role správce systému nebo úpravce systému v instanci CRM</span><span class="sxs-lookup"><span data-stu-id="b35fd-207">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="b35fd-208">Zajistěte, aby se uživatel účtu toku Power Automate přihlásil https://flow.microsoft.com alespoň jednou předem.</span><span class="sxs-lookup"><span data-stu-id="b35fd-208">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="b35fd-209">Pokud zjistíte, že při vytváření příležitosti společného prodeje chybí **kód země zákaznického účtu** , co byste měli dělat?</span><span class="sxs-lookup"><span data-stu-id="b35fd-209">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="b35fd-210">Do účtu zákazníka v aplikaci CRM budete muset přidat kód země o dvou písmenech.</span><span class="sxs-lookup"><span data-stu-id="b35fd-210">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="b35fd-211">Co byste měli dělat v případě, že se při vytváření příležitosti společného prodeje zobrazí chyba, že **se ID řešení vyžaduje** ?</span><span class="sxs-lookup"><span data-stu-id="b35fd-211">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="b35fd-212">Aby bylo možné vytvořit odkaz pro spoluprodej, potřebujete řešení připravené pro spoluprodejní účely Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="b35fd-212">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="b35fd-213">Co byste měli dělat v případě, že se v partnerském centru zobrazují příležitosti pro prodej, které nejsou synchronizované s CRM, i když nedochází k chybám toků?</span><span class="sxs-lookup"><span data-stu-id="b35fd-213">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors?</span></span>

<span data-ttu-id="b35fd-214">Postupujte následovně:</span><span class="sxs-lookup"><span data-stu-id="b35fd-214">Do the following:</span></span>

- <span data-ttu-id="b35fd-215">Po vytvoření nového společného prodeje v partnerském centru ověřte, jestli se má vyvolávat tok partnerského centra na Dynamics 365 (může se vyvolávat víckrát).</span><span class="sxs-lookup"><span data-stu-id="b35fd-215">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="b35fd-216">Pokud se tok vyvolá, zkontroluje všechny vyvolané toky a určí běh toku, který by aktualizoval CRM.</span><span class="sxs-lookup"><span data-stu-id="b35fd-216">If the flow gets invoked, check all invoked flows, and identify the flow run which that would update the CRM.</span></span> <span data-ttu-id="b35fd-217">Můžete postupovat podle těchto akcí a ověřit, jestli aktualizace CRM aktualizovala nebo nastala nějaký problém.</span><span class="sxs-lookup"><span data-stu-id="b35fd-217">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="b35fd-218">V partnerském centru pro kontrolu **nové koupě** zjistíte, jestli se naplní ID CRM.</span><span class="sxs-lookup"><span data-stu-id="b35fd-218">Check **New deal** in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="b35fd-219">Ujistěte se, že obchod se nechtěně neuzavřel v partnerském centru jako **získaná** nebo **ztracená** .</span><span class="sxs-lookup"><span data-stu-id="b35fd-219">Make sure that the deal is not accidentally closed as **Won** or **Lost** in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b35fd-220">Další kroky</span><span class="sxs-lookup"><span data-stu-id="b35fd-220">Next steps</span></span>

- [<span data-ttu-id="b35fd-221">Správa potenciálních zákazníků</span><span class="sxs-lookup"><span data-stu-id="b35fd-221">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="b35fd-222">Správa příležitostí ke spoluprodeji</span><span class="sxs-lookup"><span data-stu-id="b35fd-222">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
