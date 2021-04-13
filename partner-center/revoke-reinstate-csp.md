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
ms.openlocfilehash: f536d975d3c644a7afa29a95a3cb45608f6b2c9f
ms.sourcegitcommit: 89be77c9f35c77463d9558826293202afc6dec56
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/13/2021
ms.locfileid: "107315843"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Obnovit oprávnění správce pro předplatná Azure CSP zákazníka  

**Příslušné role**

- Globální správce
- Agent správce

Jako partner CSP vaši zákazníci často očekávají, že budete spravovat jejich využití Azure a jejich systémy. K tomu je potřeba mít oprávnění správce. Některá oprávnění se udělují v případě, že je vytvořen vztah prodejce se zákazníkem. Další vám je uděleno vaším zákazníkem.

## <a name="admin-privileges-for-azure-in-csp"></a>Oprávnění správce pro Azure v CSP

Pro Azure v CSP jsou k dispozici dvě úrovně oprávnění správce.

**Oprávnění správce na úrovni tenanta** (**delegovaná oprávnění správce**) – partneři CSP získají tato oprávnění při zřizování vztahů prodejců CSP se zákazníky. Delegovaná oprávnění správce dává partnerům CSP přístup k svým klientům, kteří jim umožní provádět funkce správy, jako je například přidání nebo Správa uživatelů, resetování hesel a Správa uživatelských licencí.

**Oprávnění správce na úrovni předplatného** – partneři CSP získají tato oprávnění při vytváření předplatných Azure CSP pro své zákazníky. Tato oprávnění poskytují partnerům CSP úplný přístup k těmto předplatným, která jim umožní zřídit a spravovat prostředky Azure.

## <a name="reinstate-csp-partners-admin-privileges"></a>Obnovit oprávnění správce pro partnery CSP

Zákazník může přiřazení role CSP znovu vytvořit, pokud zadáte ID objektu skupiny AdminAgents vašemu zákazníkovi. Chcete-li znovu získat oprávnění delegovaného správce, je nutné pracovat se zákazníkem.

1. Přihlaste se k řídicímu panelu partnerského centra a v nabídce partnerské Centrum vyberte **zákazníci**.

2. Vyberte zákazníka, se kterým pracujete, a **požádejte o něj vztah prodejce.** Tím se vygeneruje odkaz na zákazníka, který má práva správce tenanta.

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


Pokud je potřeba udělit oprávnění role vlastníka na úrovni skupiny prostředků nebo na úrovni prostředku místo oboru předplatného, můžou fungovat tyto příkazy:


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a>Další kroky

- [Správa předplatných a prostředků v rámci plánu Azure](azure-plan-manage.md)
