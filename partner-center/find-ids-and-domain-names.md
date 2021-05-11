---
title: Vyhledání ID tenanta, názvu domény, ID objektu uživatele
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak najít ID v Azure Portal – ID tenanta Azure AD organizace, název domény nebo KONKRÉTNÍ ID objektu uživatele. Některé úlohy tyto informace potřebují.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 643b1eeb96a47ee4c438f733efe3be22234d02ff
ms.sourcegitcommit: e462f562e7f26b7d6870c22638a2a841499109d6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/11/2021
ms.locfileid: "109740280"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="fa30f-104">Vyhledání důležitých ID pro uživatele</span><span class="sxs-lookup"><span data-stu-id="fa30f-104">Locate important IDs for a user</span></span>

<span data-ttu-id="fa30f-105">**Odpovídající role**</span><span class="sxs-lookup"><span data-stu-id="fa30f-105">**Appropriate roles**</span></span>

- <span data-ttu-id="fa30f-106">Globální správce</span><span class="sxs-lookup"><span data-stu-id="fa30f-106">Global admin</span></span>

<span data-ttu-id="fa30f-107">Tento článek popisuje, jak pomocí [Azure Portal](https://portal.azure.com/) najít pro uživatele následující informace:</span><span class="sxs-lookup"><span data-stu-id="fa30f-107">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="fa30f-108">ID Microsoft Azure Active Directory (Azure AD) organizace nebo společnosti uživatele</span><span class="sxs-lookup"><span data-stu-id="fa30f-108">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="fa30f-109">Primární název domény organizace nebo společnosti přidružené k tenantovi Azure AD</span><span class="sxs-lookup"><span data-stu-id="fa30f-109">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="fa30f-110">ID objektu uživatele</span><span class="sxs-lookup"><span data-stu-id="fa30f-110">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="fa30f-111">Vyhledání ID Microsoft Azure AD tenanta a názvu primární domény</span><span class="sxs-lookup"><span data-stu-id="fa30f-111">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="fa30f-112">Pomocí následujícího postupu vyhledejte ID tenanta azure AD nebo název primární domény v rámci Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="fa30f-112">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="fa30f-113">(Pokud chcete ID tenanta najít programově, podívejte se na stránku Vyhledání ID tenanta pomocí [PowerShellu nebo rozhraní příkazového řádku](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span><span class="sxs-lookup"><span data-stu-id="fa30f-113">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="fa30f-114">ID tenanta se v různých aplikacích nebo zdrojích může nazývat různé názvy.</span><span class="sxs-lookup"><span data-stu-id="fa30f-114">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="fa30f-115">ID tenanta může být například označováno jako ID adresáře, tenant Azure Active Directory (Azure AD), MICROSOFT ID nebo pro určité sestavy, a to i *tenantguid*.</span><span class="sxs-lookup"><span data-stu-id="fa30f-115">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="fa30f-116">Přihlaste se na [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="fa30f-116">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="fa30f-117">V **Azure Active Directory** vyberte Další.</span><span class="sxs-lookup"><span data-stu-id="fa30f-117">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Zobrazuje Azure Portal výběrem Azure Active Directory v nabídce.":::

3. <span data-ttu-id="fa30f-119">Zobrazí Azure Active Directory **přehledu.**</span><span class="sxs-lookup"><span data-stu-id="fa30f-119">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="fa30f-120">Pokud chcete zjistit ID tenanta Azure AD nebo název primární domény, vyhledejte pole **ID tenanta** a **pole Primární** doména.</span><span class="sxs-lookup"><span data-stu-id="fa30f-120">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="fa30f-121">Tato pole se zobrazí v části Informace o tenantovi.</span><span class="sxs-lookup"><span data-stu-id="fa30f-121">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Zobrazuje stránku Přehled se dvěma zvýrazněných poli: ID tenanta a název primární domény.":::

4. <span data-ttu-id="fa30f-123">ID tenanta můžete najít v Azure Portal několika dalšími způsoby.</span><span class="sxs-lookup"><span data-stu-id="fa30f-123">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="fa30f-124">V nabídce vyberte **Azure Active Directory** .</span><span class="sxs-lookup"><span data-stu-id="fa30f-124">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="fa30f-125">Pak v nabídce Najděte oddíl **Spravovat** a vyberte **vlastnosti**.</span><span class="sxs-lookup"><span data-stu-id="fa30f-125">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="fa30f-126">Na stránce vlastnosti se zobrazí také přidružené ID tenanta uživatele.</span><span class="sxs-lookup"><span data-stu-id="fa30f-126">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Zobrazí stránku vlastností se zvýrazněným polem ID tenanta.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="fa30f-128">Najít ID objektu uživatele</span><span class="sxs-lookup"><span data-stu-id="fa30f-128">Find the user object ID</span></span>

<span data-ttu-id="fa30f-129">Stačí najít název domény a ID tenanta nemusí být vždy dostatek.</span><span class="sxs-lookup"><span data-stu-id="fa30f-129">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="fa30f-130">Může být také nutné vyhledat konkrétní ID objektu přiřazené uživateli.</span><span class="sxs-lookup"><span data-stu-id="fa30f-130">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="fa30f-131">Pomocí těchto kroků můžete najít ID objektu uživatele v Azure Portal:</span><span class="sxs-lookup"><span data-stu-id="fa30f-131">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="fa30f-132">Přihlaste se na [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="fa30f-132">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="fa30f-133">V nabídce vyberte **Azure Active Directory** .</span><span class="sxs-lookup"><span data-stu-id="fa30f-133">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="fa30f-134">V nabídce najděte část **Správa** a pak vyberte **Uživatelé**.</span><span class="sxs-lookup"><span data-stu-id="fa30f-134">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Zobrazí nabídku Azure Active Directory se zvýrazněnou možností uživatelé.":::

4. <span data-ttu-id="fa30f-136">Na stránce Uživatelé zadejte do vyhledávacího pole jméno uživatele.</span><span class="sxs-lookup"><span data-stu-id="fa30f-136">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Zobrazí stránku Uživatelé s vyhledávacím polem pro vyhledání konkrétního uživatele.":::

5. <span data-ttu-id="fa30f-138">Vyberte jméno uživatele, kde se zobrazí v seznamu.</span><span class="sxs-lookup"><span data-stu-id="fa30f-138">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Zobrazí stránku uživatele zobrazující řádek vyhledávaného uživatele.":::

6. <span data-ttu-id="fa30f-140">Na stránce profilu uživatele Najděte oddíl identita.</span><span class="sxs-lookup"><span data-stu-id="fa30f-140">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="fa30f-141">Tady se zobrazí pole ID objektu s jedinečným ID objektu uživatele.</span><span class="sxs-lookup"><span data-stu-id="fa30f-141">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Zobrazuje stránku profilu uživatele s částí identita a jedno zvýrazněné pole pro ID objektu.":::

## <a name="next-steps"></a><span data-ttu-id="fa30f-143">Další kroky</span><span class="sxs-lookup"><span data-stu-id="fa30f-143">Next steps</span></span>

- [<span data-ttu-id="fa30f-144">Programové zjištění ID tenanta pomocí PowerShellu nebo rozhraní příkazového řádku</span><span class="sxs-lookup"><span data-stu-id="fa30f-144">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="fa30f-145">Další informace o profilech uživatelů v Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="fa30f-145">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="fa30f-146">Zjistěte, jak mohou partneři zobrazit nebo exportovat podrobnosti o zákazní Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="fa30f-146">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

