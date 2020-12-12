---
title: Potvrzení souhlasu zákazníka s zákaznickou smlouvou Microsoftu
description: Zjistěte, jak potvrdit přijetí smlouvy o zákaznících Microsoftu v rámci zákazníka. To může být nutné k objednání produktů a služeb společnosti Microsoft pro zákazníky.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/30/2020
ms.openlocfilehash: f2513213bff38a6296832253a13725ff2508f1f8
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354606"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a><span data-ttu-id="3ff6d-104">Aktualizovaná metoda, která potvrdí přijetí zákaznických smluv od Microsoftu</span><span class="sxs-lookup"><span data-stu-id="3ff6d-104">Updated method to confirm customer acceptance of the Microsoft Customer Agreement</span></span>


<span data-ttu-id="3ff6d-105">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="3ff6d-105">**Appropriate roles**</span></span>

- <span data-ttu-id="3ff6d-106">Agent správce</span><span class="sxs-lookup"><span data-stu-id="3ff6d-106">Admin agent</span></span>
- <span data-ttu-id="3ff6d-107">Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="3ff6d-107">Sales agent</span></span>

> [!NOTE]
> <span data-ttu-id="3ff6d-108">Prostředek smlouvy je aktuálně podporovaný partnerským centrem jenom ve veřejném cloudu Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-108">The Agreement resource is currently supported by Partner Center in the Microsoft public cloud only.</span></span> <span data-ttu-id="3ff6d-109">Neplatí pro:</span><span class="sxs-lookup"><span data-stu-id="3ff6d-109">It is not applicable to:</span></span>
> * <span data-ttu-id="3ff6d-110">Partnerské centrum provozovaný společností 21Vianet</span><span class="sxs-lookup"><span data-stu-id="3ff6d-110">Partner Center operated by 21Vianet</span></span>
> * <span data-ttu-id="3ff6d-111">Partnerské centrum pro Microsoft Cloud pro Německo</span><span class="sxs-lookup"><span data-stu-id="3ff6d-111">Partner Center for Microsoft Cloud Germany</span></span>
> * <span data-ttu-id="3ff6d-112">Partnerské centrum pro Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="3ff6d-112">Partner Center for Microsoft Cloud for US Government</span></span>

>[!NOTE]
><span data-ttu-id="3ff6d-113">Od 31. ledna 2020 musí všechny zákazníky, stávající a nové, podepsat nové smlouvy o zákaznících Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-113">As of January 31, 2020, all customers, existing and new, must sign the new Microsoft Customer Agreement.</span></span> <span data-ttu-id="3ff6d-114">Pokud se chcete dozvědět víc, přečtěte si téma potvrzení souhlasu zákazníka s zákaznickou [smlouvou Microsoftu](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="3ff6d-114">To learn more, read [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

<span data-ttu-id="3ff6d-115">Jako partner musíte od zákazníka získat souhlas s zákaznickou smlouvou Microsoftu, abyste mohli objednat produkty a služby Microsoftu pro daného zákazníka.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-115">As a partner, you need to obtain your customer's acceptance of the Microsoft Customer Agreement before you can order Microsoft products and services for that customer.</span></span> <span data-ttu-id="3ff6d-116">Aby lépe pomáhali partnerům plnit požadavky na dodržování předpisů, vyžádá si partneři, aby potvrdili přijetí poskytnutím následujících údajů týkajících se osoby, která smlouvu přijala:</span><span class="sxs-lookup"><span data-stu-id="3ff6d-116">To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing the following details regarding the person who accepted the agreement:</span></span>

- <span data-ttu-id="3ff6d-117">Jméno</span><span class="sxs-lookup"><span data-stu-id="3ff6d-117">First name</span></span>

- <span data-ttu-id="3ff6d-118">Příjmení</span><span class="sxs-lookup"><span data-stu-id="3ff6d-118">Last name</span></span>

- <span data-ttu-id="3ff6d-119">E-mailová adresa</span><span class="sxs-lookup"><span data-stu-id="3ff6d-119">Email address</span></span>

- <span data-ttu-id="3ff6d-120">Telefonní číslo (volitelné)</span><span class="sxs-lookup"><span data-stu-id="3ff6d-120">Phone number (optional)</span></span>

- <span data-ttu-id="3ff6d-121">Datum přijetí</span><span class="sxs-lookup"><span data-stu-id="3ff6d-121">Date of acceptance</span></span>

<span data-ttu-id="3ff6d-122">Zákazníci s přímým přístupem a nepřímými poskytovateli musí potvrdit přijetí smlouvy o zákaznících Microsoftu při vyúčtování prostřednictvím partnerského centra nebo rozhraní API partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-122">Direct bill partners and Indirect Providers must confirm customer acceptance of the Microsoft Customer Agreement when transacting through Partner Center or Partner Center API.</span></span> <span data-ttu-id="3ff6d-123">Potvrzení je *povinné*.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-123">Confirmation is *mandatory*.</span></span>

