---
title: Převod předplatného Azure v rámci plánu Azure na jiného partnera CSP
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak změnit Cloud Solution Provider programu přidruženého k předplatným Azure zákazníka v rámci plánu Azure.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: dcacc6da51fe40c7eb05997f5409ef5fadbcf693
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856045"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="26e88-103">Převod předplatných plánu Azure zákazníka na jiného partnera</span><span class="sxs-lookup"><span data-stu-id="26e88-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="26e88-104">**Odpovídající role:** Správce účtu | Sales agent | Agent fakturace</span><span class="sxs-lookup"><span data-stu-id="26e88-104">**Appropriate roles**: Account admin | Sales agent | Billing agent</span></span>

<span data-ttu-id="26e88-105">Tento článek popisuje, jak může zákazník přepnout svá předplatná Azure v rámci plánu Azure z jednoho Cloud Solution Provider (CSP) na jiný.</span><span class="sxs-lookup"><span data-stu-id="26e88-105">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="26e88-106">Pokud chcete přepnout předplatná Azure zákazníka od jiného partnera, postupujte podle těchto kroků.</span><span class="sxs-lookup"><span data-stu-id="26e88-106">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="26e88-107">Kroky k dokončení musí provést partner i zákazník.</span><span class="sxs-lookup"><span data-stu-id="26e88-107">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="26e88-108">K nástrojům pro přechod mají přístup pouze partneři s přímým fakturačním vztahem s Microsoftem.</span><span class="sxs-lookup"><span data-stu-id="26e88-108">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="26e88-109">Nepřímí prodejci musí spolupracovat se svými nepřímými poskytovateli, aby tento převodní nástroj využili.</span><span class="sxs-lookup"><span data-stu-id="26e88-109">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="26e88-110">Zákazník musí před využitím tohoto nástroje konverzovat s oběma partnery (aktuální i budoucí).</span><span class="sxs-lookup"><span data-stu-id="26e88-110">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="26e88-111">Offline konverzace se musí vyhnout nejasnostem a četnosti změn.</span><span class="sxs-lookup"><span data-stu-id="26e88-111">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="26e88-112">Partneři a zákazníci by navíc měli před zahájením přechodu porozumět těmto požadavkům a požadavkům:</span><span class="sxs-lookup"><span data-stu-id="26e88-112">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="26e88-113">**Klíčové aspekty:**</span><span class="sxs-lookup"><span data-stu-id="26e88-113">**Key considerations:**</span></span>

- <span data-ttu-id="26e88-114">Rezervace Azure se s předplatným nebudou přesouvat k budoucímu partnerovi.</span><span class="sxs-lookup"><span data-stu-id="26e88-114">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="26e88-115">Ceny CSP pro služby Azure u aktuálního partnera se nebudou přechádovat</span><span class="sxs-lookup"><span data-stu-id="26e88-115">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="26e88-116">Odpovědnosti za podporu pro zákazníka se přesunou k budoucímu partnerovi.</span><span class="sxs-lookup"><span data-stu-id="26e88-116">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="26e88-117">Fakturace a fakturace se v okamžiku převodu přesunou na budoucího partnera.</span><span class="sxs-lookup"><span data-stu-id="26e88-117">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="26e88-118">Převod Role-Based Access Control (RBAC) není ovlivněný službou Azure.</span><span class="sxs-lookup"><span data-stu-id="26e88-118">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="26e88-119">AOBO (Admin on Behalf Of) se ve výchozím nastavení neudělí budoucímu partnerovi.</span><span class="sxs-lookup"><span data-stu-id="26e88-119">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="26e88-120">Produkty z marketplace třetích stran se přenesou, dokud produkty projdou kontrolu způsobilosti pro Marketplace.</span><span class="sxs-lookup"><span data-stu-id="26e88-120">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="26e88-121">Neexistují žádné zvláštní slevy ani regionální omezení.</span><span class="sxs-lookup"><span data-stu-id="26e88-121">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="26e88-122">Produkty nejsou založené na předplatném.</span><span class="sxs-lookup"><span data-stu-id="26e88-122">The products are non-subscription based</span></span>
    - <span data-ttu-id="26e88-123">Budoucí partner by měl spolupracovat s vydavatelem a ujistit se, že je na seznamu povolení pro nasazení produktu.</span><span class="sxs-lookup"><span data-stu-id="26e88-123">The future partner should work with the publisher to make sure they are on the allow list for deployment of the product</span></span>
    - <span data-ttu-id="26e88-124">Pokud nejsou splněny všechny tyto podmínky pro převod produktů z Marketplace, měly by být zrušeny, převedená předplatná Azure a pak znovu zakoupit produkty z Marketplace s novým partnerem.</span><span class="sxs-lookup"><span data-stu-id="26e88-124">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="26e88-125">**Požadavky:**</span><span class="sxs-lookup"><span data-stu-id="26e88-125">**Prerequisites:**</span></span>

