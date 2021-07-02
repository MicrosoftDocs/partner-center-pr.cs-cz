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
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>Vytvoření a Správa privátních Azure Marketplace v Azure Portal

Privátní Azure Marketplace umožňuje správcům řídit, která řešení třetích stran můžou uživatelé používat. Tím umožníte uživateli nasadit jenom nabídky, které schválil správce a splní zásady vaší organizace. Pomocí privátních Azure Marketplace můžou uživatelé v online obchodu vyhledat odpovídající nabídky k nákupu a nasazení.

Jako správce Marketplace (přiřazená role) začnete s neaktivním a prázdným soukromým úložištěm, kde můžete přidat vaše schválené nabídky a plány. Tento článek vysvětluje, jak přiřadit potřebnou roli, vytvořit privátní úložiště, spravovat položky, schvalovat požadavky uživatelů a povolit pro uživatele soukromé Azure Marketplace.

> [!NOTE]
> - Soukromé Azure Marketplace jsou na úrovni tenanta, takže všichni uživatelé v tenantovi uvidí stejný seznam.
> - Všechna řešení společnosti Microsoft (včetně schválených [distribucí systému Linux](/azure/virtual-machines/linux/endorsed-distros)) jsou automaticky přidána do privátního Azure Marketplace.

## <a name="assign-the-marketplace-admin-role"></a>Přiřazení role správce Marketplace

Globální správce tenanta musí přiřadit roli **správce Marketplace** správci privátního Azure Marketplace, který bude spravovat soukromé úložiště.

>[!IMPORTANT]
> Přístup ke správě privátních Azure Marketplace je k dispozici jenom správcům IT, kteří mají přiřazenou roli správce Marketplace.

### <a name="prerequisites"></a>Požadavky

Tyto požadavky jsou nutné, aby bylo možné přiřadit roli správce webu Marketplace uživateli v oboru tenanta:

- Máte přístup k uživateli **globálního správce** .
- Tenant má minimálně jedno předplatné (může to být libovolný typ).
- Pro globálního správce se uživateli přiřadí role **Přispěvatel** nebo vyšší pro vybrané předplatné.

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>Přiřazení role správce Marketplace k řízení přístupu (IAM)

