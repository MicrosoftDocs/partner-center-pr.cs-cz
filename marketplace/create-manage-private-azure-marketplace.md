---
title: Vytvoření a Správa privátních Azure Marketplace v Azure Portal
description: Seznamte se s vytvářením a správou privátních Azure Marketplace (Preview) v Azure Portal.
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 09/18/2020
ms.openlocfilehash: f62c9aef13b51ba2db42b267d7620f506bbdc1ec
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/21/2020
ms.locfileid: "95006935"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a><span data-ttu-id="83769-103">Vytvoření a Správa privátních Azure Marketplace (Preview) v Azure Portal</span><span class="sxs-lookup"><span data-stu-id="83769-103">Create and manage Private Azure Marketplace (preview) in the Azure portal</span></span>

<span data-ttu-id="83769-104">Privátní Azure Marketplace (Preview) umožňuje správcům řídit, která řešení třetích stran můžou uživatelé používat.</span><span class="sxs-lookup"><span data-stu-id="83769-104">Private Azure Marketplace (preview) lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="83769-105">Díky tomu můžete nasadit jenom nabídky, které schválíte a které jsou v rozporu s podnikovými zásadami.</span><span class="sxs-lookup"><span data-stu-id="83769-105">It does this by allowing you to deploy only offers that you approve and that comply with your enterprise's policies.</span></span> <span data-ttu-id="83769-106">S privátními Azure Marketplace můžou vaši uživatelé hledat v online obchodě, aby si mohli koupit a nasadit.</span><span class="sxs-lookup"><span data-stu-id="83769-106">With Private Azure Marketplace, your users can search the online store for compliant offers to purchase and deploy.</span></span> 

<span data-ttu-id="83769-107">Jako správce Marketplace (přiřazená role) začnete s neaktivním a prázdným soukromým úložištěm, kde můžete přidat vaše schválené nabídky a plány.</span><span class="sxs-lookup"><span data-stu-id="83769-107">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="83769-108">Tento článek vysvětluje, jak vytvořit, spravovat a povolit soukromé Azure Marketplace pro vaše uživatele.</span><span class="sxs-lookup"><span data-stu-id="83769-108">This article explains how to create, manage, and enable Private Azure Marketplace for your users.</span></span>

<span data-ttu-id="83769-109">Poznámky:</span><span class="sxs-lookup"><span data-stu-id="83769-109">Notes:</span></span>

- <span data-ttu-id="83769-110">Soukromé Azure Marketplace jsou na úrovni tenanta, takže všichni uživatelé v tenantovi uvidí stejný seznam.</span><span class="sxs-lookup"><span data-stu-id="83769-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
- <span data-ttu-id="83769-111">Všechna řešení společnosti Microsoft jsou automaticky přidána do privátního Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="83769-111">All Microsoft solutions are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="83769-112">Přiřazení role správce Marketplace</span><span class="sxs-lookup"><span data-stu-id="83769-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="83769-113">Globální správce tenanta musí přiřadit roli **správce Marketplace** správci privátního Azure Marketplace, který bude spravovat soukromé úložiště.</span><span class="sxs-lookup"><span data-stu-id="83769-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="83769-114">Přístup ke správě privátních Azure Marketplace je k dispozici jenom správcům IT, kteří mají přiřazenou roli správce Marketplace.</span><span class="sxs-lookup"><span data-stu-id="83769-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="83769-115">Požadavky</span><span class="sxs-lookup"><span data-stu-id="83769-115">Prerequisites</span></span>