- <span data-ttu-id="26e88-126">Zákazník zapojuje aktuálního partnera CSP do svého záměru na přechod</span><span class="sxs-lookup"><span data-stu-id="26e88-126">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="26e88-127">Budoucí partner CSP spolupracuje se zákazníkem, aby zajistil, že bude možné splnit potřeby zákazníků.</span><span class="sxs-lookup"><span data-stu-id="26e88-127">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="26e88-128">Budoucí partner CSP vytvoří vztah se zákazníkem a před zahájením přechodu si zakoupí plán Azure.</span><span class="sxs-lookup"><span data-stu-id="26e88-128">Future CSP partner establishes a relationship with customer and purchases an Azure plan before the transition begins</span></span>  
- <span data-ttu-id="26e88-129">Zákazník se musí Smlouva se zákazníkem Microsoftu s budoucím partnerem CSP.</span><span class="sxs-lookup"><span data-stu-id="26e88-129">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="26e88-130">Budoucí partner CSP musí mít podepsanou Smlouva s partnerem Microsoftu pro použití tohoto nástroje.</span><span class="sxs-lookup"><span data-stu-id="26e88-130">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="26e88-131">Úkoly zákazníka, které se musí dokončit</span><span class="sxs-lookup"><span data-stu-id="26e88-131">Customer tasks to be completed</span></span>

<span data-ttu-id="26e88-132">Pokud chcete převést předplatné Azure v rámci plánu Azure, zákazník musí zahájit proces kontaktováním jeho aktuálního partnera.</span><span class="sxs-lookup"><span data-stu-id="26e88-132">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="26e88-133">Společnost by měla shromáždit název a doménu společnosti aktuálního partnera, aby budoucí partner mohl formulář žádosti o převod vyplnit jejich jménem.</span><span class="sxs-lookup"><span data-stu-id="26e88-133">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="26e88-134">Zákazník musí také identifikovat předplatná, která chtějí převést od svého aktuálního partnera.</span><span class="sxs-lookup"><span data-stu-id="26e88-134">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="26e88-135">Nemůžete měnit partnery pro předplatná Office 365, Enterprise Mobility Suite ani Microsoft Dynamics CRM.</span><span class="sxs-lookup"><span data-stu-id="26e88-135">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="26e88-136">Za dokončení formuláře žádosti o převod, který zahájí proces převodu, zodpovídá budoucí partner.</span><span class="sxs-lookup"><span data-stu-id="26e88-136">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="26e88-137">Microsoft nemůže jednat jménem zákazníka ani aktuálního partnera.</span><span class="sxs-lookup"><span data-stu-id="26e88-137">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="26e88-138">Zákazník by měl naplánovat úzkou spolupráci se svým budoucím a aktuálním partnerem, aby přechod plynule fungoval.</span><span class="sxs-lookup"><span data-stu-id="26e88-138">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="26e88-139">Budoucí úkoly partnerů, které se budou provádět</span><span class="sxs-lookup"><span data-stu-id="26e88-139">Future partner tasks to be completed</span></span>

<span data-ttu-id="26e88-140">Budoucí partner předplatného musí vyplnit formulář žádosti o převod od Partnerské centrum požádat o převod předplatného:</span><span class="sxs-lookup"><span data-stu-id="26e88-140">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="26e88-141">V Partnerské centrum vyberte Zákazníci a pak vyberte zákazníka, za nějž chcete formulář žádosti o převod vyplnit.</span><span class="sxs-lookup"><span data-stu-id="26e88-141">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="26e88-142">V nabídce zákazník vyberte **předplatná**.</span><span class="sxs-lookup"><span data-stu-id="26e88-142">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="26e88-143">Vyberte část **žádost o přenos** .</span><span class="sxs-lookup"><span data-stu-id="26e88-143">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="26e88-144">V **části žádost o přenos** vyberte **Přidat novou žádost**.</span><span class="sxs-lookup"><span data-stu-id="26e88-144">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Oddíl transfery":::

