---
title: Správa umístění v partnerském účtu
ms.topic: how-to
ms.date: 01/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Naučte se, jak přidat nové umístění a jak se v programu motivačních programů, v obchodních předplatných, předplatných a dalších transakcích používá umístění MPN ID.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 38ea8a451f51d80998643e2a023420ea3efaa6ba
ms.sourcegitcommit: e99882e9b6c9b1a0f7427fb133693b1d977be76b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/26/2021
ms.locfileid: "98773431"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="07683-103">Správa umístění účtu MPN a přidání nového umístění</span><span class="sxs-lookup"><span data-stu-id="07683-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="07683-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="07683-104">**Appropriate roles**</span></span>

- <span data-ttu-id="07683-105">Globální správce</span><span class="sxs-lookup"><span data-stu-id="07683-105">Global admin</span></span>
- <span data-ttu-id="07683-106">Správce účtu</span><span class="sxs-lookup"><span data-stu-id="07683-106">Account admin</span></span>

<span data-ttu-id="07683-107">ID MPN umístění identifikuje každé konkrétní umístění vaší společnosti.</span><span class="sxs-lookup"><span data-stu-id="07683-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="07683-108">K registraci v programu motivačních programů použijete umístění MPN ID, a to za transakčního poskytovatele řešení cloudu (CSP) a další obchodní transakce.</span><span class="sxs-lookup"><span data-stu-id="07683-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="07683-109">Globální ID MPN se používá pro netransakční aktivity, například žádosti o podporu.</span><span class="sxs-lookup"><span data-stu-id="07683-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="07683-110">Následuje typický scénář:</span><span class="sxs-lookup"><span data-stu-id="07683-110">The following is a typical scenario:</span></span>

<span data-ttu-id="07683-111">Společnost Contoso má svůj partnerský globální účet (PGA) ve Spojeném království.</span><span class="sxs-lookup"><span data-stu-id="07683-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="07683-112">Jedná se o své registrované právní firmy a globální ID MPN se používá ke správě všech netransakčních obchodních činností.</span><span class="sxs-lookup"><span data-stu-id="07683-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="07683-113">Společnost Contoso má také partnerské účty partnera (PLA) rovnocenné dceřiným společnostem nebo divizím v jiném umístění v USA, Francii a USA.</span><span class="sxs-lookup"><span data-stu-id="07683-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="07683-114">Ve struktuře účtu MPN se tyto PLAs reprezentují jako jedinečná ID MPN.</span><span class="sxs-lookup"><span data-stu-id="07683-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="07683-115">PLAs se používají pro transakční firmy, jako je CSP nebo pobídky programů.</span><span class="sxs-lookup"><span data-stu-id="07683-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="07683-116">Výběry jsou vázané na konkrétní umístění.</span><span class="sxs-lookup"><span data-stu-id="07683-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="07683-117">Mezi klientem CSP a ID umístění MPN je 1-1 vztah.</span><span class="sxs-lookup"><span data-stu-id="07683-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Struktura míst MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-location-for-a-csp-business"></a><span data-ttu-id="07683-119">Požadavky, aby bylo možné přidat nové umístění účtu pro firmu CSP</span><span class="sxs-lookup"><span data-stu-id="07683-119">Prerequisites in order to add a new account location for a CSP business</span></span>

<span data-ttu-id="07683-120">Chcete-li přidat nové obchodní umístění CSP, je k dispozici několik požadavků:</span><span class="sxs-lookup"><span data-stu-id="07683-120">To add a new CSP business location, there are several prerequisites:</span></span>

1. <span data-ttu-id="07683-121">V zemi, kde chcete provádět podnikání, musíte mít umístění MPN ID.</span><span class="sxs-lookup"><span data-stu-id="07683-121">You must have a location MPN ID in the country where you want to do business.</span></span>

1. <span data-ttu-id="07683-122">Budete potřebovat nového tenanta Azure AD v [oblasti podnikání](regional-authorization-overview.md) , která ještě není zaregistrovaná ve zprostředkovateli CSP.</span><span class="sxs-lookup"><span data-stu-id="07683-122">You need a new Azure AD tenant in the [region of business](regional-authorization-overview.md) which is not already enrolled into CSP.</span></span> <span data-ttu-id="07683-123">Tuto vytvořit, když se zaregistrujete v CSP.</span><span class="sxs-lookup"><span data-stu-id="07683-123">Create this when you enroll in CSP.</span></span>
 
