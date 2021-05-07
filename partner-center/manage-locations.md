---
title: Správa umístění v partnerském účtu
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Naučte se, jak přidat nové umístění a jak se v programu motivačních programů, v obchodních předplatných, předplatných a dalších transakcích používá umístění MPN ID.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a2b4fa8b204b10d5d45c0e1409ab4bc463e272f
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702888"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="38872-103">Správa umístění účtu MPN a přidání (odstranění) umístění</span><span class="sxs-lookup"><span data-stu-id="38872-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="38872-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="38872-104">**Appropriate roles**</span></span>

- <span data-ttu-id="38872-105">Globální správce</span><span class="sxs-lookup"><span data-stu-id="38872-105">Global admin</span></span>
- <span data-ttu-id="38872-106">Správce účtu</span><span class="sxs-lookup"><span data-stu-id="38872-106">Account admin</span></span>

<span data-ttu-id="38872-107">ID MPN umístění identifikuje každé konkrétní umístění vaší společnosti.</span><span class="sxs-lookup"><span data-stu-id="38872-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="38872-108">K registraci v programu motivačních programů použijete umístění MPN ID, a to za transakčního poskytovatele řešení cloudu (CSP) a další obchodní transakce.</span><span class="sxs-lookup"><span data-stu-id="38872-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="38872-109">Globální ID MPN se používá pro netransakční aktivity, například žádosti o podporu.</span><span class="sxs-lookup"><span data-stu-id="38872-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="38872-110">Typický je následující scénář:</span><span class="sxs-lookup"><span data-stu-id="38872-110">The following scenario is typical:</span></span>

