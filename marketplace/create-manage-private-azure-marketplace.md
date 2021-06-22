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
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>Vytvoření a správa privátních Azure Marketplace v Azure Portal

Privátní Azure Marketplace umožňuje správcům řídit, která řešení třetích stran můžou uživatelé používat. Umožňuje uživateli nasadit pouze nabídky, které jsou schválené správcem a jsou v souladu se zásadami vašeho podniku. Díky privátním Azure Marketplace mohou uživatelé hledat v online obchodě vyhovující nabídky, které si kupovat a nasazovat.

Jako správce Marketplace (přiřazená role) začnete se zakázaným a prázdným privátním úložištěm, ve kterém můžete přidat schválené nabídky a plány. Tento článek vysvětluje, jak přiřadit potřebnou roli, vytvořit privátní úložiště, spravovat položky, schvalovat žádosti uživatelů a povolit privátní Azure Marketplace pro vaše uživatele.

> [!NOTE]
> - Privátní Azure Marketplace je na úrovni tenanta, takže všichni uživatelé v tenantovi uvidí stejný kurátorovaný seznam.
> - Všechna řešení Microsoftu (včetně [schvalovaných linuxových](/azure/virtual-machines/linux/endorsed-distros)distribucí) se automaticky přidávají do privátních Azure Marketplace.

## <a name="assign-the-marketplace-admin-role"></a>Přiřazení role správce Marketplace

Správce tenanta Globální správce roli správce **Marketplace** správci privátního úložiště Azure Marketplace který bude privátní úložiště spravovat.

>[!IMPORTANT]
> Přístup ke správě privátních Azure Marketplace je dostupný jenom správcům IT s přiřazenou rolí správce Marketplace.

### <a name="prerequisites"></a>Požadavky

Před přiřazením role správce Marketplace uživateli v oboru tenanta se vyžaduje splnění těchto požadavků:

- Máte přístup k **Globální správce** uživateli.
- Tenant má alespoň jedno předplatné (může být libovolného typu).
- Uživatel Globální správce vybranému **předplatnému** přiřazenou roli Přispěvatel nebo vyšší.

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>Přiřazení role správce Marketplace pomocí řízení přístupu (IAM)

