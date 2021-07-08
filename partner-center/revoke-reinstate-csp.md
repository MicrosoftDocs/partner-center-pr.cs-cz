---
title: Obnovit oprávnění správce pro zprostředkovatele CSP Azure
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: naučte se, jak zákazníkům pomáhat obnovit oprávnění správce partnera, aby partner mohl spravovat předplatná Azure Cloud Solution Provider (CSP).
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 196b38d30942278beb00096529f5965db7dfb96c
ms.sourcegitcommit: b55f63a029d88c73cd5190bbac2df1b5990e6e44
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/08/2021
ms.locfileid: "113510172"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="b16e6-103">Obnovit oprávnění správce pro předplatná Azure CSP zákazníka</span><span class="sxs-lookup"><span data-stu-id="b16e6-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="b16e6-104">**Příslušné role**: globální správce | Agent správce</span><span class="sxs-lookup"><span data-stu-id="b16e6-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="b16e6-105">jako partner Cloud Solution Provider (CSP) vaši zákazníci často očekávají, že budete spravovat jejich využití Azure a jejich systémy.</span><span class="sxs-lookup"><span data-stu-id="b16e6-105">As a Cloud Solution Provider (CSP) partner, your customers often expect that you'll manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="b16e6-106">K tomu musíte mít oprávnění správce.</span><span class="sxs-lookup"><span data-stu-id="b16e6-106">You must have admin privileges to do so.</span></span> <span data-ttu-id="b16e6-107">Některá oprávnění se udělují v případě, že je vytvořen vztah prodejce se zákazníkem.</span><span class="sxs-lookup"><span data-stu-id="b16e6-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="b16e6-108">Další vám je uděleno vaším zákazníkem.</span><span class="sxs-lookup"><span data-stu-id="b16e6-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="b16e6-109">Oprávnění správce pro Azure v CSP</span><span class="sxs-lookup"><span data-stu-id="b16e6-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="b16e6-110">Pro Azure v CSP jsou k dispozici dvě úrovně oprávnění správce.</span><span class="sxs-lookup"><span data-stu-id="b16e6-110">There are two levels of admin privileges for Azure in CSP.</span></span>

- <span data-ttu-id="b16e6-111">**Oprávnění správce na úrovni tenanta (delegovaná oprávnění správce)**: partneři CSP získají tato oprávnění při zřizování vztahů prodejců CSP se zákazníky.</span><span class="sxs-lookup"><span data-stu-id="b16e6-111">**Tenant level admin privileges (Delegated admin privileges)**:  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="b16e6-112">Delegovaná oprávnění správce dávají partnerům CSP přístup ke svým klientům.</span><span class="sxs-lookup"><span data-stu-id="b16e6-112">Delegated admin privileges give CSP partners access to their customers' tenants.</span></span> <span data-ttu-id="b16e6-113">Tento přístup umožňuje správcům provádět funkce, jako je přidání a Správa uživatelů, resetování hesel a Správa uživatelských licencí.</span><span class="sxs-lookup"><span data-stu-id="b16e6-113">This access allows them to do administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>
- <span data-ttu-id="b16e6-114">**Oprávnění správce na úrovni předplatného**: partneři CSP získají tato oprávnění při vytváření předplatných Azure CSP pro své zákazníky.</span><span class="sxs-lookup"><span data-stu-id="b16e6-114">**Subscription level admin privileges**: CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="b16e6-115">Tato oprávnění poskytují partnerům CSP úplný přístup k těmto předplatným, která jim umožní zřídit a spravovat prostředky Azure.</span><span class="sxs-lookup"><span data-stu-id="b16e6-115">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-a-partners-admin-privileges"></a><span data-ttu-id="b16e6-116">Obnovit zprostředkovatele CSP oprávnění správce</span><span class="sxs-lookup"><span data-stu-id="b16e6-116">Reinstate CSP a partner's admin privileges</span></span>

<span data-ttu-id="b16e6-117">Pokud pro zákazníka zadáte skupinu AdminAgents, může váš zákazník znovu vytvořit přiřazení role CSP `object ID` .</span><span class="sxs-lookup"><span data-stu-id="b16e6-117">Your customer can re-create the CSP role assignment if you provide the `object ID` of the AdminAgents group to your customer.</span></span> <span data-ttu-id="b16e6-118">Chcete-li znovu získat oprávnění delegovaného správce, musíte s vaším zákazníkem pracovat pomocí následujících kroků.</span><span class="sxs-lookup"><span data-stu-id="b16e6-118">To regain delegated admin privileges, you need to work with your customer through the following steps.</span></span>

