---
title: Správa umístění v partnerském účtu
ms.topic: how-to
ms.date: 02/05/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Naučte se, jak přidat nové umístění a jak se v programu motivačních programů, v obchodních předplatných, předplatných a dalších transakcích používá umístění MPN ID.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c5ac31b772c6757468c5ea9d463643731571b31f
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624268"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="a05f5-103">Správa umístění účtu MPN a přidání nového umístění</span><span class="sxs-lookup"><span data-stu-id="a05f5-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="a05f5-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="a05f5-104">**Appropriate roles**</span></span>

- <span data-ttu-id="a05f5-105">Globální správce</span><span class="sxs-lookup"><span data-stu-id="a05f5-105">Global admin</span></span>
- <span data-ttu-id="a05f5-106">Správce účtu</span><span class="sxs-lookup"><span data-stu-id="a05f5-106">Account admin</span></span>

<span data-ttu-id="a05f5-107">ID MPN umístění identifikuje každé konkrétní umístění vaší společnosti.</span><span class="sxs-lookup"><span data-stu-id="a05f5-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="a05f5-108">K registraci v programu motivačních programů použijete umístění MPN ID, a to za transakčního poskytovatele řešení cloudu (CSP) a další obchodní transakce.</span><span class="sxs-lookup"><span data-stu-id="a05f5-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="a05f5-109">Globální ID MPN se používá pro netransakční aktivity, například žádosti o podporu.</span><span class="sxs-lookup"><span data-stu-id="a05f5-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="a05f5-110">Následuje typický scénář:</span><span class="sxs-lookup"><span data-stu-id="a05f5-110">The following is a typical scenario:</span></span>

<span data-ttu-id="a05f5-111">Společnost Contoso má svůj partnerský globální účet (PGA) ve Spojeném království.</span><span class="sxs-lookup"><span data-stu-id="a05f5-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="a05f5-112">Jedná se o své registrované právní firmy a globální ID MPN se používá ke správě všech netransakčních obchodních činností.</span><span class="sxs-lookup"><span data-stu-id="a05f5-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="a05f5-113">Společnost Contoso má také partnerské účty partnera (PLA) rovnocenné dceřiným společnostem nebo divizím v jiném umístění v USA, Francii a USA.</span><span class="sxs-lookup"><span data-stu-id="a05f5-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="a05f5-114">Ve struktuře účtu MPN se tyto PLAs reprezentují jako jedinečná ID MPN.</span><span class="sxs-lookup"><span data-stu-id="a05f5-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="a05f5-115">PLAs se používají pro transakční firmy, jako je CSP nebo pobídky programů.</span><span class="sxs-lookup"><span data-stu-id="a05f5-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="a05f5-116">Výběry jsou vázané na konkrétní umístění.</span><span class="sxs-lookup"><span data-stu-id="a05f5-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="a05f5-117">Mezi klientem CSP a ID umístění MPN je 1-1 vztah.</span><span class="sxs-lookup"><span data-stu-id="a05f5-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Struktura míst MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="a05f5-119">Požadavky, aby bylo možné přidat nový účet pro firmu CSP</span><span class="sxs-lookup"><span data-stu-id="a05f5-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="a05f5-120">Pokud chcete přidat nový obchodní účet CSP, začněte tím, že ověříte, že jste splnili požadavky.</span><span class="sxs-lookup"><span data-stu-id="a05f5-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="a05f5-121">Musíte mít umístění MPN ID v zemi, kde chcete, aby se zprostředkovatel CSP vystavil.</span><span class="sxs-lookup"><span data-stu-id="a05f5-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="a05f5-122">Pokud chcete vytvořit nové umístění MPN, přečtěte si níže téma "Přidání umístění MPN".</span><span class="sxs-lookup"><span data-stu-id="a05f5-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="a05f5-123">Chcete-li vytvořit nového poskytovatele nepřímých prodejců CSP, přečtěte si téma [práce s nepřímými poskytovateli](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="a05f5-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="a05f5-124">Nezapomeňte se přihlásit pomocí **nových** přihlašovacích údajů **nového** účtu CSP.</span><span class="sxs-lookup"><span data-stu-id="a05f5-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="a05f5-125">Nepoužívejte svoje stávající přihlašovací údaje, protože Partnerské centrum vám rozpozná, jak už účet máte.</span><span class="sxs-lookup"><span data-stu-id="a05f5-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="a05f5-126">Přijměte smlouvu s partnerem Microsoftu a aktivujte účet.</span><span class="sxs-lookup"><span data-stu-id="a05f5-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="a05f5-127">Pokud se chcete zaregistrovat jako přímý fakturační Server, [požadavky na čtení pro přímé partnery z fakturace](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="a05f5-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-your-mpn-locations"></a><span data-ttu-id="a05f5-128">Zobrazení umístění MPN</span><span class="sxs-lookup"><span data-stu-id="a05f5-128">View your MPN locations</span></span>

1. <span data-ttu-id="a05f5-129">Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard/home) partnerského centra s přihlašovacími údaji k účtu MPN.</span><span class="sxs-lookup"><span data-stu-id="a05f5-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="a05f5-130">(Vaše přihlašovací údaje programu MPN se můžou lišit od vašich přihlašovacích údajů CSP.)</span><span class="sxs-lookup"><span data-stu-id="a05f5-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="a05f5-131">V ikoně **Nastavení** vyberte **Nastavení účtu**, **Profil organizace**, **právní**.</span><span class="sxs-lookup"><span data-stu-id="a05f5-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="a05f5-132">Na kartě **partner** ověřte, že není k dispozici zpráva banneru s výzvou k opravě umístění migrace z PMC.</span><span class="sxs-lookup"><span data-stu-id="a05f5-132">On the **Partner** tab verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span> <span data-ttu-id="a05f5-133">Pokud je, postupujte podle pokynů a opravte tato umístění.</span><span class="sxs-lookup"><span data-stu-id="a05f5-133">If there is, follow instructions and fix those locations.</span></span> 

