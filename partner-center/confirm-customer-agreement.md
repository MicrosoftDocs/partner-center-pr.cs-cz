---
title: Jak potvrdit, že zákazník přijal Smlouva se zákazníkem Microsoftu programu CSP
description: Cloud Solution Provider (CSP) musí před objednání zákazníků potvrdit souhlas zákazníka s Smlouva se zákazníkem Microsoftu před služby Microsoft zákazníka.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: 9deebf3d9aab2d4dc7953da67a7eb17078b3d30c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277007"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a><span data-ttu-id="5f5d6-103">Jak potvrdit, že zákazník přijal Smlouva se zákazníkem Microsoftu programu CSP</span><span class="sxs-lookup"><span data-stu-id="5f5d6-103">How to confirm that your customer has accepted the Microsoft Customer Agreement to the CSP program</span></span>

<span data-ttu-id="5f5d6-104">**Odpovídající role:** Agent pro správu | Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="5f5d6-104">**Appropriate roles**: Admin agent | Sales agent</span></span>


<span data-ttu-id="5f5d6-105">Zákazníci mají dvě možnosti, jak přijmou Smlouva se zákazníkem Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-105">Customers have two options for how they accept the Microsoft Customer Agreement.</span></span>

<span data-ttu-id="5f5d6-106">**Možnost 1:** Ověření souhlasu partnera se zákazníkem – Partner může potvrdit přijetí u zákazníka pomocí Partnerské centrum API nebo sady SDK nebo prostřednictvím řídicího panelu Partnerské centrum serveru.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-106">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="5f5d6-107">**Možnost 2:** Přímé přijetí zákazníkem – Partner může pozvat zákazníka prostřednictvím adresy URL a zkontrolovat a přijmout smlouvu v centru Microsoft 365 pro správu.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-107">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="5f5d6-108">Šablona Smlouva se zákazníkem Microsoftu přístupu</span><span class="sxs-lookup"><span data-stu-id="5f5d6-108">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="5f5d6-109">Nejnovější verzi této šablony si můžete Smlouva se zákazníkem Microsoftu stáhnout [tady.](https://aka.ms/customeragreement)</span><span class="sxs-lookup"><span data-stu-id="5f5d6-109">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="5f5d6-110">Tento Smlouva se zákazníkem Microsoftu je specifický pro jednotlivé země.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-110">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="5f5d6-111">Při žádosti Smlouva se zákazníkem Microsoftu šablony aplikace nezapomeňte vybrat správnou zemi na základě polohy zákazníka.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-111">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="5f5d6-112">Možnost 1: Potvrzení přijetí zákazníkem v Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="5f5d6-112">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="5f5d6-113">Partneři s přímým vyúčtováním mohou potvrdit souhlas zákazníka s Smlouva se zákazníkem Microsoftu v Partnerské centrum pro nové i stávající zákazníky.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-113">Direct bill partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="5f5d6-114">Nepřímí prodejci nemohou provést ověření jménem svých zákazníků a potřebují spolupracovat se svým nepřímým poskytovatelem na dokončení ověření identity.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-114">Indirect resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="5f5d6-115">Potvrzení souhlasu zákazníka s novými zákazníky</span><span class="sxs-lookup"><span data-stu-id="5f5d6-115">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="5f5d6-116">Když vytvoříte nového tenanta zákazníka v Partnerské centrum, pomocí následujících kroků potvrďte souhlas zákazníka s Smlouva se zákazníkem Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-116">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="5f5d6-117">K provedení těchto kroků musíte být agentem pro správu nebo agentem Sales.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-117">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="5f5d6-118">Vyberte **Customers (Zákazníci)** a pak **New customer (Nový zákazník).**</span><span class="sxs-lookup"><span data-stu-id="5f5d6-118">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="5f5d6-119">V **části Informace o** účtu zadejte informace o společnosti a jejím primárním kontaktu.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-119">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="5f5d6-120">V **části Smlouva s Microsoftem** zaškrtněte políčko pro testování, že zákazník přijal Smlouva se zákazníkem Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-120">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="5f5d6-121">V **části Datum přijetí smlouvy** zadejte příslušné datum.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-121">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="5f5d6-122">Tuto možnost nelze nastavit na budoucí datum.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-122">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="5f5d6-123">Ujistěte se, že jsou zobrazené primární kontaktní informace uživatele správné.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-123">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="5f5d6-124">Pokud je nesprávný, vyberte **Aktualizovat a** zadejte přesné informace pro osobu, která smlouvu přijala.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-124">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="5f5d6-125">Výběrem **možnosti** Další pokračujte ve vytváření tenanta zákazníka.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-125">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Nový zákazník.":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="5f5d6-127">Potvrzení přijetí u stávajících zákazníků zákazníkem</span><span class="sxs-lookup"><span data-stu-id="5f5d6-127">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="5f5d6-128">K tomu musíte být agentem pro správu nebo agentem Sales:</span><span class="sxs-lookup"><span data-stu-id="5f5d6-128">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="5f5d6-129">Vyberte **Zákazníci**.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-129">Select **Customers**.</span></span> <span data-ttu-id="5f5d6-130">Vyhledejte a vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-130">Find and select the customer.</span></span>

2. <span data-ttu-id="5f5d6-131">Vyberte **Informace o účtu.**</span><span class="sxs-lookup"><span data-stu-id="5f5d6-131">Select **Account info**.</span></span>

3. <span data-ttu-id="5f5d6-132">V **Smlouva se zákazníkem Microsoftu** vyberte **Aktualizovat.**</span><span class="sxs-lookup"><span data-stu-id="5f5d6-132">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="5f5d6-133">Zadejte **jméno, příjmení,** **e-mailovou adresu** a telefonní číslo **(volitelné)** osoby, která smlouvu přijala. </span><span class="sxs-lookup"><span data-stu-id="5f5d6-133">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="5f5d6-134">V **části Datum přijetí smlouvy** zadejte příslušné datum.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-134">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="5f5d6-135">Tuto možnost nelze nastavit na budoucí datum.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-135">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="5f5d6-136">Vyberte **Uložit a** pokračovat.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-136">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="Stávající zákazník.":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="5f5d6-138">Načtení potvrzení přijetí zákazníkem</span><span class="sxs-lookup"><span data-stu-id="5f5d6-138">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="5f5d6-139">Pokud chcete načíst potvrzení, že stávající zákazník Smlouva se zákazníkem Microsoftu, použijte následující postup.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-139">To retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement, use the following steps.</span></span> <span data-ttu-id="5f5d6-140">K tomu musíte být agentem pro správu nebo agentem Sales.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-140">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="5f5d6-141">Vyberte **Zákazníci** a pak vyhledejte a vyberte zákazníka, kterého chcete zobrazit.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-141">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="5f5d6-142">Vyberte **Informace o účtu.**</span><span class="sxs-lookup"><span data-stu-id="5f5d6-142">Select **Account info**.</span></span>

3. <span data-ttu-id="5f5d6-143">V **části Smlouva se zákazníkem Microsoftu** zobrazte, jestli zákazník neposkytl nebo neposkytl potvrzení.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-143">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="5f5d6-144">Potvrzení přijetí zákazníkem pomocí Partnerské centrum API nebo SDK</span><span class="sxs-lookup"><span data-stu-id="5f5d6-144">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="5f5d6-145">Pomocí rozhraní API Partnerské centrum SDK můžete potvrdit souhlas zákazníka s Smlouva se zákazníkem Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-145">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="5f5d6-146">Podrobnosti o rozhraní API nebo sadě SDK najdete zde:</span><span class="sxs-lookup"><span data-stu-id="5f5d6-146">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="5f5d6-147">Získání metadat smluv pro Smlouvu se zákazníkem Microsoftu</span><span class="sxs-lookup"><span data-stu-id="5f5d6-147">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="5f5d6-148">Potvrzení přijetí Smlouvy se zákazníkem Microsoftu ze strany zákazníka</span><span class="sxs-lookup"><span data-stu-id="5f5d6-148">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="5f5d6-149">Získání potvrzení přijetí Smlouvy se zákazníkem Microsoftu ze strany zákazníka</span><span class="sxs-lookup"><span data-stu-id="5f5d6-149">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="5f5d6-150">Získání odkazu ke stažení Smlouva se zákazníkem Microsoftu šablony</span><span class="sxs-lookup"><span data-stu-id="5f5d6-150">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="5f5d6-151">Možnost 2: Přijetí zákazníkem v Microsoft 365 admin Center</span><span class="sxs-lookup"><span data-stu-id="5f5d6-151">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="5f5d6-152">Partneři mohou prostřednictvím adresy URL pozvat nové a stávající zákazníky, aby smlouvu mohli zkontrolovat a přijmout v Microsoft 365 pro správu.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-152">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="5f5d6-153">V následujících několika částech si ukážeme, jak:</span><span class="sxs-lookup"><span data-stu-id="5f5d6-153">The next few sections show you how to:</span></span>

- <span data-ttu-id="5f5d6-154">Vytvořte nového zákazníka a požádejte ho, aby smlouvu zkontrolovat a přijmout.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-154">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="5f5d6-155">Pozvěte nového zákazníka, aby přezval a přijal vztah a smlouvu na prodejci.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-155">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="5f5d6-156">Pozvěte existujícího zákazníka, aby smlouvu zkontrolovat a přijmout.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-156">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="5f5d6-157">Pomocí Partnerské centrum [API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) můžete získat stav přímého přijetí požadavku zákazníkem Smlouva se zákazníkem Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-157">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="5f5d6-158">Vytvoření nového zákazníka a pozvání zákazníka ke kontrola a přijetí smlouvy</span><span class="sxs-lookup"><span data-stu-id="5f5d6-158">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="5f5d6-159">Pomocí následujícího postupu vytvořte nového zákazníka v Partnerské centrum a pak ho pozvěte ke kontrola a přijetí tohoto Smlouva se zákazníkem Microsoftu v Microsoft 365 pro správu.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-159">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="5f5d6-160">Na kartě **Zákazníci** v Partnerské centrum vyberte **Přidat zákazníka.**</span><span class="sxs-lookup"><span data-stu-id="5f5d6-160">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="5f5d6-161">V **části Informace o** účtu zadejte informace o novém zákazníkovi do všech požadovaných polí, včetně názvu společnosti zákazníka a primárního kontaktu.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-161">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="5f5d6-162">V **části Customer Agreement**(Smlouva se zákazníkem) vyberte Customer (Zákazník) a přijměte Smlouva se zákazníkem Microsoftu v Microsoft 365 Admin **Center.**</span><span class="sxs-lookup"><span data-stu-id="5f5d6-162">Under **Customer Agreement**, select **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="5f5d6-163">Vyplňte všechna další povinná pole na stránce.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-163">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="5f5d6-164">Vyberte **Další: Projděte si** postup vytvoření tenanta zákazníka.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-164">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="5f5d6-165">Noví zákazníci nemohou provést nákup, dokud nepřijme Smlouva se zákazníkem Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-165">New customers cannot make a purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Vytvořte nového zákazníka.":::

5. <span data-ttu-id="5f5d6-167">Když se v pracovním postupu nového zákazníka dostanete na obrazovku **Potvrzení,** uložte si přihlašovací údaje zákazníka.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-167">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="5f5d6-168">Tyto přihlašovací údaje budete muset zákazníkovi poskytnout později.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-168">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="5f5d6-169">Mimo tuto Partnerské centrum vytvořte a odešlete e-mail, který pozve zákazníka, aby přijal Smlouva se zákazníkem Microsoftu v Microsoft 365 pro správu.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-169">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="5f5d6-170">Nezapomeňte do e-mailu zahrnout tyto položky:</span><span class="sxs-lookup"><span data-stu-id="5f5d6-170">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="5f5d6-171">Odkaz na tuto adresu [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (vyžaduje se přihlášení)</span><span class="sxs-lookup"><span data-stu-id="5f5d6-171">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="5f5d6-172">Přihlašovací údaje zákazníka, které jste si uložili v kroku 5.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-172">The customer's credentials that you saved in Step 5.</span></span>

7. <span data-ttu-id="5f5d6-173">Zákazník pak obdrží e-mailovou pozvánku od partnera a vybere adresu [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="5f5d6-173">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="5f5d6-174">Zákazník se přihlásí k Microsoft 365 pro správu pomocí přihlašovacích údajů zákazníka, které jste poskytli.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-174">The customer signs into Microsoft 365 Admin Center using the customer credentials you provided.</span></span>

9. <span data-ttu-id="5f5d6-175">Zákazník zaškrtnutím políčka přijme smlouvu se zákazníkem Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-175">The customer checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="5f5d6-176">Požádejte nového zákazníka, aby zkontrolovat a přijmout vztah prodejce a Smlouva se zákazníkem Microsoftu</span><span class="sxs-lookup"><span data-stu-id="5f5d6-176">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="5f5d6-177">Pomocí následujícího postupu pozvěte nového zákazníka, aby si prohlédněte a přijal vztah prodejce a Smlouva se zákazníkem Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-177">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="5f5d6-178">Na kartě **Zákazníci** v Partnerské centrum odkaz **Požádat o vztah prodejce.**</span><span class="sxs-lookup"><span data-stu-id="5f5d6-178">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="5f5d6-179">Vygeneruje se automatická e-mailová šablona, včetně textu a parametrizované adresy URL, která přesměruje zákazníka do Microsoft 365 správce.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-179">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="5f5d6-180">Můžete přizpůsobit automaticky vygenerované e-mailové šablony a pak vybrat **Zkopírovat do schránky** nebo **Otevřít v e-mailu.**</span><span class="sxs-lookup"><span data-stu-id="5f5d6-180">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="5f5d6-181">Pomocí této e-mailové šablony můžete zákazníka pozvat, aby přijal žádost o vztah **prodejce,** **a Smlouva se zákazníkem Microsoftu**.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-181">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="5f5d6-182">(Poznámka: V e-mailové pozvánce se ujistěte, že partner obsahuje také automaticky zadanou adresu URL a také nedávno vytvořené přihlašovací údaje zákazníka.)</span><span class="sxs-lookup"><span data-stu-id="5f5d6-182">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="vytvořte relaci.":::

5. <span data-ttu-id="5f5d6-184">Zákazník obdrží pozvánku e-mailem a klikne na parametrizovanou adresu URL.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-184">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="5f5d6-185">Zákazník se pomocí přihlašovacích údajů, které poskytnete v e-mailu, Microsoft 365 centru pro správu.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-185">Customer uses credentials you provide within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="5f5d6-186">Zákazník zaškrtnutím políčka přijme vztah **prodejce a** **Smlouva se zákazníkem Microsoftu**.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-186">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="5f5d6-187">V rámci stejné adresy URL může zákazník zobrazit konsolidovaný seznam různých partnerů, se kterou pracuje.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-187">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="5f5d6-188">Mohou vybrat partnera a zobrazit podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-188">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="Přijměte smlouvu.":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="5f5d6-190">Pozvání existujícího zákazníka ke kontrola a přijetí smlouvy</span><span class="sxs-lookup"><span data-stu-id="5f5d6-190">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="5f5d6-191">Pomocí následujícího postupu můžete pozvat stávajícího zákazníka, aby si tyto požadavky Smlouva se zákazníkem Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-191">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="5f5d6-192">Vytvořte e-mail zákazníka s vloženou adresou URL, která pozve zákazníka k přijetí Smlouva se zákazníkem Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-192">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="5f5d6-193">Zákazník obdrží pozvánku e-mailem a klikne na adresu [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="5f5d6-193">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="5f5d6-194">Zákazník zadá své přihlašovací údaje do Microsoft 365 admin Center.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-194">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="5f5d6-195">Zákazník zaškrtnutím políčka přijme Smlouva se zákazníkem Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-195">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="5f5d6-196">V rámci stejné adresy URL může zákazník zobrazit konsolidovaný seznam různých partnerů, se které pracují.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-196">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="5f5d6-197">Mohou vybrat partnera a zobrazit podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-197">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Zákazníka.":::

>[!NOTE]
><span data-ttu-id="5f5d6-199">V některých scénářích zákazníci nemusí být schopni přímo přijmout Smlouva se zákazníkem Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-199">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="5f5d6-200">Další informace o těchto situacích najdete níže v části Dva scénáře, ve kterých potřebujete pro své zákazníky něco otestovat.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-200">To learn more about these situations, read Two scenarios where you need to attest on behalf of your customer, below.</span></span>

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a><span data-ttu-id="5f5d6-201">Dva scénáře, kdy je potřeba to udělat jménem zákazníka</span><span class="sxs-lookup"><span data-stu-id="5f5d6-201">Two scenarios where you need to attest on behalf of your customer</span></span>

<span data-ttu-id="5f5d6-202">Existují dva scénáře, ve kterých zákazníci nemusí být schopni přímo přijmout Smlouva se zákazníkem Microsoftu v Microsoft 365 admin Center.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-202">There are two scenarios where customers may not be able to directly accept the Microsoft Customer Agreement within the Microsoft 365 Admin Center.</span></span>

<span data-ttu-id="5f5d6-203">**Scénář 1:** Stávající zákazník zakoupil prostřednictvím existujícího partnerského vztahu jakoukoli z následujících možností: nabídky, předplatná softwaru nebo softwaru, rezervované instance nebo plán Azure.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-203">**Scenario 1**: An existing customer has purchased any of the following through an existing partner relationship: offers, software or software subscriptions, Reserved Instances, or Azure Plan.</span></span> <span data-ttu-id="5f5d6-204">Zákazník se teď pokouší provést nový nákup (s výjimkou automatického prodlužování platnosti).</span><span class="sxs-lookup"><span data-stu-id="5f5d6-204">The customer is now attempting to make any new purchase (excluding auto renewal).</span></span> <span data-ttu-id="5f5d6-205">Když zákazník klikne na adresu URL, zobrazí se zpráva "Kontaktujte svého partnera a potvrďte přijetí tohoto Smlouva se zákazníkem Microsoftu."</span><span class="sxs-lookup"><span data-stu-id="5f5d6-205">When that customer clicks the URL, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="5f5d6-206">**Pokud chcete** tento problém vyřešit: Musíte to protestovat jménem zákazníka.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-206">**To resolve**: You must attest on behalf of the customer.</span></span>

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Snímek obrazovky Microsoft 365 stránce Centra pro správu s dotazem, jestli chcete kontaktovat svého partnera a potvrdit přijetí Smlouva se zákazníkem Microsoftu":::

<span data-ttu-id="5f5d6-208">**Scénář 2:** Stávající zákazník zakoupil jakoukoli z následujících nabídek, softwarových a softwarových předplatných, rezervovaných instancí a plánu Azure.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-208">**Scenario 2**: An existing customer has purchased any of the following offers, software and software subscriptions, Reserved Instances, and Azure Plan.</span></span> <span data-ttu-id="5f5d6-209">Zákazník se teď pokouší provést nový nákup s novým partnerem.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-209">The customer is now attempting to make any new purchase with a new partner.</span></span>

<span data-ttu-id="5f5d6-210">Když zákazník klikne na adresu URL centra pro správu Microsoft 365 přijme nový partnerský vztah Microsoft 365 smlouvu, zobrazí se zpráva "Obraťte se na svého partnera a potvrďte souhlas s Smlouva se zákazníkem Microsoftu".</span><span class="sxs-lookup"><span data-stu-id="5f5d6-210">When the customer clicks the URL to Microsoft 365 Admin Center to accept the new partner relationship and the agreement, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="5f5d6-211">**Pokud chcete** tento problém vyřešit: Musíte to protestovat jménem zákazníka.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-211">**To resolve**: You must attest on behalf of the customer.</span></span>  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a><span data-ttu-id="5f5d6-212">Potvrzení, že zákazník přijal smlouvu</span><span class="sxs-lookup"><span data-stu-id="5f5d6-212">Confirm that a customer has accepted the agreement</span></span>

<span data-ttu-id="5f5d6-213">Pokud se pokusíte vytvořit novou objednávku pro stávajícího zákazníka, u které jste to ještě nepotvrdili, zobrazí se výzva k dokončení potvrzení.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-213">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="5f5d6-214">Použijte k tomu následující postup.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-214">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="5f5d6-215">Zadejte **jméno, příjmení,** **e-mailovou adresu** a telefonní číslo **(volitelné)** uživatele, který smlouvu přijal. </span><span class="sxs-lookup"><span data-stu-id="5f5d6-215">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="5f5d6-216">V **části Datum přijetí smlouvy** zadejte příslušné datum.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-216">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="5f5d6-217">Tuto možnost nelze nastavit na budoucí datum.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-217">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="5f5d6-218">Vyberte **Uložit a pokračovat**.</span><span class="sxs-lookup"><span data-stu-id="5f5d6-218">Select **Save and continue**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="5f5d6-219">Další kroky</span><span class="sxs-lookup"><span data-stu-id="5f5d6-219">Next steps</span></span>

- [<span data-ttu-id="5f5d6-220">Ověření nebo aktualizace informací o profilu společnosti</span><span class="sxs-lookup"><span data-stu-id="5f5d6-220">Verify or update your company profile information</span></span>](update-your-partner-profile.md)
- [<span data-ttu-id="5f5d6-221">Smlouvy se zákazníkem Microsoftu (podle oblasti a jazyka)</span><span class="sxs-lookup"><span data-stu-id="5f5d6-221">Microsoft Customer Agreements (by region, language)</span></span>](Agreements.md)
