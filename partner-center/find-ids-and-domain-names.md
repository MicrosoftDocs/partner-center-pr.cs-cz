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
ms.openlocfilehash: 17b0100bf5e45e931a765a73fb98afddf6dba656
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172247"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="94d13-104">Vyhledat důležitá ID pro uživatele</span><span class="sxs-lookup"><span data-stu-id="94d13-104">Locate important IDs for a user</span></span>

<span data-ttu-id="94d13-105">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="94d13-105">**Appropriate roles**</span></span>

- <span data-ttu-id="94d13-106">Globální správce</span><span class="sxs-lookup"><span data-stu-id="94d13-106">Global admin</span></span>

<span data-ttu-id="94d13-107">Tento článek popisuje, jak pomocí [Azure Portal](https://portal.azure.com/) najít pro uživatele následující informace:</span><span class="sxs-lookup"><span data-stu-id="94d13-107">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="94d13-108">ID tenanta Microsoft Azure Active Directory (Azure AD) organizace nebo společnosti uživatele</span><span class="sxs-lookup"><span data-stu-id="94d13-108">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="94d13-109">Primární název domény organizace nebo společnosti přidružené k tenantovi Azure AD</span><span class="sxs-lookup"><span data-stu-id="94d13-109">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="94d13-110">ID objektu uživatele</span><span class="sxs-lookup"><span data-stu-id="94d13-110">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="94d13-111">Najít ID tenanta Microsoft Azure AD a název primární domény</span><span class="sxs-lookup"><span data-stu-id="94d13-111">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="94d13-112">Při hledání ID tenanta Azure AD nebo názvu primární domény v rámci Azure Portal postupujte podle těchto kroků.</span><span class="sxs-lookup"><span data-stu-id="94d13-112">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="94d13-113">(Pokud chcete ID tenanta najít programově, přečtěte si téma [Vyhledání ID tenanta pomocí PowerShellu nebo](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell)rozhraní příkazového řádku.)</span><span class="sxs-lookup"><span data-stu-id="94d13-113">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="94d13-114">ID tenanta se může v různých aplikacích a prostředcích volat jako jiné názvy.</span><span class="sxs-lookup"><span data-stu-id="94d13-114">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="94d13-115">ID klienta může být například označováno jako ID adresáře, tenant Azure Active Directory (Azure AD), Microsoft ID nebo pro určité sestavy, a to i pro *tenantguid*.</span><span class="sxs-lookup"><span data-stu-id="94d13-115">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="94d13-116">Přihlaste se na [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="94d13-116">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="94d13-117">V nabídce vyberte **Azure Active Directory** .</span><span class="sxs-lookup"><span data-stu-id="94d13-117">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Zobrazuje Azure Portal výběru možnosti Azure Active Directory z nabídky.":::

3. <span data-ttu-id="94d13-119">Zobrazí se stránka s **přehledem** Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="94d13-119">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="94d13-120">Pokud chcete najít ID tenanta služby Azure AD nebo název primární domény, vyhledejte pole **ID tenanta** a **Primární doména** .</span><span class="sxs-lookup"><span data-stu-id="94d13-120">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="94d13-121">Tato pole se zobrazí v části informace o Tenantovi.</span><span class="sxs-lookup"><span data-stu-id="94d13-121">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Zobrazí stránku s přehledem se dvěma zvýrazněnými poli, ID tenanta a názvem primární domény.":::

4. <span data-ttu-id="94d13-123">ID tenanta můžete najít v Azure Portal několika dalšími způsoby.</span><span class="sxs-lookup"><span data-stu-id="94d13-123">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="94d13-124">V nabídce vyberte **Azure Active Directory** .</span><span class="sxs-lookup"><span data-stu-id="94d13-124">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="94d13-125">Pak v nabídce Najděte oddíl **Spravovat** a vyberte **vlastnosti**.</span><span class="sxs-lookup"><span data-stu-id="94d13-125">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="94d13-126">Na stránce vlastnosti se zobrazí také přidružené ID tenanta uživatele.</span><span class="sxs-lookup"><span data-stu-id="94d13-126">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Zobrazí stránku vlastností se zvýrazněným polem ID tenanta.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="94d13-128">Najít ID objektu uživatele</span><span class="sxs-lookup"><span data-stu-id="94d13-128">Find the user object ID</span></span>

<span data-ttu-id="94d13-129">Stačí najít název domény a ID tenanta nemusí být vždy dostatek.</span><span class="sxs-lookup"><span data-stu-id="94d13-129">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="94d13-130">Může být také nutné vyhledat konkrétní ID objektu přiřazené uživateli.</span><span class="sxs-lookup"><span data-stu-id="94d13-130">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="94d13-131">Pomocí těchto kroků můžete najít ID objektu uživatele v Azure Portal:</span><span class="sxs-lookup"><span data-stu-id="94d13-131">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="94d13-132">Přihlaste se na [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="94d13-132">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="94d13-133">V nabídce vyberte **Azure Active Directory** .</span><span class="sxs-lookup"><span data-stu-id="94d13-133">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="94d13-134">V nabídce najděte část **Správa** a pak vyberte **Uživatelé**.</span><span class="sxs-lookup"><span data-stu-id="94d13-134">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Zobrazí nabídku Azure Active Directory se zvýrazněnou možností uživatelé.":::

4. <span data-ttu-id="94d13-136">Na stránce Uživatelé zadejte do vyhledávacího pole jméno uživatele.</span><span class="sxs-lookup"><span data-stu-id="94d13-136">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Zobrazí stránku Uživatelé s vyhledávacím polem pro vyhledání konkrétního uživatele.":::

5. <span data-ttu-id="94d13-138">Vyberte jméno uživatele, kde se zobrazí v seznamu.</span><span class="sxs-lookup"><span data-stu-id="94d13-138">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Zobrazí stránku uživatele zobrazující řádek vyhledávaného uživatele.":::

6. <span data-ttu-id="94d13-140">Na stránce profilu uživatele Najděte oddíl identita.</span><span class="sxs-lookup"><span data-stu-id="94d13-140">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="94d13-141">Tady se zobrazí pole ID objektu s jedinečným ID objektu uživatele.</span><span class="sxs-lookup"><span data-stu-id="94d13-141">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Zobrazuje stránku profilu uživatele s částí identita a jedno zvýrazněné pole pro ID objektu.":::

## <a name="next-steps"></a><span data-ttu-id="94d13-143">Další kroky</span><span class="sxs-lookup"><span data-stu-id="94d13-143">Next steps</span></span>

- [<span data-ttu-id="94d13-144">Programové zjištění ID tenanta pomocí PowerShellu nebo rozhraní příkazového řádku</span><span class="sxs-lookup"><span data-stu-id="94d13-144">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="94d13-145">Další informace o uživatelských profilech v Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="94d13-145">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="94d13-146">Zjistěte, jak můžou partneři zobrazit nebo exportovat podrobnosti o zákaznících v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="94d13-146">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

