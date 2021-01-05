---
title: Převeďte předplatné Azure v rámci plánu Azure na jiného partnera CSP.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se, jak změnit partnera programu Cloud Solution Provider přidružený k předplatným Azure v rámci plánu Azure.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: e792e4af2999924ba8be77ec0517ce56c1db7a27
ms.sourcegitcommit: ed5c873d19f0464cc986fe6e852383cd4280daf6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/05/2021
ms.locfileid: "97893202"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="97a33-103">Přenos předplatných plánu Azure pro zákazníka na jiného partnera</span><span class="sxs-lookup"><span data-stu-id="97a33-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="97a33-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="97a33-104">**Appropriate roles**</span></span>

- <span data-ttu-id="97a33-105">Partneři v programu Cloud Solution Provider (CSP)</span><span class="sxs-lookup"><span data-stu-id="97a33-105">Partners in the Cloud Solution Provider (CSP) program</span></span>

<span data-ttu-id="97a33-106">Tento článek popisuje, jak může zákazník přepnout svoje předplatné Azure v rámci plánu Azure z jednoho Cloud Solution Provider (CSP) na jiný.</span><span class="sxs-lookup"><span data-stu-id="97a33-106">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="97a33-107">Pokud chcete přepnout předplatná Azure pro zákazníka z jiného partnera, postupujte podle těchto kroků.</span><span class="sxs-lookup"><span data-stu-id="97a33-107">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="97a33-108">Oba partneři i zákazník mají postup k dokončení.</span><span class="sxs-lookup"><span data-stu-id="97a33-108">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="97a33-109">Přístup k nástrojům pro přechod mají jenom partneři s přímým fakturačním vztahem a Microsoftem.</span><span class="sxs-lookup"><span data-stu-id="97a33-109">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="97a33-110">Nepřímí prodejci musí spolupracovat s jejich nepřímými poskytovateli pro využití tohoto nástroje pro přechod.</span><span class="sxs-lookup"><span data-stu-id="97a33-110">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="97a33-111">Před využitím tohoto nástroje se zákazník musí nacházet v konverzaci s oběma partnery (aktuální i budoucí).</span><span class="sxs-lookup"><span data-stu-id="97a33-111">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="97a33-112">Aby se zabránilo nejasnostem a záměnám, musí být nutné provést konverzaci v režimu offline.</span><span class="sxs-lookup"><span data-stu-id="97a33-112">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="97a33-113">Kromě toho by měli partneři a zákazníci pochopit tyto požadavky a předpoklady před zahájením přechodu:</span><span class="sxs-lookup"><span data-stu-id="97a33-113">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="97a33-114">**Klíčové důležité pokyny:**</span><span class="sxs-lookup"><span data-stu-id="97a33-114">**Key considerations:**</span></span>

- <span data-ttu-id="97a33-115">Azure Reservations se s předplatným nepřesunou na budoucího partnera</span><span class="sxs-lookup"><span data-stu-id="97a33-115">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="97a33-116">Ceny za CSP pro služby Azure v rámci aktuálního partnera nebudou převedeny</span><span class="sxs-lookup"><span data-stu-id="97a33-116">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="97a33-117">Odpovědnosti podpory pro zákazníka se přesunou na budoucího partnera.</span><span class="sxs-lookup"><span data-stu-id="97a33-117">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="97a33-118">Fakturace a fakturace se přesunou k budoucímu partnerovi v době přenosu.</span><span class="sxs-lookup"><span data-stu-id="97a33-118">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="97a33-119">Přenos z Azure Role-Based Access Control (RBAC) není ovlivněný.</span><span class="sxs-lookup"><span data-stu-id="97a33-119">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="97a33-120">Správce jménem (ADMINISTRATE) se ve výchozím nastavení neudělí budoucímu partnerovi.</span><span class="sxs-lookup"><span data-stu-id="97a33-120">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="97a33-121">Produkty z Marketplace třetích stran se přenesou, dokud produkty nespravují kontrolu nároků na Marketplace.</span><span class="sxs-lookup"><span data-stu-id="97a33-121">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="97a33-122">Neexistují žádné zvláštní slevy ani oblastní omezení.</span><span class="sxs-lookup"><span data-stu-id="97a33-122">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="97a33-123">Produkty nejsou založené na předplatném</span><span class="sxs-lookup"><span data-stu-id="97a33-123">The products are non-subscription based</span></span>
    - <span data-ttu-id="97a33-124">Budoucí partner by měl spolupracovat s vydavatelem, aby se ujistil, že se nachází v seznamu povolených pro nasazení produktu.</span><span class="sxs-lookup"><span data-stu-id="97a33-124">The future partner should work with the publisher to make sure they are on the allow-list for deployment of the product</span></span>
    - <span data-ttu-id="97a33-125">Pokud nejsou splněné všechny tyto podmínky, aby bylo možné přenést produkty z webu Marketplace, je třeba přenášet předplatné Azure a pak znovu koupit produkty z Marketplace novým partnerem.</span><span class="sxs-lookup"><span data-stu-id="97a33-125">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="97a33-126">**Požadavky:**</span><span class="sxs-lookup"><span data-stu-id="97a33-126">**Prerequisites:**</span></span>

