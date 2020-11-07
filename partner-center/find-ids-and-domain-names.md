---
title: Najít ID tenanta, název domény, ID objektu uživatele
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si, jak najít ID v Azure Portal-ID tenanta služby Azure AD, název domény nebo konkrétní ID objektu uživatele v organizaci. Tyto informace vyžadují některé úlohy.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: b88d6e11c7f4d56cf58d136a91b530688b3e5413
ms.sourcegitcommit: fdc32c0afce88f8266f75746ec15bf04745590ad
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/07/2020
ms.locfileid: "94360067"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="e9f1c-104">Vyhledat důležitá ID pro uživatele</span><span class="sxs-lookup"><span data-stu-id="e9f1c-104">Locate important IDs for a user</span></span>

<span data-ttu-id="e9f1c-105">Tento článek popisuje, jak pomocí [Azure Portal](https://portal.azure.com/) najít pro uživatele následující informace:</span><span class="sxs-lookup"><span data-stu-id="e9f1c-105">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="e9f1c-106">ID tenanta Microsoft Azure Active Directory (Azure AD) organizace nebo společnosti uživatele</span><span class="sxs-lookup"><span data-stu-id="e9f1c-106">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="e9f1c-107">Primární název domény organizace nebo společnosti přidružené k tenantovi Azure AD</span><span class="sxs-lookup"><span data-stu-id="e9f1c-107">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="e9f1c-108">ID objektu uživatele</span><span class="sxs-lookup"><span data-stu-id="e9f1c-108">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="e9f1c-109">Najít ID tenanta Microsoft Azure AD a název primární domény</span><span class="sxs-lookup"><span data-stu-id="e9f1c-109">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="e9f1c-110">Při hledání ID tenanta Azure AD nebo názvu primární domény v rámci Azure Portal postupujte podle těchto kroků.</span><span class="sxs-lookup"><span data-stu-id="e9f1c-110">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="e9f1c-111">(Pokud chcete ID tenanta najít programově, přečtěte si téma [Vyhledání ID tenanta pomocí PowerShellu nebo](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell)rozhraní příkazového řádku.)</span><span class="sxs-lookup"><span data-stu-id="e9f1c-111">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="e9f1c-112">ID tenanta se může v různých aplikacích a prostředcích volat jako jiné názvy.</span><span class="sxs-lookup"><span data-stu-id="e9f1c-112">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="e9f1c-113">ID klienta může být například označováno jako ID adresáře, tenant Azure Active Directory (Azure AD), Microsoft ID nebo pro určité sestavy, a to i pro *tenantguid*.</span><span class="sxs-lookup"><span data-stu-id="e9f1c-113">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="e9f1c-114">Přihlaste se k webu [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="e9f1c-114">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="e9f1c-115">V nabídce vyberte **Azure Active Directory** .</span><span class="sxs-lookup"><span data-stu-id="e9f1c-115">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Zobrazuje Azure Portal výběru možnosti Azure Active Directory z nabídky.":::

3. <span data-ttu-id="e9f1c-117">Zobrazí se stránka s **přehledem** Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e9f1c-117">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="e9f1c-118">Pokud chcete najít ID tenanta služby Azure AD nebo název primární domény, vyhledejte pole **ID tenanta** a **Primární doména** .</span><span class="sxs-lookup"><span data-stu-id="e9f1c-118">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="e9f1c-119">Tato pole se zobrazí v části informace o Tenantovi.</span><span class="sxs-lookup"><span data-stu-id="e9f1c-119">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Zobrazí stránku s přehledem se dvěma zvýrazněnými poli, ID tenanta a názvem primární domény.":::

4. <span data-ttu-id="e9f1c-121">ID tenanta můžete najít v Azure Portal několika dalšími způsoby.</span><span class="sxs-lookup"><span data-stu-id="e9f1c-121">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="e9f1c-122">V nabídce vyberte **Azure Active Directory** .</span><span class="sxs-lookup"><span data-stu-id="e9f1c-122">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="e9f1c-123">Pak v nabídce Najděte oddíl **Spravovat** a vyberte **vlastnosti**.</span><span class="sxs-lookup"><span data-stu-id="e9f1c-123">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="e9f1c-124">Na stránce vlastnosti se zobrazí také přidružené ID tenanta uživatele.</span><span class="sxs-lookup"><span data-stu-id="e9f1c-124">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Zobrazí stránku vlastností se zvýrazněným polem ID tenanta.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="e9f1c-126">Najít ID objektu uživatele</span><span class="sxs-lookup"><span data-stu-id="e9f1c-126">Find the user object ID</span></span>

<span data-ttu-id="e9f1c-127">Stačí najít název domény a ID tenanta nemusí být vždy dostatek.</span><span class="sxs-lookup"><span data-stu-id="e9f1c-127">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="e9f1c-128">Může být také nutné vyhledat konkrétní ID objektu přiřazené uživateli.</span><span class="sxs-lookup"><span data-stu-id="e9f1c-128">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="e9f1c-129">Pomocí těchto kroků můžete najít ID objektu uživatele v Azure Portal:</span><span class="sxs-lookup"><span data-stu-id="e9f1c-129">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="e9f1c-130">Přihlaste se k webu [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="e9f1c-130">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="e9f1c-131">V nabídce vyberte **Azure Active Directory** .</span><span class="sxs-lookup"><span data-stu-id="e9f1c-131">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="e9f1c-132">V nabídce najděte část **Správa** a pak vyberte **Uživatelé**.</span><span class="sxs-lookup"><span data-stu-id="e9f1c-132">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Zobrazí nabídku Azure Active Directory se zvýrazněnou možností uživatelé.":::

4. <span data-ttu-id="e9f1c-134">Na stránce Uživatelé zadejte do vyhledávacího pole jméno uživatele.</span><span class="sxs-lookup"><span data-stu-id="e9f1c-134">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Zobrazí stránku Uživatelé s vyhledávacím polem pro vyhledání konkrétního uživatele.":::

5. <span data-ttu-id="e9f1c-136">Vyberte jméno uživatele, kde se zobrazí v seznamu.</span><span class="sxs-lookup"><span data-stu-id="e9f1c-136">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Zobrazí stránku uživatele zobrazující řádek vyhledávaného uživatele.":::

6. <span data-ttu-id="e9f1c-138">Na stránce profilu uživatele Najděte oddíl identita.</span><span class="sxs-lookup"><span data-stu-id="e9f1c-138">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="e9f1c-139">Tady se zobrazí pole ID objektu s jedinečným ID objektu uživatele.</span><span class="sxs-lookup"><span data-stu-id="e9f1c-139">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Zobrazuje stránku profilu uživatele s částí identita a jedno zvýrazněné pole pro ID objektu.":::

## <a name="next-steps"></a><span data-ttu-id="e9f1c-141">Další kroky</span><span class="sxs-lookup"><span data-stu-id="e9f1c-141">Next steps</span></span>

- [<span data-ttu-id="e9f1c-142">Programové zjištění ID tenanta pomocí PowerShellu nebo rozhraní příkazového řádku</span><span class="sxs-lookup"><span data-stu-id="e9f1c-142">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="e9f1c-143">Další informace o uživatelských profilech v Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="e9f1c-143">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="e9f1c-144">Zjistěte, jak můžou partneři zobrazit nebo exportovat podrobnosti o zákaznících v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="e9f1c-144">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)
