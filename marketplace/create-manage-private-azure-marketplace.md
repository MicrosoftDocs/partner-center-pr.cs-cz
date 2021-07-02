---
title: Vytvoření a Správa privátních Azure Marketplace v Azure Portal
description: Seznamte se s vytvářením a správou privátních Azure Marketplace (Preview) v Azure Portal. Privátní Azure Marketplace (Preview) umožňuje správcům řídit, která řešení třetích stran můžou uživatelé používat.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 8a3ffbe5b57c49004518341d27c785dcd1b9ce87
ms.sourcegitcommit: c4601069340445135b551fa96bee6d9923d8aa97
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/01/2021
ms.locfileid: "113173694"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="d348e-104">Vytvoření a Správa privátních Azure Marketplace v Azure Portal</span><span class="sxs-lookup"><span data-stu-id="d348e-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="d348e-105">Privátní Azure Marketplace umožňuje správcům řídit, která řešení třetích stran můžou uživatelé používat.</span><span class="sxs-lookup"><span data-stu-id="d348e-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="d348e-106">Tím umožníte uživateli nasadit jenom nabídky, které schválil správce a splní zásady vaší organizace.</span><span class="sxs-lookup"><span data-stu-id="d348e-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="d348e-107">Pomocí privátních Azure Marketplace můžou uživatelé v online obchodu vyhledat odpovídající nabídky k nákupu a nasazení.</span><span class="sxs-lookup"><span data-stu-id="d348e-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="d348e-108">Jako správce Marketplace (přiřazená role) začnete s neaktivním a prázdným soukromým úložištěm, kde můžete přidat vaše schválené nabídky a plány.</span><span class="sxs-lookup"><span data-stu-id="d348e-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="d348e-109">Tento článek vysvětluje, jak přiřadit potřebnou roli, vytvořit privátní úložiště, spravovat položky, schvalovat požadavky uživatelů a povolit pro uživatele soukromé Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="d348e-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="d348e-110">Soukromé Azure Marketplace jsou na úrovni tenanta, takže všichni uživatelé v tenantovi uvidí stejný seznam.</span><span class="sxs-lookup"><span data-stu-id="d348e-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="d348e-111">Všechna řešení společnosti Microsoft (včetně schválených [distribucí systému Linux](/azure/virtual-machines/linux/endorsed-distros)) jsou automaticky přidána do privátního Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="d348e-111">All Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="d348e-112">Přiřazení role správce Marketplace</span><span class="sxs-lookup"><span data-stu-id="d348e-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="d348e-113">Globální správce tenanta musí přiřadit roli **správce Marketplace** správci privátního Azure Marketplace, který bude spravovat soukromé úložiště.</span><span class="sxs-lookup"><span data-stu-id="d348e-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="d348e-114">Přístup ke správě privátních Azure Marketplace je k dispozici jenom správcům IT, kteří mají přiřazenou roli správce Marketplace.</span><span class="sxs-lookup"><span data-stu-id="d348e-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="d348e-115">Požadavky</span><span class="sxs-lookup"><span data-stu-id="d348e-115">Prerequisites</span></span>

<span data-ttu-id="d348e-116">Tyto požadavky jsou nutné, aby bylo možné přiřadit roli správce webu Marketplace uživateli v oboru tenanta:</span><span class="sxs-lookup"><span data-stu-id="d348e-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="d348e-117">Máte přístup k uživateli **globálního správce** .</span><span class="sxs-lookup"><span data-stu-id="d348e-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="d348e-118">Tenant má minimálně jedno předplatné (může to být libovolný typ).</span><span class="sxs-lookup"><span data-stu-id="d348e-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="d348e-119">Pro globálního správce se uživateli přiřadí role **Přispěvatel** nebo vyšší pro vybrané předplatné.</span><span class="sxs-lookup"><span data-stu-id="d348e-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="d348e-120">Přiřazení role správce Marketplace k řízení přístupu (IAM)</span><span class="sxs-lookup"><span data-stu-id="d348e-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="d348e-121">Přihlaste se na [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="d348e-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

