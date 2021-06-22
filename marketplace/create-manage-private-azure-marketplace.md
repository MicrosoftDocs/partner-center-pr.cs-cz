---
title: Vytvoření a správa privátních Azure Marketplace v Azure Portal
description: Přečtěte si o vytváření a správě privátních Azure Marketplace (Preview) v Azure Portal. Privátní Azure Marketplace (Preview) umožňuje správcům řídit, která řešení třetích stran můžou uživatelé používat.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 9da9eb4944508e815d1664fb44b13bce52f37150
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431675"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="ad914-104">Vytvoření a správa privátních Azure Marketplace v Azure Portal</span><span class="sxs-lookup"><span data-stu-id="ad914-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="ad914-105">Privátní Azure Marketplace umožňuje správcům řídit, která řešení třetích stran můžou uživatelé používat.</span><span class="sxs-lookup"><span data-stu-id="ad914-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="ad914-106">Umožňuje uživateli nasadit pouze nabídky, které jsou schválené správcem a jsou v souladu se zásadami vašeho podniku.</span><span class="sxs-lookup"><span data-stu-id="ad914-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="ad914-107">Díky privátním Azure Marketplace mohou uživatelé hledat v online obchodě vyhovující nabídky, které si kupovat a nasazovat.</span><span class="sxs-lookup"><span data-stu-id="ad914-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="ad914-108">Jako správce Marketplace (přiřazená role) začnete se zakázaným a prázdným privátním úložištěm, ve kterém můžete přidat schválené nabídky a plány.</span><span class="sxs-lookup"><span data-stu-id="ad914-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="ad914-109">Tento článek vysvětluje, jak přiřadit potřebnou roli, vytvořit privátní úložiště, spravovat položky, schvalovat žádosti uživatelů a povolit privátní Azure Marketplace pro vaše uživatele.</span><span class="sxs-lookup"><span data-stu-id="ad914-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="ad914-110">Privátní Azure Marketplace je na úrovni tenanta, takže všichni uživatelé v tenantovi uvidí stejný kurátorovaný seznam.</span><span class="sxs-lookup"><span data-stu-id="ad914-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="ad914-111">Všechna řešení Microsoftu (včetně [schvalovaných linuxových](/azure/virtual-machines/linux/endorsed-distros)distribucí) se automaticky přidávají do privátních Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="ad914-111">All Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="ad914-112">Přiřazení role správce Marketplace</span><span class="sxs-lookup"><span data-stu-id="ad914-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="ad914-113">Správce tenanta Globální správce roli správce **Marketplace** správci privátního úložiště Azure Marketplace který bude privátní úložiště spravovat.</span><span class="sxs-lookup"><span data-stu-id="ad914-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="ad914-114">Přístup ke správě privátních Azure Marketplace je dostupný jenom správcům IT s přiřazenou rolí správce Marketplace.</span><span class="sxs-lookup"><span data-stu-id="ad914-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="ad914-115">Požadavky</span><span class="sxs-lookup"><span data-stu-id="ad914-115">Prerequisites</span></span>

