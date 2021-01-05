---
title: Vytvoření a Správa privátních Azure Marketplace v Azure Portal
description: Seznamte se s vytvářením a správou privátních Azure Marketplace (Preview) v Azure Portal. Privátní Azure Marketplace (Preview) umožňuje správcům řídit, která řešení třetích stran můžou uživatelé používat.
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 12/22/2020
ms.openlocfilehash: 09f7bcb29dc619e4e31c0aa3d5c73fade5218819
ms.sourcegitcommit: 30d154cdf40aa75400be7805cd9b2685b66a1382
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/24/2020
ms.locfileid: "97760802"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a><span data-ttu-id="8cc52-104">Vytvoření a Správa privátních Azure Marketplace (Preview) v Azure Portal</span><span class="sxs-lookup"><span data-stu-id="8cc52-104">Create and manage Private Azure Marketplace (preview) in the Azure portal</span></span>

<span data-ttu-id="8cc52-105">Privátní Azure Marketplace (Preview) umožňuje správcům řídit, která řešení třetích stran můžou uživatelé používat.</span><span class="sxs-lookup"><span data-stu-id="8cc52-105">Private Azure Marketplace (preview) lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="8cc52-106">Díky tomu můžete nasadit jenom nabídky, které schválíte a které jsou v rozporu s podnikovými zásadami.</span><span class="sxs-lookup"><span data-stu-id="8cc52-106">It does this by allowing you to deploy only offers that you approve and that comply with your enterprise's policies.</span></span> <span data-ttu-id="8cc52-107">S privátními Azure Marketplace můžou vaši uživatelé hledat v online obchodě, aby si mohli koupit a nasadit.</span><span class="sxs-lookup"><span data-stu-id="8cc52-107">With Private Azure Marketplace, your users can search the online store for compliant offers to purchase and deploy.</span></span> 

<span data-ttu-id="8cc52-108">Jako správce Marketplace (přiřazená role) začnete s neaktivním a prázdným soukromým úložištěm, kde můžete přidat vaše schválené nabídky a plány.</span><span class="sxs-lookup"><span data-stu-id="8cc52-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="8cc52-109">Tento článek vysvětluje, jak vytvořit, spravovat a povolit soukromé Azure Marketplace pro vaše uživatele.</span><span class="sxs-lookup"><span data-stu-id="8cc52-109">This article explains how to create, manage, and enable Private Azure Marketplace for your users.</span></span>

<span data-ttu-id="8cc52-110">Poznámky:</span><span class="sxs-lookup"><span data-stu-id="8cc52-110">Notes:</span></span>

- <span data-ttu-id="8cc52-111">Soukromé Azure Marketplace jsou na úrovni tenanta, takže všichni uživatelé v tenantovi uvidí stejný seznam.</span><span class="sxs-lookup"><span data-stu-id="8cc52-111">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
- <span data-ttu-id="8cc52-112">Všechna řešení společnosti Microsoft jsou automaticky přidána do privátního Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="8cc52-112">All Microsoft solutions are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="8cc52-113">Přiřazení role správce Marketplace</span><span class="sxs-lookup"><span data-stu-id="8cc52-113">Assign the Marketplace admin role</span></span>

<span data-ttu-id="8cc52-114">Globální správce tenanta musí přiřadit roli **správce Marketplace** správci privátního Azure Marketplace, který bude spravovat soukromé úložiště.</span><span class="sxs-lookup"><span data-stu-id="8cc52-114">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="8cc52-115">Přístup ke správě privátních Azure Marketplace je k dispozici jenom správcům IT, kteří mají přiřazenou roli správce Marketplace.</span><span class="sxs-lookup"><span data-stu-id="8cc52-115">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="8cc52-116">Předpoklady</span><span class="sxs-lookup"><span data-stu-id="8cc52-116">Prerequisites</span></span>

