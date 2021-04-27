---
title: Obnovit oprávnění správce pro zprostředkovatele CSP Azure
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se, jak zákazníkům pomáhat obnovit oprávnění správce partnera, aby partner mohl spravovat předplatná Azure CSP zákazníka.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 26768bdf33c03145a893fa445eab6ebf92ca9b1c
ms.sourcegitcommit: efd711b0e65c55f24ce5b9636abd7b5a8cc719fe
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/27/2021
ms.locfileid: "108018183"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="efd3a-103">Obnovit oprávnění správce pro předplatná Azure CSP zákazníka</span><span class="sxs-lookup"><span data-stu-id="efd3a-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="efd3a-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="efd3a-104">**Appropriate roles**</span></span>

- <span data-ttu-id="efd3a-105">Globální správce</span><span class="sxs-lookup"><span data-stu-id="efd3a-105">Global admin</span></span>
- <span data-ttu-id="efd3a-106">Agent správce</span><span class="sxs-lookup"><span data-stu-id="efd3a-106">Admin agent</span></span>

<span data-ttu-id="efd3a-107">Jako partner CSP vaši zákazníci často očekávají, že budete spravovat jejich využití Azure a jejich systémy.</span><span class="sxs-lookup"><span data-stu-id="efd3a-107">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="efd3a-108">K tomu je potřeba mít oprávnění správce.</span><span class="sxs-lookup"><span data-stu-id="efd3a-108">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="efd3a-109">Některá oprávnění se udělují v případě, že je vytvořen vztah prodejce se zákazníkem.</span><span class="sxs-lookup"><span data-stu-id="efd3a-109">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="efd3a-110">Další vám je uděleno vaším zákazníkem.</span><span class="sxs-lookup"><span data-stu-id="efd3a-110">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="efd3a-111">Oprávnění správce pro Azure v CSP</span><span class="sxs-lookup"><span data-stu-id="efd3a-111">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="efd3a-112">Pro Azure v CSP jsou k dispozici dvě úrovně oprávnění správce.</span><span class="sxs-lookup"><span data-stu-id="efd3a-112">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="efd3a-113">**Oprávnění správce na úrovni tenanta** (**delegovaná oprávnění správce**) – partneři CSP získají tato oprávnění při zřizování vztahů prodejců CSP se zákazníky.</span><span class="sxs-lookup"><span data-stu-id="efd3a-113">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="efd3a-114">Delegovaná oprávnění správce dávají partnerům CSP přístup k svým klientům, kteří jim umožní provádět funkce správy, jako je například přidání nebo Správa uživatelů, resetování hesel a Správa uživatelských licencí.</span><span class="sxs-lookup"><span data-stu-id="efd3a-114">Delegated admin privileges give CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="efd3a-115">**Oprávnění správce na úrovni předplatného** – partneři CSP získají tato oprávnění při vytváření předplatných Azure CSP pro své zákazníky.</span><span class="sxs-lookup"><span data-stu-id="efd3a-115">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="efd3a-116">Tato oprávnění poskytují partnerům CSP úplný přístup k těmto předplatným, která jim umožní zřídit a spravovat prostředky Azure.</span><span class="sxs-lookup"><span data-stu-id="efd3a-116">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="efd3a-117">Obnovit oprávnění správce pro partnery CSP</span><span class="sxs-lookup"><span data-stu-id="efd3a-117">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="efd3a-118">Zákazník může přiřazení role CSP znovu vytvořit, pokud zadáte ID objektu skupiny AdminAgents vašemu zákazníkovi.</span><span class="sxs-lookup"><span data-stu-id="efd3a-118">Your customer can re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="efd3a-119">Chcete-li znovu získat oprávnění delegovaného správce, je nutné pracovat se zákazníkem.</span><span class="sxs-lookup"><span data-stu-id="efd3a-119">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="efd3a-120">Přihlaste se k řídicímu panelu partnerského centra a v nabídce partnerské Centrum vyberte **zákazníci**.</span><span class="sxs-lookup"><span data-stu-id="efd3a-120">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="efd3a-121">Vyberte zákazníka, se kterým pracujete, a **požádejte o něj vztah prodejce.**</span><span class="sxs-lookup"><span data-stu-id="efd3a-121">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="efd3a-122">Tato akce vygeneruje odkaz na zákazníka, který má práva správce tenanta.</span><span class="sxs-lookup"><span data-stu-id="efd3a-122">This action generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="efd3a-123">Zákazník musí vybrat odkaz a schválit žádost o vztah prodejce.</span><span class="sxs-lookup"><span data-stu-id="efd3a-123">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Příklad e-mailu pro vytvoření vztahu prodejce":::

4. <span data-ttu-id="efd3a-125">Partner se musí připojit k partnerskému tenantovi, aby získal ID objektu skupiny AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="efd3a-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="efd3a-126">Zákazník, který má roli **vlastníka nebo správce přístupu uživatele** a má oprávnění k vytvoření přiřazení role na úrovni předplatného, provede následující akce:</span><span class="sxs-lookup"><span data-stu-id="efd3a-126">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="efd3a-127">Připojí se ke klientovi, kde existuje předplatné CSP.</span><span class="sxs-lookup"><span data-stu-id="efd3a-127">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="efd3a-128">Připojí se k předplatnému (platí jenom v případě, že má uživatel oprávnění k přiřazení role pro více předplatných v tenantovi).</span><span class="sxs-lookup"><span data-stu-id="efd3a-128">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="efd3a-129">PS C:\WINDOWS\system32> Set-AzContext-SubscriptionID "ID předplatného CSP" "</span><span class="sxs-lookup"><span data-stu-id="efd3a-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="efd3a-130">Vytvoří přiřazení role.</span><span class="sxs-lookup"><span data-stu-id="efd3a-130">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="efd3a-131">Pokud chcete udělit oprávnění role vlastníka na úrovni skupiny prostředků nebo na úrovni prostředku místo oboru předplatného, můžou fungovat tyto příkazy:</span><span class="sxs-lookup"><span data-stu-id="efd3a-131">If you want to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="efd3a-132">Další kroky</span><span class="sxs-lookup"><span data-stu-id="efd3a-132">Next steps</span></span>

- [<span data-ttu-id="efd3a-133">Správa předplatných a prostředků v rámci plánu Azure</span><span class="sxs-lookup"><span data-stu-id="efd3a-133">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
