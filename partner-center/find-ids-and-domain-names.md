---
title: Vyhledání ID tenanta, názvu domény, ID objektu uživatele
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak najít ID v Azure Portal – ID tenanta Azure AD organizace, název domény nebo ID konkrétního objektu uživatele. Některé úlohy tyto informace potřebují.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 5da41cdbfa7aa1780b31e170a2398e8e7c65df27
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150858"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="72ef1-104">Vyhledání důležitých ID pro uživatele</span><span class="sxs-lookup"><span data-stu-id="72ef1-104">Locate important IDs for a user</span></span>

<span data-ttu-id="72ef1-105">**Odpovídající role:** Globální správce</span><span class="sxs-lookup"><span data-stu-id="72ef1-105">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="72ef1-106">Tento článek popisuje, jak pomocí [Azure Portal](https://portal.azure.com/) najít pro uživatele následující informace:</span><span class="sxs-lookup"><span data-stu-id="72ef1-106">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="72ef1-107">ID Microsoft Azure Active Directory (Azure AD) organizace nebo společnosti uživatele</span><span class="sxs-lookup"><span data-stu-id="72ef1-107">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="72ef1-108">Primární název domény organizace nebo společnosti přidružené k tenantovi Azure AD</span><span class="sxs-lookup"><span data-stu-id="72ef1-108">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="72ef1-109">ID objektu uživatele</span><span class="sxs-lookup"><span data-stu-id="72ef1-109">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="72ef1-110">Vyhledání ID Microsoft Azure AD tenanta a názvu primární domény</span><span class="sxs-lookup"><span data-stu-id="72ef1-110">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="72ef1-111">Pomocí následujícího postupu vyhledejte ID tenanta Azure AD nebo název primární domény v rámci Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="72ef1-111">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="72ef1-112">(Pokud chcete ID tenanta najít programově, podívejte se na stránku Vyhledání ID tenanta pomocí [PowerShellu nebo rozhraní příkazového řádku](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span><span class="sxs-lookup"><span data-stu-id="72ef1-112">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="72ef1-113">ID tenanta se v různých aplikacích nebo zdrojích může nazývat různé názvy.</span><span class="sxs-lookup"><span data-stu-id="72ef1-113">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="72ef1-114">ID tenanta může být například označováno jako ID adresáře, tenant Azure Active Directory (Azure AD), MICROSOFT ID nebo pro určité sestavy, a to i *tenantguid*.</span><span class="sxs-lookup"><span data-stu-id="72ef1-114">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="72ef1-115">Přihlaste se na [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="72ef1-115">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="72ef1-116">V **Azure Active Directory** vyberte Další.</span><span class="sxs-lookup"><span data-stu-id="72ef1-116">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Zobrazuje Azure Portal výběrem Azure Active Directory v nabídce.":::

3. <span data-ttu-id="72ef1-118">Zobrazí Azure Active Directory **přehledu.**</span><span class="sxs-lookup"><span data-stu-id="72ef1-118">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="72ef1-119">Pokud chcete najít ID tenanta Azure AD nebo název primární domény, vyhledejte pole **ID tenanta** a **pole Primární** doména.</span><span class="sxs-lookup"><span data-stu-id="72ef1-119">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="72ef1-120">Tato pole se zobrazí v části Informace o tenantovi.</span><span class="sxs-lookup"><span data-stu-id="72ef1-120">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Zobrazuje stránku Přehled se dvěma zvýrazněných poli: ID tenanta a název primární domény.":::

4. <span data-ttu-id="72ef1-122">ID tenanta můžete najít v Azure Portal několika dalšími způsoby.</span><span class="sxs-lookup"><span data-stu-id="72ef1-122">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="72ef1-123">V nabídce vyberte **Azure Active Directory** .</span><span class="sxs-lookup"><span data-stu-id="72ef1-123">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="72ef1-124">Pak v nabídce Najděte oddíl **Spravovat** a vyberte **vlastnosti**.</span><span class="sxs-lookup"><span data-stu-id="72ef1-124">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="72ef1-125">Na stránce vlastnosti se zobrazí také přidružené ID tenanta uživatele.</span><span class="sxs-lookup"><span data-stu-id="72ef1-125">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Zobrazí stránku vlastností se zvýrazněným polem ID tenanta.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="72ef1-127">Najít ID objektu uživatele</span><span class="sxs-lookup"><span data-stu-id="72ef1-127">Find the user object ID</span></span>

<span data-ttu-id="72ef1-128">Stačí najít název domény a ID tenanta nemusí být vždy dostatek.</span><span class="sxs-lookup"><span data-stu-id="72ef1-128">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="72ef1-129">Může být také nutné vyhledat konkrétní ID objektu přiřazené uživateli.</span><span class="sxs-lookup"><span data-stu-id="72ef1-129">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="72ef1-130">Pomocí těchto kroků můžete najít ID objektu uživatele v Azure Portal:</span><span class="sxs-lookup"><span data-stu-id="72ef1-130">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="72ef1-131">Přihlaste se na [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="72ef1-131">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="72ef1-132">V nabídce vyberte **Azure Active Directory** .</span><span class="sxs-lookup"><span data-stu-id="72ef1-132">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="72ef1-133">V nabídce najděte část **Správa** a pak vyberte **Uživatelé**.</span><span class="sxs-lookup"><span data-stu-id="72ef1-133">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Zobrazí nabídku Azure Active Directory se zvýrazněnou možností uživatelé.":::

4. <span data-ttu-id="72ef1-135">Na stránce Uživatelé zadejte do vyhledávacího pole jméno uživatele.</span><span class="sxs-lookup"><span data-stu-id="72ef1-135">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Zobrazí stránku Uživatelé s vyhledávacím polem pro vyhledání konkrétního uživatele.":::

5. <span data-ttu-id="72ef1-137">Vyberte jméno uživatele, kde se zobrazí v seznamu.</span><span class="sxs-lookup"><span data-stu-id="72ef1-137">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Zobrazí stránku uživatele zobrazující řádek vyhledávaného uživatele.":::

6. <span data-ttu-id="72ef1-139">Na stránce profilu uživatele Najděte oddíl identita.</span><span class="sxs-lookup"><span data-stu-id="72ef1-139">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="72ef1-140">Tady se zobrazí pole ID objektu s jedinečným ID objektu uživatele.</span><span class="sxs-lookup"><span data-stu-id="72ef1-140">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Zobrazuje stránku profilu uživatele s částí identita a jedno zvýrazněné pole pro ID objektu.":::

## <a name="next-steps"></a><span data-ttu-id="72ef1-142">Další kroky</span><span class="sxs-lookup"><span data-stu-id="72ef1-142">Next steps</span></span>

- [<span data-ttu-id="72ef1-143">Programové zjištění ID tenanta pomocí PowerShellu nebo rozhraní příkazového řádku</span><span class="sxs-lookup"><span data-stu-id="72ef1-143">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="72ef1-144">Další informace o uživatelských profilech v Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="72ef1-144">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="72ef1-145">Zjistěte, jak můžou partneři zobrazit nebo exportovat podrobnosti o zákaznících v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="72ef1-145">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

