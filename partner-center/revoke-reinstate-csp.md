---
title: Obnovení oprávnění správce pro Azure CSP
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak zákazníkům pomoct obnovit oprávnění správce partnera, aby partner mohl pomoci spravovat předplatná csP (Azure Cloud Solution Provider zákazníka).
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 5d784aef33cce2a722583a77e73c35d5fc8136b1
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551584"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="bdf13-103">Obnovení oprávnění správce pro předplatná Azure CSP zákazníka</span><span class="sxs-lookup"><span data-stu-id="bdf13-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="bdf13-104">**Odpovídající role:** Globální správce | Agent pro správu</span><span class="sxs-lookup"><span data-stu-id="bdf13-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="bdf13-105">Jako partner Cloud Solution Provider (CSP) vaši zákazníci často očekávají, že za ně budete spravovat jejich využití Azure a jejich systémy.</span><span class="sxs-lookup"><span data-stu-id="bdf13-105">As a Cloud Solution Provider (CSP) partner, your customers often expect that you'll manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="bdf13-106">K tomu musíte mít oprávnění správce.</span><span class="sxs-lookup"><span data-stu-id="bdf13-106">You must have admin privileges to do so.</span></span> <span data-ttu-id="bdf13-107">Některá oprávnění jsou udělena, když se nastane vztah prodejce se zákazníkem.</span><span class="sxs-lookup"><span data-stu-id="bdf13-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="bdf13-108">Jiné vám udělí váš zákazník.</span><span class="sxs-lookup"><span data-stu-id="bdf13-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="bdf13-109">Oprávnění správce pro Azure v CSP</span><span class="sxs-lookup"><span data-stu-id="bdf13-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="bdf13-110">Existují dvě úrovně oprávnění správce pro Azure v CSP.</span><span class="sxs-lookup"><span data-stu-id="bdf13-110">There are two levels of admin privileges for Azure in CSP.</span></span>

- <span data-ttu-id="bdf13-111">**Oprávnění správce na úrovni tenanta (delegovaná** oprávnění správce): Partneři CSP těmto oprávněním při navazování vztahu prodejce CSP se zákazníky.</span><span class="sxs-lookup"><span data-stu-id="bdf13-111">**Tenant level admin privileges (Delegated admin privileges)**:  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="bdf13-112">Delegovaná oprávnění správce poskytují partnerům CSP přístup k tenantům jejich zákazníků.</span><span class="sxs-lookup"><span data-stu-id="bdf13-112">Delegated admin privileges give CSP partners access to their customers' tenants.</span></span> <span data-ttu-id="bdf13-113">Tento přístup jim umožňuje používat funkce správy, jako je přidávání a správa uživatelů, resetování hesel a správa uživatelských licencí.</span><span class="sxs-lookup"><span data-stu-id="bdf13-113">This access allows them to do administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>
- <span data-ttu-id="bdf13-114">**Oprávnění správce na úrovni předplatného:** Partneři CSP těmto oprávněním při vytváření Azure CSP předplatných pro své zákazníky.</span><span class="sxs-lookup"><span data-stu-id="bdf13-114">**Subscription level admin privileges**: CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="bdf13-115">Díky těmto oprávněním mají partneři CSP úplný přístup k těmto předplatným, což jim umožňuje zřizování a správu prostředků Azure.</span><span class="sxs-lookup"><span data-stu-id="bdf13-115">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-a-partners-admin-privileges"></a><span data-ttu-id="bdf13-116">Obnovení oprávnění správce partnera csp</span><span class="sxs-lookup"><span data-stu-id="bdf13-116">Reinstate CSP a partner's admin privileges</span></span>

<span data-ttu-id="bdf13-117">Pokud zákazníkovi poskytnete skupinu AdminAgents, zákazník může přiřazení role CSP `object ID` vytvořit znovu.</span><span class="sxs-lookup"><span data-stu-id="bdf13-117">Your customer can re-create the CSP role assignment if you provide the `object ID` of the AdminAgents group to your customer.</span></span> <span data-ttu-id="bdf13-118">Pokud chcete znovu získat delegovaná oprávnění správce, musíte spolupracovat se zákazníkem pomocí následujících kroků.</span><span class="sxs-lookup"><span data-stu-id="bdf13-118">To regain delegated admin privileges, you need to work with your customer through the following steps.</span></span>

