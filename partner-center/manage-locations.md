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
ms.openlocfilehash: 13d6e7dc4722227035be2b24df48427f2008bb14
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151776"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="b999a-103">Správa umístění účtu MPN a přidání (odstranění) umístění</span><span class="sxs-lookup"><span data-stu-id="b999a-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="b999a-104">**Příslušné role**: globální správce | Správce účtu</span><span class="sxs-lookup"><span data-stu-id="b999a-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="b999a-105">ID MPN umístění identifikuje každé konkrétní umístění vaší společnosti.</span><span class="sxs-lookup"><span data-stu-id="b999a-105">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="b999a-106">K registraci v programu motivačních programů použijete umístění MPN ID, a to za transakčního poskytovatele řešení cloudu (CSP) a další obchodní transakce.</span><span class="sxs-lookup"><span data-stu-id="b999a-106">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="b999a-107">Globální ID MPN se používá pro netransakční aktivity, například žádosti o podporu.</span><span class="sxs-lookup"><span data-stu-id="b999a-107">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="b999a-108">Typický je následující scénář:</span><span class="sxs-lookup"><span data-stu-id="b999a-108">The following scenario is typical:</span></span>

<span data-ttu-id="b999a-109">Společnost Contoso má svůj partnerský globální účet (PGA) ve Spojeném království.</span><span class="sxs-lookup"><span data-stu-id="b999a-109">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="b999a-110">PGA je jejich registrovaná právní společnost a její globální ID MPN se používá ke správě všech netransakčních obchodních činností.</span><span class="sxs-lookup"><span data-stu-id="b999a-110">The PGA is their registered legal business, and its global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="b999a-111">Společnost Contoso má také partnerské účty partnera (PLA) rovnocenné dceřiným společnostem nebo divizím v jiném umístění v USA, Francii a USA.</span><span class="sxs-lookup"><span data-stu-id="b999a-111">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="b999a-112">Ve struktuře účtu MPN se tyto PLAs reprezentují jako jedinečná ID MPN.</span><span class="sxs-lookup"><span data-stu-id="b999a-112">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="b999a-113">PLAs se používají pro transakční firmy, jako je CSP nebo pobídky programů.</span><span class="sxs-lookup"><span data-stu-id="b999a-113">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="b999a-114">Výběry jsou vázané na konkrétní umístění.</span><span class="sxs-lookup"><span data-stu-id="b999a-114">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="b999a-115">Mezi klientem CSP a ID umístění MPN je 1-1 vztah.</span><span class="sxs-lookup"><span data-stu-id="b999a-115">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Struktura míst MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="b999a-117">Požadavky, aby bylo možné přidat nový účet pro firmu CSP</span><span class="sxs-lookup"><span data-stu-id="b999a-117">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="b999a-118">Pokud chcete přidat nový obchodní účet CSP, začněte tím, že ověříte, že jste splnili požadavky.</span><span class="sxs-lookup"><span data-stu-id="b999a-118">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="b999a-119">Musíte mít umístění MPN ID v zemi, kde chcete, aby se zprostředkovatel CSP vystavil.</span><span class="sxs-lookup"><span data-stu-id="b999a-119">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="b999a-120">Pokud chcete vytvořit nové umístění MPN, přečtěte si níže téma "Přidání umístění MPN".</span><span class="sxs-lookup"><span data-stu-id="b999a-120">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="b999a-121">Pokud chcete vytvořit novou registraci CSP Indirect Reseller, přečtěte si o [práci s nepřímými poskytovateli.](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="b999a-121">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="b999a-122">Nezapomeňte se přihlásit pomocí nových **přihlašovacích** údajů pro **nový účet** CSP.</span><span class="sxs-lookup"><span data-stu-id="b999a-122">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="b999a-123">Nepoužívejte stávající přihlašovací údaje, protože Partnerské centrum poznáte, že už účet máte.</span><span class="sxs-lookup"><span data-stu-id="b999a-123">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="b999a-124">Přijměte Smlouva s partnerem Microsoftu a aktivujte účet.</span><span class="sxs-lookup"><span data-stu-id="b999a-124">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="b999a-125">Pokud se chcete zaregistrovat jako partner s přímým vyúčtováním, přečtěte si požadavky [na partnery s přímým vyúčtováním.](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="b999a-125">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-and-update-your-mpn-locations"></a><span data-ttu-id="b999a-126">Zobrazení a aktualizace umístění MPN</span><span class="sxs-lookup"><span data-stu-id="b999a-126">View and update your MPN locations</span></span>

1. <span data-ttu-id="b999a-127">Přihlaste se k řídicímu Partnerské centrum [pomocí](https://partner.microsoft.com/dashboard/home) přihlašovacích údajů účtu MPN.</span><span class="sxs-lookup"><span data-stu-id="b999a-127">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="b999a-128">(Vaše přihlašovací údaje MPN se mohou lišit od vašich přihlašovacích údajů CSP))</span><span class="sxs-lookup"><span data-stu-id="b999a-128">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="b999a-129">V **ikoně** Nastavení vyberte **Nastavení účtu**, **Profil organizace**, **Právní.**</span><span class="sxs-lookup"><span data-stu-id="b999a-129">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="b999a-130">Na kartě **Partner** ověřte, že není chybová zpráva s upozorněním s žádostí o opravu migrovaných umístění z PMC.</span><span class="sxs-lookup"><span data-stu-id="b999a-130">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="b999a-131">Pokud vaše umístění nebyla v PMC správně nastavená a ještě nebyla přemísněna na počítač PC, musíte tato umístění aktualizovat.</span><span class="sxs-lookup"><span data-stu-id="b999a-131">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="Snímek obrazovky ukazuje, jak aktualizovat umístění.":::
 
4.  <span data-ttu-id="b999a-133">Na **obrazovce Review PMC locations (Zkontrolovat umístění PMC)** vyberte **Update (Aktualizovat).**</span><span class="sxs-lookup"><span data-stu-id="b999a-133">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="b999a-134">Aktualizujte následující pole:</span><span class="sxs-lookup"><span data-stu-id="b999a-134">Update the following fields:</span></span>

- <span data-ttu-id="b999a-135">**Pole Název:** Ujistěte se, že je název umístění společnosti správný.</span><span class="sxs-lookup"><span data-stu-id="b999a-135">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="b999a-136">Pokud se zobrazí duplicitní chyba, zkuste změnit například z Contoso na Contoso, Inc.</span><span class="sxs-lookup"><span data-stu-id="b999a-136">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="b999a-137">**Pole právní osoby:** Ujistěte se, že jste zvolili právnickou osobu, se kterou je umístění vázané.</span><span class="sxs-lookup"><span data-stu-id="b999a-137">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="b999a-138">**Řádek adresy 1 & 2:** Ujistěte se, že je adresa správná.</span><span class="sxs-lookup"><span data-stu-id="b999a-138">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="b999a-139">**Pole & stát/kraj:** Ujistěte se, že je kombinace mezi městem a krajem správná.</span><span class="sxs-lookup"><span data-stu-id="b999a-139">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="b999a-140">V některých zemích se použije rozevírací nabídka pro výběr státu/kraje a v jiných zemích bude nutné toto pole vložit ručně.</span><span class="sxs-lookup"><span data-stu-id="b999a-140">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="b999a-141">**PSČ – pole** poštovního směrovacího čísla: Ujistěte se, že pole PSČ odpovídá vaší zadané zemi, oblasti, města nebo adrese.</span><span class="sxs-lookup"><span data-stu-id="b999a-141">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="b999a-142">**Pole primárních kontaktních informací**: Ujistěte se, že pole jméno a příjmení jsou vyplněna a že e-mailová adresa je pracovní e-mailová adresa, nikoli osobní (například,, @outlook.com @live.com atd.).</span><span class="sxs-lookup"><span data-stu-id="b999a-142">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="b999a-143">**Pole telefonní číslo**: Ujistěte se, že telefonní číslo neobsahuje speciální znaky, mezery ani kód země.</span><span class="sxs-lookup"><span data-stu-id="b999a-143">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="b999a-144">Hodnota zadaná v poli telefonní číslo bude vždycky obsahovat maximálně 10 znaků.</span><span class="sxs-lookup"><span data-stu-id="b999a-144">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="b999a-145">Pokud není k dispozici žádná chybová zpráva, pak z  **Nastavení** vyberte  **Nastavení účtu**, **Profil organizace**, **identifikátory**.</span><span class="sxs-lookup"><span data-stu-id="b999a-145">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="b999a-146">Vyhledejte ID MPN s typem "umístění", které odpovídá zemi tohoto účtu CSP, a použijte ji k dokončení přidružení.</span><span class="sxs-lookup"><span data-stu-id="b999a-146">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="b999a-147">Pokud nemůžete najít umístění MPN ID, které odpovídá účtu CSP, který chcete použít, můžete přidat nové umístění, ve kterém se vytvoří nové ID MPN.</span><span class="sxs-lookup"><span data-stu-id="b999a-147">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="b999a-148">Viz téma **Přidání umístění MPN** níže.</span><span class="sxs-lookup"><span data-stu-id="b999a-148">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="b999a-149">Přidat umístění MPN</span><span class="sxs-lookup"><span data-stu-id="b999a-149">Add an MPN location</span></span>

1. <span data-ttu-id="b999a-150">Přihlaste se pomocí účtu MPN v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="b999a-150">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="b999a-151">(Vaše přihlašovací údaje programu MPN se můžou lišit od vašich přihlašovacích údajů CSP.) Účet MPN by měl mít oprávnění globálního správce nebo správce účtů.</span><span class="sxs-lookup"><span data-stu-id="b999a-151">(Your MPN credentials may be different from your CSP credentials.) The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="b999a-152">V **ikoně nastavení** vyberte **Nastavení účtu** a pak vyberte **Profil organizace**.</span><span class="sxs-lookup"><span data-stu-id="b999a-152">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="b999a-153">Vyberte možnost **právní** a pak na kartě **partner** vyberte **obchodní umístění** a vyberte **Přidat umístění.**</span><span class="sxs-lookup"><span data-stu-id="b999a-153">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and select **Add a location.**</span></span>

3. <span data-ttu-id="b999a-154">Zadejte požadované podrobnosti, včetně názvu firmy, adresy a kontaktu pro umístění, které chcete přidat do své společnosti.</span><span class="sxs-lookup"><span data-stu-id="b999a-154">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="b999a-155">Vyberte **Přidat umístění**.</span><span class="sxs-lookup"><span data-stu-id="b999a-155">Select **Add location**.</span></span> <span data-ttu-id="b999a-156">Tím se vytvoří nové ID MPN pro nové umístění, které můžete použít pro transakce a pobídky CSP.</span><span class="sxs-lookup"><span data-stu-id="b999a-156">This will create a new MPN ID for the new location that you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Přidat novou právní firmu":::

> [!NOTE]
> <span data-ttu-id="b999a-158">Jakmile je umístění přidané v partnerském centru, nemůžete ho odebrat.</span><span class="sxs-lookup"><span data-stu-id="b999a-158">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="b999a-159">Pokud jste pro přihlášení použili správné ID **MPN, zobrazí se v levé** nabídce centra pro partnery v nabídce vlevo.</span><span class="sxs-lookup"><span data-stu-id="b999a-159">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="add-the-registration-number-id"></a><span data-ttu-id="b999a-160">Přidat ID registračního čísla</span><span class="sxs-lookup"><span data-stu-id="b999a-160">Add the registration number ID</span></span>

<span data-ttu-id="b999a-161">Pokud jste nepřímý poskytovatel, partner s přímým vyúčtováním nebo nepřímý prodejce a podnikáte s novými nebo stávajícími zákazníky v následujících zemích, musíte pro svou firmu zadat identifikační čísla registrace.</span><span class="sxs-lookup"><span data-stu-id="b999a-161">If you are an Indirect provider, Direct bill partner, or Indirect reseller and you are doing business with new or existing customers in the following countries, you need to provide registration ID numbers for your business.</span></span> <span data-ttu-id="b999a-162">Pokud země, ve které podnikáte, není uvedená níže, ID registrace je volitelné.</span><span class="sxs-lookup"><span data-stu-id="b999a-162">If the country you are doing business in is not listed below, the registration ID is optional.</span></span>

- <span data-ttu-id="b999a-163">Arménie</span><span class="sxs-lookup"><span data-stu-id="b999a-163">Armenia</span></span> 
- <span data-ttu-id="b999a-164">Ázerbájdžán</span><span class="sxs-lookup"><span data-stu-id="b999a-164">Azerbaijan</span></span> 
- <span data-ttu-id="b999a-165">Bělorusko</span><span class="sxs-lookup"><span data-stu-id="b999a-165">Belarus</span></span> 
- <span data-ttu-id="b999a-166">Brazílie</span><span class="sxs-lookup"><span data-stu-id="b999a-166">Brazil</span></span> 
- <span data-ttu-id="b999a-167">Maďarsko</span><span class="sxs-lookup"><span data-stu-id="b999a-167">Hungary</span></span> 
- <span data-ttu-id="b999a-168">Indie</span><span class="sxs-lookup"><span data-stu-id="b999a-168">India</span></span> 
- <span data-ttu-id="b999a-169">Irák</span><span class="sxs-lookup"><span data-stu-id="b999a-169">Iraq</span></span> 
- <span data-ttu-id="b999a-170">Kazachstán</span><span class="sxs-lookup"><span data-stu-id="b999a-170">Kazakhstan</span></span> 
- <span data-ttu-id="b999a-171">Kyrgyzstán</span><span class="sxs-lookup"><span data-stu-id="b999a-171">Kyrgyzstan</span></span> 
- <span data-ttu-id="b999a-172">Moldavsko</span><span class="sxs-lookup"><span data-stu-id="b999a-172">Moldova</span></span> 
- <span data-ttu-id="b999a-173">Myanmar</span><span class="sxs-lookup"><span data-stu-id="b999a-173">Myanmar</span></span> 
- <span data-ttu-id="b999a-174">Polsko</span><span class="sxs-lookup"><span data-stu-id="b999a-174">Poland</span></span> 
- <span data-ttu-id="b999a-175">Rusko</span><span class="sxs-lookup"><span data-stu-id="b999a-175">Russia</span></span> 
- <span data-ttu-id="b999a-176">Saúdská Arábie</span><span class="sxs-lookup"><span data-stu-id="b999a-176">Saudi Arabia</span></span> 
- <span data-ttu-id="b999a-177">Jižní Afrika</span><span class="sxs-lookup"><span data-stu-id="b999a-177">South Africa</span></span> 
- <span data-ttu-id="b999a-178">Jižní Súdán</span><span class="sxs-lookup"><span data-stu-id="b999a-178">South Sudan</span></span>  
- <span data-ttu-id="b999a-179">Tádžikistán</span><span class="sxs-lookup"><span data-stu-id="b999a-179">Tajikistan</span></span> 
- <span data-ttu-id="b999a-180">Thajsko</span><span class="sxs-lookup"><span data-stu-id="b999a-180">Thailand</span></span>
- <span data-ttu-id="b999a-181">Turecko</span><span class="sxs-lookup"><span data-stu-id="b999a-181">Turkey</span></span> 
- <span data-ttu-id="b999a-182">Ukrajina</span><span class="sxs-lookup"><span data-stu-id="b999a-182">Ukraine</span></span> 
- <span data-ttu-id="b999a-183">Spojené arabské emiráty</span><span class="sxs-lookup"><span data-stu-id="b999a-183">United Arab Emirates</span></span> 
- <span data-ttu-id="b999a-184">Uzbekistán</span><span class="sxs-lookup"><span data-stu-id="b999a-184">Uzbekistan</span></span> 
- <span data-ttu-id="b999a-185">Venezuela</span><span class="sxs-lookup"><span data-stu-id="b999a-185">Venezuela</span></span>
- <span data-ttu-id="b999a-186">Vietnam</span><span class="sxs-lookup"><span data-stu-id="b999a-186">Vietnam</span></span> 


<span data-ttu-id="b999a-187">Další informace najdete v článku [o čísle ID registrace.](reg-number-id.md)</span><span class="sxs-lookup"><span data-stu-id="b999a-187">For more information, read [Registration ID number information](reg-number-id.md)</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="b999a-188">Odstranění umístění</span><span class="sxs-lookup"><span data-stu-id="b999a-188">Delete a location</span></span>

<span data-ttu-id="b999a-189">Pokud chcete umístění z vašeho účtu odstranit, budete se muset obrátit na [podporu partnerů.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b)</span><span class="sxs-lookup"><span data-stu-id="b999a-189">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="b999a-190">Ujistěte se, že rozumíte dopadu, který tato akce má.</span><span class="sxs-lookup"><span data-stu-id="b999a-190">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="b999a-191">Odstraněná umístění není možné načíst a cokoli svázané s konkrétním ID MPN se už nerozpozná nebo nebude pro vaši společnost aktivní.</span><span class="sxs-lookup"><span data-stu-id="b999a-191">Deleted locations cannot be retrieved and anything tied to that specific MPN ID will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="b999a-192">Změna země globálního účtu partnera</span><span class="sxs-lookup"><span data-stu-id="b999a-192">Change country of Partner global account</span></span> 

1. <span data-ttu-id="b999a-193">Přihlaste se pomocí účtu MPN v Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="b999a-193">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="b999a-194">(Vaše přihlašovací údaje MPN se mohou lišit od vašich přihlašovacích údajů CSP.) Účet MPN by měl mít oprávnění globálního správce nebo správce účtu.</span><span class="sxs-lookup"><span data-stu-id="b999a-194">(Your MPN credentials may be different from your CSP credentials.) The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="b999a-195">Na kartě **Partner (Partner)** přejděte na **Obchodní** umístění a zkontrolujte seznam umístění a ujistěte se, že je uvedená lokalita, ve které je uvedená vaše právní osoba.</span><span class="sxs-lookup"><span data-stu-id="b999a-195">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="b999a-196">Pokud chcete přidat umístění, klikněte na Přidat umístění a v okně zadejte požadované podrobnosti, včetně obchodního jména, adresy **a** primárního kontaktu pro umístění, které chcete přidat do vaší společnosti.</span><span class="sxs-lookup"><span data-stu-id="b999a-196">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="b999a-197">Vyberte **Změnit zemi** vedle rozevíracího seznamu **Země/oblast** a postupujte podle těchto kroků.</span><span class="sxs-lookup"><span data-stu-id="b999a-197">Select **Change your country** next to the **Country/region** drop-down list and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Právní informace o datech obchodního profilu":::

5. <span data-ttu-id="b999a-199">Vyberte **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="b999a-199">Select **Save**.</span></span>

6. <span data-ttu-id="b999a-200">Globální země účtu MPN se změní na novou právní zemi.</span><span class="sxs-lookup"><span data-stu-id="b999a-200">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="b999a-201">Další kroky</span><span class="sxs-lookup"><span data-stu-id="b999a-201">Next steps</span></span>

- <span data-ttu-id="b999a-202">Přečtěte si o [procesu ověřování.](verification-responses.md)</span><span class="sxs-lookup"><span data-stu-id="b999a-202">Learn about the [verification process](verification-responses.md).</span></span>