<span data-ttu-id="3ff6d-124">Pokud pro daného zákazníka není zadáno potvrzení:</span><span class="sxs-lookup"><span data-stu-id="3ff6d-124">If confirmation is not provided for a given customer:</span></span>

- <span data-ttu-id="3ff6d-125">Pro tohoto zákazníka nebudete moct vytvořit nové objednávky.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-125">You won't be able to create new orders for this customer.</span></span>

- <span data-ttu-id="3ff6d-126">Pro tohoto zákazníka nebudete moct změnit počet licencí stávajících předplatných založených na licencích.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-126">You won't be able to change the license count of existing license-based subscriptions for this customer.</span></span>

<span data-ttu-id="3ff6d-127">Potvrzení přijetí zákazníkovi se dá dělat prostřednictvím partnerského centra nebo rozhraní API partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-127">Confirmation of customer acceptance can be done via Partner Center or the Partner Center API.</span></span> <span data-ttu-id="3ff6d-128">K tomu je možné využít rozhraní API partnerského centra, které najdete v následujících tématech:</span><span class="sxs-lookup"><span data-stu-id="3ff6d-128">To do this through the Partner Center API, see the following topics:</span></span>

- [<span data-ttu-id="3ff6d-129">Získat potvrzení souhlasu zákazníka</span><span class="sxs-lookup"><span data-stu-id="3ff6d-129">Get confirmation of customer consent</span></span>](/partner-center/develop/get-confirmation-of-customer-consent)

- [<span data-ttu-id="3ff6d-130">Získat metadata smlouvy</span><span class="sxs-lookup"><span data-stu-id="3ff6d-130">Get agreement metadata</span></span>](/partner-center/develop/get-agreement-metadata)

- [<span data-ttu-id="3ff6d-131">Potvrzení souhlasu zákazníka</span><span class="sxs-lookup"><span data-stu-id="3ff6d-131">Confirm customer consent</span></span>](/partner-center/develop/confirm-customer-consent)

<span data-ttu-id="3ff6d-132">To platí pro produkční prostředí i pro prostředí izolovaného prostoru (sandbox).</span><span class="sxs-lookup"><span data-stu-id="3ff6d-132">This applies to both production and sandbox environments.</span></span>

## <a name="confirm-customer-acceptance-for-a-new-customer"></a><span data-ttu-id="3ff6d-133">Potvrzení přijetí zákazníkovi pro nového zákazníka</span><span class="sxs-lookup"><span data-stu-id="3ff6d-133">Confirm customer acceptance for a new customer</span></span>

<span data-ttu-id="3ff6d-134">Pomocí následujícího postupu potvrďte přijetí zákazníkovi při vytváření nového tenanta zákazníka v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-134">Use the following procedure to confirm customer acceptance while you create a new customer tenant in Partner Center.</span></span> <span data-ttu-id="3ff6d-135">K tomu musíte být agentem správce nebo agentem pro prodej.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-135">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="3ff6d-136">Vyberte **zákazníci** a pak **Nový zákazník** a pak vyberte **informace o účtu**.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-136">Select **Customers**, and then **New customer** and then select **Account info**.</span></span>

2. <span data-ttu-id="3ff6d-137">Zadejte informace o **společnosti** a **primárním kontaktu**.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-137">Enter the information about the **Company** and **Primary contact**.</span></span>

   :::image type="content" source="images/mca/mca1.png" alt-text="Informace o společnosti":::

3. <span data-ttu-id="3ff6d-139">V části **Smlouva o zákaznících Microsoftu** vyberte zákazníka, který **přijal nejnovější zákaznickou smlouvu Microsoftu**.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-139">Under **Microsoft customer agreement**, select **The customer has accepted the latest Microsoft customer agreement**.</span></span>

4. <span data-ttu-id="3ff6d-140">V části **Datum přijetí smlouvy** zadejte příslušné datum.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-140">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="3ff6d-141">Tuto hodnotu nelze nastavit na budoucí datum.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-141">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="3ff6d-142">Zadejte podrobnosti uživatele, který poskytl přijetí.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-142">Enter the details of the user who provided the acceptance.</span></span>

   :::image type="content" source="images/mca/MCA3.png" alt-text="Přidat datum přijetí":::

   <span data-ttu-id="3ff6d-144">Ve výchozím nastavení se zobrazí informace o primárním uživateli kontaktu.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-144">By default, the primary contact user information is displayed.</span></span> <span data-ttu-id="3ff6d-145">Pokud to není správné, vyberte **aktualizovat** a zadejte **jméno,** **příjmení**, **e-mailovou adresu** a \**telefonní číslo* (nepovinné) osoby, která smlouvu přijala.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-145">If this isn't correct, select **Update** and then enter the **First name**, **Last name**, **Email address**, and \**Phone number* (optional) of the person who accepted the agreement.</span></span>

