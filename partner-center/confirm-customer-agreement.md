---
title: Jak ověřit, že zákazník přijal do programu CSP zákaznickou smlouvu Microsoftu
description: Partneři poskytovatele Cloud Solution Provider (CSP) musí před objednáním služeb Microsoft pro zákazníky potvrdit přijetí smlouvy se zákazníkem Microsoftu.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: ebb52a3a8223d3b1101e3a8e78728fcc167e25e3
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633774"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a><span data-ttu-id="e5d30-103">Jak ověřit, že zákazník přijal do programu CSP zákaznickou smlouvu Microsoftu</span><span class="sxs-lookup"><span data-stu-id="e5d30-103">How to confirm that your customer has accepted the Microsoft Customer Agreement to the CSP program</span></span>

<span data-ttu-id="e5d30-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="e5d30-104">**Appropriate roles**</span></span>

- <span data-ttu-id="e5d30-105">Agent správce</span><span class="sxs-lookup"><span data-stu-id="e5d30-105">Admin agent</span></span>
- <span data-ttu-id="e5d30-106">Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="e5d30-106">Sales agent</span></span>


<span data-ttu-id="e5d30-107">Zákazníci mají dvě možnosti, jak přijmou zákaznickou smlouvu Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="e5d30-107">Customers have two options for how they accept the Microsoft Customer Agreement.</span></span>

<span data-ttu-id="e5d30-108">**Možnost 1**: ověření partnerského serveru pro přijetí u zákazníka – partner může potvrdit přijetí zákazníkovi pomocí rozhraní API pro partnerské centrum a sady SDK nebo prostřednictvím řídicího panelu partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="e5d30-108">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="e5d30-109">**Možnost 2**: přímé přijetí zákazníkem – partner může pozvat zákazníka přes adresu URL, aby si tuto smlouvu zkontroloval a přijal v centru pro správu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e5d30-109">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="e5d30-110">Přístup k šabloně zákaznických smluv Microsoftu</span><span class="sxs-lookup"><span data-stu-id="e5d30-110">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="e5d30-111">Nejnovější verzi šablony zákaznických smluv od Microsoftu si můžete stáhnout [ručně.](https://aka.ms/customeragreement)</span><span class="sxs-lookup"><span data-stu-id="e5d30-111">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="e5d30-112">Smlouva o zákaznících Microsoftu je specifická pro danou zemi.</span><span class="sxs-lookup"><span data-stu-id="e5d30-112">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="e5d30-113">Při požadavku na šablonu smlouvy o zákaznících Microsoftu nezapomeňte vybrat správnou zemi na základě umístění zákazníka.</span><span class="sxs-lookup"><span data-stu-id="e5d30-113">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="e5d30-114">Možnost 1: potvrzení přijetí zákazníkem v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="e5d30-114">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="e5d30-115">Partneři s přímým účtováním můžou potvrdit přijetí smlouvy o zákaznících Microsoftu v partnerském centru pro zákazníky, kteří mají nové a stávající zákazníky.</span><span class="sxs-lookup"><span data-stu-id="e5d30-115">Direct bill partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="e5d30-116">Nepřímí prodejci nemůžou v zastoupení svých zákazníků ověřit platnost a při provádění ověření identity musí spolupracovat s jejich nepřímým zprostředkovatelem.</span><span class="sxs-lookup"><span data-stu-id="e5d30-116">Indirect resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="e5d30-117">Potvrďte přijetí zákazníkovi pro nové zákazníky</span><span class="sxs-lookup"><span data-stu-id="e5d30-117">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="e5d30-118">Při vytváření nového tenanta zákazníka v partnerském centru použijte následující postup k potvrzení souhlasu zákazníka s zákaznickou smlouvou Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="e5d30-118">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="e5d30-119">K provedení těchto kroků musíte být agentem správce nebo prodejní agent.</span><span class="sxs-lookup"><span data-stu-id="e5d30-119">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="e5d30-120">Vyberte **zákazníci** a pak **Nový zákazník**.</span><span class="sxs-lookup"><span data-stu-id="e5d30-120">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="e5d30-121">V části **informace o účtu** zadejte informace pro společnost a její primární kontakt.</span><span class="sxs-lookup"><span data-stu-id="e5d30-121">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="e5d30-122">V části **smlouva Microsoft** zaškrtněte políčko s potvrzením, že zákazník přijal zákaznickou smlouvu Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="e5d30-122">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="e5d30-123">V části **Datum přijetí smlouvy** zadejte příslušné datum.</span><span class="sxs-lookup"><span data-stu-id="e5d30-123">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="e5d30-124">Tuto hodnotu nelze nastavit na budoucí datum.</span><span class="sxs-lookup"><span data-stu-id="e5d30-124">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="e5d30-125">Ujistěte se, že se zobrazují správné kontaktní informace uživatele.</span><span class="sxs-lookup"><span data-stu-id="e5d30-125">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="e5d30-126">Pokud je nesprávná, vyberte **aktualizovat** a zadejte přesné informace pro osobu, která smlouvu přijala.</span><span class="sxs-lookup"><span data-stu-id="e5d30-126">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="e5d30-127">Kliknutím na tlačítko **Další** pokračujte v vytváření tenanta zákazníka.</span><span class="sxs-lookup"><span data-stu-id="e5d30-127">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Nový zákazník":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="e5d30-129">Potvrďte přijetí zákazníky u stávajících zákazníků</span><span class="sxs-lookup"><span data-stu-id="e5d30-129">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="e5d30-130">K tomu musíte být agentem správce nebo agent pro prodej:</span><span class="sxs-lookup"><span data-stu-id="e5d30-130">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="e5d30-131">Vyberte **Zákazníci**.</span><span class="sxs-lookup"><span data-stu-id="e5d30-131">Select **Customers**.</span></span> <span data-ttu-id="e5d30-132">Vyhledejte a vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="e5d30-132">Find and select the customer.</span></span>