<span data-ttu-id="83769-116">Abyste mohli přiřadit roli správce Marketplace uživateli v oboru tenanta, musíte splnit tyto požadavky:</span><span class="sxs-lookup"><span data-stu-id="83769-116">You must meet these prerequisites before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="83769-117">Máte přístup k uživateli **globálního správce** .</span><span class="sxs-lookup"><span data-stu-id="83769-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="83769-118">Tenant má minimálně jedno předplatné (může to být libovolný typ).</span><span class="sxs-lookup"><span data-stu-id="83769-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="83769-119">Pro globálního správce se uživateli přiřadí role **Přispěvatel** nebo vyšší pro vybrané předplatné.</span><span class="sxs-lookup"><span data-stu-id="83769-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>
- <span data-ttu-id="83769-120">Uživatel globálního správce má zvýšenou úroveň přístupu nastavenou na **Ano** (viz [přístup ke správě všech předplatných Azure a skupin pro správu](/azure/role-based-access-control/elevate-access-global-admin)).</span><span class="sxs-lookup"><span data-stu-id="83769-120">The Global administrator user has elevated access set to **Yes** (see [Elevate access to manage all Azure subscriptions and management groups](/azure/role-based-access-control/elevate-access-global-admin)).</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="83769-121">Přiřazení role správce Marketplace k PowerShellu</span><span class="sxs-lookup"><span data-stu-id="83769-121">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="83769-122">K přiřazení role správce Marketplace použijte následující skript prostředí PowerShell; vyžaduje následující parametry:</span><span class="sxs-lookup"><span data-stu-id="83769-122">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="83769-123">**TenantId:** ID tenanta v oboru (role správce Marketplace se má přiřadit v oboru tenanta).</span><span class="sxs-lookup"><span data-stu-id="83769-123">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="83769-124">**SubscriptionId:** Předplatné, ke kterému má globální správce přiřazenou roli **Přispěvatel** nebo má vyšší přiřazení.</span><span class="sxs-lookup"><span data-stu-id="83769-124">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="83769-125">**GlobalAdminUsername:** Uživatelské jméno globálního správce.</span><span class="sxs-lookup"><span data-stu-id="83769-125">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="83769-126">**UsernameToAssignRoleFor:** Uživatelské jméno, ke kterému se přiřadí role správce webu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="83769-126">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="83769-127">Pro uživatele typu Host, kteří jsou pozváni do tenanta, může trvat až 48 hodin, než bude k dispozici jejich účet pro přiřazení role správce Marketplace.</span><span class="sxs-lookup"><span data-stu-id="83769-127">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace admin role.</span></span> <span data-ttu-id="83769-128">Další informace najdete v tématu [vlastnosti Azure Active Directory uživatele spolupráce B2B](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="83769-128">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName

if($MarketPlaceAdminRole -eq $null)
{
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop
}
else
{
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available"
}

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..."
$elevatedAccessOnRoot = Get-AzRoleAssignment | where {$_.RoleDefinitionName -eq "User Access Administrator" -and $_.Scope -eq "/" -and $_.SignInName.Trim().ToLower() -eq $GlobalAdminUsername.Trim().ToLower() } | ft -Property SignInName

if($elevatedAccessOnRoot.Count -eq 0)
{
Write-Error -Message "$($GlobalAdminUsername) doesn't have permissions to assign '$($MarketplaceAdminRoleDefinitionName)'. Please verify it has elevated access 'On' in portal, https://docs.microsoft.com/en-us/azure/role-based-access-control/elevate-access-global-admin" -ErrorAction Stop
}
else
{
Write-Output "$GlobalAdminUsername has elevated access on root"
}

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

}