1. <span data-ttu-id="b16e6-119">Přihlaste se na řídicí panel partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="b16e6-119">Sign into the Partner Center dashboard.</span></span>

2. <span data-ttu-id="b16e6-120">V nabídce partnerské Centrum vyberte **zákazníci**.</span><span class="sxs-lookup"><span data-stu-id="b16e6-120">On the Partner Center menu, select **Customers**.</span></span>

3. <span data-ttu-id="b16e6-121">Vyberte zákazníka, se kterým pracujete, a **požádejte o něj vztah prodejce**.</span><span class="sxs-lookup"><span data-stu-id="b16e6-121">Select the customer you are working with and **request a reseller relationship**.</span></span> <span data-ttu-id="b16e6-122">Tato akce vygeneruje odkaz na zákazníka, který má práva správce tenanta.</span><span class="sxs-lookup"><span data-stu-id="b16e6-122">This action generates a link to the customer who has tenant admin rights.</span></span>

4. <span data-ttu-id="b16e6-123">Váš zákazník musí vybrat odkaz a schválit žádost o vztah prodejce.</span><span class="sxs-lookup"><span data-stu-id="b16e6-123">Your customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Příklad e-mailu pro vytvoření vztahu prodejce":::

5. <span data-ttu-id="b16e6-125">Partner se musí připojit k partnerskému tenantovi, aby získal ID objektu skupiny AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="b16e6-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. <span data-ttu-id="b16e6-126">Váš zákazník pak musí provést následující kroky pomocí PowerShellu nebo rozhraní příkazového řádku Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="b16e6-126">Your customer must then do the following steps using either PowerShell or Azure CLI.</span></span> <span data-ttu-id="b16e6-127">Váš zákazník musí mít:</span><span class="sxs-lookup"><span data-stu-id="b16e6-127">Your customer must have:</span></span>

- <span data-ttu-id="b16e6-128">Role **vlastníka** nebo **Správce přístupu uživatele**</span><span class="sxs-lookup"><span data-stu-id="b16e6-128">The role of **owner** or **user access administrator**</span></span> 
- <span data-ttu-id="b16e6-129">Oprávnění k vytváření přiřazení rolí na úrovni předplatného</span><span class="sxs-lookup"><span data-stu-id="b16e6-129">Permissions to create role assignments at the subscription level</span></span>

   <span data-ttu-id="b16e6-130">a.</span><span class="sxs-lookup"><span data-stu-id="b16e6-130">a.</span></span> <span data-ttu-id="b16e6-131">V případě prostředí PowerShell musí zákazník aktualizovat `Az.Resources` modul.</span><span class="sxs-lookup"><span data-stu-id="b16e6-131">For PowerShell only, the customer must update the `Az.Resources` module.</span></span>
   ```powershell
   Update-Module Az.Resources
   ```

   <span data-ttu-id="b16e6-132">b.</span><span class="sxs-lookup"><span data-stu-id="b16e6-132">b.</span></span> <span data-ttu-id="b16e6-133">Zákazník se připojí ke klientovi, kde existuje předplatné CSP.</span><span class="sxs-lookup"><span data-stu-id="b16e6-133">The customer connects to the tenant where the CSP subscription exists.</span></span>
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   <span data-ttu-id="b16e6-134">c.</span><span class="sxs-lookup"><span data-stu-id="b16e6-134">c.</span></span> <span data-ttu-id="b16e6-135">Zákazník se připojí k předplatnému.</span><span class="sxs-lookup"><span data-stu-id="b16e6-135">The customer connects to the subscription.</span></span> <span data-ttu-id="b16e6-136">Toto platí *pouze* v případě, že má uživatel oprávnění k přiřazení role pro více předplatných v tenantovi.</span><span class="sxs-lookup"><span data-stu-id="b16e6-136">This is *only* applicable if the user has role assignment permissions over multiple subscriptions in the tenant.</span></span>

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   <span data-ttu-id="b16e6-137">d.</span><span class="sxs-lookup"><span data-stu-id="b16e6-137">d.</span></span> <span data-ttu-id="b16e6-138">Zákazník pak vytvoří přiřazení role.</span><span class="sxs-lookup"><span data-stu-id="b16e6-138">The customer then creates the role assignment.</span></span>
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