2. <span data-ttu-id="e5d30-133">Vyberte **informace o účtu**.</span><span class="sxs-lookup"><span data-stu-id="e5d30-133">Select **Account info**.</span></span>

3. <span data-ttu-id="e5d30-134">V části **Zákaznická smlouva Microsoftu** vyberte **aktualizovat**.</span><span class="sxs-lookup"><span data-stu-id="e5d30-134">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="e5d30-135">Zadejte **jméno**, **příjmení**, **e-mailovou adresu** a **telefonní číslo** (nepovinné) osoby, která smlouvu přijala.</span><span class="sxs-lookup"><span data-stu-id="e5d30-135">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="e5d30-136">V části **Datum přijetí smlouvy** zadejte příslušné datum.</span><span class="sxs-lookup"><span data-stu-id="e5d30-136">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="e5d30-137">Tuto hodnotu nelze nastavit na budoucí datum.</span><span class="sxs-lookup"><span data-stu-id="e5d30-137">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="e5d30-138">Vyberte **Uložit** a pokračovat.</span><span class="sxs-lookup"><span data-stu-id="e5d30-138">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="Stávající zákazník":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="e5d30-140">Načíst potvrzení přijetí u zákazníka</span><span class="sxs-lookup"><span data-stu-id="e5d30-140">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="e5d30-141">Pokud chcete načíst potvrzení, že stávající zákazník přijal smlouvu o zákaznících Microsoftu, postupujte podle následujících kroků.</span><span class="sxs-lookup"><span data-stu-id="e5d30-141">To retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement, use the following steps.</span></span> <span data-ttu-id="e5d30-142">K tomu musíte být agentem správce nebo agentem pro prodej.</span><span class="sxs-lookup"><span data-stu-id="e5d30-142">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="e5d30-143">Vyberte **zákazníci** a pak vyhledejte a vyberte zákazníka, kterého chcete zobrazit.</span><span class="sxs-lookup"><span data-stu-id="e5d30-143">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="e5d30-144">Vyberte **informace o účtu**.</span><span class="sxs-lookup"><span data-stu-id="e5d30-144">Select **Account info**.</span></span>

