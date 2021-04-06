---
title: Správa umístění v partnerském účtu
ms.topic: how-to
ms.date: 04/05/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Naučte se, jak přidat nové umístění a jak se v programu motivačních programů, v obchodních předplatných, předplatných a dalších transakcích používá umístění MPN ID.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7ca8c866479fbe153c1e0192edd33e8258b9d6e7
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441319"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="5788f-103">Správa umístění účtu MPN a přidání (odstranění) umístění</span><span class="sxs-lookup"><span data-stu-id="5788f-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="5788f-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="5788f-104">**Appropriate roles**</span></span>

- <span data-ttu-id="5788f-105">Globální správce</span><span class="sxs-lookup"><span data-stu-id="5788f-105">Global admin</span></span>
- <span data-ttu-id="5788f-106">Správce účtu</span><span class="sxs-lookup"><span data-stu-id="5788f-106">Account admin</span></span>

<span data-ttu-id="5788f-107">ID MPN umístění identifikuje každé konkrétní umístění vaší společnosti.</span><span class="sxs-lookup"><span data-stu-id="5788f-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="5788f-108">K registraci v programu motivačních programů použijete umístění MPN ID, a to za transakčního poskytovatele řešení cloudu (CSP) a další obchodní transakce.</span><span class="sxs-lookup"><span data-stu-id="5788f-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="5788f-109">Globální ID MPN se používá pro netransakční aktivity, například žádosti o podporu.</span><span class="sxs-lookup"><span data-stu-id="5788f-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="5788f-110">Typický je následující scénář:</span><span class="sxs-lookup"><span data-stu-id="5788f-110">The following scenario is typical:</span></span>

