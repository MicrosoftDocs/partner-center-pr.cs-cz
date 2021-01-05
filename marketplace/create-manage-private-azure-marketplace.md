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
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a>Vytvoření a Správa privátních Azure Marketplace (Preview) v Azure Portal

Privátní Azure Marketplace (Preview) umožňuje správcům řídit, která řešení třetích stran můžou uživatelé používat. Díky tomu můžete nasadit jenom nabídky, které schválíte a které jsou v rozporu s podnikovými zásadami. S privátními Azure Marketplace můžou vaši uživatelé hledat v online obchodě, aby si mohli koupit a nasadit. 

Jako správce Marketplace (přiřazená role) začnete s neaktivním a prázdným soukromým úložištěm, kde můžete přidat vaše schválené nabídky a plány. Tento článek vysvětluje, jak vytvořit, spravovat a povolit soukromé Azure Marketplace pro vaše uživatele.

Poznámky:

- Soukromé Azure Marketplace jsou na úrovni tenanta, takže všichni uživatelé v tenantovi uvidí stejný seznam.
- Všechna řešení společnosti Microsoft jsou automaticky přidána do privátního Azure Marketplace.

## <a name="assign-the-marketplace-admin-role"></a>Přiřazení role správce Marketplace

Globální správce tenanta musí přiřadit roli **správce Marketplace** správci privátního Azure Marketplace, který bude spravovat soukromé úložiště.

>[!IMPORTANT]
> Přístup ke správě privátních Azure Marketplace je k dispozici jenom správcům IT, kteří mají přiřazenou roli správce Marketplace.

### <a name="prerequisites"></a>Předpoklady

Abyste mohli přiřadit roli správce Marketplace uživateli v oboru tenanta, musíte splnit tyto požadavky:

- Máte přístup k uživateli **globálního správce** .
- Tenant má minimálně jedno předplatné (může to být libovolný typ).
- Pro globálního správce se uživateli přiřadí role **Přispěvatel** nebo vyšší pro vybrané předplatné.

### <a name="assign-the-marketplace-admin-role-with-iam"></a>Přiřazení role správce Marketplace k IAM

