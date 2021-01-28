---
title: Správa umístění v partnerském účtu
ms.topic: how-to
ms.date: 01/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Naučte se, jak přidat nové umístění a jak se v programu motivačních programů, v obchodních předplatných, předplatných a dalších transakcích používá umístění MPN ID.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e39f264485e71c5a96916c224c0ea1a85c17a55b
ms.sourcegitcommit: fc1f9cb5a542bdc92d62d2a7e1ab2f4e69903e49
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/28/2021
ms.locfileid: "98925009"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="4dc73-103">Správa umístění účtu MPN a přidání nového umístění</span><span class="sxs-lookup"><span data-stu-id="4dc73-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="4dc73-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="4dc73-104">**Appropriate roles**</span></span>

- <span data-ttu-id="4dc73-105">Globální správce</span><span class="sxs-lookup"><span data-stu-id="4dc73-105">Global admin</span></span>
- <span data-ttu-id="4dc73-106">Správce účtu</span><span class="sxs-lookup"><span data-stu-id="4dc73-106">Account admin</span></span>

<span data-ttu-id="4dc73-107">ID MPN umístění identifikuje každé konkrétní umístění vaší společnosti.</span><span class="sxs-lookup"><span data-stu-id="4dc73-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="4dc73-108">K registraci v programu motivačních programů použijete umístění MPN ID, a to za transakčního poskytovatele řešení cloudu (CSP) a další obchodní transakce.</span><span class="sxs-lookup"><span data-stu-id="4dc73-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="4dc73-109">Globální ID MPN se používá pro netransakční aktivity, například žádosti o podporu.</span><span class="sxs-lookup"><span data-stu-id="4dc73-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="4dc73-110">Následuje typický scénář:</span><span class="sxs-lookup"><span data-stu-id="4dc73-110">The following is a typical scenario:</span></span>

<span data-ttu-id="4dc73-111">Společnost Contoso má svůj partnerský globální účet (PGA) ve Spojeném království.</span><span class="sxs-lookup"><span data-stu-id="4dc73-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="4dc73-112">Jedná se o své registrované právní firmy a globální ID MPN se používá ke správě všech netransakčních obchodních činností.</span><span class="sxs-lookup"><span data-stu-id="4dc73-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="4dc73-113">Společnost Contoso má také partnerské účty partnera (PLA) rovnocenné dceřiným společnostem nebo divizím v jiném umístění v USA, Francii a USA.</span><span class="sxs-lookup"><span data-stu-id="4dc73-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="4dc73-114">Ve struktuře účtu MPN se tyto PLAs reprezentují jako jedinečná ID MPN.</span><span class="sxs-lookup"><span data-stu-id="4dc73-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="4dc73-115">PLAs se používají pro transakční firmy, jako je CSP nebo pobídky programů.</span><span class="sxs-lookup"><span data-stu-id="4dc73-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="4dc73-116">Výběry jsou vázané na konkrétní umístění.</span><span class="sxs-lookup"><span data-stu-id="4dc73-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="4dc73-117">Mezi klientem CSP a ID umístění MPN je 1-1 vztah.</span><span class="sxs-lookup"><span data-stu-id="4dc73-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Struktura míst MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="4dc73-119">Požadavky, aby bylo možné přidat nový účet pro firmu CSP</span><span class="sxs-lookup"><span data-stu-id="4dc73-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="4dc73-120">Pokud chcete přidat nový obchodní účet CSP, začněte tím, že ověříte, že jste splnili požadavky.</span><span class="sxs-lookup"><span data-stu-id="4dc73-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="4dc73-121">Musíte mít umístění MPN ID v zemi, kde chcete, aby se zprostředkovatel CSP vystavil.</span><span class="sxs-lookup"><span data-stu-id="4dc73-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="4dc73-122">Pokud chcete vytvořit nové umístění MPN, přečtěte si níže téma "Přidání umístění MPN".</span><span class="sxs-lookup"><span data-stu-id="4dc73-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="4dc73-123">Chcete-li vytvořit nového poskytovatele nepřímých prodejců CSP, přečtěte si téma [práce s nepřímými poskytovateli](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="4dc73-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="4dc73-124">Nezapomeňte se přihlásit pomocí **nových** přihlašovacích údajů **nového** účtu CSP.</span><span class="sxs-lookup"><span data-stu-id="4dc73-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="4dc73-125">Nepoužívejte svoje stávající přihlašovací údaje, protože Partnerské centrum vám rozpozná, jak už účet máte.</span><span class="sxs-lookup"><span data-stu-id="4dc73-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="4dc73-126">Přijměte smlouvu s partnerem Microsoftu a aktivujte účet.</span><span class="sxs-lookup"><span data-stu-id="4dc73-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="4dc73-127">Přidat umístění MPN</span><span class="sxs-lookup"><span data-stu-id="4dc73-127">Add an MPN location</span></span>