<span data-ttu-id="5788f-111">Společnost Contoso má svůj partnerský globální účet (PGA) ve Spojeném království.</span><span class="sxs-lookup"><span data-stu-id="5788f-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="5788f-112">PGA je jejich registrovaný právní podnik a globální ID MPN se používá ke správě všech netransakčních obchodních činností.</span><span class="sxs-lookup"><span data-stu-id="5788f-112">The PGA is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="5788f-113">Společnost Contoso má také partnerské účty partnera (PLA) rovnocenné dceřiným společnostem nebo divizím v jiném umístění v USA, Francii a USA.</span><span class="sxs-lookup"><span data-stu-id="5788f-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="5788f-114">Ve struktuře účtu MPN se tyto PLAs reprezentují jako jedinečná ID MPN.</span><span class="sxs-lookup"><span data-stu-id="5788f-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="5788f-115">PLAs se používají pro transakční firmy, jako je CSP nebo pobídky programů.</span><span class="sxs-lookup"><span data-stu-id="5788f-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="5788f-116">Výběry jsou vázané na konkrétní umístění.</span><span class="sxs-lookup"><span data-stu-id="5788f-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="5788f-117">Mezi klientem CSP a ID umístění MPN je 1-1 vztah.</span><span class="sxs-lookup"><span data-stu-id="5788f-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Struktura míst MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="5788f-119">Požadavky, aby bylo možné přidat nový účet pro firmu CSP</span><span class="sxs-lookup"><span data-stu-id="5788f-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="5788f-120">Pokud chcete přidat nový obchodní účet CSP, začněte tím, že ověříte, že jste splnili požadavky.</span><span class="sxs-lookup"><span data-stu-id="5788f-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="5788f-121">Musíte mít umístění MPN ID v zemi, kde chcete, aby se zprostředkovatel CSP vystavil.</span><span class="sxs-lookup"><span data-stu-id="5788f-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="5788f-122">Pokud chcete vytvořit nové umístění MPN, přečtěte si níže téma "Přidání umístění MPN".</span><span class="sxs-lookup"><span data-stu-id="5788f-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="5788f-123">Chcete-li vytvořit nového poskytovatele nepřímých prodejců CSP, přečtěte si téma [práce s nepřímými poskytovateli](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="5788f-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="5788f-124">Nezapomeňte se přihlásit pomocí **nových** přihlašovacích údajů **nového** účtu CSP.</span><span class="sxs-lookup"><span data-stu-id="5788f-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="5788f-125">Nepoužívejte svoje stávající přihlašovací údaje, protože Partnerské centrum vám rozpozná, jak už účet máte.</span><span class="sxs-lookup"><span data-stu-id="5788f-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="5788f-126">Přijměte smlouvu s partnerem Microsoftu a aktivujte účet.</span><span class="sxs-lookup"><span data-stu-id="5788f-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="5788f-127">Pokud se chcete zaregistrovat jako přímý fakturační Server, [požadavky na čtení pro přímé partnery z fakturace](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="5788f-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-your-mpn-locations"></a><span data-ttu-id="5788f-128">Zobrazení umístění MPN</span><span class="sxs-lookup"><span data-stu-id="5788f-128">View your MPN locations</span></span>

1. <span data-ttu-id="5788f-129">Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard/home) partnerského centra s přihlašovacími údaji k účtu MPN.</span><span class="sxs-lookup"><span data-stu-id="5788f-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="5788f-130">(Vaše přihlašovací údaje programu MPN se můžou lišit od vašich přihlašovacích údajů CSP.)</span><span class="sxs-lookup"><span data-stu-id="5788f-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="5788f-131">V ikoně **Nastavení** vyberte **Nastavení účtu**, **Profil organizace**, **právní**.</span><span class="sxs-lookup"><span data-stu-id="5788f-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="5788f-132">Na kartě **partner** ověřte, že se nezobrazí chybová zpráva banneru s výzvou k opravě umístění migrace z PMC.</span><span class="sxs-lookup"><span data-stu-id="5788f-132">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="5788f-133">Pokud vaše umístění nebyla správně nastavena v PMC a zatím nebyla převedena do počítačů PC, je nutné aktualizovat Tato umístění.</span><span class="sxs-lookup"><span data-stu-id="5788f-133">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="Snímek obrazovky videa ukazuje, jak aktualizovat polohu.":::
 
4.  <span data-ttu-id="5788f-135">Na obrazovce **zkontrolovat umístění PMC** vyberte **aktualizovat**.</span><span class="sxs-lookup"><span data-stu-id="5788f-135">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="5788f-136">Aktualizujte následující pole:</span><span class="sxs-lookup"><span data-stu-id="5788f-136">Update the following fields:</span></span>

- <span data-ttu-id="5788f-137">**Pole Name (název**): Ujistěte se, že název umístění společnosti je správný.</span><span class="sxs-lookup"><span data-stu-id="5788f-137">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="5788f-138">Pokud se zobrazí duplicitní Chyba, zkuste se změnit z, například contoso na contoso, Inc.</span><span class="sxs-lookup"><span data-stu-id="5788f-138">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="5788f-139">**Pole právnické osoby**: Ujistěte se, že jste zvolili právnickou entitu, se kterou je umístění svázáno.</span><span class="sxs-lookup"><span data-stu-id="5788f-139">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="5788f-140">**Řádková adresa 1 & 2 pole**: Ujistěte se, že je adresa správná.</span><span class="sxs-lookup"><span data-stu-id="5788f-140">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="5788f-141">**Města & země/provincie**: Ujistěte se, že je kombinace mezi městem a okresem správná.</span><span class="sxs-lookup"><span data-stu-id="5788f-141">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="5788f-142">K dispozici jsou země, kde se použije rozevírací nabídka pro výběr státu nebo provincie, a v ostatních zemích bude nutné ručně vložit pole.</span><span class="sxs-lookup"><span data-stu-id="5788f-142">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="5788f-143">**PSČ – pole** poštovního směrovacího čísla: Ujistěte se, že pole PSČ odpovídá vaší zadané zemi, oblasti, města nebo adrese.</span><span class="sxs-lookup"><span data-stu-id="5788f-143">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="5788f-144">**Pole primárních kontaktních informací**: Ujistěte se, že pole jméno a příjmení jsou vyplněna a že e-mailová adresa je pracovní e-mailová adresa, nikoli osobní (například,, @outlook.com @live.com atd.).</span><span class="sxs-lookup"><span data-stu-id="5788f-144">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="5788f-145">**Pole telefonní číslo**: Ujistěte se, že telefonní číslo neobsahuje speciální znaky, mezery ani kód země.</span><span class="sxs-lookup"><span data-stu-id="5788f-145">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="5788f-146">Hodnota zadaná v poli telefonní číslo bude vždycky obsahovat maximálně 10 znaků.</span><span class="sxs-lookup"><span data-stu-id="5788f-146">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="5788f-147">Pokud není k dispozici žádná chybová zpráva, pak z  **Nastavení** vyberte  **Nastavení účtu**, **Profil organizace**, **identifikátory**.</span><span class="sxs-lookup"><span data-stu-id="5788f-147">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="5788f-148">Vyhledejte ID MPN s typem "umístění", které odpovídá zemi tohoto účtu CSP, a použijte ji k dokončení přidružení.</span><span class="sxs-lookup"><span data-stu-id="5788f-148">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="5788f-149">Pokud nemůžete najít umístění MPN ID, které odpovídá účtu CSP, který chcete použít, můžete přidat nové umístění, ve kterém se vytvoří nové ID MPN.</span><span class="sxs-lookup"><span data-stu-id="5788f-149">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="5788f-150">Viz téma **Přidání umístění MPN** níže.</span><span class="sxs-lookup"><span data-stu-id="5788f-150">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="5788f-151">Přidat umístění MPN</span><span class="sxs-lookup"><span data-stu-id="5788f-151">Add an MPN location</span></span>

1. <span data-ttu-id="5788f-152">Přihlaste se pomocí účtu MPN v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="5788f-152">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="5788f-153">(Vaše přihlašovací údaje programu MPN se můžou lišit od vašich přihlašovacích údajů CSP).</span><span class="sxs-lookup"><span data-stu-id="5788f-153">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="5788f-154">Účet MPN by měl mít oprávnění globálního správce nebo správce účtů.</span><span class="sxs-lookup"><span data-stu-id="5788f-154">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="5788f-155">V **ikoně nastavení** vyberte **Nastavení účtu** a pak vyberte **Profil organizace**.</span><span class="sxs-lookup"><span data-stu-id="5788f-155">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="5788f-156">Vyberte možnost **právní** a pak na kartě **partner** vyberte **obchodní umístění** a klikněte na **Přidat umístění.**</span><span class="sxs-lookup"><span data-stu-id="5788f-156">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="5788f-157">Zadejte požadované podrobnosti, včetně názvu firmy, adresy a kontaktu pro umístění, které chcete přidat do své společnosti.</span><span class="sxs-lookup"><span data-stu-id="5788f-157">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="5788f-158">Klikněte na **Přidat umístění**.</span><span class="sxs-lookup"><span data-stu-id="5788f-158">Click **Add location**.</span></span> <span data-ttu-id="5788f-159">Tím se vytvoří nové ID MPN pro nové umístění, které můžete použít pro transakce a pobídky CSP.</span><span class="sxs-lookup"><span data-stu-id="5788f-159">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Přidat novou právní firmu":::

> [!NOTE]
> <span data-ttu-id="5788f-161">Jakmile je umístění přidané v partnerském centru, nemůžete ho odebrat.</span><span class="sxs-lookup"><span data-stu-id="5788f-161">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="5788f-162">Pokud jste pro přihlášení použili správné ID **MPN, zobrazí se v levé** nabídce centra pro partnery v nabídce vlevo.</span><span class="sxs-lookup"><span data-stu-id="5788f-162">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>


## <a name="delete-a-location"></a><span data-ttu-id="5788f-163">Odstranit umístění</span><span class="sxs-lookup"><span data-stu-id="5788f-163">Delete a location</span></span>

<span data-ttu-id="5788f-164">Pokud chcete odstranit umístění z vašeho účtu, budete se muset obrátit na [podporu partnerů](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span><span class="sxs-lookup"><span data-stu-id="5788f-164">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="5788f-165">Ujistěte se, že rozumíte dopadu, který tato akce má.</span><span class="sxs-lookup"><span data-stu-id="5788f-165">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="5788f-166">Odstraněná umístění nelze načíst a veškerá vázaná ID MPN již nebudou rozpoznána nebo bude pro vaši společnost aktivní.</span><span class="sxs-lookup"><span data-stu-id="5788f-166">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="5788f-167">Změnit zemi globálního účtu partnera</span><span class="sxs-lookup"><span data-stu-id="5788f-167">Change country of Partner global account</span></span> 

1. <span data-ttu-id="5788f-168">Přihlaste se pomocí účtu MPN v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="5788f-168">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="5788f-169">(Vaše přihlašovací údaje programu MPN se můžou lišit od vašich přihlašovacích údajů CSP).</span><span class="sxs-lookup"><span data-stu-id="5788f-169">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="5788f-170">Účet MPN by měl mít oprávnění globálního správce nebo správce účtů.</span><span class="sxs-lookup"><span data-stu-id="5788f-170">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="5788f-171">Na kartě **partner** klikněte na **obchodní umístění** a zkontrolujte seznam umístění a ujistěte se, že je v seznamu uvedeno umístění, které chcete použít jako právní entitu.</span><span class="sxs-lookup"><span data-stu-id="5788f-171">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="5788f-172">Chcete-li přidat umístění, klikněte na tlačítko **Přidat umístění** a za předpokladu zadejte požadované podrobnosti, včetně názvu firmy, adresy a primárního kontaktu pro umístění, které chcete přidat do své společnosti.</span><span class="sxs-lookup"><span data-stu-id="5788f-172">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="5788f-173">Vyberte možnost **změnit zemi** vedle rozevíracího seznamu **země/oblast** a postupujte podle pokynů.</span><span class="sxs-lookup"><span data-stu-id="5788f-173">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Oficiální informace o obchodním profilu":::

5. <span data-ttu-id="5788f-175">Klikněte na **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="5788f-175">Click **Save**.</span></span>

6. <span data-ttu-id="5788f-176">Země globálního účtu MPN se změní na novou právní zemi.</span><span class="sxs-lookup"><span data-stu-id="5788f-176">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="5788f-177">Další kroky</span><span class="sxs-lookup"><span data-stu-id="5788f-177">Next steps</span></span>

- <span data-ttu-id="5788f-178">Přečtěte si o [procesu ověřování](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="5788f-178">Learn about the [verification process](verification-responses.md).</span></span>