- <span data-ttu-id="97a33-127">Zákazník v rámci svého záměru zahájí převod na stávajícího partnera CSP</span><span class="sxs-lookup"><span data-stu-id="97a33-127">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="97a33-128">Budoucí partner CSP spolupracuje se zákazníkem, aby se zajistilo splnění zákaznických potřeb.</span><span class="sxs-lookup"><span data-stu-id="97a33-128">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="97a33-129">Budoucí partner CSP naváže vztah se zákazníkem a koupí plán Azure před zahájením přechodu.</span><span class="sxs-lookup"><span data-stu-id="97a33-129">Future CSP partner establishes a relationship with customer and purchases an Azure plan before the transition begins</span></span>  
- <span data-ttu-id="97a33-130">Zákazník musí podepsat zákaznickou smlouvu Microsoftu s budoucím partnerem CSP.</span><span class="sxs-lookup"><span data-stu-id="97a33-130">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="97a33-131">Budoucí partner CSP musí mít podepsané smlouvy Microsoftu pro použití tohoto nástroje.</span><span class="sxs-lookup"><span data-stu-id="97a33-131">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="97a33-132">Úkoly zákazníků, které se mají dokončit</span><span class="sxs-lookup"><span data-stu-id="97a33-132">Customer tasks to be completed</span></span>

<span data-ttu-id="97a33-133">Aby bylo možné přenést předplatné Azure v rámci plánu Azure, zákazník musí zahájit proces tím, že se spojí se svým aktuálním partnerem.</span><span class="sxs-lookup"><span data-stu-id="97a33-133">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="97a33-134">Měly by shromažďovat název a doménu společnosti aktuálního partnera, aby jejich budoucí partneři mohli dokončit formulář žádosti o přenos svým jménem.</span><span class="sxs-lookup"><span data-stu-id="97a33-134">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="97a33-135">Zákazník musí také identifikovat předplatná, která chtějí přenést z aktuálního partnera.</span><span class="sxs-lookup"><span data-stu-id="97a33-135">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="97a33-136">Nemůžete změnit partnery pro Office 365, Enterprise Mobility Suite nebo Microsoft Dynamics CRM Subscriptions.</span><span class="sxs-lookup"><span data-stu-id="97a33-136">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="97a33-137">Je to budoucí zodpovědnost partnera za účelem vyplnění formuláře žádosti o přenos, který zahájí proces přenosu.</span><span class="sxs-lookup"><span data-stu-id="97a33-137">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="97a33-138">Společnost Microsoft se nemůže zasáhnout jménem zákazníka ani aktuálního partnera.</span><span class="sxs-lookup"><span data-stu-id="97a33-138">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="97a33-139">Zákazník by měl v úmyslu spolupracovat s budoucím a aktuálním partnerem, aby přechod přešel do hladké míry.</span><span class="sxs-lookup"><span data-stu-id="97a33-139">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="97a33-140">Budoucí úkoly partnerských serverů</span><span class="sxs-lookup"><span data-stu-id="97a33-140">Future partner tasks to be completed</span></span>

<span data-ttu-id="97a33-141">Budoucí partner předplatného musí vyplnit formulář žádosti o přenos z partnerského centra, aby vyžádal přenos předplatného:</span><span class="sxs-lookup"><span data-stu-id="97a33-141">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="97a33-142">V nabídce partnerského centra vyberte **zákazníci** a pak vyberte zákazníka, kterému chcete vyplnit formulář žádosti o přenos.</span><span class="sxs-lookup"><span data-stu-id="97a33-142">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="97a33-143">V nabídce zákazník vyberte **předplatná**.</span><span class="sxs-lookup"><span data-stu-id="97a33-143">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="97a33-144">Vyberte část **žádost o přenos** .</span><span class="sxs-lookup"><span data-stu-id="97a33-144">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="97a33-145">V **části žádost o přenos** vyberte **Přidat novou žádost**.</span><span class="sxs-lookup"><span data-stu-id="97a33-145">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Oddíl transfery":::