1. <span data-ttu-id="4dc73-128">Přihlaste se pomocí účtu MPN v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="4dc73-128">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="4dc73-129">(Vaše přihlašovací údaje programu MPN se můžou lišit od vašich přihlašovacích údajů CSP).</span><span class="sxs-lookup"><span data-stu-id="4dc73-129">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="4dc73-130">Účet MPN by měl mít oprávnění globálního správce nebo správce účtů.</span><span class="sxs-lookup"><span data-stu-id="4dc73-130">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="4dc73-131">V **ikoně nastavení** vyberte **Nastavení účtu** a pak vyberte **Profil organizace**.</span><span class="sxs-lookup"><span data-stu-id="4dc73-131">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="4dc73-132">Vyberte možnost **právní** a pak na kartě **partner** vyberte **obchodní umístění** a klikněte na **Přidat umístění.**</span><span class="sxs-lookup"><span data-stu-id="4dc73-132">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="4dc73-133">Zadejte požadované podrobnosti, včetně názvu firmy, adresy a kontaktu pro umístění, které chcete přidat do své společnosti.</span><span class="sxs-lookup"><span data-stu-id="4dc73-133">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="4dc73-134">Klikněte na **Přidat umístění**.</span><span class="sxs-lookup"><span data-stu-id="4dc73-134">Click **Add location**.</span></span> <span data-ttu-id="4dc73-135">Tím se vytvoří nové ID MPN pro nové umístění, které můžete použít pro transakce a pobídky CSP.</span><span class="sxs-lookup"><span data-stu-id="4dc73-135">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Přidat novou právní firmu":::

> [!NOTE]
> <span data-ttu-id="4dc73-137">Po přidání umístění do partnerského centra ho nejde odebrat.</span><span class="sxs-lookup"><span data-stu-id="4dc73-137">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="4dc73-138">Pokud jste pro přihlášení použili správné ID **MPN, zobrazí se v levé** nabídce centra pro partnery v nabídce vlevo.</span><span class="sxs-lookup"><span data-stu-id="4dc73-138">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="4dc73-139">Změnit zemi globálního účtu partnera</span><span class="sxs-lookup"><span data-stu-id="4dc73-139">Change country of Partner global account</span></span> 

1. <span data-ttu-id="4dc73-140">Přihlaste se pomocí účtu MPN v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="4dc73-140">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="4dc73-141">(Vaše přihlašovací údaje programu MPN se můžou lišit od vašich přihlašovacích údajů CSP).</span><span class="sxs-lookup"><span data-stu-id="4dc73-141">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="4dc73-142">Účet MPN by měl mít oprávnění globálního správce nebo správce účtů.</span><span class="sxs-lookup"><span data-stu-id="4dc73-142">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="4dc73-143">Na kartě **partner** klikněte na **obchodní umístění** a zkontrolujte seznam umístění a ujistěte se, že je v seznamu uvedeno umístění, které chcete použít jako právní entitu.</span><span class="sxs-lookup"><span data-stu-id="4dc73-143">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="4dc73-144">Chcete-li přidat umístění, klikněte na tlačítko **Přidat umístění** a za předpokladu zadejte požadované podrobnosti, včetně názvu firmy, adresy a primárního kontaktu pro umístění, které chcete přidat do své společnosti.</span><span class="sxs-lookup"><span data-stu-id="4dc73-144">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="4dc73-145">Vyberte možnost **změnit zemi** vedle rozevíracího seznamu **země/oblast** a postupujte podle pokynů.</span><span class="sxs-lookup"><span data-stu-id="4dc73-145">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Oficiální informace o obchodním profilu":::

5. <span data-ttu-id="4dc73-147">Klikněte na **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="4dc73-147">Click **Save**.</span></span>

6. <span data-ttu-id="4dc73-148">Země globálního účtu MPN se změní na novou právní zemi.</span><span class="sxs-lookup"><span data-stu-id="4dc73-148">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="4dc73-149">Další kroky</span><span class="sxs-lookup"><span data-stu-id="4dc73-149">Next steps</span></span>

- <span data-ttu-id="4dc73-150">Přečtěte si o [procesu ověřování](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="4dc73-150">Learn about the [verification process](verification-responses.md).</span></span>