<span data-ttu-id="b16e6-139">Místo udělení oprávnění vlastníka v oboru předplatného můžete udělit na úrovni skupiny prostředků nebo prostředku.</span><span class="sxs-lookup"><span data-stu-id="b16e6-139">Instead of granting owner permissions at the subscription scope, you can grant at the resource group or resource level.</span></span> 

- <span data-ttu-id="b16e6-140">Na úrovni skupiny prostředků</span><span class="sxs-lookup"><span data-stu-id="b16e6-140">At the resource group level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- <span data-ttu-id="b16e6-141">Na úrovni prostředků</span><span class="sxs-lookup"><span data-stu-id="b16e6-141">At the resource level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

<span data-ttu-id="b16e6-142">Pokud výše uvedené kroky nefungují nebo při pokusu o jejich pokusy dojde k chybám, vyzkoušejte následující postup "catch-All", abyste mohli obnovit práva správce pro vašeho zákazníka.</span><span class="sxs-lookup"><span data-stu-id="b16e6-142">If the above steps don't work or you get errors when attempting them, try the following "catch-all" procedure to reinstate admin rights for your customer.</span></span>

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a><span data-ttu-id="b16e6-143">Poradce při potížích</span><span class="sxs-lookup"><span data-stu-id="b16e6-143">Troubleshooting</span></span>

<span data-ttu-id="b16e6-144">Pokud zákazník nemůže dokončit krok 6 výše, zkuste provést následující příkaz:</span><span class="sxs-lookup"><span data-stu-id="b16e6-144">If the customer is unable to complete step 6 above, have the customer try the following command:</span></span>

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

<span data-ttu-id="b16e6-145">Poskytněte výsledný `newRoleAssignment.log` soubor Microsoftu k další analýze.</span><span class="sxs-lookup"><span data-stu-id="b16e6-145">Provide the resulting `newRoleAssignment.log` file to Microsoft for further analysis.</span></span>

<span data-ttu-id="b16e6-146">Pokud procedura catch-All dojde k chybě během `Import-Module` , vyzkoušejte následující kroky:</span><span class="sxs-lookup"><span data-stu-id="b16e6-146">If the "catch-all" procedure fails during the `Import-Module`, try the following steps:</span></span>
- <span data-ttu-id="b16e6-147">Pokud import selhává, protože se modul používá, restartujte relaci PowerShellu tak, že zavřete a znovu otevřete všechna okna.</span><span class="sxs-lookup"><span data-stu-id="b16e6-147">If the import fails because the module is in use, restart the PowerShell session by closing and reopening all windows.</span></span>
- <span data-ttu-id="b16e6-148">Podívejte se na verzi `Az.Resources` s `Get-Module Az.Resources -ListAvailable` .</span><span class="sxs-lookup"><span data-stu-id="b16e6-148">Check version of `Az.Resources` with `Get-Module Az.Resources -ListAvailable`.</span></span>
- <span data-ttu-id="b16e6-149">Pokud verze 4.1.1 není v seznamu dostupných, je nutné použít `Update-Module Az.Resources -Force` .</span><span class="sxs-lookup"><span data-stu-id="b16e6-149">If version 4.1.1 is not within the available list, you must use `Update-Module Az.Resources -Force`.</span></span>
- <span data-ttu-id="b16e6-150">Pokud chyba uvádí, že se `Az.Accounts` musí jednat o konkrétní verzi, aktualizujte také tento modul a nahraďte ho `Az.Resources` `Az.Accounts` .</span><span class="sxs-lookup"><span data-stu-id="b16e6-150">If the error states that `Az.Accounts` needs to be a specific version, update that module as well, replacing `Az.Resources` with `Az.Accounts`.</span></span> <span data-ttu-id="b16e6-151">Pak musíte restartovat relaci PowerShellu.</span><span class="sxs-lookup"><span data-stu-id="b16e6-151">You must then restart the PowerShell session.</span></span>


## <a name="next-steps"></a><span data-ttu-id="b16e6-152">Další kroky</span><span class="sxs-lookup"><span data-stu-id="b16e6-152">Next steps</span></span>

- [<span data-ttu-id="b16e6-153">Správa předplatných a prostředků v rámci plánu Azure</span><span class="sxs-lookup"><span data-stu-id="b16e6-153">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