5.  <span data-ttu-id="97a33-147">Vyplňte formulář **nové žádosti o přenos** .</span><span class="sxs-lookup"><span data-stu-id="97a33-147">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="97a33-148">Vyberte odeslat **žádost o odeslání žádosti o přenos**  >  .</span><span class="sxs-lookup"><span data-stu-id="97a33-148">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Formulář žádosti o dokončení přenosu":::

7.  <span data-ttu-id="97a33-150">Kontrola potvrzení žádosti o přenos</span><span class="sxs-lookup"><span data-stu-id="97a33-150">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Kontrola probíhajícího přenosu":::

    >[!Note]
    ><span data-ttu-id="97a33-152">Budoucí partner může žádost o přenos zrušit tak, že v pravém horním rohu vybere možnost **zrušit žádost** jenom v případě, že stav žádosti o přenos čeká na vyřízení.</span><span class="sxs-lookup"><span data-stu-id="97a33-152">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="97a33-153">Jakmile je stav požadavku na přenos "probíhá" nebo "dokončeno", zrušení nebudou možné.</span><span class="sxs-lookup"><span data-stu-id="97a33-153">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="97a33-154">Aktuální úkoly partnerského serveru, které se mají dokončit</span><span class="sxs-lookup"><span data-stu-id="97a33-154">Current partner tasks to be completed</span></span>

<span data-ttu-id="97a33-155">Agent pro správce aktuálního partnera dostane e-mail, že zákazník požaduje přenos svých předplatných:</span><span class="sxs-lookup"><span data-stu-id="97a33-155">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Opakování":::

<span data-ttu-id="97a33-157">Pokud chcete dokončit přenos předplatného, přečtěte si a přijměte formulář žádosti o přenos z partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="97a33-157">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="97a33-158">Pokud aktuální partner neprovede žádnou akci během 30 dnů, vyprší platnost žádosti a budoucí partner bude mít k dispozici vytvoření nové žádosti o přenos.</span><span class="sxs-lookup"><span data-stu-id="97a33-158">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="97a33-159">Vyberte **zkontrolovat žádost o přenos** z e-MAILu nebo</span><span class="sxs-lookup"><span data-stu-id="97a33-159">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="97a33-160">V nabídce partnerské Centrum vyberte **zákazníci** a pak vyberte zákazníka, kterému byla odeslána žádost o přenos jménem.</span><span class="sxs-lookup"><span data-stu-id="97a33-160">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="97a33-161">V nabídce zákazník vyberte **předplatná**.</span><span class="sxs-lookup"><span data-stu-id="97a33-161">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="97a33-162">Vyberte část **žádost o přenos** .</span><span class="sxs-lookup"><span data-stu-id="97a33-162">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="97a33-163">Rozbalte informace o přenosu výběrem zvoleného **ID žádosti o přenos** v části **přijaté požadavky** .</span><span class="sxs-lookup"><span data-stu-id="97a33-163">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Revize zdrojového kódu požadavek na přenos":::

5.  <span data-ttu-id="97a33-165">Zkontrolujte požadavek na přenos.</span><span class="sxs-lookup"><span data-stu-id="97a33-165">Review transfer request.</span></span> <span data-ttu-id="97a33-166">Vyberte požadovaná předplatná Azure, která chcete přenést.</span><span class="sxs-lookup"><span data-stu-id="97a33-166">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="97a33-167">Než budete pokračovat, nezapomeňte prosím, že už nebudete mít přístup k vybraným předplatným.</span><span class="sxs-lookup"><span data-stu-id="97a33-167">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="97a33-168">Nebudeme vám fakturovat za další využití.</span><span class="sxs-lookup"><span data-stu-id="97a33-168">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="97a33-169">Rezervace Azure se nepřenášejí s předplatnými.</span><span class="sxs-lookup"><span data-stu-id="97a33-169">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="97a33-170">Pak vyberte **přijmout a přenést** a dokončete proces přenosu.</span><span class="sxs-lookup"><span data-stu-id="97a33-170">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Vyberte předplatná, která se mají přenést do vašich plánů Azure.":::