3. <span data-ttu-id="e5d30-145">V části **Smlouva o zákaznících Microsoftu** se zobrazí potvrzení, jestli ho zákazník zadal nebo neposkytl.</span><span class="sxs-lookup"><span data-stu-id="e5d30-145">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="e5d30-146">Potvrzení přijetí zákazníkovi pomocí rozhraní API pro partnerské centrum a sady SDK</span><span class="sxs-lookup"><span data-stu-id="e5d30-146">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="e5d30-147">Pomocí rozhraní API a sady SDK partnerského centra můžete potvrdit přijetí smlouvy o zákaznících Microsoftu v rámci zákazníka.</span><span class="sxs-lookup"><span data-stu-id="e5d30-147">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="e5d30-148">Podrobnosti o rozhraní API nebo sadě SDK najdete v tématu:</span><span class="sxs-lookup"><span data-stu-id="e5d30-148">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="e5d30-149">Získání metadat smluv pro Smlouvu se zákazníkem Microsoftu</span><span class="sxs-lookup"><span data-stu-id="e5d30-149">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="e5d30-150">Potvrzení přijetí Smlouvy se zákazníkem Microsoftu ze strany zákazníka</span><span class="sxs-lookup"><span data-stu-id="e5d30-150">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="e5d30-151">Získání potvrzení přijetí Smlouvy se zákazníkem Microsoftu ze strany zákazníka</span><span class="sxs-lookup"><span data-stu-id="e5d30-151">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="e5d30-152">Získat odkaz ke stažení pro šablonu zákaznických smluv Microsoftu</span><span class="sxs-lookup"><span data-stu-id="e5d30-152">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="e5d30-153">Možnost 2: přijetí zákazníkem v centru pro správu Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="e5d30-153">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="e5d30-154">Partneři můžou pozvat nové a stávající zákazníky přes adresu URL, aby si tuto smlouvu zkontrolovali a přijali v rámci centra pro správu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e5d30-154">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="e5d30-155">V následujících částech se dozvíte, jak:</span><span class="sxs-lookup"><span data-stu-id="e5d30-155">The next few sections show you how to:</span></span>

- <span data-ttu-id="e5d30-156">Vytvořte nového zákazníka a pozvěte zákazníka, aby smlouvu zkontroloval a přijal.</span><span class="sxs-lookup"><span data-stu-id="e5d30-156">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="e5d30-157">Pozvěte nového zákazníka, aby zkontroloval a přijal vztah prodejce a smlouvu.</span><span class="sxs-lookup"><span data-stu-id="e5d30-157">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="e5d30-158">Pozvání stávajícího zákazníka ke kontrole a přijetí smlouvy.</span><span class="sxs-lookup"><span data-stu-id="e5d30-158">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="e5d30-159">Pomocí [rozhraní API a sady SDK pro partnery](/partner-center/develop/get-direct-sign-status-of-customer-agreement) můžete získat stav přímého přijetí smlouvy o zákaznících Microsoftu od zákazníka.</span><span class="sxs-lookup"><span data-stu-id="e5d30-159">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="e5d30-160">Vytvoření nového zákazníka a pozvání zákazníka ke kontrole a přijetí smlouvy</span><span class="sxs-lookup"><span data-stu-id="e5d30-160">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="e5d30-161">Pomocí následujících kroků můžete vytvořit nového zákazníka v partnerském centru a pak je pozvat k revizi a přijetí smlouvy o zákaznících Microsoftu v rámci centra pro správu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e5d30-161">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="e5d30-162">Na kartě **zákazníci** v partnerském centru vyberte **Přidat zákazníka**.</span><span class="sxs-lookup"><span data-stu-id="e5d30-162">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="e5d30-163">V části **informace o účtu** zadejte informace o novém zákazníkovi ve všech povinných polích, včetně názvu společnosti zákazníka a primárního kontaktu.</span><span class="sxs-lookup"><span data-stu-id="e5d30-163">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="e5d30-164">V části **smlouva se zákazníkem** vyberte **Zákazník se žádost o přijetí smlouvy o zákaznících Microsoftu v centru pro správu Microsoft 365**.</span><span class="sxs-lookup"><span data-stu-id="e5d30-164">Under **Customer Agreement**, select **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="e5d30-165">Vyplňte všechna další povinná pole na stránce.</span><span class="sxs-lookup"><span data-stu-id="e5d30-165">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="e5d30-166">Vyberte **Další: Zkontrolujte** a pokračujte postupem vytvoření tenanta zákazníka.</span><span class="sxs-lookup"><span data-stu-id="e5d30-166">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="e5d30-167">Noví zákazníci si nemůžou koupit nákup, dokud nepřijmou zákaznickou smlouvu Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="e5d30-167">New customers cannot make a purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Vytvořit nového zákazníka":::

