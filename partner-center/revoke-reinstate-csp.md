---
title: Obnovit oprávnění správce pro zprostředkovatele CSP Azure
ms.topic: how-to
ms.date: 07/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se, jak zákazníkům pomáhat obnovit oprávnění správce partnera, aby partner mohl spravovat předplatná Azure CSP zákazníka.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 13fdeb01ecd73dc1a63d174a4ad5cb8e1bdc813a
ms.sourcegitcommit: 455894365fa488368f7572ac72312e84a267ef5e
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/10/2020
ms.locfileid: "97011498"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Obnovit oprávnění správce pro předplatná Azure CSP zákazníka  

**Příslušné role**

- Globální správce
- Agent správce

Jako partner CSP vaši zákazníci často očekávají, že budete spravovat jejich využití Azure a jejich systémy. K tomu je potřeba mít oprávnění správce. Některá oprávnění jsou udělována v případě, že je vytvořen vztah prodejce se zákazníkem. Další vám je uděleno vaším zákazníkem.

## <a name="admin-privileges-for-azure-in-csp"></a>Oprávnění správce pro Azure v CSP

Pro Azure v CSP jsou k dispozici dvě úrovně oprávnění správce.

**Oprávnění správce na úrovni tenanta** (**delegovaná oprávnění správce**) – partneři CSP získají tato oprávnění při zřizování vztahů prodejců CSP se zákazníky. To dává partnerům CSP přístup k svým klientům, kteří jim umožní provádět funkce správy, jako je například přidávání a Správa uživatelů, resetování hesel a Správa uživatelských licencí.

**Oprávnění správce na úrovni předplatného** – partneři CSP získají tato oprávnění při vytváření předplatných Azure CSP pro své zákazníky. Tato oprávnění poskytují partnerům CSP úplný přístup k těmto předplatným, která jim umožní zřídit a spravovat prostředky Azure.

## <a name="reinstate-csp-partners-admin-privileges"></a>Obnovit oprávnění správce pro partnery CSP

Chcete-li znovu získat oprávnění delegovaného správce, je nutné pracovat se zákazníkem.

1. Přihlaste se na řídicí panel partnerského centra a v nabídce partnerské Centrum vyberte **zákazníci**.

2. Vyberte zákazníka, se kterým pracujete, a **požádejte o něj vztah prodejce.** Tím se vygeneruje odkaz na zákazníka, který má práva správce tenanta.

3. Tento uživatel musí vybrat odkaz a schválit žádost o vztah prodejce.

   :::image type="content" source="images/azure/revoke4.png" alt-text="vztah prodejce":::

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a>Přidání skupiny agentů pro správu jako vlastníka pro předplatné služby Azure CSP

Zákazník bude muset přidat skupinu agentů pro správu jako vlastníka předplatného služby Azure CSP, skupiny prostředků nebo prostředku. 

1. Použijte konzolu PowerShellu nebo Integrované skriptovací prostředí (ISE) prostředí PowerShell. Ujistěte se, že jsou nainstalované moduly AzureAD.

2. Připojte se k Tenantovi služby Azure AD.

   ```powershell
   Connect-AzureAD
   ```

3. Získat ID ObjectId skupin agentů pro správu.

   ```powershell
   Get-AzureADGroup
   ```
   Následující kroky provádí uživatel ve společnosti zákazníka, který má oprávnění vlastníka k předplatnému služby Azure CSP.

4. Uživatel s přístupem vlastníka k předplatnému Azure CSP se do Azure přihlásí pomocí svých přihlašovacích údajů.

   ```powershell
   Connect-AzureRmAccount
   ```

5. Pak může přidat skupinu agentů pro správu jako vlastníka do předplatného služby CSP Azure, skupiny prostředků nebo prostředku použitím správného identifikátoru URI prostředku v parametru Scope. 

    ```powershell
    # Grant owner role at subscription level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"

    # Grant owner role at resource group level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>/resourceGroups/<Resource group name>"

    # Grant owner role at resource level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "<Resource Uri>"
    ```

## <a name="next-steps"></a>Další kroky

[Správa předplatných a prostředků v rámci plánu Azure](azure-plan-manage.md)