7.  <span data-ttu-id="97a33-172">Zobrazení potvrzení přijetí přenosu.</span><span class="sxs-lookup"><span data-stu-id="97a33-172">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="97a33-173">V tomto okamžiku bude budoucí partner, zákazník a aktuální partner upozorněni na přijatý požadavek na přenos prostřednictvím e-mailu.</span><span class="sxs-lookup"><span data-stu-id="97a33-173">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="97a33-174">Po je tento přechod přijatý až do 15 minut, než se systém aktualizuje, takže stav přenosu může zůstat nedokončený.</span><span class="sxs-lookup"><span data-stu-id="97a33-174">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="97a33-175">Pokud bude trvat déle, systém se postará o tři dny.</span><span class="sxs-lookup"><span data-stu-id="97a33-175">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="97a33-176">Pokud stav přenosu stále ještě čeká na vyřízení, partner by měl odeslat žádost o služby.</span><span class="sxs-lookup"><span data-stu-id="97a33-176">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="97a33-177">Po dokončení přenosu se předplatná obsažená v žádosti zobrazí v plánu Azure budoucího partnera a už se nebude zobrazovat v seznamu.</span><span class="sxs-lookup"><span data-stu-id="97a33-177">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="97a33-178">U nepřímých zprostředkovatelů: Informujte prosím svého nepřímý prodejce o přijetí žádosti o přenos.</span><span class="sxs-lookup"><span data-stu-id="97a33-178">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="97a33-179">Správa přenesených zákaznických předplatných</span><span class="sxs-lookup"><span data-stu-id="97a33-179">Managing your transferred customer subscriptions</span></span>
- <span data-ttu-id="97a33-180">Převod nebude mít vliv na přístup ke stávajícím uživatelům, skupinám nebo instančním objektům přiděleným pomocí řízení přístupu na základě role v Azure (RBAC).</span><span class="sxs-lookup"><span data-stu-id="97a33-180">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="97a33-181">Řízení přístupu na základě role Azure [(Azure RBAC)](/azure/role-based-access-control/overview) pomáhá zákazníkům spravovat, kdo má přístup k prostředkům Azure, co s těmito prostředky může dělat a k jakým oblastem mají přístup.</span><span class="sxs-lookup"><span data-stu-id="97a33-181">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="97a33-182">Jako nový partner jste nedostali přístup k prostředkům vašeho zákazníka po převodu předplatného.</span><span class="sxs-lookup"><span data-stu-id="97a33-182">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="97a33-183">Předchozí partner vašeho zákazníka si zachová přístup RBAC.</span><span class="sxs-lookup"><span data-stu-id="97a33-183">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="97a33-184">Spolupracujte se svým zákazníkem a zjistěte, kdo má ve svých předplatných nějaké informace a jakým způsobem je možné provést požadované změny.</span><span class="sxs-lookup"><span data-stu-id="97a33-184">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="97a33-185">V důsledku toho je důležité, aby váš zákazník odebral přístup k Azure RBAC pro svého předchozího partnera a přidal přístup pro nového partnera.</span><span class="sxs-lookup"><span data-stu-id="97a33-185">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="97a33-186">Další informace o zákazníkovi, který poskytuje nový přístup, najdete v tématu [co je řízení přístupu na základě role Azure (Azure RBAC)?](/azure/role-based-access-control/overview)</span><span class="sxs-lookup"><span data-stu-id="97a33-186">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="97a33-187">Další informace o tom, jak zákazník odebírá přístup k organizaci RBAC z předchozího partnera, najdete v tématu [Odebrání přiřazení role](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span><span class="sxs-lookup"><span data-stu-id="97a33-187">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="97a33-188">K vašemu předplatnému navíc nezískáte automaticky oprávnění [správce (administrate)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) .</span><span class="sxs-lookup"><span data-stu-id="97a33-188">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="97a33-189">ADMINISTRATE je nutné, aby partneři spravovali svoje předplatná Azure na svých zákaznících jménem.</span><span class="sxs-lookup"><span data-stu-id="97a33-189">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="97a33-190">Další informace o oprávněních Azure najdete v tématu [získání oprávnění ke správě služby nebo předplatného zákazníka.](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="97a33-190">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="97a33-191">Další kroky:</span><span class="sxs-lookup"><span data-stu-id="97a33-191">Next steps:</span></span>

- [<span data-ttu-id="97a33-192">(Azure RBAC)</span><span class="sxs-lookup"><span data-stu-id="97a33-192">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="97a33-193">Získejte oprávnění ke správě služby nebo předplatného zákazníka.</span><span class="sxs-lookup"><span data-stu-id="97a33-193">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