1. Přihlaste se na [Azure Portal](https://portal.azure.com/).

1. Vyberte **všechny služby** a potom **Marketplace**.

1. V nabídce na levé straně vyberte **soukromé tržiště** .

   :::image type="content" source="media/private-azure/private-marketplace.png" lightbox="media/private-azure/private-marketplace-zoom.png" alt-text="Zobrazuje možnost nabídky privátní Marketplace na levé straně webu Marketplace.":::

1. Vyberte **řízení přístupu (IAM)** a přiřaďte roli správce webu Marketplace.

   :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Zobrazuje obrazovku řízení přístupu I M.":::

1. Vyberte **+ Přidat** > **Přidat přiřazení role**.

1. V části **role** vyberte **správce Marketplace**.

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Zobrazuje nabídku přiřazení role.":::

1. V rozevíracím seznamu vyberte požadovaného uživatele a potom vyberte **Hotovo**.

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>Přiřazení role správce Marketplace k PowerShellu

K přiřazení role správce Marketplace použijte následující skript prostředí PowerShell; vyžaduje následující parametry:

- **TenantId:** ID tenanta v oboru (role správce Marketplace se má přiřadit v oboru tenanta).
- **SubscriptionId:** Předplatné, ke kterému má globální správce přiřazenou roli **Přispěvatel** nebo má vyšší přiřazení.
- **GlobalAdminUsername:** Uživatelské jméno globálního správce.
- **UsernameToAssignRoleFor:** Uživatelské jméno, ke kterému se přiřadí role správce webu Marketplace.

> [!NOTE]
> Pro uživatele typu Host, kteří jsou pozváni do tenanta, může trvat až 48 hodin, než bude k dispozici jejich účet pro přiřazení role správce Marketplace. další informace najdete v tématu [vlastnosti Azure Active Directory uživatele spolupráce B2B](/azure/active-directory/b2b/user-properties).

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

další informace o rutinách obsažených v modulu příkazového portálu Az. Portal PowerShell najdete v tématu [Microsoft Azure PowerShell: rutiny řídicího panelu portálu](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Vytvořit soukromé Azure Marketplace

1. Přihlaste se na [Azure Portal](https://portal.azure.com/).
2. Vyberte **všechny služby** a potom **Marketplace**.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Zobrazuje hlavní okno Azure Portal.":::

3. V nabídce na levé straně vyberte **soukromé tržiště** .

4. vyberte **Začínáme** pro vytvoření privátních Azure Marketplace (stačí to udělat jenom jednou).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="ukazuje, jak vybrat Začínáme v hlavním okně Azure Portal.":::

    Pokud pro tohoto tenanta už existuje privátní Azure Marketplace, bude ve výchozím nastavení vybraná možnost **Spravovat Marketplace** .

5. Po dokončení budete mít prázdné a zakázané soukromé Azure Marketplace.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Zobrazí prázdnou obrazovku Private Azure Marketplace.":::

## <a name="add-items-from-gallery"></a>Přidat položky z Galerie

Položka je kombinací nabídky a plánu. Na stránce Spravovat web Marketplace můžete hledat a přidávat položky.

1. Vyberte **Přidat položky**.

2. Přejděte do **Galerie** nebo vyhledejte požadovanou položku pomocí vyhledávacího pole.

   :::image type="content" source="media/private-azure/marketplace-gallery.png" lightbox="media/private-azure/marketplace-gallery-zoom.png" alt-text="Ukazuje, jak procházet galerii nebo použít vyhledávací pole.":::

3. Ve výchozím nastavení se při přidávání nové nabídky do seznamu schválených přidá všechny aktuální plány. Chcete-li před přidáním vybraných položek změnit výběr plánu, vyberte rozevírací nabídku v dlaždici nabídky a aktualizujte požadované plány.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Ukazuje, jak aktualizovat požadované plány.":::

4. Vyberte **Hotovo** vlevo dole po provedení výběru.

>[!Note]
> **Přidat položky** na web Marketplace budou k dispozici pouze pro nabídky, které nejsou od Microsoftu. Řešení Microsoftu (včetně schválených [distribucí systému Linux](/azure/virtual-machines/linux/endorsed-distros)) budou označena jako schválená ve výchozím nastavení a nelze je spravovat na soukromém webu Marketplace.

## <a name="edit-items-plans"></a>Upravit plány položky

Plány položky můžete upravit na stránce Spravovat web Marketplace.

1. Ve sloupci **plány** zkontrolujte dostupné plány z rozevírací nabídky pro danou položku.

2. Zaškrtnutím nebo zrušením zaškrtnutí políček zvolte, které plány mají být uživatelům k dispozici.

   :::image type="content" source="media/private-azure/edit-items.png" alt-text="Ukazuje, jak vybrat nebo zrušit zaškrtnutí políčka pro požadovanou položku.":::

   > [!NOTE]
   > Každá nabídka potřebuje aspoň jeden plán vybraný k aktualizaci. Chcete-li odebrat všechny plány související s nabídkou, odstraňte celou nabídku (viz další oddíl).

## <a name="delete-offers"></a>Odstranit nabídky

Na stránce Spravovat Marketplace zaškrtněte políčko vedle názvu nabídky (viz obrazovka výše) a vyberte **Odstranit položky**.

## <a name="enabledisable-private-azure-marketplace"></a>Povolit nebo zakázat privátní Azure Marketplace

Na stránce Spravovat Marketplace se zobrazí jedna z těchto proužkových proužků, která zobrazí aktuální stav privátních Azure Marketplace:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Zobrazuje informační zprávu &quot;zakázat stav&quot;.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Zobrazuje informační zprávu &quot;Povolit stav&quot;.":::

V případě potřeby můžete povolit nebo zakázat privátní Azure Marketplace.

- Pokud je tato možnost zakázaná, vyberte **Povolit privátní tržiště** .
- Pokud je povoleno, vyberte **Zakázat privátní tržiště** , které chcete zakázat.

## <a name="private-azure-marketplace-notification-center"></a>Soukromé Azure Marketplace centra oznámení

Centrum oznámení se skládá ze tří typů oznámení a umožňuje správci Marketplace provádět akce na základě oznámení:

- Žádosti o schválení od uživatelů pro položky, které nejsou v seznamu schválených (viz [žádost o přidání nabídek nebo plánů](#request-to-add-offers-or-plans) níže).
- Nové oznámení plánu pro nabídky, které již mají jeden nebo více plánů v seznamu schválených.
- Byla odebrána oznámení plánu pro položky, které jsou v seznamu schválených, ale byly odebrány z globálního Azure Marketplace.

Přístup k centru oznámení:

1. V nabídce na levé straně vyberte **oznámení** .

   :::image type="content" source="media/private-azure/marketplace-notifications-small.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="Zobrazí nabídku oznámení.":::

1. Pro další akce vyberte nabídku se třemi tečkami.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Zobrazí další výsledky nabídky možností.":::

1. V případě požadavků na plán se otevře formulář žádosti o **schválení, kde** můžete zkontrolovat všechny požadavky uživatelů na konkrétní nabídku.
1. Vyberte **schválit** nebo **zamítnout**.

   :::image type="content" source="media/private-azure/notifications-approve-reject-small.png" lightbox="media/private-azure/notifications-approve-reject.png" alt-text="Zobrazuje možnosti schválení a odmítnutí.":::

1. Z rozevírací nabídky vyberte plán, který chcete schválit.
1. Přidejte komentář a vyberte **Odeslat**.

## <a name="browsing-private-azure-marketplace"></a>Procházení soukromých Azure Marketplace

Když je povolený privátní Azure Marketplace, zobrazí se uživatelům, kteří plánují schválení správcem Marketplace.

- Zelená **schválená** zpráva indikuje, že partnerská nabídka (jiná než Microsoft) je schválená.
- Modré **schválené** oznámení indikuje, že nabídka Microsoft (včetně schválených [distribucí systému Linux](/azure/virtual-machines/linux/endorsed-distros)) je schválená.

Uživatelé mohou filtrovat mezi nabídkami, které jsou a nejsou schváleny:

   :::image type="content" source="media/private-azure/filter-option-small.png" lightbox="media/private-azure/filter-option.png" alt-text="Zobrazuje možnost filtrování.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Koupit nebo nasadit v privátních Azure Marketplace

I když se zobrazí stránka s podrobnostmi o produktu, která je podobná globálním Azure Marketplace, existují tři privátní Azure Marketplace specifické scénáře.

- Když uživatel vybere schválený plán, aktivuje se tlačítko **vytvořit** :

   :::image type="content" source="media/private-azure/button-create-enabled-small.png" lightbox="media/private-azure/button-create-enabled.png" alt-text="Zobrazuje hlavičku nabídky s informacemi o plánu, který se dá vytvořit.":::

- Pokud se výběr plánu produktu nezobrazuje na stránce s podrobnostmi o produktu, ale správce schválil jeden nebo více plánů, poznamenejte si, které plány se schvalují a že je povolené tlačítko **vytvořit** :

   :::image type="content" source="media/private-azure/button-create-enabled-and-plans-small.png" lightbox="media/private-azure/button-create-enabled-and-plans.png" alt-text="Zobrazuje hlavičku nabídky, která označuje, že je možné vytvořit plán a Zobrazit dostupné plány.":::

- Když uživatel vybere neschválený plán, banner se naplánuje jako Neschváleno a tlačítko **vytvořit** je zakázané. Uživatel si stále může vyžádat přidání plánu do seznamu schválených (viz další část).

## <a name="request-to-add-offers-or-plans"></a>Žádost o přidání nabídek nebo plánů

Můžete požádat o přidání veřejné nabídky nebo plánu, který není aktuálně schválen v soukromém Azure Marketplace.

1. Vyberte **požadavek, který chcete přidat** do banneru pro otevření **formuláře žádosti o přístup**.

   :::image type="content" source="media/private-azure/request-banner-small.png" lightbox="media/private-azure/request-banner.png" alt-text="Zobrazí banner s odkazem požadavek na přidání.":::

   :::image type="content" source="media/private-azure/access-request-form-small.png" lightbox="media/private-azure/access-request-form.png" alt-text="Zobrazí formulář žádosti o přístup pro nabídky nebo plány.":::

1. Vyberte plány, které chcete přidat do žádosti (**jakýkoliv plán** oznamuje správci Marketplace, že nemáte předvolbu plánu v rámci nabídky).

1. Přidejte **odůvodnění** a vyberte **žádost** o odeslání žádosti.

   :::image type="content" source="media/private-azure/access-request-form-filled-small.png" lightbox="media/private-azure/access-request-form-filled.png" alt-text="Zobrazuje formulář žádosti o přístup pro nabídky nebo plány s ukázkovými položkami.":::

1. Ve formuláři žádosti o přístup se zobrazí označení pro nevyřízenou žádost s možností **odvolání žádosti**.

   :::image type="content" source="media/private-azure/approved-pending-plans-small.png" lightbox="media/private-azure/approved-pending-plans.png" alt-text="Zobrazuje seznam schválených nebo nevyřízených plánů s odkazem na žádost o stažení.":::

> [!NOTE]
> Po odeslání se formulář žádosti o schválení pošle do [centra oznámení](#private-azure-marketplace-notification-center) pro správce Marketplace, aby zkontroloval požadavek a provedl akci.

> [!CAUTION]
> Schválení na soukromý web Marketplace neindikuje nákup řešení.

## <a name="frequently-asked-questions-faqs"></a>Nejčastější dotazy

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>Již jsem blokoval aplikaci třetí strany Marketplace prostřednictvím Azure Policy. Jak se to liší?

V současné době existují dva způsoby, jak omezit služby třetích stran na webu Marketplace:

1. Prostřednictvím portálu EA nebo Azure Portal zakažte služby třetích stran nebo omezte pouze na bezplatné nebo BYOL SKU.

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Ukazuje, jak omezit služby v Azure Portal.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Ukazuje, jak omezit služby na portálu E.":::

2. Vytvořte zásadu Azure, která povolí jenom konkrétní virtuální počítače. podrobnosti o tom, jak vynutilit zásady pro Windows virtuálních počítačů, najdete v tématu věnovaném [použití zásad pro Windows virtuálních počítačů pomocí Azure Resource Manager](/azure/virtual-machines/windows/policy).

Soukromé Azure Marketplace umožňují větší flexibilitu při omezování a povolování konkrétních nabídek a plánů. Informuje koncové uživatele o dostupnosti pro nasazení v galerii Marketplace, a to i předtím, než se pokusí nasadit služby třetích stran. Pokud chcete povolit nasazení služeb třetích stran, nastavte Azure Marketplace na zapnuto nebo povoleno na portálu EA a v Azure Portal.

- Privátní Azure Marketplace můžou využívat Partnerská řešení, která nejsou omezená na virtuální počítače.
- Privátní Azure Marketplace můžou obsloužit na úrovni plánu a můžou také nastavit "aktuální a budoucí plán".
- Privátní Azure Marketplace můžou koncovým uživatelům informovat o tom, co můžou a nemůžou být nasazené.

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>Jaký je rozdíl mezi soukromou nabídkou a soukromým Azure Marketplace?

**Soukromá nabídka** umožňuje vydavatelům vytvářet plány, které jsou viditelné pouze cílovým zákazníkům. To jim umožní soukromě sdílet přizpůsobená řešení s vyjednávacími cenami, soukromými podmínkami a podmínkami a specializovanými konfiguracemi. Podrobnosti najdete v tématu [soukromé nabídky na komerčním webu Marketplace](/azure/marketplace/private-offers).

**Soukromý Azure Marketplace** v Azure Portal umožňuje správcům předem schvalovat, která řešení třetích stran můžou uživatelé nasazovat. Pomocí privátního Azure Marketplace můžou uživatelé využít výhod Azure Marketplace tak, že si vyhledají, kupují a nasazují vyhovující nabídky. Aby bylo možné spravovat soukromé nabídky na základě předplatného na soukromém webu Marketplace, musí mít správce webu Marketplace minimálně roli "číst" na daném předplatném.

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>K privátním Azure Marketplace jsem přidal soukromou nabídku, proč se na kartě Spravovat Marketplace nezobrazuje?

Soukromé nabídky na základě předplatného jsou viditelné jenom pro uvedená předplatná v nastavení soukromé nabídky. Pokud chcete zobrazit soukromou nabídku, ujistěte se, že globální filtr předplatného zobrazuje všechna předplatná.

   :::image type="content" source="media/private-azure/private-marketplace-filter.png" lightbox="media/private-azure/private-marketplace-filter.png" alt-text="Zobrazuje soukromý filtr Marketplace.":::

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>Můžeme do privátních Azure Marketplace zahrnout vlastní image?

No. Privátní Azure Marketplace umožňuje všem správcům IT spravovat řešení třetích stran z globálních Azure Marketplace. Vzhledem k tomu, že vlastní image nejsou na globálním Azure Marketplace, nemůže správce IT vybírat a vybírat vlastní image. Chcete-li sdílet vlastní image, použijte [galerii sdílených imagí](/azure/virtual-machines/shared-image-galleries).

1. Podrobný průvodce vytvořením Galerie sdílených imagí (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).
2. Vytvoří definici obrázku v rámci SIG. Zákazník by měl zvolit **zobecněný** pro pole stav operačního systému. (Rozhraní příkazového[řádku](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShellu](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).
3. Přeneste spravovanou bitovou kopii do galerie sdílených imagí ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).
4. Image virtuálního počítače SIG by se měly nacházet v jednom předplatném. Pokud ho chcete zpřístupnit ostatním předplatným, použijte registraci aplikace (rozhraní příkazového[řádku](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShellu](/azure/virtual-machines/windows/share-images-across-tenants)).

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>Proč se mi zobrazují některé nabídky **schválené ve výchozím nastavení,** i když Vydavatel není Microsoft?

Microsoft podporuje v Azure technologii Linux a open source. [Schválené distribuce systému Linux](/azure/virtual-machines/linux/endorsed-distros) jsou podporovány v Azure a cena je integrována do virtuálních počítačů. Vzhledem k tomu, že je agent Azure Linux už v Azure Marketplace předinstalovaný, považuje se za nabídku Microsoftu. Vzhledem k tomu, že jsou nabídky společnosti Microsoft schváleny ve výchozím nastavení, nelze spravovat schválené distribuce systému Linux v privátních Azure Marketplace a jsou schváleny ve výchozím nastavení.

## <a name="contact-support"></a>Kontaktování podpory

- Podporu Azure Marketplace najdete na webu [Microsoft Q&A](/answers/products/).