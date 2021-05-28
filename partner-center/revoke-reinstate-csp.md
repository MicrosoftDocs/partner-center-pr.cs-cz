---
title: Obnovení oprávnění správce pro Azure CSP
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak zákazníkům pomoct obnovit oprávnění správce partnera, aby partner mohl pomoci spravovat předplatná Azure CSP předplatného zákazníka.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: ca4c8323562e6c6f1d762465cad86e7ae113eb19
ms.sourcegitcommit: beba696954b62ab5396a893d050d0c2c211aeafc
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/28/2021
ms.locfileid: "110601422"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="48ece-103">Obnovení oprávnění správce pro předplatná Azure CSP zákazníka</span><span class="sxs-lookup"><span data-stu-id="48ece-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="48ece-104">**Odpovídající role:** Globální správce | Agent pro správu</span><span class="sxs-lookup"><span data-stu-id="48ece-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="48ece-105">Jako partner CSP vaši zákazníci často očekávají, že za ně budete spravovat využití Azure a jejich systémy.</span><span class="sxs-lookup"><span data-stu-id="48ece-105">As a CSP partner, your customers often expect that you'll manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="48ece-106">K tomu musíte mít oprávnění správce.</span><span class="sxs-lookup"><span data-stu-id="48ece-106">You must have admin privileges to do so.</span></span> <span data-ttu-id="48ece-107">Některá oprávnění jsou udělena, když se nastane vztah prodejce se zákazníkem.</span><span class="sxs-lookup"><span data-stu-id="48ece-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="48ece-108">Jiné vám udělí váš zákazník.</span><span class="sxs-lookup"><span data-stu-id="48ece-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="48ece-109">Oprávnění správce pro Azure v CSP</span><span class="sxs-lookup"><span data-stu-id="48ece-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="48ece-110">Existují dvě úrovně oprávnění správce pro Azure v CSP.</span><span class="sxs-lookup"><span data-stu-id="48ece-110">There are two levels of admin privileges for Azure in CSP.</span></span>

- <span data-ttu-id="48ece-111">**Oprávnění správce na úrovni tenanta (delegovaná** oprávnění správce): Partneři CSP těmto oprávněním při navazování vztahu prodejce CSP se zákazníky.</span><span class="sxs-lookup"><span data-stu-id="48ece-111">**Tenant level admin privileges (Delegated admin privileges)**:  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="48ece-112">Delegovaná oprávnění správce poskytují partnerům CSP přístup k tenantům jejich zákazníků.</span><span class="sxs-lookup"><span data-stu-id="48ece-112">Delegated admin privileges give CSP partners access to their customers' tenants.</span></span> <span data-ttu-id="48ece-113">Tento přístup jim umožňuje používat funkce správy, jako je přidávání a správa uživatelů, resetování hesel a správa uživatelských licencí.</span><span class="sxs-lookup"><span data-stu-id="48ece-113">This access allows them to do administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>
- <span data-ttu-id="48ece-114">**Oprávnění správce na úrovni předplatného:** Partneři CSP těmto oprávněním při vytváření Azure CSP předplatných pro své zákazníky.</span><span class="sxs-lookup"><span data-stu-id="48ece-114">**Subscription level admin privileges**: CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="48ece-115">Díky těmto oprávněním mají partneři CSP úplný přístup k těmto předplatným, což jim umožňuje zřizování a správu prostředků Azure.</span><span class="sxs-lookup"><span data-stu-id="48ece-115">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-a-partners-admin-privileges"></a><span data-ttu-id="48ece-116">Obnovení oprávnění správce partnera csp</span><span class="sxs-lookup"><span data-stu-id="48ece-116">Reinstate CSP a partner's admin privileges</span></span>

<span data-ttu-id="48ece-117">Pokud zákazníkovi poskytnete skupinu AdminAgents, zákazník může přiřazení role CSP `object ID` vytvořit znovu.</span><span class="sxs-lookup"><span data-stu-id="48ece-117">Your customer can re-create the CSP role assignment if you provide the `object ID` of the AdminAgents group to your customer.</span></span> <span data-ttu-id="48ece-118">Pokud chcete znovu získat delegovaná oprávnění správce, musíte spolupracovat se zákazníkem pomocí následujících kroků.</span><span class="sxs-lookup"><span data-stu-id="48ece-118">To regain delegated admin privileges, you need to work with your customer through the following steps.</span></span>

1. <span data-ttu-id="48ece-119">Přihlaste se k řídicímu Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="48ece-119">Sign into the Partner Center dashboard.</span></span>

2. <span data-ttu-id="48ece-120">V nabídce Partnerské centrum vyberte **Zákazníci.**</span><span class="sxs-lookup"><span data-stu-id="48ece-120">On the Partner Center menu, select **Customers**.</span></span>

