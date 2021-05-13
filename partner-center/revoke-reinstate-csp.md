---
title: Obnovení oprávnění správce pro Azure CSP
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak zákazníkům pomoct obnovit oprávnění správce partnera, aby partner mohl pomoci spravovat předplatná Azure CSP předplatného zákazníka.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: ad29283001ec542944da4f0cac835c6a5d339251
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855416"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="9d462-103">Obnovení oprávnění správce pro předplatná Azure CSP zákazníka</span><span class="sxs-lookup"><span data-stu-id="9d462-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="9d462-104">**Odpovídající role:** Globální správce | Agent pro správu</span><span class="sxs-lookup"><span data-stu-id="9d462-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="9d462-105">Jako partner CSP vaši zákazníci často očekávají, že za ně budete spravovat jejich využití Azure a jejich systémy.</span><span class="sxs-lookup"><span data-stu-id="9d462-105">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="9d462-106">To vyžaduje, abyste měli oprávnění správce.</span><span class="sxs-lookup"><span data-stu-id="9d462-106">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="9d462-107">Některá oprávnění jsou udělena, když se nastane vztah prodejce se zákazníkem.</span><span class="sxs-lookup"><span data-stu-id="9d462-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="9d462-108">Jiné vám udělí váš zákazník.</span><span class="sxs-lookup"><span data-stu-id="9d462-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="9d462-109">Oprávnění správce pro Azure v CSP</span><span class="sxs-lookup"><span data-stu-id="9d462-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="9d462-110">Existují dvě úrovně oprávnění správce pro Azure v CSP.</span><span class="sxs-lookup"><span data-stu-id="9d462-110">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="9d462-111">**Oprávnění správce na úrovni tenanta** **(delegovaná** oprávnění správce) – Partneři CSP těmto oprávněním při navazování vztahu prodejce CSP se zákazníky.</span><span class="sxs-lookup"><span data-stu-id="9d462-111">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="9d462-112">Delegovaná oprávnění správce poskytují partnerům CSP přístup k tenantům jejich zákazníků, což jim umožňuje provádět funkce správy, jako je přidávání a správa uživatelů, resetování hesel a správa uživatelských licencí.</span><span class="sxs-lookup"><span data-stu-id="9d462-112">Delegated admin privileges give CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="9d462-113">**Oprávnění správce na úrovni předplatného** – partneři CSP těmto oprávněním při vytváření Azure CSP předplatných pro své zákazníky.</span><span class="sxs-lookup"><span data-stu-id="9d462-113">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="9d462-114">Díky těmto oprávněním mají partneři CSP úplný přístup k těmto předplatným, což jim umožňuje zř vytvářet a spravovat prostředky Azure.</span><span class="sxs-lookup"><span data-stu-id="9d462-114">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="9d462-115">Obnovení oprávnění správce partnerů CSP</span><span class="sxs-lookup"><span data-stu-id="9d462-115">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="9d462-116">Zákazník může přiřazení role CSP vytvořit znovu, pokud zákazníkovi poskytnete ID objektu skupiny AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="9d462-116">Your customer can re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="9d462-117">Pokud chcete znovu získat delegovaná oprávnění správce, musíte spolupracovat se zákazníkem.</span><span class="sxs-lookup"><span data-stu-id="9d462-117">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="9d462-118">Přihlaste se k Partnerské centrum a v nabídce Partnerské centrum vyberte **Zákazníci.**</span><span class="sxs-lookup"><span data-stu-id="9d462-118">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="9d462-119">Vyberte zákazníka, se který **pracujete, a požádejte o vztah prodejce.**</span><span class="sxs-lookup"><span data-stu-id="9d462-119">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="9d462-120">Tato akce vygeneruje odkaz na zákazníka, který má práva správce tenanta.</span><span class="sxs-lookup"><span data-stu-id="9d462-120">This action generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="9d462-121">Zákazník musí vybrat odkaz a schválit žádost o vztah prodejce.</span><span class="sxs-lookup"><span data-stu-id="9d462-121">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Příklad e-mailu pro vytvoření vztahu prodejce":::

4. <span data-ttu-id="9d462-123">Partner se musí připojit k partnerskému tenantovi, aby získal ID objektu skupiny AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="9d462-123">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="9d462-124">Zákazník, který má roli **vlastníka nebo správce přístupu uživatele** a má oprávnění k vytvoření přiřazení role na úrovni předplatného, provede následující akce:</span><span class="sxs-lookup"><span data-stu-id="9d462-124">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="9d462-125">Připojí se ke klientovi, kde existuje předplatné CSP.</span><span class="sxs-lookup"><span data-stu-id="9d462-125">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="9d462-126">Připojí se k předplatnému (platí jenom v případě, že má uživatel oprávnění k přiřazení role pro více předplatných v tenantovi).</span><span class="sxs-lookup"><span data-stu-id="9d462-126">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="9d462-127">PS C:\WINDOWS\system32> Set-AzContext-SubscriptionID "ID předplatného CSP" "</span><span class="sxs-lookup"><span data-stu-id="9d462-127">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="9d462-128">Vytvoří přiřazení role.</span><span class="sxs-lookup"><span data-stu-id="9d462-128">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="9d462-129">Pokud chcete udělit oprávnění role vlastníka na úrovni skupiny prostředků nebo na úrovni prostředku místo oboru předplatného, můžou fungovat tyto příkazy:</span><span class="sxs-lookup"><span data-stu-id="9d462-129">If you want to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="9d462-130">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9d462-130">Next steps</span></span>

- [<span data-ttu-id="9d462-131">Správa předplatných a prostředků v rámci plánu Azure</span><span class="sxs-lookup"><span data-stu-id="9d462-131">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
