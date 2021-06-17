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
ms.openlocfilehash: 81df7578f7f15def64a3c20b15f95f3b89a28d1c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277772"
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

3. Vyberte zákazníka, se nímž **pracujete, a požádejte o vztah prodejce.** Tato akce vygeneruje odkaz na zákazníka, který má oprávnění správce tenanta.

4. Zákazník musí odkaz vybrat a schválit žádost o vztah prodejce.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Příklad e-mailu s vytvořením vztahu prodejce":::

5. Vy, partner, se musíte připojit k partnerskému tenantovi, abyste měli ID objektu skupiny AdminAgents.
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. Zákazník pak musí provést následující kroky pomocí PowerShellu nebo Azure CLI. Váš zákazník musí mít:

- Role **vlastníka nebo** **správce uživatelských přístupů** 
- Oprávnění k vytváření přiřazení rolí na úrovni předplatného

   a. Pouze pro PowerShell musí zákazník aktualizovat `Az.Resources` modul.
   ```powershell
   Update-Module Az.Resources
   ```

   b. Zákazník se připojí k tenantovi, ve kterém je předplatné CSP.
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   c. Zákazník se připojí k předplatnému. To platí *jenom v* případě, že má uživatel oprávnění k přiřazení role pro více předplatných v tenantovi.

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

Místo udělení oprávnění vlastníka v oboru předplatného můžete oprávnění udělit na úrovni skupiny prostředků nebo prostředku. 

- Na úrovni skupiny prostředků

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- Na úrovni prostředku

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

Pokud výše uvedený postup nefunguje nebo když se o ně pokusíte, zkuste obnovit práva správce zákazníka pomocí následujícího postupu "catch-all".

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a>Řešení potíží

Pokud se zákazníkovi nedaří dokončit krok 6 výše, zkuste použít následující příkaz:

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

Poskytněte `newRoleAssignment.log` microsoftu výsledný soubor k další analýze.

Pokud se během operace nezdaří procedura "catch-all", `Import-Module` zkuste následující kroky:
- Pokud import selže, protože se modul používá, restartujte relaci PowerShellu tak, že zavřete a znovu otevřete všechna okna.
- Zkontrolujte verzi nástroje `Az.Resources` pomocí `Get-Module Az.Resources -ListAvailable` .
- Pokud verze 4.1.1 není v seznamu dostupných verzí, musíte použít `Update-Module Az.Resources -Force` .
- Pokud chyba uvádí, že musí být konkrétní verze, aktualizujte také tento `Az.Accounts` modul a nahraďte `Az.Resources` za `Az.Accounts` . Pak musíte restartovat relaci PowerShellu.


## <a name="next-steps"></a>Další kroky

- [Správa předplatných a prostředků v rámci plánu Azure](azure-plan-manage.md)