1. <span data-ttu-id="bdf13-119">Přihlaste se k řídicímu Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="bdf13-119">Sign into the Partner Center dashboard.</span></span>

2. <span data-ttu-id="bdf13-120">V nabídce Partnerské centrum vyberte **Zákazníci.**</span><span class="sxs-lookup"><span data-stu-id="bdf13-120">On the Partner Center menu, select **Customers**.</span></span>

3. <span data-ttu-id="bdf13-121">Vyberte zákazníka, se nímž **pracujete, a požádejte o vztah prodejce.**</span><span class="sxs-lookup"><span data-stu-id="bdf13-121">Select the customer you are working with and **request a reseller relationship**.</span></span> <span data-ttu-id="bdf13-122">Tato akce vygeneruje odkaz na zákazníka, který má oprávnění správce tenanta.</span><span class="sxs-lookup"><span data-stu-id="bdf13-122">This action generates a link to the customer who has tenant admin rights.</span></span>

4. <span data-ttu-id="bdf13-123">Zákazník musí odkaz vybrat a schválit žádost o vztah prodejce.</span><span class="sxs-lookup"><span data-stu-id="bdf13-123">Your customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Příklad e-mailu s vytvořením vztahu prodejce":::

5. <span data-ttu-id="bdf13-125">Vy, partner, se musíte připojit k partnerskému tenantovi, abyste měli ID objektu skupiny AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="bdf13-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. <span data-ttu-id="bdf13-126">Zákazník pak musí provést následující kroky pomocí PowerShellu nebo Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="bdf13-126">Your customer must then do the following steps using either PowerShell or Azure CLI.</span></span> <span data-ttu-id="bdf13-127">Váš zákazník musí mít:</span><span class="sxs-lookup"><span data-stu-id="bdf13-127">Your customer must have:</span></span>

- <span data-ttu-id="bdf13-128">Role **vlastníka nebo** **správce uživatelských přístupů**</span><span class="sxs-lookup"><span data-stu-id="bdf13-128">The role of **owner** or **user access administrator**</span></span> 
- <span data-ttu-id="bdf13-129">Oprávnění k vytváření přiřazení rolí na úrovni předplatného</span><span class="sxs-lookup"><span data-stu-id="bdf13-129">Permissions to create role assignments at the subscription level</span></span>

   <span data-ttu-id="bdf13-130">a.</span><span class="sxs-lookup"><span data-stu-id="bdf13-130">a.</span></span> <span data-ttu-id="bdf13-131">Pouze pro PowerShell musí zákazník aktualizovat `Az.Resources` modul.</span><span class="sxs-lookup"><span data-stu-id="bdf13-131">For PowerShell only, the customer must update the `Az.Resources` module.</span></span>
   ```powershell
   Update-Module Az.Resources
   ```

   <span data-ttu-id="bdf13-132">b.</span><span class="sxs-lookup"><span data-stu-id="bdf13-132">b.</span></span> <span data-ttu-id="bdf13-133">Zákazník se připojí k tenantovi, ve kterém je předplatné CSP.</span><span class="sxs-lookup"><span data-stu-id="bdf13-133">The customer connects to the tenant where the CSP subscription exists.</span></span>
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   <span data-ttu-id="bdf13-134">c.</span><span class="sxs-lookup"><span data-stu-id="bdf13-134">c.</span></span> <span data-ttu-id="bdf13-135">Zákazník se připojí k předplatnému.</span><span class="sxs-lookup"><span data-stu-id="bdf13-135">The customer connects to the subscription.</span></span> <span data-ttu-id="bdf13-136">To platí *jenom v* případě, že má uživatel oprávnění k přiřazení role pro více předplatných v tenantovi.</span><span class="sxs-lookup"><span data-stu-id="bdf13-136">This is *only* applicable if the user has role assignment permissions over multiple subscriptions in the tenant.</span></span>

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   <span data-ttu-id="bdf13-137">d.</span><span class="sxs-lookup"><span data-stu-id="bdf13-137">d.</span></span> <span data-ttu-id="bdf13-138">Zákazník pak vytvoří přiřazení role.</span><span class="sxs-lookup"><span data-stu-id="bdf13-138">The customer then creates the role assignment.</span></span>
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