5. <span data-ttu-id="e5d30-169">Až se dostanete na obrazovku pro **potvrzení** v pracovním postupu nový zákazník, uložte přihlašovací údaje zákazníka.</span><span class="sxs-lookup"><span data-stu-id="e5d30-169">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="e5d30-170">Tyto přihlašovací údaje budete muset později poskytnout zákazníkovi.</span><span class="sxs-lookup"><span data-stu-id="e5d30-170">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="e5d30-171">Mimo partnerské Centrum vytvořte a odešlete e-mail, který vyzývá zákazníka, aby přijal zákaznickou smlouvu Microsoftu v centru pro správu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e5d30-171">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="e5d30-172">Nezapomeňte zahrnout tyto položky do e-mailu:</span><span class="sxs-lookup"><span data-stu-id="e5d30-172">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="e5d30-173">Odkaz na tuto [adresu URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (vyžaduje se přihlášení)</span><span class="sxs-lookup"><span data-stu-id="e5d30-173">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="e5d30-174">Přihlašovací údaje zákazníka, které jste uložili v kroku 5.</span><span class="sxs-lookup"><span data-stu-id="e5d30-174">The customer's credentials that you saved in Step 5.</span></span>

7. <span data-ttu-id="e5d30-175">Zákazník pak obdrží pozvánku e-mailu od partnera a vybere [adresu URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="e5d30-175">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="e5d30-176">Zákazník se přihlásí do centra pro správu Microsoft 365 pomocí zadaných přihlašovacích údajů zákazníka.</span><span class="sxs-lookup"><span data-stu-id="e5d30-176">The customer signs into Microsoft 365 Admin Center using the customer credentials you provided.</span></span>

9. <span data-ttu-id="e5d30-177">Zákazník zkontroluje pole, aby přijal zákaznickou smlouvu od Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="e5d30-177">The customer checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="e5d30-178">Pozvání nového zákazníka ke kontrole a přijetí vztahu prodejce a smlouvy o zákaznících Microsoftu</span><span class="sxs-lookup"><span data-stu-id="e5d30-178">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="e5d30-179">Pomocí následujícího postupu můžete pozvat nového zákazníka ke kontrole a přijetí vztahu prodejce a smlouvy o zákaznících Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="e5d30-179">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="e5d30-180">Na kartě **zákazníci** v partnerském centru vyberte odkaz **požádat o vztah prodejce** .</span><span class="sxs-lookup"><span data-stu-id="e5d30-180">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="e5d30-181">Automaticky se vytvoří šablona e-mailu, včetně textu a parametrizované adresy URL, která zákazníka přesměruje na centrum pro správu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e5d30-181">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="e5d30-182">Můžete přizpůsobit automaticky vygenerovanou šablonu e-mailu a pak vybrat **Kopírovat do schránky** nebo **otevřít v e-mailu**.</span><span class="sxs-lookup"><span data-stu-id="e5d30-182">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="e5d30-183">Tato e-mailová šablona slouží k pozvání zákazníka k přijetí žádosti o **vztah prodejce** a **smlouvy o zákaznících Microsoftu**.</span><span class="sxs-lookup"><span data-stu-id="e5d30-183">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="e5d30-184">(Poznámka: v pozvánce k e-mailu zajistěte, aby partner zahrnoval taky adresu URL, která se automaticky zadala, a také přihlašovací údaje zákazníka, které se nedávno vytvořily.)</span><span class="sxs-lookup"><span data-stu-id="e5d30-184">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="Vytvoření relace":::

5. <span data-ttu-id="e5d30-186">Zákazník obdrží pozvánku prostřednictvím e-mailu a klikne na parametrizovanou adresu URL.</span><span class="sxs-lookup"><span data-stu-id="e5d30-186">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="e5d30-187">Zákazník používá přihlašovací údaje, které poskytnete v e-mailu pro přihlášení do centra pro správu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e5d30-187">Customer uses credentials you provide within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="e5d30-188">Zákazník zkontroluje pole, aby přijal **vztah prodejce** a **Zákaznickou smlouvu od Microsoftu**.</span><span class="sxs-lookup"><span data-stu-id="e5d30-188">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="e5d30-189">V rámci stejné adresy URL je zákazník schopný zobrazit konsolidovaný seznam různých partnerů, se kterými pracují.</span><span class="sxs-lookup"><span data-stu-id="e5d30-189">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="e5d30-190">Pokud si chcete zobrazit podrobnosti, můžete vybrat partnera.</span><span class="sxs-lookup"><span data-stu-id="e5d30-190">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="Přijetí smlouvy":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="e5d30-192">Pozvání stávajícího zákazníka ke kontrole a přijetí smlouvy</span><span class="sxs-lookup"><span data-stu-id="e5d30-192">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="e5d30-193">Pomocí následujících kroků můžete pozvat stávajícího zákazníka, aby zkontroloval a přijal zákaznickou smlouvu Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="e5d30-193">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="e5d30-194">Vytvořte e-mail zákazníka s vloženou adresou URL, která vyzývá zákazníka, aby přijal zákaznickou smlouvu Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="e5d30-194">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="e5d30-195">Váš zákazník obdrží pozvánku prostřednictvím e-mailu a klikne na [adresu URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="e5d30-195">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="e5d30-196">Zákazník zadá své přihlašovací údaje do centra pro správu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e5d30-196">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="e5d30-197">Zákazník toto políčko přijme, aby přijal zákaznickou smlouvu od Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="e5d30-197">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="e5d30-198">V rámci stejné adresy URL může zákazník zobrazit konsolidovaný seznam různých partnerů, se kterými pracují.</span><span class="sxs-lookup"><span data-stu-id="e5d30-198">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="e5d30-199">Pokud si chcete zobrazit podrobnosti, můžete vybrat partnera.</span><span class="sxs-lookup"><span data-stu-id="e5d30-199">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="zákazníka":::

>[!NOTE]
><span data-ttu-id="e5d30-201">V některých scénářích nemusí zákazníci být schopni zákaznickou smlouvu od Microsoftu přijmout přímo.</span><span class="sxs-lookup"><span data-stu-id="e5d30-201">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="e5d30-202">Pokud chcete získat další informace o těchto situacích, přečtěte si dva scénáře, kdy potřebujete ověřit jménem zákazníka níže.</span><span class="sxs-lookup"><span data-stu-id="e5d30-202">To learn more about these situations, read Two scenarios where you need to attest on behalf of your customer, below.</span></span>

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a><span data-ttu-id="e5d30-203">Dva scénáře, kdy potřebujete ověřit jménem zákazníka</span><span class="sxs-lookup"><span data-stu-id="e5d30-203">Two scenarios where you need to attest on behalf of your customer</span></span>

<span data-ttu-id="e5d30-204">Existují dva scénáře, kdy zákazníci nemusí být schopni přímo přijmout smlouvu o zákaznících Microsoftu v centru pro správu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e5d30-204">There are two scenarios where customers may not be able to directly accept the Microsoft Customer Agreement within the Microsoft 365 Admin Center.</span></span>

<span data-ttu-id="e5d30-205">**Scénář 1**: stávající zákazník si koupil některý z následujících stávajících partnerských vztahů: nabídky, předplatné softwaru nebo softwaru, rezervované instance nebo plán Azure.</span><span class="sxs-lookup"><span data-stu-id="e5d30-205">**Scenario 1**: An existing customer has purchased any of the following through an existing partner relationship: offers, software or software subscriptions, Reserved Instances, or Azure Plan.</span></span> <span data-ttu-id="e5d30-206">Zákazník se teď snaží vytvořit nový nákup (kromě automatického obnovování).</span><span class="sxs-lookup"><span data-stu-id="e5d30-206">The customer is now attempting to make any new purchase (excluding auto renewal).</span></span> <span data-ttu-id="e5d30-207">Když zákazník klikne na adresu URL, obdrží zprávu "kontaktujte svého partnera a potvrďte přijetí smlouvy o zákaznících Microsoftu."</span><span class="sxs-lookup"><span data-stu-id="e5d30-207">When that customer clicks the URL, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="e5d30-208">**Řešení**: je nutné, abyste byli jménem zákazníka ověřeni.</span><span class="sxs-lookup"><span data-stu-id="e5d30-208">**To resolve**: You must attest on behalf of the customer.</span></span>

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Snímek obrazovky se stránkou centra pro správu Microsoft 365 s výzvou, abyste se mohli obrátit na svého partnera a potvrdit přijetí smlouvy o zákaznících Microsoftu.":::

<span data-ttu-id="e5d30-210">**Scénář 2**: stávající zákazník si koupil některou z následujících nabídek, předplatných softwaru a softwaru, rezervovaných instancí a plánu Azure.</span><span class="sxs-lookup"><span data-stu-id="e5d30-210">**Scenario 2**: An existing customer has purchased any of the following offers, software and software subscriptions, Reserved Instances, and Azure Plan.</span></span> <span data-ttu-id="e5d30-211">Zákazník se teď snaží vytvořit nový nákup s novým partnerem.</span><span class="sxs-lookup"><span data-stu-id="e5d30-211">The customer is now attempting to make any new purchase with a new partner.</span></span>

<span data-ttu-id="e5d30-212">Když zákazník klikne na adresu URL, Microsoft 365 centrum pro správu, aby přijal nový partnerský vztah a smlouvu, obdrží zprávu "kontaktujte svého partnera a potvrďte přijetí smlouvy o zákaznících Microsoftu."</span><span class="sxs-lookup"><span data-stu-id="e5d30-212">When the customer clicks the URL to Microsoft 365 Admin Center to accept the new partner relationship and the agreement, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="e5d30-213">**Řešení**: je nutné, abyste byli jménem zákazníka ověřeni.</span><span class="sxs-lookup"><span data-stu-id="e5d30-213">**To resolve**: You must attest on behalf of the customer.</span></span>  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a><span data-ttu-id="e5d30-214">Potvrďte, že zákazník přijal smlouvu.</span><span class="sxs-lookup"><span data-stu-id="e5d30-214">Confirm that a customer has accepted the agreement</span></span>

<span data-ttu-id="e5d30-215">Pokud se pokusíte vytvořit novou objednávku pro existujícího zákazníka, kterého jste ještě nepotvrzuji, zobrazí se výzva k dokončení potvrzení.</span><span class="sxs-lookup"><span data-stu-id="e5d30-215">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="e5d30-216">K tomu použijte následující postup.</span><span class="sxs-lookup"><span data-stu-id="e5d30-216">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="e5d30-217">Zadejte **jméno**, **příjmení**, **e-mailovou adresu** a **telefonní číslo** (nepovinné) uživatele, který smlouvu přijal.</span><span class="sxs-lookup"><span data-stu-id="e5d30-217">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="e5d30-218">V části **Datum přijetí smlouvy** zadejte příslušné datum.</span><span class="sxs-lookup"><span data-stu-id="e5d30-218">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="e5d30-219">Tuto hodnotu nelze nastavit na budoucí datum.</span><span class="sxs-lookup"><span data-stu-id="e5d30-219">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="e5d30-220">Vyberte **Uložit a pokračovat**.</span><span class="sxs-lookup"><span data-stu-id="e5d30-220">Select **Save and continue**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="e5d30-221">Další kroky</span><span class="sxs-lookup"><span data-stu-id="e5d30-221">Next steps</span></span>

- [<span data-ttu-id="e5d30-222">Ověření nebo aktualizace informací o profilu společnosti</span><span class="sxs-lookup"><span data-stu-id="e5d30-222">Verify or update your company profile information</span></span>](update-your-partner-profile.md)
- [<span data-ttu-id="e5d30-223">Smlouvy se zákazníkem Microsoftu (podle oblasti a jazyka)</span><span class="sxs-lookup"><span data-stu-id="e5d30-223">Microsoft Customer Agreements (by region, language)</span></span>](Agreements.md)