<span data-ttu-id="ad914-116">Před přiřazením role správce Marketplace uživateli v oboru tenanta se vyžaduje splnění těchto požadavků:</span><span class="sxs-lookup"><span data-stu-id="ad914-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="ad914-117">Máte přístup k **Globální správce** uživateli.</span><span class="sxs-lookup"><span data-stu-id="ad914-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="ad914-118">Tenant má alespoň jedno předplatné (může být libovolného typu).</span><span class="sxs-lookup"><span data-stu-id="ad914-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="ad914-119">Uživatel Globální správce vybranému **předplatnému** přiřazenou roli Přispěvatel nebo vyšší.</span><span class="sxs-lookup"><span data-stu-id="ad914-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="ad914-120">Přiřazení role správce Marketplace pomocí řízení přístupu (IAM)</span><span class="sxs-lookup"><span data-stu-id="ad914-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="ad914-121">Přihlaste se k webu [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="ad914-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
1. <span data-ttu-id="ad914-122">Vyberte **Všechny služby a** pak **Marketplace.**</span><span class="sxs-lookup"><span data-stu-id="ad914-122">Select **All services** and then **Marketplace**.</span></span>
1. <span data-ttu-id="ad914-123">V **nabídce na** levé straně vyberte Privátní Marketplace.</span><span class="sxs-lookup"><span data-stu-id="ad914-123">Select **Private Marketplace** from the menu on the left.</span></span>

    <span data-ttu-id="ad914-124">[![Zobrazuje možnost nabídky privátního marketplace na levé straně Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ad914-124">[![Shows the private marketplace menu option on the left side of the Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span></span>

1. <span data-ttu-id="ad914-125">Vyberte **Řízení přístupu (IAM)** a přiřaďte roli správce Marketplace.</span><span class="sxs-lookup"><span data-stu-id="ad914-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Zobrazuje obrazovku řízení přístupu K A M.":::

1. <span data-ttu-id="ad914-127">Vyberte **+ Přidat** > **Přidat přiřazení role**.</span><span class="sxs-lookup"><span data-stu-id="ad914-127">Select **+ Add** > **Add role assignment**.</span></span>
1. <span data-ttu-id="ad914-128">V **části Role** zvolte Správce **Marketplace.**</span><span class="sxs-lookup"><span data-stu-id="ad914-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Zobrazí nabídku Přiřazení role.":::

1. <span data-ttu-id="ad914-130">V rozevíracím seznamu vyberte požadovaného uživatele a pak vyberte **Hotovo.**</span><span class="sxs-lookup"><span data-stu-id="ad914-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="ad914-131">Přiřazení role správce Marketplace pomocí PowerShellu</span><span class="sxs-lookup"><span data-stu-id="ad914-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="ad914-132">Pomocí následujícího skriptu PowerShellu přiřaďte roli správce Marketplace. Vyžaduje následující parametry:</span><span class="sxs-lookup"><span data-stu-id="ad914-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="ad914-133">**Id tenanta:** ID tenanta v oboru (roli správce Marketplace je možné přiřadit v oboru tenanta).</span><span class="sxs-lookup"><span data-stu-id="ad914-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="ad914-134">**Id předplatného:** Předplatné, ke kterému má globální správce **přiřazenou** roli Přispěvatel nebo vyšší.</span><span class="sxs-lookup"><span data-stu-id="ad914-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="ad914-135">**GlobalAdminUsername:** Uživatelské jméno globálního správce.</span><span class="sxs-lookup"><span data-stu-id="ad914-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="ad914-136">**UsernameToAssignRoleFor:** Uživatelské jméno, ke kterému bude přiřazena role správce Marketplace.</span><span class="sxs-lookup"><span data-stu-id="ad914-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="ad914-137">Pro uživatele hosta pozvané do tenanta může trvat až 48 hodin, než bude jejich účet k dispozici pro přiřazení role správce Marketplace.</span><span class="sxs-lookup"><span data-stu-id="ad914-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="ad914-138">Další informace najdete v tématu [Vlastnosti uživatele Azure Active Directory B2B.](/azure/active-directory/b2b/user-properties)</span><span class="sxs-lookup"><span data-stu-id="ad914-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="ad914-139">Další informace o rutinách obsažených v modulu Az.Portal PowerShellu najdete v [Microsoft Azure PowerShell: Rutiny řídicího panelu portálu](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="ad914-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="ad914-140">Vytvoření privátního Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="ad914-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="ad914-141">Přihlaste se k webu [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="ad914-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="ad914-142">Vyberte **Všechny služby a** pak **Marketplace.**</span><span class="sxs-lookup"><span data-stu-id="ad914-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Zobrazí hlavní Azure Portal okno.":::

3. <span data-ttu-id="ad914-144">V **nabídce na** levé straně vyberte Privátní Marketplace.</span><span class="sxs-lookup"><span data-stu-id="ad914-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="ad914-145">Vyberte **Začínáme a** vytvořte privátní Azure Marketplace (to musíte udělat jenom jednou).</span><span class="sxs-lookup"><span data-stu-id="ad914-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Ukazuje, jak vybrat hlavní okno Začínáme Azure Portal okně.":::

    <span data-ttu-id="ad914-147">Pokud privátní Azure Marketplace pro tohoto tenanta již existuje, bude ve výchozím nastavení vybraná možnost Spravovat **Marketplace.**</span><span class="sxs-lookup"><span data-stu-id="ad914-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="ad914-148">Po dokončení budete mít prázdný a zakázaný privátní Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="ad914-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Zobrazí prázdnou obrazovku privátního Azure Marketplace obrazovky.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="ad914-150">Přidání položek z galerie</span><span class="sxs-lookup"><span data-stu-id="ad914-150">Add items from gallery</span></span>

<span data-ttu-id="ad914-151">Položka je kombinací nabídky a plánu.</span><span class="sxs-lookup"><span data-stu-id="ad914-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="ad914-152">Položky můžete vyhledat a přidat na stránce Spravovat Marketplace.</span><span class="sxs-lookup"><span data-stu-id="ad914-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="ad914-153">Vyberte **Přidat položky.**</span><span class="sxs-lookup"><span data-stu-id="ad914-153">Select **Add items**.</span></span>

2. <span data-ttu-id="ad914-154">Přejděte do **Galerie** nebo pomocí vyhledávacího pole najděte položku, kterou chcete.</span><span class="sxs-lookup"><span data-stu-id="ad914-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    <span data-ttu-id="ad914-155">[![Ukazuje, jak procházet galerii nebo použít vyhledávací pole.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ad914-155">[![Shows how to browse the gallery or use the search field.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span></span>

3. <span data-ttu-id="ad914-156">Ve výchozím nastavení se při přidávání nové nabídky všechny aktuální plány přidávají do seznamu schválených plánů.</span><span class="sxs-lookup"><span data-stu-id="ad914-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="ad914-157">Pokud chcete před přidáním vybraných položek upravit výběr plánu, vyberte rozevírací nabídku na dlaždici nabídky a aktualizujte požadované plány.</span><span class="sxs-lookup"><span data-stu-id="ad914-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Ukazuje, jak aktualizovat požadované plány.":::

4. <span data-ttu-id="ad914-159">Po **provedení** výběru vyberte v levém dolním rohu Hotovo.</span><span class="sxs-lookup"><span data-stu-id="ad914-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="ad914-160">**Možnost Přidat** položky na Marketplace bude dostupná jenom pro nabídky od jiných společností než Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ad914-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="ad914-161">Řešení Microsoftu (včetně [schválených linuxových](/azure/virtual-machines/linux/endorsed-distros)distribucí) budou ve výchozím nastavení označená jako Schválená a nelze je spravovat na privátním marketplace.</span><span class="sxs-lookup"><span data-stu-id="ad914-161">Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) will be tagged as “Approved by default” and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="ad914-162">Úprava plánů položek</span><span class="sxs-lookup"><span data-stu-id="ad914-162">Edit item's plans</span></span>

<span data-ttu-id="ad914-163">Plány položky můžete upravit na stránce Spravovat Marketplace.</span><span class="sxs-lookup"><span data-stu-id="ad914-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="ad914-164">Ve **sloupci** Plány zkontrolujte dostupné plány z rozevírací nabídky pro tuto položku.</span><span class="sxs-lookup"><span data-stu-id="ad914-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="ad914-165">Zaškrtnutím nebo zrušte zaškrtnutí políček, abyste zvolili, které plány budou uživatelům k dispozici.</span><span class="sxs-lookup"><span data-stu-id="ad914-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Ukazuje, jak vybrat nebo vymazat zaškrtávací políčko pro požadovanou položku.":::

> [!NOTE]
> <span data-ttu-id="ad914-167">Každá nabídka musí mít vybraný alespoň jeden plán, aby k aktualizaci došlo.</span><span class="sxs-lookup"><span data-stu-id="ad914-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="ad914-168">Pokud chcete odebrat všechny plány související s nabídkou, odstraňte celou nabídku (viz další část).</span><span class="sxs-lookup"><span data-stu-id="ad914-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="ad914-169">Odstranění nabídek</span><span class="sxs-lookup"><span data-stu-id="ad914-169">Delete offers</span></span>

<span data-ttu-id="ad914-170">Na stránce Spravovat Marketplace zaškrtněte políčko vedle názvu nabídky (viz obrazovka výše) a vyberte **Odstranit položky**.</span><span class="sxs-lookup"><span data-stu-id="ad914-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="ad914-171">Povolení nebo zakázání privátních Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="ad914-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="ad914-172">Na stránce Spravovat Marketplace se zobrazí jeden z těchto bannerů, které zobrazují aktuální stav privátních Azure Marketplace:</span><span class="sxs-lookup"><span data-stu-id="ad914-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Zobrazí banner Disable state (Zakázat stav).":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Zobrazí banner Enable state (Povolit stav).":::

<span data-ttu-id="ad914-175">Podle potřeby můžete privátní Azure Marketplace zakázat.</span><span class="sxs-lookup"><span data-stu-id="ad914-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="ad914-176">Pokud je zakázané, **povolte povolení výběrem možnosti** Povolit privátní marketplace.</span><span class="sxs-lookup"><span data-stu-id="ad914-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="ad914-177">Pokud je tato možnost povolená, **zakažte** ji výběrem možnosti Zakázat privátní marketplace.</span><span class="sxs-lookup"><span data-stu-id="ad914-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="ad914-178">Centrum Azure Marketplace oznámení služby Private Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="ad914-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="ad914-179">Centrum oznámení se skládá ze tří typů oznámení a umožňuje správci Marketplace provádět akce na základě oznámení:</span><span class="sxs-lookup"><span data-stu-id="ad914-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="ad914-180">Žádosti uživatelů o schválení položek, které nejsou v seznamu schválených položek (viz žádost o [přidání nabídek nebo plánů](#request-to-add-offers-or-plans) níže).</span><span class="sxs-lookup"><span data-stu-id="ad914-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="ad914-181">Oznámení o novém plánu pro nabídky, které už mají jeden nebo více plánů v seznamu schválených</span><span class="sxs-lookup"><span data-stu-id="ad914-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="ad914-182">Odebrání oznámení plánu pro položky, které jsou v seznamu schválených položek, které byly odebrány z globálního Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="ad914-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="ad914-183">Přístup k centru oznámení:</span><span class="sxs-lookup"><span data-stu-id="ad914-183">To access the notification center:</span></span>

1. <span data-ttu-id="ad914-184">V **nabídce vlevo** vyberte Oznámení.</span><span class="sxs-lookup"><span data-stu-id="ad914-184">Select **Notifications** from the left-side menu.</span></span>

    <span data-ttu-id="ad914-185">[![Zobrazí nabídku Oznámení.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ad914-185">[![Shows the Notifications menu.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span></span>

1. <span data-ttu-id="ad914-186">Výběrem nabídky se třemi tečkami zobrazíte další akce.</span><span class="sxs-lookup"><span data-stu-id="ad914-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Zobrazí výsledky nabídky Další možnosti.":::

1. <span data-ttu-id="ad914-188">V případě žádostí o plán **otevře možnost** Zobrazit žádosti formulář žádosti o schválení, kde můžete zkontrolovat všechny žádosti uživatelů o konkrétní nabídku.</span><span class="sxs-lookup"><span data-stu-id="ad914-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="ad914-189">Vyberte **Schválit** nebo **Odmítnout.**</span><span class="sxs-lookup"><span data-stu-id="ad914-189">Select **Approve** or **Reject**.</span></span>

    <span data-ttu-id="ad914-190">[![Zobrazí možnosti schválit a odmítnout.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ad914-190">[![Shows the approve and reject options.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span></span>

1. <span data-ttu-id="ad914-191">V rozevírací nabídce vyberte plán ke schválení.</span><span class="sxs-lookup"><span data-stu-id="ad914-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="ad914-192">Přidejte komentář a vyberte **Odeslat.**</span><span class="sxs-lookup"><span data-stu-id="ad914-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="ad914-193">Procházení privátních Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="ad914-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="ad914-194">Když je Azure Marketplace privátní účet povolený, uživatelé uvidí, které plány správce Marketplace schválil.</span><span class="sxs-lookup"><span data-stu-id="ad914-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="ad914-195">Zelené schválené **oznámení** značí schválenou nabídku partnera (jiné společnosti než Microsoft).</span><span class="sxs-lookup"><span data-stu-id="ad914-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="ad914-196">Modré schválené **oznámení** označuje nabídku Microsoftu (včetně [schválených linuxových](/azure/virtual-machines/linux/endorsed-distros)distribucí), která je schválená.</span><span class="sxs-lookup"><span data-stu-id="ad914-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="ad914-197">Uživatelé mohou filtrovat mezi nabídkami, které jsou a nejsou schválené:</span><span class="sxs-lookup"><span data-stu-id="ad914-197">Users can filter between offers that are and are not approved:</span></span>

<span data-ttu-id="ad914-198">[![Zobrazí možnost filtrování.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ad914-198">[![Shows the filtering option.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span></span>

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="ad914-199">Nákup nebo nasazení v privátním Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="ad914-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="ad914-200">Stránka s podrobnostmi o produktu se podobá globálnímu prostředí Azure Marketplace, ale existují tři scénáře, které Azure Marketplace privátním prostředím.</span><span class="sxs-lookup"><span data-stu-id="ad914-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="ad914-201">Když uživatel vybere schválený plán, **tlačítko** Vytvořit se povolí:</span><span class="sxs-lookup"><span data-stu-id="ad914-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

    <span data-ttu-id="ad914-202">[![Zobrazuje banner nabídky s nápisem, že je možné vytvořit plán.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ad914-202">[![Shows the offer banner noting a plan can be created.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span></span>

- <span data-ttu-id="ad914-203">Pokud se výběr plánu produktu nezobrazí na stránce s podrobnostmi o produktu, ale správce  schválil jeden nebo více plánů, zobrazí se banner s upozorněním, které plány jsou schválené a tlačítko Vytvořit je povolené:</span><span class="sxs-lookup"><span data-stu-id="ad914-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

    <span data-ttu-id="ad914-204">[![Zobrazuje banner nabídky s nápisem, že plán je možné vytvořit a zobrazit dostupné plány.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ad914-204">[![Shows the offer banner noting that a plan can be created and showing available plans.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span></span>

- <span data-ttu-id="ad914-205">Když uživatel vybere neschválený plán, zobrazí se banner s upozorněním, že se plán neschválí, a tlačítko Vytvořit **se** deaktivuje.</span><span class="sxs-lookup"><span data-stu-id="ad914-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="ad914-206">Uživatel může požádat o přidání plánu do seznamu schválených položek (viz další část).</span><span class="sxs-lookup"><span data-stu-id="ad914-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="ad914-207">Žádost o přidání nabídek nebo plánů</span><span class="sxs-lookup"><span data-stu-id="ad914-207">Request to add offers or plans</span></span>

<span data-ttu-id="ad914-208">Můžete požádat o přidání veřejné nabídky nebo plánu, které nejsou aktuálně schválené v privátním Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="ad914-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="ad914-209">Výběrem **možnosti Request to add** (Žádost o přidání) v banneru otevřete formulář žádosti o **přístup.**</span><span class="sxs-lookup"><span data-stu-id="ad914-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

    <span data-ttu-id="ad914-210">[![Zobrazí banner s odkazem Požádat o přidání.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ad914-210">[![Shows the banner with the 'Request to add' link.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span></span>

    <span data-ttu-id="ad914-211">[![Zobrazí formulář žádosti o přístup pro nabídky nebo plány.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ad914-211">[![Shows the access request form for offers or plans.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span></span>

1. <span data-ttu-id="ad914-212">Vyberte plány, které chcete k žádosti přidat **(Jakýkoli** plán informuje správce Marketplace, že pro plán v rámci nabídky nemáte nějaké preference).</span><span class="sxs-lookup"><span data-stu-id="ad914-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="ad914-213">Přidejte **justification (Odůvodnění)** a **vyberte Request** to submit your request (Žádost o odeslání žádosti).</span><span class="sxs-lookup"><span data-stu-id="ad914-213">Add a **Justification** and select **Request** to submit your request.</span></span>
  
    <span data-ttu-id="ad914-214">[![Zobrazí formulář žádosti o přístup pro nabídky nebo plány s ukázkovými položkami.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ad914-214">[![Shows the access request form for offers or plans with sample entries.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span></span>

1. <span data-ttu-id="ad914-215">Ve formuláři žádosti o přístup se zobrazí indikace čekající žádosti s možností Žádosti **o žádost o přístup**.</span><span class="sxs-lookup"><span data-stu-id="ad914-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

    <span data-ttu-id="ad914-216">[![Zobrazí seznam schválených nebo nevyřízených plánů s odkazem Na žádost o schválení.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ad914-216">[![Shows a list of approved or pending plans with Withdraw Request link.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span></span>

> [!NOTE]
> <span data-ttu-id="ad914-217">Po odeslání se formulář žádosti o [](#private-azure-marketplace-notification-center) schválení zasílá správci Marketplace do Centra oznámení, aby žádost zkontrolovat a provést akci.</span><span class="sxs-lookup"><span data-stu-id="ad914-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

> [!CAUTION]
> <span data-ttu-id="ad914-218">Schválení na privátním marketplace neznačí nákup řešení.</span><span class="sxs-lookup"><span data-stu-id="ad914-218">Approval into Private Marketplace does not indicate procurement of a solution.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="ad914-219">Nejčastější dotazy</span><span class="sxs-lookup"><span data-stu-id="ad914-219">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="ad914-220">Aplikaci třetí strany z Marketplace už blokujem prostřednictvím Azure Policy.</span><span class="sxs-lookup"><span data-stu-id="ad914-220">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="ad914-221">Jak se to liší?</span><span class="sxs-lookup"><span data-stu-id="ad914-221">How is this different?</span></span>

<span data-ttu-id="ad914-222">V současné době existují dva způsoby, jak na Marketplace omezit služby třetích stran:</span><span class="sxs-lookup"><span data-stu-id="ad914-222">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="ad914-223">Prostřednictvím portálu EA portal nebo Azure Portal zakažte služby třetích stran nebo omezte na "Pouze skladové sklady Free nebo BYOL".</span><span class="sxs-lookup"><span data-stu-id="ad914-223">Through EA portal or the Azure portal, disable third-party services or restrict to “Free or BYOL SKUs only”.</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Ukazuje, jak omezit služby v Azure Portal.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Ukazuje, jak omezit služby na portálu E A.":::

2. <span data-ttu-id="ad914-226">Vytvořte zásadu Azure, která povolí jenom konkrétní virtuální počítače.</span><span class="sxs-lookup"><span data-stu-id="ad914-226">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="ad914-227">Podrobnosti o tom, jak vynutit zásady pro virtuální počítače s Windows, najdete v tématu Použití zásad na virtuální počítače s [Windows pomocí Azure Resource Manager](/azure/virtual-machines/windows/policy).</span><span class="sxs-lookup"><span data-stu-id="ad914-227">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="ad914-228">Privátní Azure Marketplace nabízí větší flexibilitu při omezování a povolování konkrétních nabídek a plánů.</span><span class="sxs-lookup"><span data-stu-id="ad914-228">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="ad914-229">Informuje koncové uživatele o dostupnosti nasazení v galerii Marketplace ještě předtím, než se pokusí nasadit služby třetích stran.</span><span class="sxs-lookup"><span data-stu-id="ad914-229">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="ad914-230">Pokud chcete povolit nasazení služeb třetích stran, nastavte Azure Marketplace na Zapnuto/povoleno v EA Portal a Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="ad914-230">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="ad914-231">Privátní Azure Marketplace může partnerská řešení nastavit nejen na virtuální počítače.</span><span class="sxs-lookup"><span data-stu-id="ad914-231">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="ad914-232">Privátní Azure Marketplace může být na úrovni plánu a může také nastavit aktuální a budoucí plán.</span><span class="sxs-lookup"><span data-stu-id="ad914-232">Private Azure Marketplace can curate at the plan level and can also set “Current and future plan”.</span></span>
- <span data-ttu-id="ad914-233">Privátní Azure Marketplace může předem informovat koncové uživatele o tom, co může a nemůže být nasazeno.</span><span class="sxs-lookup"><span data-stu-id="ad914-233">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="ad914-234">Jaký je rozdíl mezi privátní nabídkou a privátní nabídkou Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="ad914-234">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="ad914-235">Privátní **nabídka umožňuje vydavatelům** vytvářet plány, které jsou viditelné pouze cílovým zákazníkům.</span><span class="sxs-lookup"><span data-stu-id="ad914-235">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="ad914-236">Díky tomu mohou soukromě sdílet přizpůsobená řešení s vyjednanou cenou, privátními podmínkami a zvláštními konfiguracemi.</span><span class="sxs-lookup"><span data-stu-id="ad914-236">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="ad914-237">Podrobnosti najdete v tématu [Privátní nabídky na komerčním marketplace.](/azure/marketplace/private-offers)</span><span class="sxs-lookup"><span data-stu-id="ad914-237">For details, see [Private offers in the commercial marketplace](/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="ad914-238">**Privátní Azure Marketplace** v Azure Portal umožňuje správcům předem schválit, která řešení třetích stran můžou jejich uživatelé nasadit.</span><span class="sxs-lookup"><span data-stu-id="ad914-238">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="ad914-239">Díky privátní Azure Marketplace mohou uživatelé využívat výhody těchto Azure Marketplace hledáním, nákupem a nasazením vyhovujících nabídek.</span><span class="sxs-lookup"><span data-stu-id="ad914-239">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="ad914-240">Pokud chcete spravovat privátní nabídky založené na předplatném na privátním marketplace, musí mít správce Marketplace minimální roli čtení pro konkrétní předplatné.</span><span class="sxs-lookup"><span data-stu-id="ad914-240">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of “read” role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="ad914-241">Proč se privátní nabídka po přidání Azure Marketplace nezobrazuje na kartě Spravovat marketplace?</span><span class="sxs-lookup"><span data-stu-id="ad914-241">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="ad914-242">Privátní nabídky založené na předplatném jsou viditelné jenom pro uvedená předplatná v nastavení privátní nabídky.</span><span class="sxs-lookup"><span data-stu-id="ad914-242">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="ad914-243">Pokud chcete zobrazit privátní nabídku, ujistěte se, že globální filtr předplatných zobrazuje všechna předplatná.</span><span class="sxs-lookup"><span data-stu-id="ad914-243">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

<span data-ttu-id="ad914-244">[![Zobrazí filtr privátního marketplace.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="ad914-244">[![Shows the private marketplace filter.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span></span>

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="ad914-245">Můžeme do privátních imagí zahrnout Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="ad914-245">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="ad914-246">No.</span><span class="sxs-lookup"><span data-stu-id="ad914-246">No.</span></span> <span data-ttu-id="ad914-247">Privátní Azure Marketplace umožňuje libovolnému správci IT spravovat a spravovat řešení třetích stran z globálních Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="ad914-247">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="ad914-248">Vzhledem k tomu, že vlastní image nejsou v globální Azure Marketplace, správce IT nemůže vybrat a vybrat vlastní image.</span><span class="sxs-lookup"><span data-stu-id="ad914-248">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="ad914-249">Pokud chcete sdílet vlastní image, použijte [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).</span><span class="sxs-lookup"><span data-stu-id="ad914-249">If you would like to share custom images, use [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="ad914-250">Podrobný průvodce Vytvořením Shared Image Gallery (SIG)[(CLI,](/azure/virtual-machines/shared-images-cli) [PowerShell).](/azure/virtual-machines/shared-images-powershell)</span><span class="sxs-lookup"><span data-stu-id="ad914-250">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="ad914-251">Vytvořte definici image v rámci SKUPINY SIG.</span><span class="sxs-lookup"><span data-stu-id="ad914-251">Create an image definition within a SIG.</span></span> <span data-ttu-id="ad914-252">Zákazník by měl **jako pole** Stav operačního systému zvolit Generalized (Generalizované).</span><span class="sxs-lookup"><span data-stu-id="ad914-252">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="ad914-253">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span><span class="sxs-lookup"><span data-stu-id="ad914-253">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="ad914-254">Přenést spravovanou image do Shared Image Gallery ([ROZHRANÍ příkazového řádku](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span><span class="sxs-lookup"><span data-stu-id="ad914-254">Bring managed image into the Shared Image Gallery ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="ad914-255">Image virtuálních počítače SIG se nacházejí v jednom předplatném.</span><span class="sxs-lookup"><span data-stu-id="ad914-255">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="ad914-256">K jeho zvidilení pro ostatní předplatná použijte registraci aplikace ([CLI,](/azure/virtual-machines/linux/share-images-across-tenants) [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).</span><span class="sxs-lookup"><span data-stu-id="ad914-256">To make it available to other subscriptions, use an app registration ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="ad914-257">Proč se některé nabídky ve výchozím nastavení **schvalují,** i když vydavatel není Microsoft?</span><span class="sxs-lookup"><span data-stu-id="ad914-257">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="ad914-258">Microsoft podporuje linuxovou a open source technologii v Azure.</span><span class="sxs-lookup"><span data-stu-id="ad914-258">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="ad914-259">[Schválené linuxové distribuce jsou](/azure/virtual-machines/linux/endorsed-distros) podporované v Azure a cena je integrovaná ve virtuálních počítačích.</span><span class="sxs-lookup"><span data-stu-id="ad914-259">[Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="ad914-260">Vzhledem k tomu, že agent Azure Linux je už na zařízeních Azure Marketplace, je považován za nabídku Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="ad914-260">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="ad914-261">Vzhledem k tomu, že nabídky Microsoftu jsou standardně schválené, schválené linuxové distribuce se nespravují v privátních Azure Marketplace a ve výchozím nastavení se schvalují.</span><span class="sxs-lookup"><span data-stu-id="ad914-261">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="ad914-262">Kontaktování podpory</span><span class="sxs-lookup"><span data-stu-id="ad914-262">Contact support</span></span>

- <span data-ttu-id="ad914-263">Další Azure Marketplace najdete na webu [Microsoft Q&A.](/answers/products/)</span><span class="sxs-lookup"><span data-stu-id="ad914-263">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>