<span data-ttu-id="bdf13-139">Místo udělení oprávnění vlastníka v oboru předplatného můžete oprávnění udělit na úrovni skupiny prostředků nebo prostředku.</span><span class="sxs-lookup"><span data-stu-id="bdf13-139">Instead of granting owner permissions at the subscription scope, you can grant at the resource group or resource level.</span></span> 

- <span data-ttu-id="bdf13-140">Na úrovni skupiny prostředků</span><span class="sxs-lookup"><span data-stu-id="bdf13-140">At the resource group level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- <span data-ttu-id="bdf13-141">Na úrovni prostředku</span><span class="sxs-lookup"><span data-stu-id="bdf13-141">At the resource level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

<span data-ttu-id="bdf13-142">Pokud výše uvedený postup nefunguje nebo když se o ně pokusíte, zkuste obnovit práva správce zákazníka pomocí následujícího postupu "catch-all".</span><span class="sxs-lookup"><span data-stu-id="bdf13-142">If the above steps don't work or you get errors when attempting them, try the following "catch-all" procedure to reinstate admin rights for your customer.</span></span>

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a><span data-ttu-id="bdf13-143">Řešení potíží</span><span class="sxs-lookup"><span data-stu-id="bdf13-143">Troubleshooting</span></span>

<span data-ttu-id="bdf13-144">Pokud se zákazníkovi nedaří dokončit krok 6 výše, zkuste použít následující příkaz:</span><span class="sxs-lookup"><span data-stu-id="bdf13-144">If the customer is unable to complete step 6 above, have the customer try the following command:</span></span>

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

<span data-ttu-id="bdf13-145">Poskytněte `newRoleAssignment.log` microsoftu výsledný soubor k další analýze.</span><span class="sxs-lookup"><span data-stu-id="bdf13-145">Provide the resulting `newRoleAssignment.log` file to Microsoft for further analysis.</span></span>

<span data-ttu-id="bdf13-146">Pokud se během operace nezdaří procedura "catch-all", `Import-Module` zkuste následující kroky:</span><span class="sxs-lookup"><span data-stu-id="bdf13-146">If the "catch-all" procedure fails during the `Import-Module`, try the following steps:</span></span>
- <span data-ttu-id="bdf13-147">Pokud import selže, protože se modul používá, restartujte relaci PowerShellu tak, že zavřete a znovu otevřete všechna okna.</span><span class="sxs-lookup"><span data-stu-id="bdf13-147">If the import fails because the module is in use, restart the PowerShell session by closing and reopening all windows.</span></span>
- <span data-ttu-id="bdf13-148">Zkontrolujte verzi nástroje `Az.Resources` pomocí `Get-Module Az.Resources -ListAvailable` .</span><span class="sxs-lookup"><span data-stu-id="bdf13-148">Check version of `Az.Resources` with `Get-Module Az.Resources -ListAvailable`.</span></span>
- <span data-ttu-id="bdf13-149">Pokud verze 4.1.1 není v seznamu dostupných verzí, musíte použít `Update-Module Az.Resources -Force` .</span><span class="sxs-lookup"><span data-stu-id="bdf13-149">If version 4.1.1 is not within the available list, you must use `Update-Module Az.Resources -Force`.</span></span>
- <span data-ttu-id="bdf13-150">Pokud chyba uvádí, že musí být konkrétní verze, aktualizujte také tento `Az.Accounts` modul a nahraďte `Az.Resources` za `Az.Accounts` .</span><span class="sxs-lookup"><span data-stu-id="bdf13-150">If the error states that `Az.Accounts` needs to be a specific version, update that module as well, replacing `Az.Resources` with `Az.Accounts`.</span></span> <span data-ttu-id="bdf13-151">Pak musíte restartovat relaci PowerShellu.</span><span class="sxs-lookup"><span data-stu-id="bdf13-151">You must then restart the PowerShell session.</span></span>


## <a name="next-steps"></a><span data-ttu-id="bdf13-152">Další kroky</span><span class="sxs-lookup"><span data-stu-id="bdf13-152">Next steps</span></span>

- [<span data-ttu-id="bdf13-153">Správa předplatných a prostředků v rámci plánu Azure</span><span class="sxs-lookup"><span data-stu-id="bdf13-153">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
