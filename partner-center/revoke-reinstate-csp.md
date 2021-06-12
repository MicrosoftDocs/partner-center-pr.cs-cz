---
title: Obnovit oprávnění správce pro zprostředkovatele CSP Azure
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se, jak zákazníkům pomáhat obnovit oprávnění správce partnera, aby partner mohl spravovat předplatná Azure CSP zákazníka.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 90c8f413398fcb9f65f7fef402a1cdcd092abbc4
ms.sourcegitcommit: 212471150efc8fd2c30023bc6a981a7e052e79ef
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/11/2021
ms.locfileid: "112025951"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Obnovit oprávnění správce pro předplatná Azure CSP zákazníka  

**Příslušné role**: globální správce | Agent správce

Jako partner CSP si zákazníci často očekávají, že budete spravovat jejich využití Azure a jejich systémy. K tomu musíte mít oprávnění správce. Některá oprávnění se udělují v případě, že je vytvořen vztah prodejce se zákazníkem. Další vám je uděleno vaším zákazníkem.

## <a name="admin-privileges-for-azure-in-csp"></a>Oprávnění správce pro Azure v CSP

Pro Azure v CSP jsou k dispozici dvě úrovně oprávnění správce.

- **Oprávnění správce na úrovni tenanta (delegovaná oprávnění správce)**: partneři CSP získají tato oprávnění při zřizování vztahů prodejců CSP se zákazníky. Delegovaná oprávnění správce dávají partnerům CSP přístup ke svým klientům. Tento přístup umožňuje správcům provádět funkce, jako je přidání a Správa uživatelů, resetování hesel a Správa uživatelských licencí.
- **Oprávnění správce na úrovni předplatného**: partneři CSP získají tato oprávnění při vytváření předplatných Azure CSP pro své zákazníky. Tato oprávnění poskytují partnerům CSP úplný přístup k těmto předplatným, která jim umožní zřídit a spravovat prostředky Azure.

## <a name="reinstate-csp-a-partners-admin-privileges"></a>Obnovit zprostředkovatele CSP oprávnění správce

Pokud pro zákazníka zadáte skupinu AdminAgents, může váš zákazník znovu vytvořit přiřazení role CSP `object ID` . Chcete-li znovu získat oprávnění delegovaného správce, musíte s vaším zákazníkem pracovat pomocí následujících kroků.

1. Přihlaste se na řídicí panel partnerského centra.

2. V nabídce partnerské Centrum vyberte **zákazníci**.

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

Pokud výše uvedené kroky nefungují nebo při pokusu o jejich pokusy dojde k chybám, vyzkoušejte následující postup "catch-All", abyste mohli obnovit práva správce pro vašeho zákazníka.

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a>Řešení potíží

Pokud zákazník nemůže dokončit krok 6 výše, zkuste provést následující příkaz:

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

Poskytněte výsledný `newRoleAssignment.log` soubor Microsoftu k další analýze.

Pokud procedura catch-All dojde k chybě během `Import-Module` , vyzkoušejte následující kroky:
- Pokud import selhává, protože se modul používá, restartujte relaci PowerShellu tak, že zavřete a znovu otevřete všechna okna.
- Podívejte se na verzi `Az.Resources` s `Get-Module Az.Resources -ListAvailable` .
- Pokud verze 4.1.1 není v seznamu dostupných, je nutné použít `Update-Module Az.Resources -Force` .
- Pokud chyba uvádí, že se `Az.Accounts` musí jednat o konkrétní verzi, aktualizujte také tento modul a nahraďte ho `Az.Resources` `Az.Accounts` . Pak musíte restartovat relaci PowerShellu.


## <a name="next-steps"></a>Další kroky

- [Správa předplatných a prostředků v rámci plánu Azure](azure-plan-manage.md)