3. <span data-ttu-id="48ece-121">Vyberte zákazníka, se kterým pracujete, a **požádejte o něj vztah prodejce**.</span><span class="sxs-lookup"><span data-stu-id="48ece-121">Select the customer you are working with and **request a reseller relationship**.</span></span> <span data-ttu-id="48ece-122">Tato akce vygeneruje odkaz na zákazníka, který má práva správce tenanta.</span><span class="sxs-lookup"><span data-stu-id="48ece-122">This action generates a link to the customer who has tenant admin rights.</span></span>

4. <span data-ttu-id="48ece-123">Váš zákazník musí vybrat odkaz a schválit žádost o vztah prodejce.</span><span class="sxs-lookup"><span data-stu-id="48ece-123">Your customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Příklad e-mailu pro vytvoření vztahu prodejce":::

5. <span data-ttu-id="48ece-125">Partner se musí připojit k partnerskému tenantovi, aby získal ID objektu skupiny AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="48ece-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. <span data-ttu-id="48ece-126">Váš zákazník pak musí provést následující kroky pomocí PowerShellu nebo rozhraní příkazového řádku Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="48ece-126">Your customer must then do the following steps using either PowerShell or Azure CLI.</span></span> <span data-ttu-id="48ece-127">Váš zákazník musí mít:</span><span class="sxs-lookup"><span data-stu-id="48ece-127">Your customer must have:</span></span>

- <span data-ttu-id="48ece-128">Role **vlastníka** nebo **Správce přístupu uživatele**</span><span class="sxs-lookup"><span data-stu-id="48ece-128">The role of **owner** or **user access administrator**</span></span> 
- <span data-ttu-id="48ece-129">Oprávnění k vytváření přiřazení rolí na úrovni předplatného</span><span class="sxs-lookup"><span data-stu-id="48ece-129">Permissions to create role assignments at the subscription level</span></span>

   <span data-ttu-id="48ece-130">a.</span><span class="sxs-lookup"><span data-stu-id="48ece-130">a.</span></span> <span data-ttu-id="48ece-131">V případě prostředí PowerShell musí zákazník aktualizovat `Az.Resources` modul.</span><span class="sxs-lookup"><span data-stu-id="48ece-131">For PowerShell only, the customer must update the `Az.Resources` module.</span></span>
   ```powershell
   Update-Module Az.Resources
   ```

   <span data-ttu-id="48ece-132">b.</span><span class="sxs-lookup"><span data-stu-id="48ece-132">b.</span></span> <span data-ttu-id="48ece-133">Zákazník se připojí ke klientovi, kde existuje předplatné CSP.</span><span class="sxs-lookup"><span data-stu-id="48ece-133">The customer connects to the tenant where the CSP subscription exists.</span></span>
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   <span data-ttu-id="48ece-134">c.</span><span class="sxs-lookup"><span data-stu-id="48ece-134">c.</span></span> <span data-ttu-id="48ece-135">Zákazník se připojí k předplatnému.</span><span class="sxs-lookup"><span data-stu-id="48ece-135">The customer connects to the subscription.</span></span> <span data-ttu-id="48ece-136">Toto platí *pouze* v případě, že má uživatel oprávnění k přiřazení role pro více předplatných v tenantovi.</span><span class="sxs-lookup"><span data-stu-id="48ece-136">This is *only* applicable if the user has role assignment permissions over multiple subscriptions in the tenant.</span></span>

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   <span data-ttu-id="48ece-137">d.</span><span class="sxs-lookup"><span data-stu-id="48ece-137">d.</span></span> <span data-ttu-id="48ece-138">Zákazník pak vytvoří přiřazení role.</span><span class="sxs-lookup"><span data-stu-id="48ece-138">The customer then creates the role assignment.</span></span>
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

<span data-ttu-id="48ece-139">Místo udělení oprávnění vlastníka v oboru předplatného můžete udělit na úrovni skupiny prostředků nebo prostředku.</span><span class="sxs-lookup"><span data-stu-id="48ece-139">Instead of granting owner permissions at the subscription scope, you can grant at the resource group or resource level.</span></span> 

- <span data-ttu-id="48ece-140">Na úrovni skupiny prostředků</span><span class="sxs-lookup"><span data-stu-id="48ece-140">At the resource group level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- <span data-ttu-id="48ece-141">Na úrovni prostředků</span><span class="sxs-lookup"><span data-stu-id="48ece-141">At the resource level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

## <a name="next-steps"></a><span data-ttu-id="48ece-142">Další kroky</span><span class="sxs-lookup"><span data-stu-id="48ece-142">Next steps</span></span>

- [<span data-ttu-id="48ece-143">Správa předplatných a prostředků v rámci plánu Azure</span><span class="sxs-lookup"><span data-stu-id="48ece-143">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
