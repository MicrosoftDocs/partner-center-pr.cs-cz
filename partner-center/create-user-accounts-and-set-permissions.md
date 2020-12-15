---
title: Vytváření uživatelských účtů a přiřazování rolí
description: Každý zaměstnanec musí mít přiřazenou roli, aby mohl získat přístup k partnerskému centru. Naučte se vytvářet uživatelské účty, přiřazovat role a nastavovat oprávnění.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperf-fy21q2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: c8fad4432f9aabba69877d80038ec9e2665c639d
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/15/2020
ms.locfileid: "97492530"
---
# <a name="create-user-accounts"></a><span data-ttu-id="9fffb-104">Vytváření uživatelských účtů</span><span class="sxs-lookup"><span data-stu-id="9fffb-104">Create user accounts</span></span>  

<span data-ttu-id="9fffb-105">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="9fffb-105">**Appropriate roles**</span></span>

- <span data-ttu-id="9fffb-106">Správce účtu</span><span class="sxs-lookup"><span data-stu-id="9fffb-106">Account admin</span></span>
- <span data-ttu-id="9fffb-107">Globální správce</span><span class="sxs-lookup"><span data-stu-id="9fffb-107">Global admin</span></span>
- <span data-ttu-id="9fffb-108">Správce správy uživatelů</span><span class="sxs-lookup"><span data-stu-id="9fffb-108">User management admin</span></span>

<span data-ttu-id="9fffb-109">Vytvořte uživatelské účty pro zaměstnance, kteří potřebují přístup k partnerskému centru.</span><span class="sxs-lookup"><span data-stu-id="9fffb-109">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="9fffb-110">Tyto úlohy musí provádět správce správy uživatelů, účty správce nebo globální správce. Uživatel, který provádí tyto úlohy, musí také přiřadit role Azure Active Directory (AAD) Správce uživatelů nebo globální správce.</span><span class="sxs-lookup"><span data-stu-id="9fffb-110">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="9fffb-111">Další informace o rolích AAD najdete v tématu [oprávnění role správce v Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="9fffb-111">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>

## <a name="add-a-new-user"></a><span data-ttu-id="9fffb-112">Přidání nového uživatele</span><span class="sxs-lookup"><span data-stu-id="9fffb-112">Add a new user</span></span>

1. <span data-ttu-id="9fffb-113">Z ikony **Nastavení** v pravém horním rohu partnerského centra vyberte **Nastavení účtu** a pak vyberte **Správa uživatelů**.</span><span class="sxs-lookup"><span data-stu-id="9fffb-113">From the **Settings** icon at the top right of the Partner Center, select **Account settings** and then select **User management**.</span></span>

2. <span data-ttu-id="9fffb-114">Vyberte možnost **Přidat uživatele**.</span><span class="sxs-lookup"><span data-stu-id="9fffb-114">Select **Add user**.</span></span>

3. <span data-ttu-id="9fffb-115">Zadejte celé jméno uživatele a jedinečnou e-mailovou adresu.</span><span class="sxs-lookup"><span data-stu-id="9fffb-115">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="9fffb-116">Vyberte typ agenta nebo typu správce, kterého chcete přiřadit uživateli.</span><span class="sxs-lookup"><span data-stu-id="9fffb-116">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="9fffb-117">Přístup k partnerskému centru je založený na rolích, takže můžete přiřadit oprávnění k přizpůsobení zobrazení uživatele, aby se zobrazily jenom ty funkce, které uživatel potřebuje k dokončení konkrétních úkolů.</span><span class="sxs-lookup"><span data-stu-id="9fffb-117">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="9fffb-118">Pokud uživatelé chtějí přiřazení role, můžou najít globální správce, aby se obrátili na **správu uživatelů** a filtrování na globálním správci.</span><span class="sxs-lookup"><span data-stu-id="9fffb-118">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="9fffb-119">Výběrem **Přidat** vytvořte uživatelský účet.</span><span class="sxs-lookup"><span data-stu-id="9fffb-119">Select **Add** to create the user account.</span></span> <span data-ttu-id="9fffb-120">Potvrďte podrobnosti uživatele na další stránce.</span><span class="sxs-lookup"><span data-stu-id="9fffb-120">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="9fffb-121">Poznamenejte si informace o přihlášení nového uživatele zobrazené na této stránce.</span><span class="sxs-lookup"><span data-stu-id="9fffb-121">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="9fffb-122">Nezapomeňte tyto informace zkopírovat a odeslat novému uživateli, protože k němu už nebudete mít přístup později.</span><span class="sxs-lookup"><span data-stu-id="9fffb-122">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 

<span data-ttu-id="9fffb-123">Uživatel se bude muset přihlásit do partnerského centra s uživatelským jménem a dočasným heslem.</span><span class="sxs-lookup"><span data-stu-id="9fffb-123">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="9fffb-124">Když se uživatel poprvé přihlásí k partnerskému centru, zobrazí se výzva ke změně hesla.</span><span class="sxs-lookup"><span data-stu-id="9fffb-124">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span>

## <a name="assign-user-roles"></a><span data-ttu-id="9fffb-125">Přiřazení uživatelských rolí</span><span class="sxs-lookup"><span data-stu-id="9fffb-125">Assign user roles</span></span>

<span data-ttu-id="9fffb-126">Pokud chcete pracovat v partnerském centru, musíte mít přiřazenou roli.</span><span class="sxs-lookup"><span data-stu-id="9fffb-126">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="9fffb-127">V současné době role zahrnují Azure Active Directory role tenanta, role poskytovatele Cloud Solution Provider (CSP) a role společnosti bez AAD.</span><span class="sxs-lookup"><span data-stu-id="9fffb-127">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="9fffb-128">Každá z těchto rolí může mít jednotlivé společnosti potřebnou.</span><span class="sxs-lookup"><span data-stu-id="9fffb-128">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="9fffb-129">Jednotlivci musí být uvedeni ve vašem tenantovi pro přístup k partnerskému centru.</span><span class="sxs-lookup"><span data-stu-id="9fffb-129">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="9fffb-130">Přiřazení rolí poskytují další přístup.</span><span class="sxs-lookup"><span data-stu-id="9fffb-130">Role assignments provide additional access.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9fffb-131">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9fffb-131">Next steps</span></span>

- [<span data-ttu-id="9fffb-132">Přiřazení rolí a oprávnění uživatelů pro zaměstnance, kteří potřebují pracovat v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="9fffb-132">Assign users roles and permissions for employees needing to work in Partner Center</span></span>](permissions-overview.md)