5.  <span data-ttu-id="26e88-146">Vyplňte formulář **nové žádosti o přenos** .</span><span class="sxs-lookup"><span data-stu-id="26e88-146">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="26e88-147">Vyberte odeslat **žádost o odeslání žádosti o přenos**  >  .</span><span class="sxs-lookup"><span data-stu-id="26e88-147">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Formulář žádosti o dokončení přenosu":::

7.  <span data-ttu-id="26e88-149">Kontrola potvrzení žádosti o přenos</span><span class="sxs-lookup"><span data-stu-id="26e88-149">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Kontrola probíhajícího přenosu":::

    >[!Note]
    ><span data-ttu-id="26e88-151">Budoucí partner může žádost o přenos zrušit tak, že v pravém horním rohu vybere možnost **zrušit žádost** jenom v případě, že stav žádosti o přenos čeká na vyřízení.</span><span class="sxs-lookup"><span data-stu-id="26e88-151">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="26e88-152">Jakmile je stav požadavku na přenos "probíhá" nebo "dokončeno", zrušení nebudou možné.</span><span class="sxs-lookup"><span data-stu-id="26e88-152">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="26e88-153">Aktuální úkoly partnerského serveru, které se mají dokončit</span><span class="sxs-lookup"><span data-stu-id="26e88-153">Current partner tasks to be completed</span></span>

<span data-ttu-id="26e88-154">Agent pro správce aktuálního partnera dostane e-mail, že zákazník požaduje přenos svých předplatných:</span><span class="sxs-lookup"><span data-stu-id="26e88-154">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Opakování":::

<span data-ttu-id="26e88-156">Pokud chcete dokončit přenos předplatného, přečtěte si a přijměte formulář žádosti o přenos z partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="26e88-156">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="26e88-157">Pokud aktuální partner neprovede žádnou akci během 30 dnů, vyprší platnost žádosti a budoucí partner bude mít k dispozici vytvoření nové žádosti o přenos.</span><span class="sxs-lookup"><span data-stu-id="26e88-157">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="26e88-158">Vyberte **zkontrolovat žádost o přenos** z e-MAILu nebo</span><span class="sxs-lookup"><span data-stu-id="26e88-158">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="26e88-159">V nabídce partnerské Centrum vyberte **zákazníci** a pak vyberte zákazníka, kterému byla odeslána žádost o přenos jménem.</span><span class="sxs-lookup"><span data-stu-id="26e88-159">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="26e88-160">V nabídce zákazník vyberte **předplatná**.</span><span class="sxs-lookup"><span data-stu-id="26e88-160">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="26e88-161">Vyberte část **žádost o přenos** .</span><span class="sxs-lookup"><span data-stu-id="26e88-161">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="26e88-162">Rozbalte informace o přenosu výběrem zvoleného **ID žádosti o přenos** v části **přijaté požadavky** .</span><span class="sxs-lookup"><span data-stu-id="26e88-162">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Žádost o převod zdrojových recenzí":::

5.  <span data-ttu-id="26e88-164">Zkontrolujte žádost o převod.</span><span class="sxs-lookup"><span data-stu-id="26e88-164">Review transfer request.</span></span> <span data-ttu-id="26e88-165">Vyberte požadovaná předplatná Azure, která chcete převést.</span><span class="sxs-lookup"><span data-stu-id="26e88-165">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="26e88-166">Než budete pokračovat, mějte na vědomí, že už nebudete mít přístup k vybraným předplatným.</span><span class="sxs-lookup"><span data-stu-id="26e88-166">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="26e88-167">Další využití se vám nebude fakturovat.</span><span class="sxs-lookup"><span data-stu-id="26e88-167">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="26e88-168">Rezervace Azure se nepřenesou s předplatným.</span><span class="sxs-lookup"><span data-stu-id="26e88-168">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="26e88-169">Pak **výběrem přijmout a přenést** proces převodu dokončete.</span><span class="sxs-lookup"><span data-stu-id="26e88-169">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Výběr předplatných, která se budou převést v rámci vašich plánů Azure":::

