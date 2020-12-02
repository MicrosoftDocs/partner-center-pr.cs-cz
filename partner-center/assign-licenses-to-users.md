---
title: Správa uživatelů a uživatelských licencí pro zákaznické účty
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se spravovat uživatele pro vaše zákazníky v partnerském centru, jako je vytváření uživatelských účtů, přidávání nebo odebírání uživatelských licencí, Resetování uživatelských hesel a odstraňování nebo obnovování uživatelských účtů.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: fb7906b006540ef939e443a21855488e9d2c36f9
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/01/2020
ms.locfileid: "96474066"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a>Správa uživatelů a uživatelských licencí pro zákaznické účty

**Příslušné role**

- Globální správce
- Správce správy uživatelů
- Agent správce


Můžete vytvářet a odstraňovat nové uživatele v účtu zákazníka. Můžete také obnovit jeden nebo více uživatelských účtů, které jste dříve odstranili během 30 dnů od odstranění. Budou obnovena i předchozí přiřazení předplatného uživatele (za předpokladu, že jsou k dispozici jejich předchozí přidělení).

Když si koupíte nové předplatné pro zákazníka, zákazník by vám měl poskytnout seznam všech uživatelů, kteří budou potřebovat účty, jejich uživatelská oprávnění a to, které služby jednotliví uživatelé potřebují.  

[Odběry můžete přiřadit více uživatelům](bulk-license-provisioning-for-multiple-users.md) najednou pomocí importu názvů pomocí [souboru tabulky. csv kompatibilního s Excelem](adding-multiple-users-to-a-customer-account.md).

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>Vytvoření uživatelských účtů pro zákazníka

1. Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.

2. V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.

3. V nabídce zákazník vyberte **Uživatelé a licence**.

4. Pro každého uživatele, kterého přidáte, vyberte **Přidat předplatné** a pak vyplňte informace, včetně oprávnění a licencí. **Uložte** změny.

5. Nezapomeňte zaznamenat uživatelské jméno a dočasné heslo pro odeslání uživateli.

6. Pokud současně přidáváte více uživatelů, použijte **Přidat jiného uživatele**.

7. Můžete také přidat více uživatelů najednou [importováním souboru tabulky CSV kompatibilního s Excelem](adding-multiple-users-to-a-customer-account.md). Před odesláním e-mailu nebo tiskem názvů a hesel z potvrzovací obrazovky můžete počkat, dokud nedokončíte celou sadu.

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>Přidání nebo odebrání uživatelských licencí pro zákazníka

Následující postup platí pro přidání nebo odebrání uživatelských licencí pro produkty společnosti Microsoft. Pokud chcete přidat nebo odebrat uživatelské licence pro odběry SaaS založené na licencích na komerčním webu Marketplace, přečtěte si téma [Přidání nebo odebrání licencí pro předplatné SaaS](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).

1. Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.

2. V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.

3. V nabídce zákazník vyberte **Uživatelé a licence**.

4. Vyberte jednoho nebo více uživatelů ze seznamu. Pokud například zákazník právě koupil nové licence a chtěli jste jim přiřadit lidi, kteří je ještě nemají, můžete k vyhledání správné skupiny použít možnost **filtrovat uživatele podle..** ..

5. Vyberte **spravovat licence**. Proveďte změny a pak ho **uložte**.

> [!NOTE]
> U [Azure Marketplace produktů](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)se přiřazení licencí a aktivace spravují prostřednictvím nezávislého výrobce softwaru (ISV), který produkt zveřejnil.

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a>Resetování hesla uživatele pro zákazníka

1. Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.

2. V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.

3.  V nabídce zákazník vyberte **Uživatelé a licence**. Vyberte uživatele ze seznamu.

4.  V dolní části obrazovky vyberte **resetovat heslo**. 

5.  Poslat uživateli nové dočasné heslo.

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a>Odstranění uživatelských účtů pro zákazníka

1.  V nabídce **Partnerské centrum** vyberte **zákazníci**. Vyberte zákazníka ze seznamu.

2.  V nabídce zákazník vyberte **Uživatelé a licence**. Vyberte uživatele ze seznamu.

3.  V dolní části obrazovky vyberte **Odstranit uživatelský účet**.

Pokud potřebujete tento účet obnovit, můžete ho najít na kartě **odstraněné uživatele** v seznamu **Uživatelé a licence** zákazníka. K obnovení odstraněného uživatele máte 30 dní.

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a>Obnovení odstraněných uživatelských účtů

1.  V nabídce **Partnerské centrum** vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.

2.  Vyberte **Uživatelé a licence**.

3.  Vyberte kartu **odstraněné uživatele ()** . V případě odstranění uživatelů, které lze obnovit, by mělo být přečteno **(1)** nebo vyšší.

4.  Zaškrtněte jedno nebo více políček Odstraněná uživatelé a pak vyberte **obnovit**.

    Všechny vybrané uživatelské účty se znovu zobrazí na stránce **Uživatelé a licence** .

## <a name="related-topics"></a>Související témata


[Přiřazení licencí několika uživatelům nebo jejich odvolání](bulk-license-provisioning-for-multiple-users.md)

[Vytvoření více uživatelů pro účet zákazníka](adding-multiple-users-to-a-customer-account.md)