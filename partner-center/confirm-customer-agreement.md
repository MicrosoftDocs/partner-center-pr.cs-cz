---
title: Jak potvrdit, že zákazník přijal Smlouva se zákazníkem Microsoftu programu CSP
description: Cloud Solution Provider (CSP) musí před objednání zákazníků potvrdit přijetí podmínek Smlouva se zákazníkem Microsoftu zákazníkem služby Microsoft zákazníka.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: c75f129ae5a0755833462138f60901cc7ff36732
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148512"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a><span data-ttu-id="2b987-103">Jak potvrdit, že zákazník přijal Smlouva se zákazníkem Microsoftu programu CSP</span><span class="sxs-lookup"><span data-stu-id="2b987-103">How to confirm that your customer has accepted the Microsoft Customer Agreement to the CSP program</span></span>

<span data-ttu-id="2b987-104">**Odpovídající role:** Agent pro správu | Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="2b987-104">**Appropriate roles**: Admin agent | Sales agent</span></span>


<span data-ttu-id="2b987-105">Zákazníci mají dvě možnosti, jak přijmou Smlouva se zákazníkem Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="2b987-105">Customers have two options for how they accept the Microsoft Customer Agreement.</span></span>

<span data-ttu-id="2b987-106">**Možnost 1:** Ověření souhlasu partnera se zákazníkem – Partner může potvrdit přijetí u zákazníka pomocí Partnerské centrum API nebo sady SDK nebo prostřednictvím řídicího panelu Partnerské centrum serveru.</span><span class="sxs-lookup"><span data-stu-id="2b987-106">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="2b987-107">**Možnost 2:** Přímé přijetí zákazníkem – Partner může pozvat zákazníka prostřednictvím adresy URL a zkontrolovat a přijmout smlouvu v centru Microsoft 365 pro správu.</span><span class="sxs-lookup"><span data-stu-id="2b987-107">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="2b987-108">Šablona Smlouva se zákazníkem Microsoftu přístupu</span><span class="sxs-lookup"><span data-stu-id="2b987-108">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="2b987-109">Nejnovější verzi této šablony si můžete Smlouva se zákazníkem Microsoftu stáhnout [tady.](https://aka.ms/customeragreement)</span><span class="sxs-lookup"><span data-stu-id="2b987-109">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="2b987-110">Tento Smlouva se zákazníkem Microsoftu je specifický pro jednotlivé země.</span><span class="sxs-lookup"><span data-stu-id="2b987-110">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="2b987-111">Při Smlouva se zákazníkem Microsoftu šablony aplikace nezapomeňte vybrat správnou zemi na základě polohy zákazníka.</span><span class="sxs-lookup"><span data-stu-id="2b987-111">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="2b987-112">Možnost 1: Potvrzení přijetí zákazníkem v Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="2b987-112">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="2b987-113">Partneři s přímým vyúčtováním mohou potvrdit souhlas zákazníka s Smlouva se zákazníkem Microsoftu v Partnerské centrum pro nové i stávající zákazníky.</span><span class="sxs-lookup"><span data-stu-id="2b987-113">Direct bill partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="2b987-114">Nepřímí prodejci nemohou provést ověření jménem svých zákazníků a potřebují spolupracovat se svým nepřímým poskytovatelem na dokončení ověření identity.</span><span class="sxs-lookup"><span data-stu-id="2b987-114">Indirect resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="2b987-115">Potvrzení souhlasu zákazníka s novými zákazníky</span><span class="sxs-lookup"><span data-stu-id="2b987-115">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="2b987-116">Když vytvoříte nového tenanta zákazníka v Partnerské centrum, pomocí následujících kroků potvrďte souhlas zákazníka s Smlouva se zákazníkem Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="2b987-116">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="2b987-117">K provedení těchto kroků musíte být agentem pro správu nebo agentem Sales.</span><span class="sxs-lookup"><span data-stu-id="2b987-117">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="2b987-118">Vyberte **Customers (Zákazníci)** a pak **New customer (Nový zákazník).**</span><span class="sxs-lookup"><span data-stu-id="2b987-118">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="2b987-119">V **části Informace o** účtu zadejte informace o společnosti a jejím primárním kontaktu.</span><span class="sxs-lookup"><span data-stu-id="2b987-119">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="2b987-120">V části **smlouva Microsoft** zaškrtněte políčko s potvrzením, že zákazník přijal zákaznickou smlouvu Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="2b987-120">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="2b987-121">V části **Datum přijetí smlouvy** zadejte příslušné datum.</span><span class="sxs-lookup"><span data-stu-id="2b987-121">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="2b987-122">Tuto hodnotu nelze nastavit na budoucí datum.</span><span class="sxs-lookup"><span data-stu-id="2b987-122">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="2b987-123">Ujistěte se, že se zobrazují správné kontaktní informace uživatele.</span><span class="sxs-lookup"><span data-stu-id="2b987-123">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="2b987-124">Pokud je nesprávná, vyberte **aktualizovat** a zadejte přesné informace pro osobu, která smlouvu přijala.</span><span class="sxs-lookup"><span data-stu-id="2b987-124">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="2b987-125">Kliknutím na tlačítko **Další** pokračujte v vytváření tenanta zákazníka.</span><span class="sxs-lookup"><span data-stu-id="2b987-125">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Nový zákazník":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="2b987-127">Potvrďte přijetí zákazníky u stávajících zákazníků</span><span class="sxs-lookup"><span data-stu-id="2b987-127">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="2b987-128">K tomu musíte být agentem správce nebo agent pro prodej:</span><span class="sxs-lookup"><span data-stu-id="2b987-128">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="2b987-129">Vyberte **Zákazníci**.</span><span class="sxs-lookup"><span data-stu-id="2b987-129">Select **Customers**.</span></span> <span data-ttu-id="2b987-130">Vyhledejte a vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="2b987-130">Find and select the customer.</span></span>

2. <span data-ttu-id="2b987-131">Vyberte **informace o účtu**.</span><span class="sxs-lookup"><span data-stu-id="2b987-131">Select **Account info**.</span></span>

3. <span data-ttu-id="2b987-132">V části **Zákaznická smlouva Microsoftu** vyberte **aktualizovat**.</span><span class="sxs-lookup"><span data-stu-id="2b987-132">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="2b987-133">Zadejte **jméno**, **příjmení**, **e-mailovou adresu** a **telefonní číslo** (nepovinné) osoby, která smlouvu přijala.</span><span class="sxs-lookup"><span data-stu-id="2b987-133">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="2b987-134">V části **Datum přijetí smlouvy** zadejte příslušné datum.</span><span class="sxs-lookup"><span data-stu-id="2b987-134">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="2b987-135">Tuto hodnotu nelze nastavit na budoucí datum.</span><span class="sxs-lookup"><span data-stu-id="2b987-135">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="2b987-136">Vyberte **Uložit** a pokračovat.</span><span class="sxs-lookup"><span data-stu-id="2b987-136">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="Stávající zákazník":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="2b987-138">Načíst potvrzení přijetí u zákazníka</span><span class="sxs-lookup"><span data-stu-id="2b987-138">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="2b987-139">Pokud chcete načíst potvrzení, že stávající zákazník přijal smlouvu o zákaznících Microsoftu, postupujte podle následujících kroků.</span><span class="sxs-lookup"><span data-stu-id="2b987-139">To retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement, use the following steps.</span></span> <span data-ttu-id="2b987-140">K tomu musíte být agentem správce nebo agentem pro prodej.</span><span class="sxs-lookup"><span data-stu-id="2b987-140">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="2b987-141">Vyberte **zákazníci** a pak vyhledejte a vyberte zákazníka, kterého chcete zobrazit.</span><span class="sxs-lookup"><span data-stu-id="2b987-141">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="2b987-142">Vyberte **informace o účtu**.</span><span class="sxs-lookup"><span data-stu-id="2b987-142">Select **Account info**.</span></span>

3. <span data-ttu-id="2b987-143">V části **Smlouva o zákaznících Microsoftu** se zobrazí potvrzení, jestli ho zákazník zadal nebo neposkytl.</span><span class="sxs-lookup"><span data-stu-id="2b987-143">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="2b987-144">Potvrzení přijetí zákazníkovi pomocí rozhraní API pro partnerské centrum a sady SDK</span><span class="sxs-lookup"><span data-stu-id="2b987-144">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="2b987-145">Pomocí rozhraní API a sady SDK partnerského centra můžete potvrdit přijetí smlouvy o zákaznících Microsoftu v rámci zákazníka.</span><span class="sxs-lookup"><span data-stu-id="2b987-145">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="2b987-146">Podrobnosti o rozhraní API nebo sadě SDK najdete v tématu:</span><span class="sxs-lookup"><span data-stu-id="2b987-146">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="2b987-147">Získání metadat smluv pro Smlouvu se zákazníkem Microsoftu</span><span class="sxs-lookup"><span data-stu-id="2b987-147">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="2b987-148">Potvrzení přijetí Smlouvy se zákazníkem Microsoftu ze strany zákazníka</span><span class="sxs-lookup"><span data-stu-id="2b987-148">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="2b987-149">Získání potvrzení přijetí Smlouvy se zákazníkem Microsoftu ze strany zákazníka</span><span class="sxs-lookup"><span data-stu-id="2b987-149">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="2b987-150">Získat odkaz ke stažení pro šablonu zákaznických smluv Microsoftu</span><span class="sxs-lookup"><span data-stu-id="2b987-150">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="2b987-151">Možnost 2: přijetí zákazníkem v centru pro správu Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="2b987-151">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="2b987-152">Partneři můžou pozvat nové a stávající zákazníky přes adresu URL, aby si tuto smlouvu zkontrolovali a přijali v rámci centra pro správu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2b987-152">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="2b987-153">V následujících částech se dozvíte, jak:</span><span class="sxs-lookup"><span data-stu-id="2b987-153">The next few sections show you how to:</span></span>

- <span data-ttu-id="2b987-154">Vytvořte nového zákazníka a pozvěte zákazníka, aby smlouvu zkontroloval a přijal.</span><span class="sxs-lookup"><span data-stu-id="2b987-154">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="2b987-155">Pozvěte nového zákazníka, aby zkontroloval a přijal vztah prodejce a smlouvu.</span><span class="sxs-lookup"><span data-stu-id="2b987-155">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="2b987-156">Pozvání stávajícího zákazníka ke kontrole a přijetí smlouvy.</span><span class="sxs-lookup"><span data-stu-id="2b987-156">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="2b987-157">Pomocí [rozhraní API a sady SDK pro partnery](/partner-center/develop/get-direct-sign-status-of-customer-agreement) můžete získat stav přímého přijetí smlouvy o zákaznících Microsoftu od zákazníka.</span><span class="sxs-lookup"><span data-stu-id="2b987-157">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="2b987-158">Vytvoření nového zákazníka a pozvání zákazníka ke kontrole a přijetí smlouvy</span><span class="sxs-lookup"><span data-stu-id="2b987-158">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="2b987-159">Pomocí následujících kroků můžete vytvořit nového zákazníka v partnerském centru a pak je pozvat k revizi a přijetí smlouvy o zákaznících Microsoftu v rámci centra pro správu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2b987-159">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="2b987-160">Na kartě **zákazníci** v partnerském centru vyberte **Přidat zákazníka**.</span><span class="sxs-lookup"><span data-stu-id="2b987-160">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="2b987-161">V části **informace o účtu** zadejte informace o novém zákazníkovi ve všech povinných polích, včetně názvu společnosti zákazníka a primárního kontaktu.</span><span class="sxs-lookup"><span data-stu-id="2b987-161">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="2b987-162">V části **smlouva se zákazníkem** vyberte **Zákazník se žádost o přijetí smlouvy o zákaznících Microsoftu v centru pro správu Microsoft 365**.</span><span class="sxs-lookup"><span data-stu-id="2b987-162">Under **Customer Agreement**, select **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="2b987-163">Vyplňte všechna další povinná pole na stránce.</span><span class="sxs-lookup"><span data-stu-id="2b987-163">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="2b987-164">Vyberte **Další: Zkontrolujte** a pokračujte postupem vytvoření tenanta zákazníka.</span><span class="sxs-lookup"><span data-stu-id="2b987-164">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="2b987-165">Noví zákazníci si nemůžou koupit nákup, dokud nepřijmou zákaznickou smlouvu Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="2b987-165">New customers cannot make a purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Vytvořit nového zákazníka":::

5. <span data-ttu-id="2b987-167">Až se dostanete na obrazovku pro **potvrzení** v pracovním postupu nový zákazník, uložte přihlašovací údaje zákazníka.</span><span class="sxs-lookup"><span data-stu-id="2b987-167">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="2b987-168">Tyto přihlašovací údaje budete muset později poskytnout zákazníkovi.</span><span class="sxs-lookup"><span data-stu-id="2b987-168">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="2b987-169">Mimo partnerské Centrum vytvořte a odešlete e-mail, který vyzývá zákazníka, aby přijal zákaznickou smlouvu Microsoftu v centru pro správu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2b987-169">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="2b987-170">Nezapomeňte zahrnout tyto položky do e-mailu:</span><span class="sxs-lookup"><span data-stu-id="2b987-170">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="2b987-171">Odkaz na tuto [adresu URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (vyžaduje se přihlášení)</span><span class="sxs-lookup"><span data-stu-id="2b987-171">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="2b987-172">Přihlašovací údaje zákazníka, které jste uložili v kroku 5.</span><span class="sxs-lookup"><span data-stu-id="2b987-172">The customer's credentials that you saved in Step 5.</span></span>

7. <span data-ttu-id="2b987-173">Zákazník pak obdrží pozvánku e-mailu od partnera a vybere [adresu URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="2b987-173">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="2b987-174">Zákazník se přihlásí do centra pro správu Microsoft 365 pomocí zadaných přihlašovacích údajů zákazníka.</span><span class="sxs-lookup"><span data-stu-id="2b987-174">The customer signs into Microsoft 365 Admin Center using the customer credentials you provided.</span></span>

9. <span data-ttu-id="2b987-175">Zákazník zkontroluje pole, aby přijal zákaznickou smlouvu od Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="2b987-175">The customer checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="2b987-176">Pozvání nového zákazníka ke kontrole a přijetí vztahu prodejce a smlouvy o zákaznících Microsoftu</span><span class="sxs-lookup"><span data-stu-id="2b987-176">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="2b987-177">Pomocí následujícího postupu můžete pozvat nového zákazníka ke kontrole a přijetí vztahu prodejce a smlouvy o zákaznících Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="2b987-177">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="2b987-178">Na kartě **zákazníci** v partnerském centru vyberte odkaz **požádat o vztah prodejce** .</span><span class="sxs-lookup"><span data-stu-id="2b987-178">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="2b987-179">Automaticky se vytvoří šablona e-mailu, včetně textu a parametrizované adresy URL, která zákazníka přesměruje na centrum pro správu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2b987-179">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="2b987-180">Můžete přizpůsobit automaticky vygenerovanou šablonu e-mailu a pak vybrat **Kopírovat do schránky** nebo **otevřít v e-mailu**.</span><span class="sxs-lookup"><span data-stu-id="2b987-180">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="2b987-181">Tato e-mailová šablona slouží k pozvání zákazníka k přijetí žádosti o **vztah prodejce** a **smlouvy o zákaznících Microsoftu**.</span><span class="sxs-lookup"><span data-stu-id="2b987-181">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="2b987-182">(Poznámka: v pozvánce k e-mailu zajistěte, aby partner zahrnoval taky adresu URL, která se automaticky zadala, a také přihlašovací údaje zákazníka, které se nedávno vytvořily.)</span><span class="sxs-lookup"><span data-stu-id="2b987-182">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="Vytvoření relace":::

5. <span data-ttu-id="2b987-184">Zákazník obdrží pozvánku prostřednictvím e-mailu a klikne na parametrizovanou adresu URL.</span><span class="sxs-lookup"><span data-stu-id="2b987-184">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="2b987-185">Zákazník používá přihlašovací údaje, které poskytnete v e-mailu pro přihlášení do centra pro správu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2b987-185">Customer uses credentials you provide within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="2b987-186">Zákazník zkontroluje pole, aby přijal **vztah prodejce** a **Zákaznickou smlouvu od Microsoftu**.</span><span class="sxs-lookup"><span data-stu-id="2b987-186">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="2b987-187">V rámci stejné adresy URL je zákazník schopný zobrazit konsolidovaný seznam různých partnerů, se kterými pracují.</span><span class="sxs-lookup"><span data-stu-id="2b987-187">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="2b987-188">Pokud si chcete zobrazit podrobnosti, můžete vybrat partnera.</span><span class="sxs-lookup"><span data-stu-id="2b987-188">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="Přijetí smlouvy":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="2b987-190">Pozvání stávajícího zákazníka ke kontrole a přijetí smlouvy</span><span class="sxs-lookup"><span data-stu-id="2b987-190">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="2b987-191">Pomocí následujících kroků můžete pozvat stávajícího zákazníka, aby zkontroloval a přijal zákaznickou smlouvu Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="2b987-191">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="2b987-192">Vytvořte e-mail zákazníka s vloženou adresou URL, která vyzývá zákazníka, aby přijal zákaznickou smlouvu Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="2b987-192">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="2b987-193">Váš zákazník obdrží pozvánku prostřednictvím e-mailu a klikne na [adresu URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="2b987-193">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="2b987-194">Zákazník zadá své přihlašovací údaje do centra pro správu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2b987-194">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="2b987-195">Zákazník toto políčko přijme, aby přijal zákaznickou smlouvu od Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="2b987-195">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="2b987-196">V rámci stejné adresy URL může zákazník zobrazit konsolidovaný seznam různých partnerů, se kterými pracují.</span><span class="sxs-lookup"><span data-stu-id="2b987-196">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="2b987-197">Pokud si chcete zobrazit podrobnosti, můžete vybrat partnera.</span><span class="sxs-lookup"><span data-stu-id="2b987-197">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="zákazníka":::

>[!NOTE]
><span data-ttu-id="2b987-199">V některých scénářích nemusí zákazníci být schopni zákaznickou smlouvu od Microsoftu přijmout přímo.</span><span class="sxs-lookup"><span data-stu-id="2b987-199">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="2b987-200">Pokud chcete získat další informace o těchto situacích, přečtěte si dva scénáře, kdy potřebujete ověřit jménem zákazníka níže.</span><span class="sxs-lookup"><span data-stu-id="2b987-200">To learn more about these situations, read Two scenarios where you need to attest on behalf of your customer, below.</span></span>

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a><span data-ttu-id="2b987-201">Dva scénáře, kdy potřebujete ověřit jménem zákazníka</span><span class="sxs-lookup"><span data-stu-id="2b987-201">Two scenarios where you need to attest on behalf of your customer</span></span>

<span data-ttu-id="2b987-202">Existují dva scénáře, kdy zákazníci nemusí být schopni přímo přijmout smlouvu o zákaznících Microsoftu v centru pro správu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2b987-202">There are two scenarios where customers may not be able to directly accept the Microsoft Customer Agreement within the Microsoft 365 Admin Center.</span></span>

<span data-ttu-id="2b987-203">**Scénář 1**: stávající zákazník si koupil některý z následujících stávajících partnerských vztahů: nabídky, předplatné softwaru nebo softwaru, rezervované instance nebo plán Azure.</span><span class="sxs-lookup"><span data-stu-id="2b987-203">**Scenario 1**: An existing customer has purchased any of the following through an existing partner relationship: offers, software or software subscriptions, Reserved Instances, or Azure Plan.</span></span> <span data-ttu-id="2b987-204">Zákazník se teď snaží vytvořit nový nákup (kromě automatického obnovování).</span><span class="sxs-lookup"><span data-stu-id="2b987-204">The customer is now attempting to make any new purchase (excluding auto renewal).</span></span> <span data-ttu-id="2b987-205">Když zákazník klikne na adresu URL, obdrží zprávu "kontaktujte svého partnera a potvrďte přijetí smlouvy o zákaznících Microsoftu."</span><span class="sxs-lookup"><span data-stu-id="2b987-205">When that customer clicks the URL, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="2b987-206">**Řešení**: je nutné, abyste byli jménem zákazníka ověřeni.</span><span class="sxs-lookup"><span data-stu-id="2b987-206">**To resolve**: You must attest on behalf of the customer.</span></span>

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Snímek obrazovky se stránkou centra pro správu Microsoft 365 s výzvou, abyste se mohli obrátit na svého partnera a potvrdit přijetí smlouvy o zákaznících Microsoftu.":::

<span data-ttu-id="2b987-208">**Scénář 2**: stávající zákazník si koupil některou z následujících nabídek, předplatných softwaru a softwaru, rezervovaných instancí a plánu Azure.</span><span class="sxs-lookup"><span data-stu-id="2b987-208">**Scenario 2**: An existing customer has purchased any of the following offers, software and software subscriptions, Reserved Instances, and Azure Plan.</span></span> <span data-ttu-id="2b987-209">Zákazník se teď snaží vytvořit nový nákup s novým partnerem.</span><span class="sxs-lookup"><span data-stu-id="2b987-209">The customer is now attempting to make any new purchase with a new partner.</span></span>

<span data-ttu-id="2b987-210">Když zákazník klikne na adresu URL, Microsoft 365 centrum pro správu, aby přijal nový partnerský vztah a smlouvu, obdrží zprávu "kontaktujte svého partnera a potvrďte přijetí smlouvy o zákaznících Microsoftu."</span><span class="sxs-lookup"><span data-stu-id="2b987-210">When the customer clicks the URL to Microsoft 365 Admin Center to accept the new partner relationship and the agreement, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="2b987-211">**Řešení**: je nutné, abyste byli jménem zákazníka ověřeni.</span><span class="sxs-lookup"><span data-stu-id="2b987-211">**To resolve**: You must attest on behalf of the customer.</span></span>  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a><span data-ttu-id="2b987-212">Potvrďte, že zákazník přijal smlouvu.</span><span class="sxs-lookup"><span data-stu-id="2b987-212">Confirm that a customer has accepted the agreement</span></span>

<span data-ttu-id="2b987-213">Pokud se pokusíte vytvořit novou objednávku pro existujícího zákazníka, kterého jste ještě nepotvrzuji, zobrazí se výzva k dokončení potvrzení.</span><span class="sxs-lookup"><span data-stu-id="2b987-213">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="2b987-214">K tomu použijte následující postup.</span><span class="sxs-lookup"><span data-stu-id="2b987-214">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="2b987-215">Zadejte **jméno**, **příjmení**, **e-mailovou adresu** a **telefonní číslo** (nepovinné) uživatele, který smlouvu přijal.</span><span class="sxs-lookup"><span data-stu-id="2b987-215">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="2b987-216">V části **Datum přijetí smlouvy** zadejte příslušné datum.</span><span class="sxs-lookup"><span data-stu-id="2b987-216">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="2b987-217">Tuto hodnotu nelze nastavit na budoucí datum.</span><span class="sxs-lookup"><span data-stu-id="2b987-217">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="2b987-218">Vyberte **Uložit a pokračovat**.</span><span class="sxs-lookup"><span data-stu-id="2b987-218">Select **Save and continue**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="2b987-219">Další kroky</span><span class="sxs-lookup"><span data-stu-id="2b987-219">Next steps</span></span>

- [<span data-ttu-id="2b987-220">Ověření nebo aktualizace informací o profilu společnosti</span><span class="sxs-lookup"><span data-stu-id="2b987-220">Verify or update your company profile information</span></span>](update-your-partner-profile.md)
- [<span data-ttu-id="2b987-221">Smlouvy se zákazníkem Microsoftu (podle oblasti a jazyka)</span><span class="sxs-lookup"><span data-stu-id="2b987-221">Microsoft Customer Agreements (by region, language)</span></span>](Agreements.md)