1. Přihlaste se na web [Azure Portal](https://portal.azure.com/).
1. Vyberte **všechny služby** a potom **Marketplace**.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure Portal hlavní okno.":::

3. Z možností na levé straně vyberte **soukromé tržiště** .
1. Vyberte **řízení přístupu (IAM)** a přiřaďte roli správce webu Marketplace.

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Obrazovka řízení přístupu IAM.":::

1. Vyberte **+ Přidat** > **Přidat přiřazení role**.
1. V části **role** vyberte **správce Marketplace**.

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Nabídka přiřazení role":::

1. V rozevíracím seznamu vyberte požadovaného uživatele a potom vyberte **Hotovo**.

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>Přiřazení role správce Marketplace k PowerShellu

K přiřazení role správce Marketplace použijte následující skript prostředí PowerShell; vyžaduje následující parametry:

- **TenantId:** ID tenanta v oboru (role správce Marketplace se má přiřadit v oboru tenanta).
- **SubscriptionId:** Předplatné, ke kterému má globální správce přiřazenou roli **Přispěvatel** nebo má vyšší přiřazení.
- **GlobalAdminUsername:** Uživatelské jméno globálního správce.
- **UsernameToAssignRoleFor:** Uživatelské jméno, ke kterému se přiřadí role správce webu Marketplace.

> [!NOTE]
> Pro uživatele typu Host, kteří jsou pozváni do tenanta, může trvat až 48 hodin, než bude k dispozici jejich účet pro přiřazení role správce Marketplace. Další informace najdete v tématu [vlastnosti Azure Active Directory uživatele spolupráce B2B](/azure/active-directory/b2b/user-properties).

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

Další informace o rutinách obsažených v modulu příkazového portálu AZ. Portal PowerShell najdete v tématu [Microsoft Azure PowerShell: rutiny řídicího panelu portálu](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Vytvořit soukromé Azure Marketplace

1. Přihlaste se na web [Azure Portal](https://portal.azure.com/).
2. Vyberte **všechny služby** a potom **Marketplace**.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure Portal hlavní okno.":::

3. Z možností na levé straně vyberte **soukromé tržiště** .

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Výběr privátního tržiště v Azure Portal hlavním okně.":::

4. Vyberte **Začínáme** pro vytvoření privátního Azure Marketplace (stačí to udělat jenom jednou).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Výběr možnosti Začínáme v hlavním okně Azure Portal.":::

    Pokud pro tohoto tenanta už existuje privátní Azure Marketplace, bude ve výchozím nastavení vybraná možnost **Spravovat Marketplace** .

5. Po dokončení budete mít prázdné a zakázané soukromé Azure Marketplace.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Prázdná obrazovka privátního Azure Marketplace.":::

## <a name="add-items-from-gallery"></a>Přidat položky z Galerie

Položka je kombinací nabídky a plánu. Položku můžete vyhledat a přidat na stránce Spravovat web Marketplace.

1. Vyberte **Přidat položky**.

2. Přejděte do **Galerie** nebo vyhledejte požadovanou položku pomocí vyhledávacího pole.

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Procházení Galerie nebo použití vyhledávacího pole.":::

3. Ve výchozím nastavení se při přidávání nové nabídky přidají všechny aktuální plány do seznamu povolených. Chcete-li před přidáním vybraných položek změnit výběr plánu, vyberte rozevírací nabídku v dlaždici nabídky a aktualizujte požadované plány.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Aktualizujte požadované plány.":::

4. Vyberte **Hotovo** vlevo dole po provedení výběru.

>[!Note]
> **Přidat položky** na web Marketplace budou k dispozici pouze pro nabídky, které nejsou od Microsoftu. Nabídky společnosti Microsoft jsou ve výchozím nastavení povoleny.

## <a name="edit-item-plans"></a>Upravit plány položek

Plány položky můžete upravit na stránce Spravovat web Marketplace.

1. Ve sloupci **plány** zkontrolujte dostupné plány z rozevírací nabídky pro danou položku.
2. Zaškrtnutím nebo zrušením zaškrtnutí políček zvolte, které plány mají být uživatelům k dispozici.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Zaškrtněte nebo zrušte zaškrtnutí políčka pro požadovanou položku.":::

> [!NOTE]
> U každé nabídky je nutné vybrat alespoň jeden plán, aby došlo k aktualizaci. Chcete-li odebrat všechny plány související s nabídkou, odstraňte celou nabídku (viz další oddíl).

## <a name="delete-offers"></a>Odstranit nabídky

Na stránce Spravovat Marketplace zaškrtněte políčko vedle názvu nabídky (viz obrazovka výše) a vyberte **Odstranit položky**.

## <a name="enabledisable-private-azure-marketplace"></a>Povolit nebo zakázat privátní Azure Marketplace

Na stránce Spravovat Marketplace se zobrazí jedna z těchto proužkových proužků, která zobrazí aktuální stav privátních Azure Marketplace:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Deaktivovat banner stavu":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Povolit banner stavu":::

V případě potřeby můžete povolit nebo zakázat privátní Azure Marketplace.

- Pokud je tato možnost zakázaná, vyberte **Povolit privátní tržiště** .
- Pokud je povoleno, vyberte **Zakázat privátní tržiště** , které chcete zakázat.

## <a name="browsing-private-azure-marketplace"></a>Procházení soukromých Azure Marketplace

Když je povolený privátní Azure Marketplace, uživatelé uvidí, které plány má správce Marketplace povolený.

- Zelené **povolené** oznámení značí, že je povolená nabídka partnera (jiné než Microsoft).
- Modré **povolené** oznámení indikuje, že je povolená nabídka Microsoftu.

Uživatelé mohou filtrovat mezi nabídkami, které nejsou a nejsou povoleny:

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Možnost filtrování":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Koupit nebo nasadit v privátních Azure Marketplace

I když je prostředí stránky s podrobnostmi o produktu podobné veřejnému Azure Marketplace, existují tři privátní Azure Marketplace specifické scénáře.

- Když uživatel vybere povolený plán, aktivuje se tlačítko **vytvořit** :

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Informační zpráva nabídky, která označuje plán, se dá vytvořit.":::

- Když uživatel vybere nepovolený plán, banner se zaznamená, že plán není povolený a tlačítko **vytvořit** je zakázané.

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Banner nabídky, který označuje plán, nejde vytvořit.":::

- Pokud se výběr plánu produktu nezobrazuje na stránce s podrobnostmi o produktu, ale správce schválil jeden nebo více plánů, poznamenejte si, které plány jsou povolené a že je povolené tlačítko **vytvořit** :

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Banner s informacemi o tom, že je možné vytvořit plán a Zobrazit dostupné plány.":::

## <a name="contact-support"></a>Kontaktování podpory

Podporu Azure Marketplace najdete na webu [Microsoft Q&A](/answers/products/). 
