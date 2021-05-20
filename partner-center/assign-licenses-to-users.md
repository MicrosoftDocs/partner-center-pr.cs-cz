---
title: Správa uživatelů pro zákaznické účty
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Správa uživatelů pro zákazníky v Partnerské centrum – vytváření uživatelských účtů, přidávání nebo odebírání uživatelských licencí, resetování hesel a odstraňování nebo obnovení uživatelských účtů.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc896ec3ce16ab0f05a8131de14f573ad96a8141
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149889"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a>Správa uživatelů a uživatelských licencí pro zákaznické účty 

**Odpovídající role:** Globální správce | Správce správy uživatelů | Agent pro správu


V účtu zákazníka můžete vytvářet a odstraňovat nové uživatele. Můžete také obnovit jeden nebo více uživatelských účtů, které jste předtím odstranili do 30 dnů od odstranění. Obnoví se také předchozí přiřazení předplatného uživatele (za předpokladu, že jsou k dispozici jeho předchozí přidělení).

Když zákazníkovi zakoupíte nová předplatná, měl by vám poskytnout seznam všech uživatelů, kteří budou potřebovat účty, jejich uživatelská oprávnění a služby, které každý uživatel potřebuje.  

>[!NOTE]
>V **části** Uživatelé a  licence na kartě Zákazník se zobrazují všichni uživatelé vytvoření v tenantovi konkrétního zákazníka, včetně uživatelů, kteří mají licence zakoupené od jiného partnera CSP nebo z jiného nákupního kanálu.

Odběry [můžete přiřadit více uživatelům](bulk-license-provisioning-for-multiple-users.md) najednou importem názvů pomocí souboru tabulky CSV [kompatibilního s Excelem.](adding-multiple-users-to-a-customer-account.md)

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>Vytvoření uživatelských účtů pro zákazníka

1. Přihlaste se k Partnerské centrum [řídicího panelu.](https://partner.microsoft.com/dashboard)

2. V Partnerské centrum vyberte **Zákazníci** a pak v seznamu zvolte zákazníka.

3. V nabídce zákazníka vyberte **Uživatelé a licence.**

4. Pro každého uživatele, který přidáte, vyberte **Přidat předplatné** a vyplňte informace, včetně oprávnění a licencí. **Uložte** změny.

5. Nezapomeňte si zaznamenat uživatelské jméno a dočasné heslo, které chcete uživateli odeslat.

6. Pokud přidáváte více uživatelů po jednom, použijte **možnost Přidat dalšího uživatele**.

7. Můžete také přidat více uživatelů najednou importem souboru tabulky .csv kompatibilního [s Excelem.](adding-multiple-users-to-a-customer-account.md) Před odesláním e-mailu nebo tisku jmen a hesel z potvrzovací obrazovky můžete počkat, až s celou sadu skončíte.

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>Přiřazení nebo odebrání uživatelských licencí zákazníkovi

Následující postup se týká přidávání nebo odebírání uživatelských licencí pro produkty Microsoftu. Pokud chcete přidat nebo odebrat uživatelské licence pro předplatná SaaS založená na licencích na komerčním marketplace, podívejte se na stránku Přidání nebo odebrání licencí [pro předplatné SaaS.](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)

1. Přihlaste se k Partnerské centrum [řídicího panelu.](https://partner.microsoft.com/dashboard)

2. V Partnerské centrum vyberte **Zákazníci** a pak v seznamu zvolte zákazníka.

3. V nabídce zákazníka vyberte **Uživatelé a licence.**

4. Vyberte v seznamu alespoň jednoho uživatele. Pokud například zákazník právě zakoupil nové licence a vy jste je chtěli přiřadit lidem, kteří je  ještě nemají, můžete najít správnou skupinu pomocí možnosti Filtrovat uživatele podle.

5. Vyberte **Spravovat licence**. Proveďte změny a pak **klikněte na Uložit.**

> [!NOTE]
> U [Azure Marketplace se](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)přiřazení licencí a aktivace spravují prostřednictvím nezávislého výrobce softwaru (ISV), který produkt publikoval.

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a>Resetování hesla uživatele pro zákazníka

1. Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard) pro Partnerské centrum.

2. V Partnerské centrum vyberte **Zákazníci** a pak v seznamu zvolte zákazníka.

3. V nabídce zákazníka vyberte **Uživatelé a licence.** Vyberte uživatele ze seznamu.

4. V dolní části obrazovky vyberte **Resetovat heslo.** 

5. Odešlete nové dočasné heslo uživateli.

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a>Odstranění uživatelských účtů pro zákazníka

1. V **nabídce Partnerské centrum** vyberte **Zákazníci.** V seznamu vyberte zákazníka.

2. V nabídce zákazníka vyberte **Uživatelé a licence.** Vyberte uživatele ze seznamu.

3. V dolní části obrazovky vyberte **Odstranit uživatelský účet**.

Pokud potřebujete tento účet obnovit, najdete ho  v seznamu Uživatelé a licence zákazníka na **kartě Odstranění** uživatelé. K obnovení odstraněného uživatele máte 30 dní.

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a>Obnovení odstraněných uživatelských účtů

1. V nabídce **Partnerské centrum** vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.

2. Vyberte **Uživatelé a licence**.

3. Vyberte kartu **odstraněné uživatele ()** . V případě odstranění uživatelů, které lze obnovit, by mělo být přečteno **(1)** nebo vyšší.

4. Zaškrtněte jedno nebo více políček Odstraněná uživatelé a pak vyberte **obnovit**.

    Všechny vybrané uživatelské účty se znovu zobrazí na stránce **Uživatelé a licence** .

## <a name="next-steps"></a>Další kroky

- [Přiřazení licencí několika uživatelům nebo jejich odvolání](bulk-license-provisioning-for-multiple-users.md)

- [Vytvoření více uživatelů pro účet zákazníka](adding-multiple-users-to-a-customer-account.md)