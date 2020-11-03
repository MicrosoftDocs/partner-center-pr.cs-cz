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
ms.openlocfilehash: c694f48fb62fc031bfaf78be6a1c4e43629a7adb
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2020
ms.locfileid: "92527140"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Obnovit oprávnění správce pro předplatná Azure CSP zákazníka  

**Příslušné role**

- Globální správce
- Agent správce

Jako partner CSP vaši zákazníci často očekávají, že budete spravovat jejich využití Azure a jejich systémy. K tomu je potřeba mít oprávnění správce. Některá oprávnění jsou udělována v případě, že je vytvořen vztah prodejce se zákazníkem. Další vám je uděleno vaším zákazníkem.

## <a name="admin-privileges-for-azure-in-csp"></a>Oprávnění správce pro Azure v CSP

Pro Azure v CSP jsou k dispozici dvě úrovně oprávnění správce.

**Oprávnění správce na úrovni tenanta** ( **delegovaná oprávnění správce** ) – partneři CSP získají tato oprávnění při zřizování vztahů prodejců CSP se zákazníky. To dává partnerům CSP přístup k svým klientům, kteří jim umožní provádět funkce správy, jako je například přidávání a Správa uživatelů, resetování hesel a Správa uživatelských licencí.

**Oprávnění správce na úrovni předplatného** – partneři CSP získají tato oprávnění při vytváření předplatných Azure CSP pro své zákazníky. Tato oprávnění poskytují partnerům CSP úplný přístup k těmto předplatným, která jim umožní zřídit a spravovat prostředky Azure.

## <a name="reinstate-csp-partners-admin-privileges"></a>Obnovit oprávnění správce pro partnery CSP

Chcete-li znovu získat oprávnění delegovaného správce, je nutné pracovat se zákazníkem.

1. Přihlaste se na řídicí panel partnerského centra a v nabídce partnerské Centrum vyberte **zákazníci** .

2. Vyberte zákazníka, se kterým pracujete, a **požádejte o něj vztah prodejce.** Tím se vygeneruje odkaz na zákazníka, který má práva správce tenanta.

3. Tento uživatel musí vybrat odkaz a schválit žádost o vztah prodejce.

   :::image type="content" source="images/azure/revoke4.png" alt-text="vztah prodejce":::

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a>Přidání skupiny agentů pro správu jako vlastníka pro předplatné služby Azure CSP

Zákazník bude muset přidat vaši skupinu agentů pro správu jako vlastníka předplatného služby Azure CSP.

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
   Connect-AzAccount
   ```

5. Pak může přidat skupinu agentů pro správu jako vlastníka do předplatného služby CSP Azure.

    ```powershell
    New-AzureRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"
    ```

## <a name="next-steps"></a>Další kroky

[Správa předplatných a prostředků v rámci plánu Azure](azure-plan-manage.md)