7.  <span data-ttu-id="26e88-171">Zobrazení potvrzení přijetí převodu</span><span class="sxs-lookup"><span data-stu-id="26e88-171">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="26e88-172">V tomto okamžiku bude budoucí partner, zákazník a aktuální partner upozorněni na přijatou žádost o převod e-mailem.</span><span class="sxs-lookup"><span data-stu-id="26e88-172">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="26e88-173">Po přijetí přechodu může stav přenosu během aktualizace systému zůstat až 15 minut ve stavu Čeká na vyřízení.</span><span class="sxs-lookup"><span data-stu-id="26e88-173">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="26e88-174">Pokud to trvá déle, systém to bude zkoušet tři dny.</span><span class="sxs-lookup"><span data-stu-id="26e88-174">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="26e88-175">Pokud stav převodu stále zůstává ve stavu Čeká na vyřízení, partner by měl odeslat žádost o služby.</span><span class="sxs-lookup"><span data-stu-id="26e88-175">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="26e88-176">Po dokončení převodu se předplatná zahrnutá v žádosti zobrazí v plánu Azure budoucího partnera a už nebudou uvedená u vás.</span><span class="sxs-lookup"><span data-stu-id="26e88-176">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="26e88-177">Nepřímí poskytovatelé: Informujte svého nepřímého prodejce, že žádost o převod byla přijata.</span><span class="sxs-lookup"><span data-stu-id="26e88-177">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="26e88-178">Správa převedených zákaznických předplatných</span><span class="sxs-lookup"><span data-stu-id="26e88-178">Managing your transferred customer subscriptions</span></span>

- <span data-ttu-id="26e88-179">Převod nebude mít vliv na přístup ke stávajícím uživatelům, skupinám nebo instančním objektům přiděleným pomocí řízení přístupu na základě role v Azure (RBAC).</span><span class="sxs-lookup"><span data-stu-id="26e88-179">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="26e88-180">Řízení přístupu na základě role v Azure [(Azure RBAC)](/azure/role-based-access-control/overview) pomáhá zákazníkům spravovat, kdo má přístup k prostředkům Azure, co může s těmito prostředky dělat a k jakým oblastem má přístup.</span><span class="sxs-lookup"><span data-stu-id="26e88-180">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="26e88-181">Jako nový partner nemáte po převodu předplatného žádný přístup RBAC k prostředkům zákazníka.</span><span class="sxs-lookup"><span data-stu-id="26e88-181">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="26e88-182">Předchozí partner vašeho zákazníka si zachová přístup RBAC.</span><span class="sxs-lookup"><span data-stu-id="26e88-182">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="26e88-183">Spolupracujte se zákazníkem, abyste pochopili, kdo má přehled o svých předplatných a jak provádět požadované změny.</span><span class="sxs-lookup"><span data-stu-id="26e88-183">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="26e88-184">V důsledku toho je důležité, aby váš zákazník odebral přístup k Azure RBAC pro svého předchozího partnera a přidal přístup pro nového partnera.</span><span class="sxs-lookup"><span data-stu-id="26e88-184">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="26e88-185">Další informace o zákazníkovi, který poskytuje nový přístup, najdete v tématu [co je řízení přístupu na základě role Azure (Azure RBAC)?](/azure/role-based-access-control/overview)</span><span class="sxs-lookup"><span data-stu-id="26e88-185">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="26e88-186">Další informace o tom, jak zákazník odebírá přístup k organizaci RBAC z předchozího partnera, najdete v tématu [Odebrání přiřazení role](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span><span class="sxs-lookup"><span data-stu-id="26e88-186">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="26e88-187">K vašemu předplatnému navíc nezískáte automaticky oprávnění [správce (administrate)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) .</span><span class="sxs-lookup"><span data-stu-id="26e88-187">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="26e88-188">ADMINISTRATE je nutné, aby partneři spravovali svoje předplatná Azure na svých zákaznících jménem.</span><span class="sxs-lookup"><span data-stu-id="26e88-188">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="26e88-189">Další informace o oprávněních Azure najdete v tématu [získání oprávnění ke správě služby nebo předplatného zákazníka.](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="26e88-189">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="26e88-190">Další kroky:</span><span class="sxs-lookup"><span data-stu-id="26e88-190">Next steps:</span></span>

- [<span data-ttu-id="26e88-191">(Azure RBAC)</span><span class="sxs-lookup"><span data-stu-id="26e88-191">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="26e88-192">Získejte oprávnění ke správě služby nebo předplatného zákazníka.</span><span class="sxs-lookup"><span data-stu-id="26e88-192">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