<span data-ttu-id="8cc52-117">Abyste mohli přiřadit roli správce Marketplace uživateli v oboru tenanta, musíte splnit tyto požadavky:</span><span class="sxs-lookup"><span data-stu-id="8cc52-117">You must meet these prerequisites before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="8cc52-118">Máte přístup k uživateli **globálního správce** .</span><span class="sxs-lookup"><span data-stu-id="8cc52-118">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="8cc52-119">Tenant má minimálně jedno předplatné (může to být libovolný typ).</span><span class="sxs-lookup"><span data-stu-id="8cc52-119">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="8cc52-120">Pro globálního správce se uživateli přiřadí role **Přispěvatel** nebo vyšší pro vybrané předplatné.</span><span class="sxs-lookup"><span data-stu-id="8cc52-120">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-iam"></a><span data-ttu-id="8cc52-121">Přiřazení role správce Marketplace k IAM</span><span class="sxs-lookup"><span data-stu-id="8cc52-121">Assign the Marketplace admin role with IAM</span></span>

1. <span data-ttu-id="8cc52-122">Přihlaste se na web [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="8cc52-122">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
1. <span data-ttu-id="8cc52-123">Vyberte **všechny služby** a potom **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="8cc52-123">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure Portal hlavní okno.":::

3. <span data-ttu-id="8cc52-125">Z možností na levé straně vyberte **soukromé tržiště** .</span><span class="sxs-lookup"><span data-stu-id="8cc52-125">Select **Private Marketplace** from the options on the left.</span></span>
1. <span data-ttu-id="8cc52-126">Vyberte **řízení přístupu (IAM)** a přiřaďte roli správce webu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="8cc52-126">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Obrazovka řízení přístupu IAM.":::

1. <span data-ttu-id="8cc52-128">Vyberte **+ Přidat** > **Přidat přiřazení role**.</span><span class="sxs-lookup"><span data-stu-id="8cc52-128">Select **+ Add** > **Add role assignment**.</span></span>
1. <span data-ttu-id="8cc52-129">V části **role** vyberte **správce Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="8cc52-129">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Nabídka přiřazení role":::

1. <span data-ttu-id="8cc52-131">V rozevíracím seznamu vyberte požadovaného uživatele a potom vyberte **Hotovo**.</span><span class="sxs-lookup"><span data-stu-id="8cc52-131">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="8cc52-132">Přiřazení role správce Marketplace k PowerShellu</span><span class="sxs-lookup"><span data-stu-id="8cc52-132">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="8cc52-133">K přiřazení role správce Marketplace použijte následující skript prostředí PowerShell; vyžaduje následující parametry:</span><span class="sxs-lookup"><span data-stu-id="8cc52-133">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="8cc52-134">**TenantId:** ID tenanta v oboru (role správce Marketplace se má přiřadit v oboru tenanta).</span><span class="sxs-lookup"><span data-stu-id="8cc52-134">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="8cc52-135">**SubscriptionId:** Předplatné, ke kterému má globální správce přiřazenou roli **Přispěvatel** nebo má vyšší přiřazení.</span><span class="sxs-lookup"><span data-stu-id="8cc52-135">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="8cc52-136">**GlobalAdminUsername:** Uživatelské jméno globálního správce.</span><span class="sxs-lookup"><span data-stu-id="8cc52-136">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="8cc52-137">**UsernameToAssignRoleFor:** Uživatelské jméno, ke kterému se přiřadí role správce webu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="8cc52-137">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="8cc52-138">Pro uživatele typu Host, kteří jsou pozváni do tenanta, může trvat až 48 hodin, než bude k dispozici jejich účet pro přiřazení role správce Marketplace.</span><span class="sxs-lookup"><span data-stu-id="8cc52-138">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace admin role.</span></span> <span data-ttu-id="8cc52-139">Další informace najdete v tématu [vlastnosti Azure Active Directory uživatele spolupráce B2B](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="8cc52-139">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="8cc52-140">Další informace o rutinách obsažených v modulu příkazového portálu AZ. Portal PowerShell najdete v tématu [Microsoft Azure PowerShell: rutiny řídicího panelu portálu](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="8cc52-140">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="8cc52-141">Vytvořit soukromé Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="8cc52-141">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="8cc52-142">Přihlaste se na web [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="8cc52-142">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="8cc52-143">Vyberte **všechny služby** a potom **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="8cc52-143">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure Portal hlavní okno.":::

3. <span data-ttu-id="8cc52-145">Z možností na levé straně vyberte **soukromé tržiště** .</span><span class="sxs-lookup"><span data-stu-id="8cc52-145">Select **Private Marketplace** from the options on the left.</span></span>

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Výběr privátního tržiště v Azure Portal hlavním okně.":::

4. <span data-ttu-id="8cc52-147">Vyberte **Začínáme** pro vytvoření privátního Azure Marketplace (stačí to udělat jenom jednou).</span><span class="sxs-lookup"><span data-stu-id="8cc52-147">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Výběr možnosti Začínáme v hlavním okně Azure Portal.":::

    <span data-ttu-id="8cc52-149">Pokud pro tohoto tenanta už existuje privátní Azure Marketplace, bude ve výchozím nastavení vybraná možnost **Spravovat Marketplace** .</span><span class="sxs-lookup"><span data-stu-id="8cc52-149">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="8cc52-150">Po dokončení budete mít prázdné a zakázané soukromé Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="8cc52-150">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Prázdná obrazovka privátního Azure Marketplace.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="8cc52-152">Přidat položky z Galerie</span><span class="sxs-lookup"><span data-stu-id="8cc52-152">Add items from gallery</span></span>

<span data-ttu-id="8cc52-153">Položka je kombinací nabídky a plánu.</span><span class="sxs-lookup"><span data-stu-id="8cc52-153">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="8cc52-154">Položku můžete vyhledat a přidat na stránce Spravovat web Marketplace.</span><span class="sxs-lookup"><span data-stu-id="8cc52-154">You can search for and add item in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="8cc52-155">Vyberte **Přidat položky**.</span><span class="sxs-lookup"><span data-stu-id="8cc52-155">Select **Add items**.</span></span>

2. <span data-ttu-id="8cc52-156">Přejděte do **Galerie** nebo vyhledejte požadovanou položku pomocí vyhledávacího pole.</span><span class="sxs-lookup"><span data-stu-id="8cc52-156">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Procházení Galerie nebo použití vyhledávacího pole.":::

3. <span data-ttu-id="8cc52-158">Ve výchozím nastavení se při přidávání nové nabídky přidají všechny aktuální plány do seznamu povolených.</span><span class="sxs-lookup"><span data-stu-id="8cc52-158">As default, when adding a new offer, all current plans will be added to the allowed list.</span></span> <span data-ttu-id="8cc52-159">Chcete-li před přidáním vybraných položek změnit výběr plánu, vyberte rozevírací nabídku v dlaždici nabídky a aktualizujte požadované plány.</span><span class="sxs-lookup"><span data-stu-id="8cc52-159">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Aktualizujte požadované plány.":::

4. <span data-ttu-id="8cc52-161">Vyberte **Hotovo** vlevo dole po provedení výběru.</span><span class="sxs-lookup"><span data-stu-id="8cc52-161">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="8cc52-162">**Přidat položky** na web Marketplace budou k dispozici pouze pro nabídky, které nejsou od Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="8cc52-162">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="8cc52-163">Nabídky společnosti Microsoft jsou ve výchozím nastavení povoleny.</span><span class="sxs-lookup"><span data-stu-id="8cc52-163">Microsoft offers are allowed by default.</span></span>

## <a name="edit-item-plans"></a><span data-ttu-id="8cc52-164">Upravit plány položek</span><span class="sxs-lookup"><span data-stu-id="8cc52-164">Edit item plans</span></span>

<span data-ttu-id="8cc52-165">Plány položky můžete upravit na stránce Spravovat web Marketplace.</span><span class="sxs-lookup"><span data-stu-id="8cc52-165">You can edit an item's plans in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="8cc52-166">Ve sloupci **plány** zkontrolujte dostupné plány z rozevírací nabídky pro danou položku.</span><span class="sxs-lookup"><span data-stu-id="8cc52-166">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="8cc52-167">Zaškrtnutím nebo zrušením zaškrtnutí políček zvolte, které plány mají být uživatelům k dispozici.</span><span class="sxs-lookup"><span data-stu-id="8cc52-167">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Zaškrtněte nebo zrušte zaškrtnutí políčka pro požadovanou položku.":::

> [!NOTE]
> <span data-ttu-id="8cc52-169">U každé nabídky je nutné vybrat alespoň jeden plán, aby došlo k aktualizaci.</span><span class="sxs-lookup"><span data-stu-id="8cc52-169">Each offer needs at least one plan selected in order for the update to occur.</span></span> <span data-ttu-id="8cc52-170">Chcete-li odebrat všechny plány související s nabídkou, odstraňte celou nabídku (viz další oddíl).</span><span class="sxs-lookup"><span data-stu-id="8cc52-170">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="8cc52-171">Odstranit nabídky</span><span class="sxs-lookup"><span data-stu-id="8cc52-171">Delete offers</span></span>

<span data-ttu-id="8cc52-172">Na stránce Spravovat Marketplace zaškrtněte políčko vedle názvu nabídky (viz obrazovka výše) a vyberte **Odstranit položky**.</span><span class="sxs-lookup"><span data-stu-id="8cc52-172">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="8cc52-173">Povolit nebo zakázat privátní Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="8cc52-173">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="8cc52-174">Na stránce Spravovat Marketplace se zobrazí jedna z těchto proužkových proužků, která zobrazí aktuální stav privátních Azure Marketplace:</span><span class="sxs-lookup"><span data-stu-id="8cc52-174">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Deaktivovat banner stavu":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Povolit banner stavu":::

<span data-ttu-id="8cc52-177">V případě potřeby můžete povolit nebo zakázat privátní Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="8cc52-177">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="8cc52-178">Pokud je tato možnost zakázaná, vyberte **Povolit privátní tržiště** .</span><span class="sxs-lookup"><span data-stu-id="8cc52-178">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="8cc52-179">Pokud je povoleno, vyberte **Zakázat privátní tržiště** , které chcete zakázat.</span><span class="sxs-lookup"><span data-stu-id="8cc52-179">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="8cc52-180">Procházení soukromých Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="8cc52-180">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="8cc52-181">Když je povolený privátní Azure Marketplace, uživatelé uvidí, které plány má správce Marketplace povolený.</span><span class="sxs-lookup"><span data-stu-id="8cc52-181">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has allowed.</span></span>

- <span data-ttu-id="8cc52-182">Zelené **povolené** oznámení značí, že je povolená nabídka partnera (jiné než Microsoft).</span><span class="sxs-lookup"><span data-stu-id="8cc52-182">A green **Allowed** notice indicates a Partner (non-Microsoft) offer that is allowed.</span></span>
- <span data-ttu-id="8cc52-183">Modré **povolené** oznámení indikuje, že je povolená nabídka Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="8cc52-183">A blue **Allowed** notice indicates a Microsoft offer that is allowed.</span></span>

<span data-ttu-id="8cc52-184">Uživatelé mohou filtrovat mezi nabídkami, které nejsou a nejsou povoleny:</span><span class="sxs-lookup"><span data-stu-id="8cc52-184">Users can filter between offers that are and are not allowed:</span></span>

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Možnost filtrování":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="8cc52-186">Koupit nebo nasadit v privátních Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="8cc52-186">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="8cc52-187">I když je prostředí stránky s podrobnostmi o produktu podobné veřejnému Azure Marketplace, existují tři privátní Azure Marketplace specifické scénáře.</span><span class="sxs-lookup"><span data-stu-id="8cc52-187">While the product details page experience is similar to the public Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="8cc52-188">Když uživatel vybere povolený plán, aktivuje se tlačítko **vytvořit** :</span><span class="sxs-lookup"><span data-stu-id="8cc52-188">When a user selects an allowed plan, the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Informační zpráva nabídky, která označuje plán, se dá vytvořit.":::

- <span data-ttu-id="8cc52-190">Když uživatel vybere nepovolený plán, banner se zaznamená, že plán není povolený a tlačítko **vytvořit** je zakázané.</span><span class="sxs-lookup"><span data-stu-id="8cc52-190">When a user selects a non-allowed plan, a banner notes that the plan is not allowed and the **Create** button is disabled.</span></span>

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Banner nabídky, který označuje plán, nejde vytvořit.":::

- <span data-ttu-id="8cc52-192">Pokud se výběr plánu produktu nezobrazuje na stránce s podrobnostmi o produktu, ale správce schválil jeden nebo více plánů, poznamenejte si, které plány jsou povolené a že je povolené tlačítko **vytvořit** :</span><span class="sxs-lookup"><span data-stu-id="8cc52-192">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are allowed and the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Banner s informacemi o tom, že je možné vytvořit plán a Zobrazit dostupné plány.":::

## <a name="contact-support"></a><span data-ttu-id="8cc52-194">Kontaktování podpory</span><span class="sxs-lookup"><span data-stu-id="8cc52-194">Contact support</span></span>

<span data-ttu-id="8cc52-195">Podporu Azure Marketplace najdete na webu [Microsoft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="8cc52-195">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span> 