Assign-MarketplaceAdminRole
```

<span data-ttu-id="83769-129">Další informace o rutinách obsažených v modulu příkazového portálu AZ. Portal PowerShell najdete v tématu [Microsoft Azure PowerShell: rutiny řídicího panelu portálu](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="83769-129">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="83769-130">Vytvořit soukromé Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="83769-130">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="83769-131">Přihlaste se na [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="83769-131">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="83769-132">Vyberte **všechny služby** a potom **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="83769-132">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure Portal hlavní okno.":::

3. <span data-ttu-id="83769-134">Z možností na levé straně vyberte **soukromé tržiště** .</span><span class="sxs-lookup"><span data-stu-id="83769-134">Select **Private Marketplace** from the options on the left.</span></span>

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Výběr privátního tržiště v Azure Portal hlavním okně.":::

4. <span data-ttu-id="83769-136">Vyberte **Začínáme** pro vytvoření privátního Azure Marketplace (stačí to udělat jenom jednou).</span><span class="sxs-lookup"><span data-stu-id="83769-136">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Výběr možnosti Začínáme v hlavním okně Azure Portal.":::

    <span data-ttu-id="83769-138">Pokud pro tohoto tenanta už existuje privátní Azure Marketplace, bude ve výchozím nastavení vybraná možnost **Spravovat Marketplace** .</span><span class="sxs-lookup"><span data-stu-id="83769-138">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="83769-139">Po dokončení budete mít prázdné a zakázané soukromé Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="83769-139">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Prázdná obrazovka privátního Azure Marketplace.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="83769-141">Přidat položky z Galerie</span><span class="sxs-lookup"><span data-stu-id="83769-141">Add items from gallery</span></span>

<span data-ttu-id="83769-142">Položka je kombinací nabídky a plánu.</span><span class="sxs-lookup"><span data-stu-id="83769-142">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="83769-143">Položku můžete vyhledat a přidat na stránce Spravovat web Marketplace.</span><span class="sxs-lookup"><span data-stu-id="83769-143">You can search for and add item in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="83769-144">Vyberte **Přidat položky**.</span><span class="sxs-lookup"><span data-stu-id="83769-144">Select **Add items**.</span></span>

2. <span data-ttu-id="83769-145">Přejděte do **Galerie** nebo vyhledejte požadovanou položku pomocí vyhledávacího pole.</span><span class="sxs-lookup"><span data-stu-id="83769-145">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Procházení Galerie nebo použití vyhledávacího pole.":::

3. <span data-ttu-id="83769-147">Ve výchozím nastavení se při přidávání nové nabídky přidají všechny aktuální plány do seznamu povolených.</span><span class="sxs-lookup"><span data-stu-id="83769-147">As default, when adding a new offer, all current plans will be added to the allowed list.</span></span> <span data-ttu-id="83769-148">Chcete-li před přidáním vybraných položek změnit výběr plánu, vyberte rozevírací nabídku v dlaždici nabídky a aktualizujte požadované plány.</span><span class="sxs-lookup"><span data-stu-id="83769-148">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Aktualizujte požadované plány.":::

4. <span data-ttu-id="83769-150">Vyberte **Hotovo** vlevo dole po provedení výběru.</span><span class="sxs-lookup"><span data-stu-id="83769-150">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="83769-151">**Přidat položky** na web Marketplace budou k dispozici pouze pro nabídky, které nejsou od Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="83769-151">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="83769-152">Nabídky společnosti Microsoft jsou ve výchozím nastavení povoleny.</span><span class="sxs-lookup"><span data-stu-id="83769-152">Microsoft offers are allowed by default.</span></span>

## <a name="edit-item-plans"></a><span data-ttu-id="83769-153">Upravit plány položek</span><span class="sxs-lookup"><span data-stu-id="83769-153">Edit item plans</span></span>

<span data-ttu-id="83769-154">Plány položky můžete upravit na stránce Spravovat web Marketplace.</span><span class="sxs-lookup"><span data-stu-id="83769-154">You can edit an item's plans in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="83769-155">Ve sloupci **plány** zkontrolujte dostupné plány z rozevírací nabídky pro danou položku.</span><span class="sxs-lookup"><span data-stu-id="83769-155">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="83769-156">Zaškrtnutím nebo zrušením zaškrtnutí políček zvolte, které plány mají být uživatelům k dispozici.</span><span class="sxs-lookup"><span data-stu-id="83769-156">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Zaškrtněte nebo zrušte zaškrtnutí políčka pro požadovanou položku.":::

> [!NOTE]
> <span data-ttu-id="83769-158">U každé nabídky je nutné vybrat alespoň jeden plán, aby došlo k aktualizaci.</span><span class="sxs-lookup"><span data-stu-id="83769-158">Each offer needs at least one plan selected in order for the update to occur.</span></span> <span data-ttu-id="83769-159">Chcete-li odebrat všechny plány související s nabídkou, odstraňte celou nabídku (viz další oddíl).</span><span class="sxs-lookup"><span data-stu-id="83769-159">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="83769-160">Odstranit nabídky</span><span class="sxs-lookup"><span data-stu-id="83769-160">Delete offers</span></span>

<span data-ttu-id="83769-161">Na stránce Spravovat Marketplace zaškrtněte políčko vedle názvu nabídky (viz obrazovka výše) a vyberte **Odstranit položky**.</span><span class="sxs-lookup"><span data-stu-id="83769-161">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="83769-162">Povolit nebo zakázat privátní Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="83769-162">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="83769-163">Na stránce Spravovat Marketplace se zobrazí jedna z těchto proužkových proužků, která zobrazí aktuální stav privátních Azure Marketplace:</span><span class="sxs-lookup"><span data-stu-id="83769-163">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Deaktivovat banner stavu":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Povolit banner stavu":::

<span data-ttu-id="83769-166">V případě potřeby můžete povolit nebo zakázat privátní Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="83769-166">You can enable or disable Private Azure Marketplace as needed.</span></span>

1. <span data-ttu-id="83769-167">Pokud je tato možnost zakázaná, vyberte **Povolit privátní tržiště** .</span><span class="sxs-lookup"><span data-stu-id="83769-167">If disabled, select **Enable Private Marketplace** to enable.</span></span>
2. <span data-ttu-id="83769-168">Pokud je povoleno, vyberte **Zakázat privátní tržiště** , které chcete zakázat.</span><span class="sxs-lookup"><span data-stu-id="83769-168">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="83769-169">Procházení soukromých Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="83769-169">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="83769-170">Když je povolený privátní Azure Marketplace, uživatelé uvidí, které plány má správce Marketplace povolený.</span><span class="sxs-lookup"><span data-stu-id="83769-170">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has allowed.</span></span>

- <span data-ttu-id="83769-171">Zelené **povolené** oznámení značí, že je povolená nabídka partnera (jiné než Microsoft).</span><span class="sxs-lookup"><span data-stu-id="83769-171">A green **Allowed** notice indicates a Partner (non-Microsoft) offer that is allowed.</span></span>
- <span data-ttu-id="83769-172">Modré **povolené** oznámení indikuje, že je povolená nabídka Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="83769-172">A blue **Allowed** notice indicates a Microsoft offer that is allowed.</span></span>

<span data-ttu-id="83769-173">Uživatelé mohou filtrovat mezi nabídkami, které nejsou a nejsou povoleny:</span><span class="sxs-lookup"><span data-stu-id="83769-173">Users can filter between offers that are and are not allowed:</span></span>

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Možnost filtrování":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="83769-175">Koupit nebo nasadit v privátních Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="83769-175">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="83769-176">I když je prostředí stránky s podrobnostmi o produktu podobné veřejnému Azure Marketplace, existují tři privátní Azure Marketplace specifické scénáře.</span><span class="sxs-lookup"><span data-stu-id="83769-176">While the product details page experience is similar to the public Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="83769-177">Když uživatel vybere povolený plán, aktivuje se tlačítko **vytvořit** :</span><span class="sxs-lookup"><span data-stu-id="83769-177">When a user selects an allowed plan, the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Informační zpráva nabídky, která označuje plán, se dá vytvořit.":::

- <span data-ttu-id="83769-179">Když uživatel vybere nepovolený plán, banner se zaznamená, že plán není povolený a tlačítko **vytvořit** je zakázané.</span><span class="sxs-lookup"><span data-stu-id="83769-179">When a user selects a non-allowed plan, a banner notes that the plan is not allowed and the **Create** button is disabled.</span></span>

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Banner nabídky, který označuje plán, nejde vytvořit.":::

- <span data-ttu-id="83769-181">Pokud se výběr plánu produktu nezobrazuje na stránce s podrobnostmi o produktu, ale správce schválil jeden nebo více plánů, poznamenejte si, které plány jsou povolené a že je povolené tlačítko **vytvořit** :</span><span class="sxs-lookup"><span data-stu-id="83769-181">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are allowed and the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Banner nabídky, který označuje plán, se dá vytvořit a Zobrazit dostupné plány.":::

## <a name="contact-support"></a><span data-ttu-id="83769-183">Kontaktování podpory</span><span class="sxs-lookup"><span data-stu-id="83769-183">Contact support</span></span>

<span data-ttu-id="83769-184">Podporu Azure Marketplace najdete na webu [Microsoft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="83769-184">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span> 