3. <span data-ttu-id="a05f5-134">Pokud není k dispozici žádná chybová zpráva, pak z  **Nastavení** vyberte  **Nastavení účtu**, **Profil organizace**, **identifikátory**.</span><span class="sxs-lookup"><span data-stu-id="a05f5-134">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

4. <span data-ttu-id="a05f5-135">Vyhledejte ID MPN s typem "umístění", které odpovídá zemi tohoto účtu CSP, a použijte ji k vyhledávání níže a dokončení přidružení.</span><span class="sxs-lookup"><span data-stu-id="a05f5-135">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to search below and complete association.</span></span>

5. <span data-ttu-id="a05f5-136">Pokud nemůžete najít umístění MPN ID, které odpovídá účtu CSP, který chcete použít, můžete přidat nové umístění, ve kterém se vytvoří nové ID MPN.</span><span class="sxs-lookup"><span data-stu-id="a05f5-136">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location which will create a new MPN ID.</span></span> <span data-ttu-id="a05f5-137">Viz téma **Přidání umístění MPN** níže.</span><span class="sxs-lookup"><span data-stu-id="a05f5-137">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="a05f5-138">Přidat umístění MPN</span><span class="sxs-lookup"><span data-stu-id="a05f5-138">Add an MPN location</span></span>

1. <span data-ttu-id="a05f5-139">Přihlaste se pomocí účtu MPN v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="a05f5-139">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="a05f5-140">(Vaše přihlašovací údaje programu MPN se můžou lišit od vašich přihlašovacích údajů CSP).</span><span class="sxs-lookup"><span data-stu-id="a05f5-140">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="a05f5-141">Účet MPN by měl mít oprávnění globálního správce nebo správce účtů.</span><span class="sxs-lookup"><span data-stu-id="a05f5-141">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="a05f5-142">V **ikoně nastavení** vyberte **Nastavení účtu** a pak vyberte **Profil organizace**.</span><span class="sxs-lookup"><span data-stu-id="a05f5-142">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="a05f5-143">Vyberte možnost **právní** a pak na kartě **partner** vyberte **obchodní umístění** a klikněte na **Přidat umístění.**</span><span class="sxs-lookup"><span data-stu-id="a05f5-143">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="a05f5-144">Zadejte požadované podrobnosti, včetně názvu firmy, adresy a kontaktu pro umístění, které chcete přidat do své společnosti.</span><span class="sxs-lookup"><span data-stu-id="a05f5-144">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="a05f5-145">Klikněte na **Přidat umístění**.</span><span class="sxs-lookup"><span data-stu-id="a05f5-145">Click **Add location**.</span></span> <span data-ttu-id="a05f5-146">Tím se vytvoří nové ID MPN pro nové umístění, které můžete použít pro transakce a pobídky CSP.</span><span class="sxs-lookup"><span data-stu-id="a05f5-146">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Přidat novou právní firmu":::

> [!NOTE]
> <span data-ttu-id="a05f5-148">Po přidání umístění do partnerského centra ho nejde odebrat.</span><span class="sxs-lookup"><span data-stu-id="a05f5-148">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="a05f5-149">Pokud jste pro přihlášení použili správné ID **MPN, zobrazí se v levé** nabídce centra pro partnery v nabídce vlevo.</span><span class="sxs-lookup"><span data-stu-id="a05f5-149">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="a05f5-150">Změnit zemi globálního účtu partnera</span><span class="sxs-lookup"><span data-stu-id="a05f5-150">Change country of Partner global account</span></span> 

1. <span data-ttu-id="a05f5-151">Přihlaste se pomocí účtu MPN v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="a05f5-151">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="a05f5-152">(Vaše přihlašovací údaje programu MPN se můžou lišit od vašich přihlašovacích údajů CSP).</span><span class="sxs-lookup"><span data-stu-id="a05f5-152">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="a05f5-153">Účet MPN by měl mít oprávnění globálního správce nebo správce účtů.</span><span class="sxs-lookup"><span data-stu-id="a05f5-153">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="a05f5-154">Na kartě **partner** klikněte na **obchodní umístění** a zkontrolujte seznam umístění a ujistěte se, že je v seznamu uvedeno umístění, které chcete použít jako právní entitu.</span><span class="sxs-lookup"><span data-stu-id="a05f5-154">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="a05f5-155">Chcete-li přidat umístění, klikněte na tlačítko **Přidat umístění** a za předpokladu zadejte požadované podrobnosti, včetně názvu firmy, adresy a primárního kontaktu pro umístění, které chcete přidat do své společnosti.</span><span class="sxs-lookup"><span data-stu-id="a05f5-155">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="a05f5-156">Vyberte možnost **změnit zemi** vedle rozevíracího seznamu **země/oblast** a postupujte podle pokynů.</span><span class="sxs-lookup"><span data-stu-id="a05f5-156">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Oficiální informace o obchodním profilu":::

5. <span data-ttu-id="a05f5-158">Klikněte na **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="a05f5-158">Click **Save**.</span></span>

6. <span data-ttu-id="a05f5-159">Země globálního účtu MPN se změní na novou právní zemi.</span><span class="sxs-lookup"><span data-stu-id="a05f5-159">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="a05f5-160">Další kroky</span><span class="sxs-lookup"><span data-stu-id="a05f5-160">Next steps</span></span>

- <span data-ttu-id="a05f5-161">Přečtěte si o [procesu ověřování](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="a05f5-161">Learn about the [verification process](verification-responses.md).</span></span>
