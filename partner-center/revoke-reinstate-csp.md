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
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Obnovení oprávnění správce pro předplatná Azure CSP zákazníka  

**Odpovídající role:** Globální správce | Agent pro správu

Jako partner CSP vaši zákazníci často očekávají, že za ně budete spravovat využití Azure a jejich systémy. K tomu musíte mít oprávnění správce. Některá oprávnění jsou udělena, když se nastane vztah prodejce se zákazníkem. Jiné vám udělí váš zákazník.

## <a name="admin-privileges-for-azure-in-csp"></a>Oprávnění správce pro Azure v CSP

Existují dvě úrovně oprávnění správce pro Azure v CSP.

- **Oprávnění správce na úrovni tenanta (delegovaná** oprávnění správce): Partneři CSP těmto oprávněním při navazování vztahu prodejce CSP se zákazníky. Delegovaná oprávnění správce poskytují partnerům CSP přístup k tenantům jejich zákazníků. Tento přístup jim umožňuje používat funkce správy, jako je přidávání a správa uživatelů, resetování hesel a správa uživatelských licencí.
- **Oprávnění správce na úrovni předplatného:** Partneři CSP těmto oprávněním při vytváření Azure CSP předplatných pro své zákazníky. Díky těmto oprávněním mají partneři CSP úplný přístup k těmto předplatným, což jim umožňuje zřizování a správu prostředků Azure.

## <a name="reinstate-csp-a-partners-admin-privileges"></a>Obnovení oprávnění správce partnera csp

Pokud zákazníkovi poskytnete skupinu AdminAgents, zákazník může přiřazení role CSP `object ID` vytvořit znovu. Pokud chcete znovu získat delegovaná oprávnění správce, musíte spolupracovat se zákazníkem pomocí následujících kroků.

1. Přihlaste se k řídicímu Partnerské centrum.

2. V nabídce Partnerské centrum vyberte **Zákazníci.**

3. Vyberte zákazníka, se kterým pracujete, a **požádejte o něj vztah prodejce**. Tato akce vygeneruje odkaz na zákazníka, který má práva správce tenanta.

4. Váš zákazník musí vybrat odkaz a schválit žádost o vztah prodejce.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Příklad e-mailu pro vytvoření vztahu prodejce":::

5. Partner se musí připojit k partnerskému tenantovi, aby získal ID objektu skupiny AdminAgents.
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. Váš zákazník pak musí provést následující kroky pomocí PowerShellu nebo rozhraní příkazového řádku Azure CLI. Váš zákazník musí mít:

- Role **vlastníka** nebo **Správce přístupu uživatele** 
- Oprávnění k vytváření přiřazení rolí na úrovni předplatného

   a. V případě prostředí PowerShell musí zákazník aktualizovat `Az.Resources` modul.
   ```powershell
   Update-Module Az.Resources
   ```

   b. Zákazník se připojí ke klientovi, kde existuje předplatné CSP.
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   c. Zákazník se připojí k předplatnému. Toto platí *pouze* v případě, že má uživatel oprávnění k přiřazení role pro více předplatných v tenantovi.

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   d. Zákazník pak vytvoří přiřazení role.
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

Místo udělení oprávnění vlastníka v oboru předplatného můžete udělit na úrovni skupiny prostředků nebo prostředku. 

- Na úrovni skupiny prostředků

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- Na úrovni prostředků

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

## <a name="next-steps"></a>Další kroky

- [Správa předplatných a prostředků v rámci plánu Azure](azure-plan-manage.md)