1. <span data-ttu-id="d348e-122">Vyberte **všechny služby** a potom **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="d348e-122">Select **All services** and then **Marketplace**.</span></span>

1. <span data-ttu-id="d348e-123">V nabídce na levé straně vyberte **soukromé tržiště** .</span><span class="sxs-lookup"><span data-stu-id="d348e-123">Select **Private Marketplace** from the menu on the left.</span></span>

   :::image type="content" source="media/private-azure/private-marketplace.png" lightbox="media/private-azure/private-marketplace-zoom.png" alt-text="Zobrazuje možnost nabídky privátní Marketplace na levé straně webu Marketplace.":::

1. <span data-ttu-id="d348e-125">Vyberte **řízení přístupu (IAM)** a přiřaďte roli správce webu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="d348e-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

   :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Zobrazuje obrazovku řízení přístupu I M.":::

1. <span data-ttu-id="d348e-127">Vyberte **+ Přidat** > **Přidat přiřazení role**.</span><span class="sxs-lookup"><span data-stu-id="d348e-127">Select **+ Add** > **Add role assignment**.</span></span>

1. <span data-ttu-id="d348e-128">V části **role** vyberte **správce Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="d348e-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Zobrazuje nabídku přiřazení role.":::

1. <span data-ttu-id="d348e-130">V rozevíracím seznamu vyberte požadovaného uživatele a potom vyberte **Hotovo**.</span><span class="sxs-lookup"><span data-stu-id="d348e-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="d348e-131">Přiřazení role správce Marketplace k PowerShellu</span><span class="sxs-lookup"><span data-stu-id="d348e-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="d348e-132">K přiřazení role správce Marketplace použijte následující skript prostředí PowerShell; vyžaduje následující parametry:</span><span class="sxs-lookup"><span data-stu-id="d348e-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="d348e-133">**TenantId:** ID tenanta v oboru (role správce Marketplace se má přiřadit v oboru tenanta).</span><span class="sxs-lookup"><span data-stu-id="d348e-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="d348e-134">**SubscriptionId:** Předplatné, ke kterému má globální správce přiřazenou roli **Přispěvatel** nebo má vyšší přiřazení.</span><span class="sxs-lookup"><span data-stu-id="d348e-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="d348e-135">**GlobalAdminUsername:** Uživatelské jméno globálního správce.</span><span class="sxs-lookup"><span data-stu-id="d348e-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="d348e-136">**UsernameToAssignRoleFor:** Uživatelské jméno, ke kterému se přiřadí role správce webu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="d348e-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="d348e-137">Pro uživatele typu Host, kteří jsou pozváni do tenanta, může trvat až 48 hodin, než bude k dispozici jejich účet pro přiřazení role správce Marketplace.</span><span class="sxs-lookup"><span data-stu-id="d348e-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="d348e-138">další informace najdete v tématu [vlastnosti Azure Active Directory uživatele spolupráce B2B](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="d348e-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

```PowerShell
function Assign-MarketplaceAdminRole { 
[CmdletBinding()] 
param( 
[Parameter(Mandatory)] 
[string]$TenantId, 
 
[Parameter(Mandatory)] 
[string]$SubscriptionId, 

 

[Parameter(Mandatory)] 
[string]$GlobalAdminUsername, 

 

[Parameter(Mandatory)] 
[string]$UsernameToAssignRoleFor 
) 

$MarketplaceAdminRoleDefinitionName = "Marketplace Admin" 

 

Write-Output "TenantId = $TenantId" 
Write-Output "SubscriptionId = $SubscriptionId" 
Write-Output "GlobalAdminUsername = $GlobalAdminUsername" 
Write-Output "UsernameToAssignRoleFor = $UsernameToAssignRoleFor" 

 

Write-Output "$($GlobalAdminUsername) is about to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)" 

 

$profile = Connect-AzAccount -Tenant $TenantId -SubscriptionId $SubscriptionId

 

 
if($profile -eq $null) 
{ 
Write-Error -Message "Failed to connect to tenant and/or subscription" -ErrorAction Stop 
} 
elseif($profile.Context.Account.Id -ne $GlobalAdminUsername) 
{ 
Write-Error "Connected with $($profile.Context.Account.Id) instead of with the global admin that was specified in the script parameters, which is $($GlobalAdminUsername)" 
} 
else 
{ 
Write-Output "$($GlobalAdminUsername) was connected successfully to Tenant=$($profile.Context.Tenant), Subscription=$($profile.Context.Subscription), AccountId=$($profile.Context.Account.Id), Environment=$($profile.Context.Environment)" 
} 

 

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

 

if($MarketPlaceAdminRole -eq $null) 
{ 
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop 
} 
else 
{ 
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available" 
} 

 

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..." 

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace" 

} 

Assign-MarketplaceAdminRole 
```

<span data-ttu-id="d348e-139">další informace o rutinách obsažených v modulu příkazového portálu Az. Portal PowerShell najdete v tématu [Microsoft Azure PowerShell: rutiny řídicího panelu portálu](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="d348e-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="d348e-140">Vytvořit soukromé Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="d348e-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="d348e-141">Přihlaste se na [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="d348e-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="d348e-142">Vyberte **všechny služby** a potom **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="d348e-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Zobrazuje hlavní okno Azure Portal.":::

3. <span data-ttu-id="d348e-144">V nabídce na levé straně vyberte **soukromé tržiště** .</span><span class="sxs-lookup"><span data-stu-id="d348e-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="d348e-145">vyberte **Začínáme** pro vytvoření privátních Azure Marketplace (stačí to udělat jenom jednou).</span><span class="sxs-lookup"><span data-stu-id="d348e-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="ukazuje, jak vybrat Začínáme v hlavním okně Azure Portal.":::

    <span data-ttu-id="d348e-147">Pokud pro tohoto tenanta už existuje privátní Azure Marketplace, bude ve výchozím nastavení vybraná možnost **Spravovat Marketplace** .</span><span class="sxs-lookup"><span data-stu-id="d348e-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="d348e-148">Po dokončení budete mít prázdné a zakázané soukromé Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="d348e-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Zobrazí prázdnou obrazovku Private Azure Marketplace.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="d348e-150">Přidat položky z Galerie</span><span class="sxs-lookup"><span data-stu-id="d348e-150">Add items from gallery</span></span>

<span data-ttu-id="d348e-151">Položka je kombinací nabídky a plánu.</span><span class="sxs-lookup"><span data-stu-id="d348e-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="d348e-152">Na stránce Spravovat web Marketplace můžete hledat a přidávat položky.</span><span class="sxs-lookup"><span data-stu-id="d348e-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="d348e-153">Vyberte **Přidat položky**.</span><span class="sxs-lookup"><span data-stu-id="d348e-153">Select **Add items**.</span></span>

2. <span data-ttu-id="d348e-154">Přejděte do **Galerie** nebo vyhledejte požadovanou položku pomocí vyhledávacího pole.</span><span class="sxs-lookup"><span data-stu-id="d348e-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

   :::image type="content" source="media/private-azure/marketplace-gallery.png" lightbox="media/private-azure/marketplace-gallery-zoom.png" alt-text="Ukazuje, jak procházet galerii nebo použít vyhledávací pole.":::

3. <span data-ttu-id="d348e-156">Ve výchozím nastavení se při přidávání nové nabídky do seznamu schválených přidá všechny aktuální plány.</span><span class="sxs-lookup"><span data-stu-id="d348e-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="d348e-157">Chcete-li před přidáním vybraných položek změnit výběr plánu, vyberte rozevírací nabídku v dlaždici nabídky a aktualizujte požadované plány.</span><span class="sxs-lookup"><span data-stu-id="d348e-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer's tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Ukazuje, jak aktualizovat požadované plány.":::

4. <span data-ttu-id="d348e-159">Vyberte **Hotovo** vlevo dole po provedení výběru.</span><span class="sxs-lookup"><span data-stu-id="d348e-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="d348e-160">**Přidat položky** na web Marketplace budou k dispozici pouze pro nabídky, které nejsou od Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="d348e-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="d348e-161">Řešení Microsoftu (včetně schválených [distribucí systému Linux](/azure/virtual-machines/linux/endorsed-distros)) budou označena jako schválená ve výchozím nastavení a nelze je spravovat na soukromém webu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="d348e-161">Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) will be tagged as "Approved by default" and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="d348e-162">Upravit plány položky</span><span class="sxs-lookup"><span data-stu-id="d348e-162">Edit item's plans</span></span>

<span data-ttu-id="d348e-163">Plány položky můžete upravit na stránce Spravovat web Marketplace.</span><span class="sxs-lookup"><span data-stu-id="d348e-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="d348e-164">Ve sloupci **plány** zkontrolujte dostupné plány z rozevírací nabídky pro danou položku.</span><span class="sxs-lookup"><span data-stu-id="d348e-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>

2. <span data-ttu-id="d348e-165">Zaškrtnutím nebo zrušením zaškrtnutí políček zvolte, které plány mají být uživatelům k dispozici.</span><span class="sxs-lookup"><span data-stu-id="d348e-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

   :::image type="content" source="media/private-azure/edit-items.png" alt-text="Ukazuje, jak vybrat nebo zrušit zaškrtnutí políčka pro požadovanou položku.":::

   > [!NOTE]
   > <span data-ttu-id="d348e-167">Každá nabídka potřebuje aspoň jeden plán vybraný k aktualizaci.</span><span class="sxs-lookup"><span data-stu-id="d348e-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="d348e-168">Chcete-li odebrat všechny plány související s nabídkou, odstraňte celou nabídku (viz další oddíl).</span><span class="sxs-lookup"><span data-stu-id="d348e-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="d348e-169">Odstranit nabídky</span><span class="sxs-lookup"><span data-stu-id="d348e-169">Delete offers</span></span>

<span data-ttu-id="d348e-170">Na stránce Spravovat Marketplace zaškrtněte políčko vedle názvu nabídky (viz obrazovka výše) a vyberte **Odstranit položky**.</span><span class="sxs-lookup"><span data-stu-id="d348e-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="d348e-171">Povolit nebo zakázat privátní Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="d348e-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="d348e-172">Na stránce Spravovat Marketplace se zobrazí jedna z těchto proužkových proužků, která zobrazí aktuální stav privátních Azure Marketplace:</span><span class="sxs-lookup"><span data-stu-id="d348e-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Zobrazuje informační zprávu &quot;zakázat stav&quot;.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Zobrazuje informační zprávu &quot;Povolit stav&quot;.":::

<span data-ttu-id="d348e-175">V případě potřeby můžete povolit nebo zakázat privátní Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="d348e-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="d348e-176">Pokud je tato možnost zakázaná, vyberte **Povolit privátní tržiště** .</span><span class="sxs-lookup"><span data-stu-id="d348e-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="d348e-177">Pokud je povoleno, vyberte **Zakázat privátní tržiště** , které chcete zakázat.</span><span class="sxs-lookup"><span data-stu-id="d348e-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="d348e-178">Soukromé Azure Marketplace centra oznámení</span><span class="sxs-lookup"><span data-stu-id="d348e-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="d348e-179">Centrum oznámení se skládá ze tří typů oznámení a umožňuje správci Marketplace provádět akce na základě oznámení:</span><span class="sxs-lookup"><span data-stu-id="d348e-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="d348e-180">Žádosti o schválení od uživatelů pro položky, které nejsou v seznamu schválených (viz [žádost o přidání nabídek nebo plánů](#request-to-add-offers-or-plans) níže).</span><span class="sxs-lookup"><span data-stu-id="d348e-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="d348e-181">Nové oznámení plánu pro nabídky, které již mají jeden nebo více plánů v seznamu schválených.</span><span class="sxs-lookup"><span data-stu-id="d348e-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="d348e-182">Byla odebrána oznámení plánu pro položky, které jsou v seznamu schválených, ale byly odebrány z globálního Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="d348e-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="d348e-183">Přístup k centru oznámení:</span><span class="sxs-lookup"><span data-stu-id="d348e-183">To access the notification center:</span></span>

1. <span data-ttu-id="d348e-184">V nabídce na levé straně vyberte **oznámení** .</span><span class="sxs-lookup"><span data-stu-id="d348e-184">Select **Notifications** from the left-side menu.</span></span>

   :::image type="content" source="media/private-azure/marketplace-notifications-small.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="Zobrazí nabídku oznámení.":::

1. <span data-ttu-id="d348e-186">Pro další akce vyberte nabídku se třemi tečkami.</span><span class="sxs-lookup"><span data-stu-id="d348e-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Zobrazí další výsledky nabídky možností.":::

1. <span data-ttu-id="d348e-188">V případě požadavků na plán se otevře formulář žádosti o **schválení, kde** můžete zkontrolovat všechny požadavky uživatelů na konkrétní nabídku.</span><span class="sxs-lookup"><span data-stu-id="d348e-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="d348e-189">Vyberte **schválit** nebo **zamítnout**.</span><span class="sxs-lookup"><span data-stu-id="d348e-189">Select **Approve** or **Reject**.</span></span>

   :::image type="content" source="media/private-azure/notifications-approve-reject-small.png" lightbox="media/private-azure/notifications-approve-reject.png" alt-text="Zobrazuje možnosti schválení a odmítnutí.":::

1. <span data-ttu-id="d348e-191">Z rozevírací nabídky vyberte plán, který chcete schválit.</span><span class="sxs-lookup"><span data-stu-id="d348e-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="d348e-192">Přidejte komentář a vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="d348e-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="d348e-193">Procházení soukromých Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="d348e-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="d348e-194">Když je povolený privátní Azure Marketplace, zobrazí se uživatelům, kteří plánují schválení správcem Marketplace.</span><span class="sxs-lookup"><span data-stu-id="d348e-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="d348e-195">Zelená **schválená** zpráva indikuje, že partnerská nabídka (jiná než Microsoft) je schválená.</span><span class="sxs-lookup"><span data-stu-id="d348e-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="d348e-196">Modré **schválené** oznámení indikuje, že nabídka Microsoft (včetně schválených [distribucí systému Linux](/azure/virtual-machines/linux/endorsed-distros)) je schválená.</span><span class="sxs-lookup"><span data-stu-id="d348e-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="d348e-197">Uživatelé mohou filtrovat mezi nabídkami, které jsou a nejsou schváleny:</span><span class="sxs-lookup"><span data-stu-id="d348e-197">Users can filter between offers that are and are not approved:</span></span>

   :::image type="content" source="media/private-azure/filter-option-small.png" lightbox="media/private-azure/filter-option.png" alt-text="Zobrazuje možnost filtrování.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="d348e-199">Koupit nebo nasadit v privátních Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="d348e-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="d348e-200">I když se zobrazí stránka s podrobnostmi o produktu, která je podobná globálním Azure Marketplace, existují tři privátní Azure Marketplace specifické scénáře.</span><span class="sxs-lookup"><span data-stu-id="d348e-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="d348e-201">Když uživatel vybere schválený plán, aktivuje se tlačítko **vytvořit** :</span><span class="sxs-lookup"><span data-stu-id="d348e-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

   :::image type="content" source="media/private-azure/button-create-enabled-small.png" lightbox="media/private-azure/button-create-enabled.png" alt-text="Zobrazuje hlavičku nabídky s informacemi o plánu, který se dá vytvořit.":::

- <span data-ttu-id="d348e-203">Pokud se výběr plánu produktu nezobrazuje na stránce s podrobnostmi o produktu, ale správce schválil jeden nebo více plánů, poznamenejte si, které plány se schvalují a že je povolené tlačítko **vytvořit** :</span><span class="sxs-lookup"><span data-stu-id="d348e-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

   :::image type="content" source="media/private-azure/button-create-enabled-and-plans-small.png" lightbox="media/private-azure/button-create-enabled-and-plans.png" alt-text="Zobrazuje hlavičku nabídky, která označuje, že je možné vytvořit plán a Zobrazit dostupné plány.":::

- <span data-ttu-id="d348e-205">Když uživatel vybere neschválený plán, banner se naplánuje jako Neschváleno a tlačítko **vytvořit** je zakázané.</span><span class="sxs-lookup"><span data-stu-id="d348e-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="d348e-206">Uživatel si stále může vyžádat přidání plánu do seznamu schválených (viz další část).</span><span class="sxs-lookup"><span data-stu-id="d348e-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="d348e-207">Žádost o přidání nabídek nebo plánů</span><span class="sxs-lookup"><span data-stu-id="d348e-207">Request to add offers or plans</span></span>

<span data-ttu-id="d348e-208">Můžete požádat o přidání veřejné nabídky nebo plánu, který není aktuálně schválen v soukromém Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="d348e-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="d348e-209">Vyberte **požadavek, který chcete přidat** do banneru pro otevření **formuláře žádosti o přístup**.</span><span class="sxs-lookup"><span data-stu-id="d348e-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

   :::image type="content" source="media/private-azure/request-banner-small.png" lightbox="media/private-azure/request-banner.png" alt-text="Zobrazí banner s odkazem požadavek na přidání.":::

   :::image type="content" source="media/private-azure/access-request-form-small.png" lightbox="media/private-azure/access-request-form.png" alt-text="Zobrazí formulář žádosti o přístup pro nabídky nebo plány.":::

1. <span data-ttu-id="d348e-212">Vyberte plány, které chcete přidat do žádosti (**jakýkoliv plán** oznamuje správci Marketplace, že nemáte předvolbu plánu v rámci nabídky).</span><span class="sxs-lookup"><span data-stu-id="d348e-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="d348e-213">Přidejte **odůvodnění** a vyberte **žádost** o odeslání žádosti.</span><span class="sxs-lookup"><span data-stu-id="d348e-213">Add a **Justification** and select **Request** to submit your request.</span></span>

   :::image type="content" source="media/private-azure/access-request-form-filled-small.png" lightbox="media/private-azure/access-request-form-filled.png" alt-text="Zobrazuje formulář žádosti o přístup pro nabídky nebo plány s ukázkovými položkami.":::

1. <span data-ttu-id="d348e-215">Ve formuláři žádosti o přístup se zobrazí označení pro nevyřízenou žádost s možností **odvolání žádosti**.</span><span class="sxs-lookup"><span data-stu-id="d348e-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

   :::image type="content" source="media/private-azure/approved-pending-plans-small.png" lightbox="media/private-azure/approved-pending-plans.png" alt-text="Zobrazuje seznam schválených nebo nevyřízených plánů s odkazem na žádost o stažení.":::

> [!NOTE]
> <span data-ttu-id="d348e-217">Po odeslání se formulář žádosti o schválení pošle do [centra oznámení](#private-azure-marketplace-notification-center) pro správce Marketplace, aby zkontroloval požadavek a provedl akci.</span><span class="sxs-lookup"><span data-stu-id="d348e-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

> [!CAUTION]
> <span data-ttu-id="d348e-218">Schválení na soukromý web Marketplace neindikuje nákup řešení.</span><span class="sxs-lookup"><span data-stu-id="d348e-218">Approval into Private Marketplace does not indicate procurement of a solution.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="d348e-219">Nejčastější dotazy</span><span class="sxs-lookup"><span data-stu-id="d348e-219">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="d348e-220">Již jsem blokoval aplikaci třetí strany Marketplace prostřednictvím Azure Policy.</span><span class="sxs-lookup"><span data-stu-id="d348e-220">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="d348e-221">Jak se to liší?</span><span class="sxs-lookup"><span data-stu-id="d348e-221">How is this different?</span></span>

<span data-ttu-id="d348e-222">V současné době existují dva způsoby, jak omezit služby třetích stran na webu Marketplace:</span><span class="sxs-lookup"><span data-stu-id="d348e-222">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="d348e-223">Prostřednictvím portálu EA nebo Azure Portal zakažte služby třetích stran nebo omezte pouze na bezplatné nebo BYOL SKU.</span><span class="sxs-lookup"><span data-stu-id="d348e-223">Through EA portal or the Azure portal, disable third-party services or restrict to "Free or BYOL SKUs only".</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Ukazuje, jak omezit služby v Azure Portal.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Ukazuje, jak omezit služby na portálu E.":::

2. <span data-ttu-id="d348e-226">Vytvořte zásadu Azure, která povolí jenom konkrétní virtuální počítače.</span><span class="sxs-lookup"><span data-stu-id="d348e-226">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="d348e-227">podrobnosti o tom, jak vynutilit zásady pro Windows virtuálních počítačů, najdete v tématu věnovaném [použití zásad pro Windows virtuálních počítačů pomocí Azure Resource Manager](/azure/virtual-machines/windows/policy).</span><span class="sxs-lookup"><span data-stu-id="d348e-227">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="d348e-228">Soukromé Azure Marketplace umožňují větší flexibilitu při omezování a povolování konkrétních nabídek a plánů.</span><span class="sxs-lookup"><span data-stu-id="d348e-228">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="d348e-229">Informuje koncové uživatele o dostupnosti pro nasazení v galerii Marketplace, a to i předtím, než se pokusí nasadit služby třetích stran.</span><span class="sxs-lookup"><span data-stu-id="d348e-229">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="d348e-230">Pokud chcete povolit nasazení služeb třetích stran, nastavte Azure Marketplace na zapnuto nebo povoleno na portálu EA a v Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="d348e-230">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="d348e-231">Privátní Azure Marketplace můžou využívat Partnerská řešení, která nejsou omezená na virtuální počítače.</span><span class="sxs-lookup"><span data-stu-id="d348e-231">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="d348e-232">Privátní Azure Marketplace můžou obsloužit na úrovni plánu a můžou také nastavit "aktuální a budoucí plán".</span><span class="sxs-lookup"><span data-stu-id="d348e-232">Private Azure Marketplace can curate at the plan level and can also set "Current and future plan".</span></span>
- <span data-ttu-id="d348e-233">Privátní Azure Marketplace můžou koncovým uživatelům informovat o tom, co můžou a nemůžou být nasazené.</span><span class="sxs-lookup"><span data-stu-id="d348e-233">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="d348e-234">Jaký je rozdíl mezi soukromou nabídkou a soukromým Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="d348e-234">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="d348e-235">**Soukromá nabídka** umožňuje vydavatelům vytvářet plány, které jsou viditelné pouze cílovým zákazníkům.</span><span class="sxs-lookup"><span data-stu-id="d348e-235">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="d348e-236">To jim umožní soukromě sdílet přizpůsobená řešení s vyjednávacími cenami, soukromými podmínkami a podmínkami a specializovanými konfiguracemi.</span><span class="sxs-lookup"><span data-stu-id="d348e-236">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="d348e-237">Podrobnosti najdete v tématu [soukromé nabídky na komerčním webu Marketplace](/azure/marketplace/private-offers).</span><span class="sxs-lookup"><span data-stu-id="d348e-237">For details, see [Private offers in the commercial marketplace](/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="d348e-238">**Soukromý Azure Marketplace** v Azure Portal umožňuje správcům předem schvalovat, která řešení třetích stran můžou uživatelé nasazovat.</span><span class="sxs-lookup"><span data-stu-id="d348e-238">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="d348e-239">Pomocí privátního Azure Marketplace můžou uživatelé využít výhod Azure Marketplace tak, že si vyhledají, kupují a nasazují vyhovující nabídky.</span><span class="sxs-lookup"><span data-stu-id="d348e-239">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="d348e-240">Aby bylo možné spravovat soukromé nabídky na základě předplatného na soukromém webu Marketplace, musí mít správce webu Marketplace minimálně roli "číst" na daném předplatném.</span><span class="sxs-lookup"><span data-stu-id="d348e-240">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of "read" role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="d348e-241">K privátním Azure Marketplace jsem přidal soukromou nabídku, proč se na kartě Spravovat Marketplace nezobrazuje?</span><span class="sxs-lookup"><span data-stu-id="d348e-241">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="d348e-242">Soukromé nabídky na základě předplatného jsou viditelné jenom pro uvedená předplatná v nastavení soukromé nabídky.</span><span class="sxs-lookup"><span data-stu-id="d348e-242">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="d348e-243">Pokud chcete zobrazit soukromou nabídku, ujistěte se, že globální filtr předplatného zobrazuje všechna předplatná.</span><span class="sxs-lookup"><span data-stu-id="d348e-243">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

   :::image type="content" source="media/private-azure/private-marketplace-filter.png" lightbox="media/private-azure/private-marketplace-filter.png" alt-text="Zobrazuje soukromý filtr Marketplace.":::

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="d348e-245">Můžeme do privátních Azure Marketplace zahrnout vlastní image?</span><span class="sxs-lookup"><span data-stu-id="d348e-245">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="d348e-246">No.</span><span class="sxs-lookup"><span data-stu-id="d348e-246">No.</span></span> <span data-ttu-id="d348e-247">Privátní Azure Marketplace umožňuje všem správcům IT spravovat řešení třetích stran z globálních Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="d348e-247">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="d348e-248">Vzhledem k tomu, že vlastní image nejsou na globálním Azure Marketplace, nemůže správce IT vybírat a vybírat vlastní image.</span><span class="sxs-lookup"><span data-stu-id="d348e-248">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="d348e-249">Chcete-li sdílet vlastní image, použijte [galerii sdílených imagí](/azure/virtual-machines/shared-image-galleries).</span><span class="sxs-lookup"><span data-stu-id="d348e-249">If you would like to share custom images, use [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="d348e-250">Podrobný průvodce vytvořením Galerie sdílených imagí (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span><span class="sxs-lookup"><span data-stu-id="d348e-250">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="d348e-251">Vytvoří definici obrázku v rámci SIG.</span><span class="sxs-lookup"><span data-stu-id="d348e-251">Create an image definition within a SIG.</span></span> <span data-ttu-id="d348e-252">Zákazník by měl zvolit **zobecněný** pro pole stav operačního systému.</span><span class="sxs-lookup"><span data-stu-id="d348e-252">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="d348e-253">(Rozhraní příkazového[řádku](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShellu](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span><span class="sxs-lookup"><span data-stu-id="d348e-253">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="d348e-254">Přeneste spravovanou bitovou kopii do galerie sdílených imagí ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span><span class="sxs-lookup"><span data-stu-id="d348e-254">Bring managed image into the Shared Image Gallery ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="d348e-255">Image virtuálního počítače SIG by se měly nacházet v jednom předplatném.</span><span class="sxs-lookup"><span data-stu-id="d348e-255">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="d348e-256">Pokud ho chcete zpřístupnit ostatním předplatným, použijte registraci aplikace (rozhraní příkazového[řádku](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShellu](/azure/virtual-machines/windows/share-images-across-tenants)).</span><span class="sxs-lookup"><span data-stu-id="d348e-256">To make it available to other subscriptions, use an app registration ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="d348e-257">Proč se mi zobrazují některé nabídky **schválené ve výchozím nastavení,** i když Vydavatel není Microsoft?</span><span class="sxs-lookup"><span data-stu-id="d348e-257">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="d348e-258">Microsoft podporuje v Azure technologii Linux a open source.</span><span class="sxs-lookup"><span data-stu-id="d348e-258">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="d348e-259">[Schválené distribuce systému Linux](/azure/virtual-machines/linux/endorsed-distros) jsou podporovány v Azure a cena je integrována do virtuálních počítačů.</span><span class="sxs-lookup"><span data-stu-id="d348e-259">[Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="d348e-260">Vzhledem k tomu, že je agent Azure Linux už v Azure Marketplace předinstalovaný, považuje se za nabídku Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="d348e-260">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="d348e-261">Vzhledem k tomu, že jsou nabídky společnosti Microsoft schváleny ve výchozím nastavení, nelze spravovat schválené distribuce systému Linux v privátních Azure Marketplace a jsou schváleny ve výchozím nastavení.</span><span class="sxs-lookup"><span data-stu-id="d348e-261">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="d348e-262">Kontaktování podpory</span><span class="sxs-lookup"><span data-stu-id="d348e-262">Contact support</span></span>

- <span data-ttu-id="d348e-263">Podporu Azure Marketplace najdete na webu [Microsoft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="d348e-263">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>