3. <span data-ttu-id="07683-124">Použijte nového tenanta AAD k registraci do programu CSP v oblasti.</span><span class="sxs-lookup"><span data-stu-id="07683-124">Use the new AAD tenant to enroll into CSP program in the region.</span></span>
<span data-ttu-id="07683-125">Poskytování právních informací o společnosti, včetně právního jména společnosti, adresy, primárního kontaktního údaje.</span><span class="sxs-lookup"><span data-stu-id="07683-125">Providing legal company details including the legal company name, address, primary contact details.</span></span> <span data-ttu-id="07683-126">Tento účet se bude podrobit ověření, takže nezapomeňte přidat platné informace.</span><span class="sxs-lookup"><span data-stu-id="07683-126">This account will undergo verification, so make sure to add valid information.</span></span>

>[!NOTE] 
 ><span data-ttu-id="07683-127">Nezapomeňte se přihlásit pomocí **nových** přihlašovacích údajů pro **nového** tenanta Azure AD.</span><span class="sxs-lookup"><span data-stu-id="07683-127">Remember to sign in with the **new** credentials for the **new** Azure AD tenant.</span></span> <span data-ttu-id="07683-128">Nepoužívejte svoje stávající přihlašovací údaje, protože Partnerské centrum vám rozpozná, jak už účet máte.</span><span class="sxs-lookup"><span data-stu-id="07683-128">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

4. <span data-ttu-id="07683-129">Přijměte smlouvu s partnerem Microsoftu a aktivujte účet.</span><span class="sxs-lookup"><span data-stu-id="07683-129">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="07683-130">Přidat umístění MPN</span><span class="sxs-lookup"><span data-stu-id="07683-130">Add an MPN location</span></span>

1. <span data-ttu-id="07683-131">Přihlaste se pomocí účtu MPN v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="07683-131">Sign in using the MPN account in Partner Center .</span></span> <span data-ttu-id="07683-132">Účet MPN by měl mít oprávnění globálního správce nebo správce účtů.</span><span class="sxs-lookup"><span data-stu-id="07683-132">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="07683-133">V **ikoně nastavení** vyberte **Nastavení organizace**.</span><span class="sxs-lookup"><span data-stu-id="07683-133">From the **Setting icon**, select the **Organization settings**.</span></span>

2. <span data-ttu-id="07683-134">Vyberte **právní** a potom vyberte **umístění.**</span><span class="sxs-lookup"><span data-stu-id="07683-134">Select **Legal** and then select **Locations.**</span></span>

3. <span data-ttu-id="07683-135">Vyberte **Přidat umístění** a vložte podrobnosti o umístění, které chcete přidat do své společnosti, i k primárnímu kontaktu pro dané umístění.</span><span class="sxs-lookup"><span data-stu-id="07683-135">Select **Add a location**, and insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="07683-136">Po přidání umístění do partnerského centra ho nejde odebrat.</span><span class="sxs-lookup"><span data-stu-id="07683-136">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="07683-137">Pokud jste pro přihlášení použili správné ID **MPN, zobrazí se v levé** nabídce centra pro partnery v nabídce vlevo.</span><span class="sxs-lookup"><span data-stu-id="07683-137">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-global-partner-account-location"></a><span data-ttu-id="07683-138">Změnit umístění globálního účtu partnera</span><span class="sxs-lookup"><span data-stu-id="07683-138">Change Global partner account location</span></span>

1. <span data-ttu-id="07683-139">V části **[obchodní umístění](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)** zkontrolujte seznam umístění a ujistěte se, že je v seznamu uvedeno umístění, které chcete jako právní entita.</span><span class="sxs-lookup"><span data-stu-id="07683-139">On **[Business locations](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)**, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="07683-140">Pokud není, přidejte ho.</span><span class="sxs-lookup"><span data-stu-id="07683-140">If it isn't, add it.</span></span>

   :::image type="content" source="images/accountsettings/location1.png" alt-text="Snímek obrazovky se stránkou pro umístění účtů partnerského centra se seznamem všech aktuálních umístění":::

2. <span data-ttu-id="07683-142">Vyberte **právní** a pak vyberte **aktualizovat platný obchodní profil** .</span><span class="sxs-lookup"><span data-stu-id="07683-142">Select **Legal** and then select **Update legal business profile**</span></span>
  
3. <span data-ttu-id="07683-143">Vyberte oblast a právní entitu a **odešlete** ji.</span><span class="sxs-lookup"><span data-stu-id="07683-143">Select the region and legal entity and **Submit** it.</span></span>

  
## <a name="next-steps"></a><span data-ttu-id="07683-144">Další kroky</span><span class="sxs-lookup"><span data-stu-id="07683-144">Next steps</span></span>

- <span data-ttu-id="07683-145">Přečtěte si o [procesu ověřování](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="07683-145">Learn about the [verification process](verification-responses.md).</span></span>