<span data-ttu-id="38872-111">Společnost Contoso má svůj partnerský globální účet (PGA) ve Spojeném království.</span><span class="sxs-lookup"><span data-stu-id="38872-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="38872-112">PGA je jejich registrovaný právní podnik a globální ID MPN se používá ke správě všech netransakčních obchodních činností.</span><span class="sxs-lookup"><span data-stu-id="38872-112">The PGA is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="38872-113">Společnost Contoso má také partnerské účty partnera (PLA) rovnocenné dceřiným společnostem nebo divizím v jiném umístění v USA, Francii a USA.</span><span class="sxs-lookup"><span data-stu-id="38872-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="38872-114">Ve struktuře účtu MPN se tyto PLAs reprezentují jako jedinečná ID MPN.</span><span class="sxs-lookup"><span data-stu-id="38872-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="38872-115">PLAs se používají pro transakční firmy, jako je CSP nebo pobídky programů.</span><span class="sxs-lookup"><span data-stu-id="38872-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="38872-116">Výběry jsou vázané na konkrétní umístění.</span><span class="sxs-lookup"><span data-stu-id="38872-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="38872-117">Mezi klientem CSP a ID umístění MPN je 1-1 vztah.</span><span class="sxs-lookup"><span data-stu-id="38872-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Struktura míst MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="38872-119">Požadavky, aby bylo možné přidat nový účet pro firmu CSP</span><span class="sxs-lookup"><span data-stu-id="38872-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="38872-120">Pokud chcete přidat nový obchodní účet CSP, začněte tím, že ověříte, že jste splnili požadavky.</span><span class="sxs-lookup"><span data-stu-id="38872-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="38872-121">Musíte mít umístění MPN ID v zemi, kde chcete, aby se zprostředkovatel CSP vystavil.</span><span class="sxs-lookup"><span data-stu-id="38872-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="38872-122">Pokud chcete vytvořit nové umístění MPN, přečtěte si níže téma "Přidání umístění MPN".</span><span class="sxs-lookup"><span data-stu-id="38872-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="38872-123">Chcete-li vytvořit nového poskytovatele nepřímých prodejců CSP, přečtěte si téma [práce s nepřímými poskytovateli](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="38872-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="38872-124">Nezapomeňte se přihlásit pomocí **nových** přihlašovacích údajů **nového** účtu CSP.</span><span class="sxs-lookup"><span data-stu-id="38872-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="38872-125">Nepoužívejte svoje stávající přihlašovací údaje, protože Partnerské centrum vám rozpozná, jak už účet máte.</span><span class="sxs-lookup"><span data-stu-id="38872-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="38872-126">Přijměte smlouvu s partnerem Microsoftu a aktivujte účet.</span><span class="sxs-lookup"><span data-stu-id="38872-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="38872-127">Pokud se chcete zaregistrovat jako přímý fakturační Server, [požadavky na čtení pro přímé partnery z fakturace](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="38872-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-and-update-your-mpn-locations"></a><span data-ttu-id="38872-128">Zobrazení a aktualizace umístění MPN</span><span class="sxs-lookup"><span data-stu-id="38872-128">View and update your MPN locations</span></span>

1. <span data-ttu-id="38872-129">Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard/home) partnerského centra s přihlašovacími údaji k účtu MPN.</span><span class="sxs-lookup"><span data-stu-id="38872-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="38872-130">(Vaše přihlašovací údaje programu MPN se můžou lišit od vašich přihlašovacích údajů CSP.)</span><span class="sxs-lookup"><span data-stu-id="38872-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="38872-131">V ikoně **Nastavení** vyberte **Nastavení účtu**, **Profil organizace**, **právní**.</span><span class="sxs-lookup"><span data-stu-id="38872-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="38872-132">Na kartě **partner** ověřte, že se nezobrazí chybová zpráva banneru s výzvou k opravě umístění migrace z PMC.</span><span class="sxs-lookup"><span data-stu-id="38872-132">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="38872-133">Pokud vaše umístění nebyla správně nastavena v PMC a zatím nebyla převedena do počítačů PC, je nutné aktualizovat Tato umístění.</span><span class="sxs-lookup"><span data-stu-id="38872-133">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="Snímek obrazovky videa ukazuje, jak aktualizovat polohu.":::
 
4.  <span data-ttu-id="38872-135">Na obrazovce **zkontrolovat umístění PMC** vyberte **aktualizovat**.</span><span class="sxs-lookup"><span data-stu-id="38872-135">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="38872-136">Aktualizujte následující pole:</span><span class="sxs-lookup"><span data-stu-id="38872-136">Update the following fields:</span></span>

- <span data-ttu-id="38872-137">**Pole Name (název**): Ujistěte se, že název umístění společnosti je správný.</span><span class="sxs-lookup"><span data-stu-id="38872-137">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="38872-138">Pokud se zobrazí duplicitní Chyba, zkuste se změnit z, například contoso na contoso, Inc.</span><span class="sxs-lookup"><span data-stu-id="38872-138">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="38872-139">**Pole právnické osoby**: Ujistěte se, že jste zvolili právnickou entitu, se kterou je umístění svázáno.</span><span class="sxs-lookup"><span data-stu-id="38872-139">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="38872-140">**Řádková adresa 1 & 2 pole**: Ujistěte se, že je adresa správná.</span><span class="sxs-lookup"><span data-stu-id="38872-140">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="38872-141">**Města & země/provincie**: Ujistěte se, že je kombinace mezi městem a okresem správná.</span><span class="sxs-lookup"><span data-stu-id="38872-141">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="38872-142">K dispozici jsou země, kde se použije rozevírací nabídka pro výběr státu nebo provincie, a v ostatních zemích bude nutné ručně vložit pole.</span><span class="sxs-lookup"><span data-stu-id="38872-142">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="38872-143">**PSČ – pole** poštovního směrovacího čísla: Ujistěte se, že pole PSČ odpovídá vaší zadané zemi, oblasti, města nebo adrese.</span><span class="sxs-lookup"><span data-stu-id="38872-143">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="38872-144">**Pole primárních kontaktních informací**: Ujistěte se, že pole jméno a příjmení jsou vyplněna a že e-mailová adresa je pracovní e-mailová adresa, nikoli osobní (například,, @outlook.com @live.com atd.).</span><span class="sxs-lookup"><span data-stu-id="38872-144">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="38872-145">**Pole telefonní číslo**: Ujistěte se, že telefonní číslo neobsahuje speciální znaky, mezery ani kód země.</span><span class="sxs-lookup"><span data-stu-id="38872-145">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="38872-146">Hodnota zadaná v poli telefonní číslo bude vždycky obsahovat maximálně 10 znaků.</span><span class="sxs-lookup"><span data-stu-id="38872-146">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="38872-147">Pokud není k dispozici žádná chybová zpráva, pak z  **Nastavení** vyberte  **Nastavení účtu**, **Profil organizace**, **identifikátory**.</span><span class="sxs-lookup"><span data-stu-id="38872-147">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="38872-148">Vyhledejte ID MPN s typem "umístění", které odpovídá zemi tohoto účtu CSP, a použijte ji k dokončení přidružení.</span><span class="sxs-lookup"><span data-stu-id="38872-148">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="38872-149">Pokud nemůžete najít umístění MPN ID, které odpovídá účtu CSP, který chcete použít, můžete přidat nové umístění, ve kterém se vytvoří nové ID MPN.</span><span class="sxs-lookup"><span data-stu-id="38872-149">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="38872-150">Viz téma **Přidání umístění MPN** níže.</span><span class="sxs-lookup"><span data-stu-id="38872-150">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="38872-151">Přidat umístění MPN</span><span class="sxs-lookup"><span data-stu-id="38872-151">Add an MPN location</span></span>

1. <span data-ttu-id="38872-152">Přihlaste se pomocí účtu MPN v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="38872-152">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="38872-153">(Vaše přihlašovací údaje programu MPN se můžou lišit od vašich přihlašovacích údajů CSP).</span><span class="sxs-lookup"><span data-stu-id="38872-153">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="38872-154">Účet MPN by měl mít oprávnění globálního správce nebo správce účtů.</span><span class="sxs-lookup"><span data-stu-id="38872-154">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="38872-155">V **ikoně nastavení** vyberte **Nastavení účtu** a pak vyberte **Profil organizace**.</span><span class="sxs-lookup"><span data-stu-id="38872-155">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="38872-156">Vyberte možnost **právní** a pak na kartě **partner** vyberte **obchodní umístění** a klikněte na **Přidat umístění.**</span><span class="sxs-lookup"><span data-stu-id="38872-156">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="38872-157">Zadejte požadované podrobnosti, včetně názvu firmy, adresy a kontaktu pro umístění, které chcete přidat do své společnosti.</span><span class="sxs-lookup"><span data-stu-id="38872-157">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="38872-158">Klikněte na **Přidat umístění**.</span><span class="sxs-lookup"><span data-stu-id="38872-158">Click **Add location**.</span></span> <span data-ttu-id="38872-159">Tím se vytvoří nové ID MPN pro nové umístění, které můžete použít pro transakce a pobídky CSP.</span><span class="sxs-lookup"><span data-stu-id="38872-159">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Přidat novou právní firmu":::

> [!NOTE]
> <span data-ttu-id="38872-161">Jakmile je umístění přidané v partnerském centru, nemůžete ho odebrat.</span><span class="sxs-lookup"><span data-stu-id="38872-161">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="38872-162">Pokud jste pro přihlášení použili správné ID **MPN, zobrazí se v levé** nabídce centra pro partnery v nabídce vlevo.</span><span class="sxs-lookup"><span data-stu-id="38872-162">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="add-the-registration-number-id"></a><span data-ttu-id="38872-163">Přidat ID registračního čísla</span><span class="sxs-lookup"><span data-stu-id="38872-163">Add the registration number ID</span></span>

<span data-ttu-id="38872-164">Pokud jste nepřímý poskytovatel, přímý účet pro fakturaci nebo nepřímý prodejce a obchodujete s novými nebo stávajícími zákazníky v následujících zemích, musíte pro svůj podnik zadat registrační čísla ID.</span><span class="sxs-lookup"><span data-stu-id="38872-164">If you are an Indirect provider, Direct bill partner, or Indirect reseller and you are doing business with new or existing customers in the following countries, you need to provide registration ID numbers for your business.</span></span> <span data-ttu-id="38872-165">Pokud země, ve které obchodujete, není uvedená níže, ID registrace je volitelné.</span><span class="sxs-lookup"><span data-stu-id="38872-165">If the country you are doing business in is not listed below, the registration ID is optional.</span></span>

- <span data-ttu-id="38872-166">Arménie</span><span class="sxs-lookup"><span data-stu-id="38872-166">Armenia</span></span> 
- <span data-ttu-id="38872-167">Ázerbájdžán</span><span class="sxs-lookup"><span data-stu-id="38872-167">Azerbaijan</span></span> 
- <span data-ttu-id="38872-168">Bělorusko</span><span class="sxs-lookup"><span data-stu-id="38872-168">Belarus</span></span> 
- <span data-ttu-id="38872-169">Brazílie</span><span class="sxs-lookup"><span data-stu-id="38872-169">Brazil</span></span> 
- <span data-ttu-id="38872-170">Maďarsko</span><span class="sxs-lookup"><span data-stu-id="38872-170">Hungary</span></span> 
- <span data-ttu-id="38872-171">Indie</span><span class="sxs-lookup"><span data-stu-id="38872-171">India</span></span> 
- <span data-ttu-id="38872-172">Irák</span><span class="sxs-lookup"><span data-stu-id="38872-172">Iraq</span></span> 
- <span data-ttu-id="38872-173">Kazachstán</span><span class="sxs-lookup"><span data-stu-id="38872-173">Kazakhstan</span></span> 
- <span data-ttu-id="38872-174">Kyrgyzstán</span><span class="sxs-lookup"><span data-stu-id="38872-174">Kyrgyzstan</span></span> 
- <span data-ttu-id="38872-175">Moldavsko</span><span class="sxs-lookup"><span data-stu-id="38872-175">Moldova</span></span> 
- <span data-ttu-id="38872-176">Myanmar</span><span class="sxs-lookup"><span data-stu-id="38872-176">Myanmar</span></span> 
- <span data-ttu-id="38872-177">Polsko</span><span class="sxs-lookup"><span data-stu-id="38872-177">Poland</span></span> 
- <span data-ttu-id="38872-178">Rusko</span><span class="sxs-lookup"><span data-stu-id="38872-178">Russia</span></span> 
- <span data-ttu-id="38872-179">Saúdská Arábie</span><span class="sxs-lookup"><span data-stu-id="38872-179">Saudi Arabia</span></span> 
- <span data-ttu-id="38872-180">Jižní Afrika</span><span class="sxs-lookup"><span data-stu-id="38872-180">South Africa</span></span> 
- <span data-ttu-id="38872-181">Jižní Súdán</span><span class="sxs-lookup"><span data-stu-id="38872-181">South Sudan</span></span>  
- <span data-ttu-id="38872-182">Tádžikistán</span><span class="sxs-lookup"><span data-stu-id="38872-182">Tajikistan</span></span> 
- <span data-ttu-id="38872-183">Thajsko</span><span class="sxs-lookup"><span data-stu-id="38872-183">Thailand</span></span>
- <span data-ttu-id="38872-184">Turecko</span><span class="sxs-lookup"><span data-stu-id="38872-184">Turkey</span></span> 
- <span data-ttu-id="38872-185">Ukrajina</span><span class="sxs-lookup"><span data-stu-id="38872-185">Ukraine</span></span> 
- <span data-ttu-id="38872-186">Spojené arabské emiráty</span><span class="sxs-lookup"><span data-stu-id="38872-186">United Arab Emirates</span></span> 
- <span data-ttu-id="38872-187">Uzbekistán</span><span class="sxs-lookup"><span data-stu-id="38872-187">Uzbekistan</span></span> 
- <span data-ttu-id="38872-188">Venezuela</span><span class="sxs-lookup"><span data-stu-id="38872-188">Venezuela</span></span>
- <span data-ttu-id="38872-189">Vietnam</span><span class="sxs-lookup"><span data-stu-id="38872-189">Vietnam</span></span> 


<span data-ttu-id="38872-190">Další informace najdete v tématu [ID registrace – informace o čísle](reg-number-id.md) .</span><span class="sxs-lookup"><span data-stu-id="38872-190">For more information, read [Registration ID number information](reg-number-id.md)</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="38872-191">Odstranit umístění</span><span class="sxs-lookup"><span data-stu-id="38872-191">Delete a location</span></span>

<span data-ttu-id="38872-192">Pokud chcete odstranit umístění z vašeho účtu, budete se muset obrátit na [podporu partnerů](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span><span class="sxs-lookup"><span data-stu-id="38872-192">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="38872-193">Ujistěte se, že rozumíte dopadu, který tato akce má.</span><span class="sxs-lookup"><span data-stu-id="38872-193">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="38872-194">Odstraněná umístění nelze načíst a veškerá vázaná ID MPN již nebudou rozpoznána nebo bude pro vaši společnost aktivní.</span><span class="sxs-lookup"><span data-stu-id="38872-194">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="38872-195">Změnit zemi globálního účtu partnera</span><span class="sxs-lookup"><span data-stu-id="38872-195">Change country of Partner global account</span></span> 

1. <span data-ttu-id="38872-196">Přihlaste se pomocí účtu MPN v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="38872-196">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="38872-197">(Vaše přihlašovací údaje programu MPN se můžou lišit od vašich přihlašovacích údajů CSP).</span><span class="sxs-lookup"><span data-stu-id="38872-197">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="38872-198">Účet MPN by měl mít oprávnění globálního správce nebo správce účtů.</span><span class="sxs-lookup"><span data-stu-id="38872-198">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="38872-199">Na kartě **partner** klikněte na **obchodní umístění** a zkontrolujte seznam umístění a ujistěte se, že je v seznamu uvedeno umístění, které chcete použít jako právní entitu.</span><span class="sxs-lookup"><span data-stu-id="38872-199">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="38872-200">Chcete-li přidat umístění, klikněte na tlačítko **Přidat umístění** a za předpokladu zadejte požadované podrobnosti, včetně názvu firmy, adresy a primárního kontaktu pro umístění, které chcete přidat do své společnosti.</span><span class="sxs-lookup"><span data-stu-id="38872-200">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="38872-201">Vyberte možnost **změnit zemi** vedle rozevíracího seznamu **země/oblast** a postupujte podle pokynů.</span><span class="sxs-lookup"><span data-stu-id="38872-201">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Oficiální informace o obchodním profilu":::

5. <span data-ttu-id="38872-203">Klikněte na **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="38872-203">Click **Save**.</span></span>

6. <span data-ttu-id="38872-204">Země globálního účtu MPN se změní na novou právní zemi.</span><span class="sxs-lookup"><span data-stu-id="38872-204">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="38872-205">Další kroky</span><span class="sxs-lookup"><span data-stu-id="38872-205">Next steps</span></span>

- <span data-ttu-id="38872-206">Přečtěte si o [procesu ověřování](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="38872-206">Learn about the [verification process](verification-responses.md).</span></span>