1. Přihlaste se k webu [Azure Portal](https://portal.azure.com/).
1. Vyberte **Všechny služby a** pak **Marketplace.**
1. V **nabídce na** levé straně vyberte Privátní Marketplace.

    [![Zobrazuje možnost nabídky privátního marketplace na levé straně Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)

1. Vyberte **Řízení přístupu (IAM)** a přiřaďte roli správce Marketplace.

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Zobrazuje obrazovku řízení přístupu K A M.":::

1. Vyberte **+ Přidat** > **Přidat přiřazení role**.
1. V **části Role** zvolte Správce **Marketplace.**

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Zobrazí nabídku Přiřazení role.":::

1. V rozevíracím seznamu vyberte požadovaného uživatele a pak vyberte **Hotovo.**

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>Přiřazení role správce Marketplace pomocí PowerShellu

Pomocí následujícího skriptu PowerShellu přiřaďte roli správce Marketplace. Vyžaduje následující parametry:

- **Id tenanta:** ID tenanta v oboru (roli správce Marketplace je možné přiřadit v oboru tenanta).
- **Id předplatného:** Předplatné, ke kterému má globální správce **přiřazenou** roli Přispěvatel nebo vyšší.
- **GlobalAdminUsername:** Uživatelské jméno globálního správce.
- **UsernameToAssignRoleFor:** Uživatelské jméno, ke kterému bude přiřazena role správce Marketplace.

> [!NOTE]
> Pro uživatele hosta pozvané do tenanta může trvat až 48 hodin, než bude jejich účet k dispozici pro přiřazení role správce Marketplace. Další informace najdete v tématu [Vlastnosti uživatele Azure Active Directory B2B.](/azure/active-directory/b2b/user-properties)

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

Další informace o rutinách obsažených v modulu Az.Portal PowerShellu najdete v [Microsoft Azure PowerShell: Rutiny řídicího panelu portálu](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Vytvoření privátního Azure Marketplace

1. Přihlaste se k webu [Azure Portal](https://portal.azure.com/).
2. Vyberte **Všechny služby a** pak **Marketplace.**

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Zobrazí hlavní Azure Portal okno.":::

3. V **nabídce na** levé straně vyberte Privátní Marketplace.

4. Vyberte **Začínáme a** vytvořte privátní Azure Marketplace (to musíte udělat jenom jednou).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Ukazuje, jak vybrat hlavní okno Začínáme Azure Portal okně.":::

    Pokud privátní Azure Marketplace pro tohoto tenanta již existuje, bude ve výchozím nastavení vybraná možnost Spravovat **Marketplace.**

5. Po dokončení budete mít prázdný a zakázaný privátní Azure Marketplace.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Zobrazí prázdnou obrazovku privátního Azure Marketplace obrazovky.":::

## <a name="add-items-from-gallery"></a>Přidání položek z galerie

Položka je kombinací nabídky a plánu. Položky můžete vyhledat a přidat na stránce Spravovat Marketplace.

1. Vyberte **Přidat položky.**

2. Přejděte do **Galerie** nebo pomocí vyhledávacího pole najděte položku, kterou chcete.

    [![Ukazuje, jak procházet galerii nebo použít vyhledávací pole.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)

3. Ve výchozím nastavení se při přidávání nové nabídky všechny aktuální plány přidávají do seznamu schválených plánů. Pokud chcete před přidáním vybraných položek upravit výběr plánu, vyberte rozevírací nabídku na dlaždici nabídky a aktualizujte požadované plány.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Ukazuje, jak aktualizovat požadované plány.":::

4. Po **provedení** výběru vyberte v levém dolním rohu Hotovo.

>[!Note]
> **Možnost Přidat** položky na Marketplace bude dostupná jenom pro nabídky od jiných společností než Microsoft. Řešení Microsoftu (včetně [schválených linuxových](/azure/virtual-machines/linux/endorsed-distros)distribucí) budou ve výchozím nastavení označená jako Schválená a nelze je spravovat na privátním marketplace.

## <a name="edit-items-plans"></a>Úprava plánů položek

Plány položky můžete upravit na stránce Spravovat Marketplace.

1. Ve **sloupci** Plány zkontrolujte dostupné plány z rozevírací nabídky pro tuto položku.
2. Zaškrtnutím nebo zrušte zaškrtnutí políček, abyste zvolili, které plány budou uživatelům k dispozici.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Ukazuje, jak vybrat nebo vymazat zaškrtávací políčko pro požadovanou položku.":::

> [!NOTE]
> Každá nabídka musí mít vybraný alespoň jeden plán, aby k aktualizaci došlo. Pokud chcete odebrat všechny plány související s nabídkou, odstraňte celou nabídku (viz další část).

## <a name="delete-offers"></a>Odstranění nabídek

Na stránce Spravovat Marketplace zaškrtněte políčko vedle názvu nabídky (viz obrazovka výše) a vyberte **Odstranit položky**.

## <a name="enabledisable-private-azure-marketplace"></a>Povolení nebo zakázání privátních Azure Marketplace

Na stránce Spravovat Marketplace se zobrazí jeden z těchto bannerů, které zobrazují aktuální stav privátních Azure Marketplace:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Zobrazí banner Disable state (Zakázat stav).":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Zobrazí banner Enable state (Povolit stav).":::

Podle potřeby můžete privátní Azure Marketplace zakázat.

- Pokud je zakázané, **povolte povolení výběrem možnosti** Povolit privátní marketplace.
- Pokud je tato možnost povolená, **zakažte** ji výběrem možnosti Zakázat privátní marketplace.

## <a name="private-azure-marketplace-notification-center"></a>Centrum Azure Marketplace oznámení služby Private Azure Marketplace

Centrum oznámení se skládá ze tří typů oznámení a umožňuje správci Marketplace provádět akce na základě oznámení:

- Žádosti uživatelů o schválení položek, které nejsou v seznamu schválených položek (viz žádost o [přidání nabídek nebo plánů](#request-to-add-offers-or-plans) níže).
- Oznámení o novém plánu pro nabídky, které už mají jeden nebo více plánů v seznamu schválených
- Odebrání oznámení plánu pro položky, které jsou v seznamu schválených položek, které byly odebrány z globálního Azure Marketplace.

Přístup k centru oznámení:

1. V **nabídce vlevo** vyberte Oznámení.

    [![Zobrazí nabídku Oznámení.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)

1. Výběrem nabídky se třemi tečkami zobrazíte další akce.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Zobrazí výsledky nabídky Další možnosti.":::

1. V případě žádostí o plán **otevře možnost** Zobrazit žádosti formulář žádosti o schválení, kde můžete zkontrolovat všechny žádosti uživatelů o konkrétní nabídku.
1. Vyberte **Schválit** nebo **Odmítnout.**

    [![Zobrazí možnosti schválit a odmítnout.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)

1. V rozevírací nabídce vyberte plán ke schválení.
1. Přidejte komentář a vyberte **Odeslat.**

## <a name="browsing-private-azure-marketplace"></a>Procházení privátních Azure Marketplace

Když je Azure Marketplace privátní účet povolený, uživatelé uvidí, které plány správce Marketplace schválil.

- Zelené schválené **oznámení** značí schválenou nabídku partnera (jiné společnosti než Microsoft).
- Modré schválené **oznámení** označuje nabídku Microsoftu (včetně [schválených linuxových](/azure/virtual-machines/linux/endorsed-distros)distribucí), která je schválená.

Uživatelé mohou filtrovat mezi nabídkami, které jsou a nejsou schválené:

[![Zobrazí možnost filtrování.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Nákup nebo nasazení v privátním Azure Marketplace

Stránka s podrobnostmi o produktu se podobá globálnímu prostředí Azure Marketplace, ale existují tři scénáře, které Azure Marketplace privátním prostředím.

- Když uživatel vybere schválený plán, **tlačítko** Vytvořit se povolí:

    [![Zobrazuje banner nabídky s nápisem, že je možné vytvořit plán.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)

- Pokud se výběr plánu produktu nezobrazí na stránce s podrobnostmi o produktu, ale správce  schválil jeden nebo více plánů, zobrazí se banner s upozorněním, které plány jsou schválené a tlačítko Vytvořit je povolené:

    [![Zobrazuje banner nabídky s nápisem, že plán je možné vytvořit a zobrazit dostupné plány.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)

- Když uživatel vybere neschválený plán, zobrazí se banner s upozorněním, že se plán neschválí, a tlačítko Vytvořit **se** deaktivuje. Uživatel může požádat o přidání plánu do seznamu schválených položek (viz další část).

## <a name="request-to-add-offers-or-plans"></a>Žádost o přidání nabídek nebo plánů

Můžete požádat o přidání veřejné nabídky nebo plánu, které nejsou aktuálně schválené v privátním Azure Marketplace.

1. Výběrem **možnosti Request to add** (Žádost o přidání) v banneru otevřete formulář žádosti o **přístup.**

    [![Zobrazí banner s odkazem Požádat o přidání.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)

    [![Zobrazí formulář žádosti o přístup pro nabídky nebo plány.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)

1. Vyberte plány, které chcete k žádosti přidat **(Jakýkoli** plán informuje správce Marketplace, že pro plán v rámci nabídky nemáte nějaké preference).

1. Přidejte **justification (Odůvodnění)** a **vyberte Request** to submit your request (Žádost o odeslání žádosti).
  
    [![Zobrazí formulář žádosti o přístup pro nabídky nebo plány s ukázkovými položkami.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)

1. Ve formuláři žádosti o přístup se zobrazí indikace čekající žádosti s možností Žádosti **o žádost o přístup**.

    [![Zobrazí seznam schválených nebo nevyřízených plánů s odkazem Na žádost o schválení.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)

> [!NOTE]
> Po odeslání se formulář žádosti o [](#private-azure-marketplace-notification-center) schválení zasílá správci Marketplace do Centra oznámení, aby žádost zkontrolovat a provést akci.

> [!CAUTION]
> Schválení na privátním marketplace neznačí nákup řešení.

## <a name="frequently-asked-questions-faqs"></a>Nejčastější dotazy

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>Aplikaci třetí strany z Marketplace už blokujem prostřednictvím Azure Policy. Jak se to liší?

V současné době existují dva způsoby, jak na Marketplace omezit služby třetích stran:

1. Prostřednictvím portálu EA portal nebo Azure Portal zakažte služby třetích stran nebo omezte na "Pouze skladové sklady Free nebo BYOL".

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Ukazuje, jak omezit služby v Azure Portal.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Ukazuje, jak omezit služby na portálu E A.":::

2. Vytvořte zásadu Azure, která povolí jenom konkrétní virtuální počítače. Podrobnosti o tom, jak vynutit zásady pro virtuální počítače s Windows, najdete v tématu Použití zásad na virtuální počítače s [Windows pomocí Azure Resource Manager](/azure/virtual-machines/windows/policy).

Privátní Azure Marketplace nabízí větší flexibilitu při omezování a povolování konkrétních nabídek a plánů. Informuje koncové uživatele o dostupnosti nasazení v galerii Marketplace ještě předtím, než se pokusí nasadit služby třetích stran. Pokud chcete povolit nasazení služeb třetích stran, nastavte Azure Marketplace na Zapnuto/povoleno v EA Portal a Azure Portal.

- Privátní Azure Marketplace může partnerská řešení nastavit nejen na virtuální počítače.
- Privátní Azure Marketplace může být na úrovni plánu a může také nastavit aktuální a budoucí plán.
- Privátní Azure Marketplace může předem informovat koncové uživatele o tom, co může a nemůže být nasazeno.

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>Jaký je rozdíl mezi privátní nabídkou a privátní nabídkou Azure Marketplace?

Privátní **nabídka umožňuje vydavatelům** vytvářet plány, které jsou viditelné pouze cílovým zákazníkům. Díky tomu mohou soukromě sdílet přizpůsobená řešení s vyjednanou cenou, privátními podmínkami a zvláštními konfiguracemi. Podrobnosti najdete v tématu [Privátní nabídky na komerčním marketplace.](/azure/marketplace/private-offers)

**Privátní Azure Marketplace** v Azure Portal umožňuje správcům předem schválit, která řešení třetích stran můžou jejich uživatelé nasadit. Díky privátní Azure Marketplace mohou uživatelé využívat výhody těchto Azure Marketplace hledáním, nákupem a nasazením vyhovujících nabídek. Pokud chcete spravovat privátní nabídky založené na předplatném na privátním marketplace, musí mít správce Marketplace minimální roli čtení pro konkrétní předplatné.

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>Proč se privátní nabídka po přidání Azure Marketplace nezobrazuje na kartě Spravovat marketplace?

Privátní nabídky založené na předplatném jsou viditelné jenom pro uvedená předplatná v nastavení privátní nabídky. Pokud chcete zobrazit privátní nabídku, ujistěte se, že globální filtr předplatných zobrazuje všechna předplatná.

[![Zobrazí filtr privátního marketplace.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>Můžeme do privátních imagí zahrnout Azure Marketplace?

No. Privátní Azure Marketplace umožňuje libovolnému správci IT spravovat a spravovat řešení třetích stran z globálních Azure Marketplace. Vzhledem k tomu, že vlastní image nejsou v globální Azure Marketplace, správce IT nemůže vybrat a vybrat vlastní image. Pokud chcete sdílet vlastní image, použijte [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).

1. Podrobný průvodce Vytvořením Shared Image Gallery (SIG)[(CLI,](/azure/virtual-machines/shared-images-cli) [PowerShell).](/azure/virtual-machines/shared-images-powershell)
2. Vytvořte definici image v rámci SKUPINY SIG. Zákazník by měl **jako pole** Stav operačního systému zvolit Generalized (Generalizované). ([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).
3. Přenést spravovanou image do Shared Image Gallery ([ROZHRANÍ příkazového řádku](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).
4. Image virtuálních počítače SIG se nacházejí v jednom předplatném. K jeho zvidilení pro ostatní předplatná použijte registraci aplikace ([CLI,](/azure/virtual-machines/linux/share-images-across-tenants) [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>Proč se některé nabídky ve výchozím nastavení **schvalují,** i když vydavatel není Microsoft?

Microsoft podporuje linuxovou a open source technologii v Azure. [Schválené linuxové distribuce jsou](/azure/virtual-machines/linux/endorsed-distros) podporované v Azure a cena je integrovaná ve virtuálních počítačích. Vzhledem k tomu, že agent Azure Linux je už na zařízeních Azure Marketplace, je považován za nabídku Microsoftu. Vzhledem k tomu, že nabídky Microsoftu jsou standardně schválené, schválené linuxové distribuce se nespravují v privátních Azure Marketplace a ve výchozím nastavení se schvalují.

## <a name="contact-support"></a>Kontaktování podpory

- Další Azure Marketplace najdete na webu [Microsoft Q&A.](/answers/products/)