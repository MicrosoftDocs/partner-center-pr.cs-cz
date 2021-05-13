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
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Obnovení oprávnění správce pro předplatná Azure CSP zákazníka  

**Odpovídající role:** Globální správce | Agent pro správu

Jako partner CSP vaši zákazníci často očekávají, že za ně budete spravovat jejich využití Azure a jejich systémy. To vyžaduje, abyste měli oprávnění správce. Některá oprávnění jsou udělena, když se nastane vztah prodejce se zákazníkem. Jiné vám udělí váš zákazník.

## <a name="admin-privileges-for-azure-in-csp"></a>Oprávnění správce pro Azure v CSP

Existují dvě úrovně oprávnění správce pro Azure v CSP.

**Oprávnění správce na úrovni tenanta** **(delegovaná** oprávnění správce) – Partneři CSP těmto oprávněním při navazování vztahu prodejce CSP se zákazníky. Delegovaná oprávnění správce poskytují partnerům CSP přístup k tenantům jejich zákazníků, což jim umožňuje provádět funkce správy, jako je přidávání a správa uživatelů, resetování hesel a správa uživatelských licencí.

**Oprávnění správce na úrovni předplatného** – partneři CSP těmto oprávněním při vytváření Azure CSP předplatných pro své zákazníky. Díky těmto oprávněním mají partneři CSP úplný přístup k těmto předplatným, což jim umožňuje zř vytvářet a spravovat prostředky Azure.

## <a name="reinstate-csp-partners-admin-privileges"></a>Obnovení oprávnění správce partnerů CSP

Zákazník může přiřazení role CSP vytvořit znovu, pokud zákazníkovi poskytnete ID objektu skupiny AdminAgents. Pokud chcete znovu získat delegovaná oprávnění správce, musíte spolupracovat se zákazníkem.

1. Přihlaste se k Partnerské centrum a v nabídce Partnerské centrum vyberte **Zákazníci.**

2. Vyberte zákazníka, se který **pracujete, a požádejte o vztah prodejce.** Tato akce vygeneruje odkaz na zákazníka, který má práva správce tenanta.

3. Zákazník musí vybrat odkaz a schválit žádost o vztah prodejce.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Příklad e-mailu pro vytvoření vztahu prodejce":::

4. Partner se musí připojit k partnerskému tenantovi, aby získal ID objektu skupiny AdminAgents.

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. Zákazník, který má roli **vlastníka nebo správce přístupu uživatele** a má oprávnění k vytvoření přiřazení role na úrovni předplatného, provede následující akce:


    1. Připojí se ke klientovi, kde existuje předplatné CSP.
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. Připojí se k předplatnému (platí jenom v případě, že má uživatel oprávnění k přiřazení role pro více předplatných v tenantovi).
   
         PS C:\WINDOWS\system32> Set-AzContext-SubscriptionID "ID předplatného CSP" "


    3. Vytvoří přiřazení role.
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


Pokud chcete udělit oprávnění role vlastníka na úrovni skupiny prostředků nebo na úrovni prostředku místo oboru předplatného, můžou fungovat tyto příkazy:


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a>Další kroky

- [Správa předplatných a prostředků v rámci plánu Azure](azure-plan-manage.md)