6. <span data-ttu-id="3ff6d-146">Kliknutím na tlačítko **Další** pokračujte podle zbývajících kroků a vytvořte tenanta zákazníka.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-146">Select **Next** to continue with the remaining steps to create the customer tenant.</span></span>

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="3ff6d-147">Potvrzení přijetí zákazníkovi pro existujícího zákazníka</span><span class="sxs-lookup"><span data-stu-id="3ff6d-147">Confirm customer acceptance for an existing customer</span></span>

<span data-ttu-id="3ff6d-148">K tomu musíte být agentem správce nebo agentem pro prodej.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-148">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="3ff6d-149">Vyberte **zákazníci** a pak vyhledejte a vyberte zákazníka, kterého chcete zobrazit.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-149">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="3ff6d-150">Vyberte **informace o účtu**.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-150">Select **Account info**.</span></span>

3. <span data-ttu-id="3ff6d-151">V části **Zákaznická smlouva Microsoftu** vyberte **aktualizovat**.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-151">Under **Microsoft customer agreement**, select **Update**.</span></span>

   :::image type="content" source="images/mca/mca4.png" alt-text="Aktualizace":::

4. <span data-ttu-id="3ff6d-153">Zadejte **jméno**, **příjmení**, **e-mailovou adresu** a **telefonní číslo** (nepovinné) uživatele, který smlouvu přijal.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-153">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

5. <span data-ttu-id="3ff6d-154">V části **Datum přijetí smlouvy** zadejte příslušné datum.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-154">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="3ff6d-155">Tuto hodnotu nelze nastavit na budoucí datum.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-155">You cannot set this to a future date.</span></span>

6. <span data-ttu-id="3ff6d-156">Vyberte **Uložit a pokračovat**.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-156">Select **Save and continue**.</span></span>

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a><span data-ttu-id="3ff6d-157">Potvrdit přijetí zákazníkovi při vytváření nové objednávky pro existujícího zákazníka</span><span class="sxs-lookup"><span data-stu-id="3ff6d-157">Confirm customer acceptance while creating new order for an existing customer</span></span>

<span data-ttu-id="3ff6d-158">Pokud se pokusíte vytvořit novou objednávku pro existujícího zákazníka, kterého jste ještě nepotvrzuji, zobrazí se výzva k dokončení potvrzení.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-158">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="3ff6d-159">K tomu použijte následující postup.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-159">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="3ff6d-160">Zadejte **jméno**, **příjmení**, **e-mailovou adresu** a **telefonní číslo** (nepovinné) uživatele, který smlouvu přijal.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-160">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="3ff6d-161">V části **Datum přijetí smlouvy** zadejte příslušné datum.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-161">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="3ff6d-162">Tuto hodnotu nelze nastavit na budoucí datum.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-162">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="3ff6d-163">Vyberte **Uložit a pokračovat**.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-163">Select **Save and continue**.</span></span>

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="3ff6d-164">Načtení potvrzení přijetí zákazníkovi pro existujícího zákazníka</span><span class="sxs-lookup"><span data-stu-id="3ff6d-164">Retrieve confirmation of customer acceptance for an existing customer</span></span>

<span data-ttu-id="3ff6d-165">Potvrzení přijetí zákazníkovi můžete načíst pro existujícího zákazníka, který jste zadali dříve pomocí níže uvedeného postupu.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-165">You can retrieve confirmation of customer acceptance for an existing customer that you have provided previously using the procedure below.</span></span> <span data-ttu-id="3ff6d-166">K tomu musíte být agentem správce nebo agentem pro prodej.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-166">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="3ff6d-167">Vyberte **zákazníci** a pak vyhledejte a vyberte zákazníka, kterého chcete zobrazit.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-167">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="3ff6d-168">Vyberte **informace o účtu**.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-168">Select **Account info**.</span></span>

3. <span data-ttu-id="3ff6d-169">V části **Smlouva o zákaznících Microsoftu** se zobrazí informace o tom, jestli se pro tohoto zákazníka zadalo potvrzení.</span><span class="sxs-lookup"><span data-stu-id="3ff6d-169">Under **Microsoft customer agreement**, you'll see whether or not confirmation has been provided for this customer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3ff6d-170">Další kroky</span><span class="sxs-lookup"><span data-stu-id="3ff6d-170">Next steps</span></span>

- [<span data-ttu-id="3ff6d-171">Potvrzení souhlasu zákazníka s zákaznickou smlouvou Microsoftu v partnerském programu CSP</span><span class="sxs-lookup"><span data-stu-id="3ff6d-171">Confirm customer acceptance of the Microsoft Customer Agreement in the CSP partner program</span></span>](confirm-customer-agreement.md)

- [<span data-ttu-id="3ff6d-172">Potvrzení souhlasu smlouvy se zákazníkem Microsoftu jménem vašeho zákazníka</span><span class="sxs-lookup"><span data-stu-id="3ff6d-172">Attest acceptance of the Microsoft Customer Agreement on behalf of your customer</span></span>](attest-acceptance-customer-agreement.md)