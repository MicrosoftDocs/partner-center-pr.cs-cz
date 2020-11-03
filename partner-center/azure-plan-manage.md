---
title: Plán Azure – Správa předplatných & prostředky
ms.topic: article
ms.date: 05/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si, jak můžou partneři používat různé možnosti řízení přístupu na základě role (RBAC), abyste získali provozní kontrolu a správu prostředků Azure zákazníka.
author: amitravat
ms.author: amrava
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 4bbeb417fdc5964d66f754a789873c1dbc8b1d25
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/22/2020
ms.locfileid: "92527596"
---
# <a name="manage-subscriptions-and-resources-under-the-azure-plan"></a>Správa předplatných a prostředků v rámci plánu Azure

Při převodu zákazníka na plán Azure vám standardně přiřadíte oprávnění správce v Azure (práva vlastníka předplatného prostřednictvím Správce jménem).

 > [!NOTE]
 > Oprávnění správce k předplatnému Azure může odebrat zákazník na základě předplatného, skupiny prostředků nebo úrovně zatížení. 

 Partneři můžou pomocí různých možností poskytovaných prostřednictvím funkce řízení přístupu na základě rolí (RBAC) získat nepřetržitou provozní kontrolu a správu prostředků Azure u zákazníka v CSP. 

- **Správce jménem (administrate)** – s [administrate](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO)bude mít každý uživatel s rolí agenta správce v partnerském tenantovi přístup k předplatným Azure, které vytvoříte prostřednictvím programu CSP.

- **Azure Lighthouse** : administrate neumožňuje flexibilitu vytvářet odlišné skupiny, které pracují s různými zákazníky, nebo pro skupiny nebo uživatele povolit různé role. Pomocí Azure Lighthouse můžete přiřadit různé skupiny různým zákazníkům nebo rolím. Vzhledem k tomu, že uživatelé budou mít odpovídající úroveň přístupu prostřednictvím delegované správy prostředků Azure, můžete snížit počet uživatelů, kteří mají roli agenta správce (a mít tak úplný přístup k ADMINISTRATE). To pomáhá zlepšovat zabezpečení tím, že omezuje zbytečný přístup k prostředkům vašich zákazníků. Nabízí také větší flexibilitu při správě více zákazníků ve velkém měřítku. Další informace najdete v tématu věnovaném nástroji [Azure Lighthouse a programu Cloud Solution Provider](/azure/lighthouse/concepts/cloud-solution-provider).

-  **Uživatelé adresáře nebo hostů nebo [instanční objekty](/azure/active-directory/develop/app-objects-and-service-principals)** : podrobnější přístup k předplatným CSP můžete delegovat přidáním uživatelů v adresáři zákazníka nebo přidáním uživatelů typu Host a přiřazením konkrétních rolí RBAC.

Microsoft doporučuje, aby uživatelé měli minimální oprávnění, která potřebují k tomu, aby pracovali jako bezpečnostní postupy. Viz [Azure Active Directory Privileged Identity Management prostředky](/azure/active-directory/privileged-identity-management/pim-configure).

## <a name="link-your-partner-id-mpn-idto-your-credentials-for-managing-customers-azure-resources"></a>Propojit ID partnera (MPN ID) s přihlašovacími údaji pro správu prostředků Azure zákazníka

Následující tabulka uvádí metody použité k přidružení ID partnera k různým možnostem přístupu RBAC.

|**Kategorie**   |**Scénář**   |**Přidružení ID MPN**|
|-----------------|:------------------------|:------------------|
|ADMINISTRATE   |Přímý partner CSP nebo nepřímý poskytovatel vytvoří předplatné pro zákazníka, kterému je výchozí vlastník poskytovatele CSP nebo nepřímý poskytovatel, který používá ADMINISTRATE.; Přímý partner CSP nebo nepřímý poskytovatel poskytují nepřímým prodejcům přístup k předplatnému pomocí ADMINISTRATE.|Automaticky (nevyžaduje se žádná práce v partnerovi)|
|Azure Lighthouse|Partner vytvoří novou [nabídku spravované služby na webu Marketplace](/azure/lighthouse/concepts/managed-services-offers). Tato nabídka je přijatá na předplatném CSP a partner získá přístup k předplatnému CSP.|Automaticky (nevyžaduje se žádná práce v partnerovi)|
|Azure Lighthouse|[Šablona ARM](/azure/lighthouse/how-to/onboard-customer) nasazení partnera v předplatném Azure|Partner musí přidružit ID MPN k uživatelskému nebo instančnímu objektu v partnerském tenantovi. Další informace najdete v [odkazu s ID partnera](/azure/billing/billing-partner-admin-link-started).|
|Adresář nebo uživatel typu Host|Partner vytvoří nového uživatele nebo instanční objekt v adresáři zákazníka a poskytne uživateli přístup k předplatnému CSP. Partner vytvoří nového uživatele nebo instanční objekt v adresáři zákazníka. Partner přidá uživatele do skupiny a poskytne skupině přístup k předplatnému CSP.|Partner musí přidružit ID MPN k uživatelskému nebo instančnímu objektu v tenantovi zákazníka. Další informace najdete v [odkazu s ID partnera](/azure/billing/billing-partner-admin-link-started).|

## <a name="confirm-that-you-have-admin-access"></a>Potvrďte, že máte přístup správce.

Pro správu služeb zákazníka a přijímání realizovaných kreditů vyžadujete přístup správce. Přečtěte si [kredity získané partnerem](partner-earned-credit.md) , kde najdete podrobné informace o získaných kreditech. Máte dva způsoby, jak se ujistit, že máte oprávnění správce.

- Projděte si soubor denního využití – můžete ho určit tak, že zkontrolujete cenu za jednotku a platnou jednotkovou cenu v souboru denního využití a potvrdíte, jestli se sleva uplatňuje. Pokud obdržíte slevu, kterou jste správcem.

- Vytvoření upozornění na Azure monitor – můžete vytvořit [Upozornění](/azure/azure-monitor/platform/alerts-activity-log) protokolu aktivit Azure monitor, abyste byli informováni o tom, kdy se přístup k RBAC odebere z předplatného CSP.

### <a name="create-an-azure-monitor-alert"></a>Vytvoření výstrahy Azure monitoru

1. Vytvořit výstrahu.

   :::image type="content" source="images/azure/azurealert1.png" alt-text="Výstraha Azure":::

2. Vyberte typ akce, kterou má výstraha provést. Pokud například zadáte, že chcete e-mailem, obdržíte e-mail s upozorněním, pokud dojde k odstranění přiřazení role.

   :::image type="content" source="images/azure/azureconfigurealert2.png" alt-text="Výstraha Azure":::

### <a name="aobo-removal"></a>Odebrání ADMINISTRATE

Zákazníci mohou spravovat přístup ke svým předplatným, a to tak, že v Azure Portal **Access Control** . Na kartě **přiřazení rolí** vyberte možnost **Odebrat přístup** . Pokud k tomu dojde, můžete:

- Poraďte se se zákazníkem a zjistěte, jestli je možné obnovit přístup správce.

- Použijte přístup poskytnutý prostřednictvím [řízení přístupu na základě role (RBAC)](/azure/role-based-access-control/overview).

- Použijte přístup k poskytovanému prostřednictvím [Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/).

Přístup založený na rolích se liší od přístupu správce. Role přesně vymezují, co můžete a nemůžete dělat. Přístup správce je širší.

Chcete-li zobrazit role, které mají nárok na získání řadiče PEC, přečtěte si [role a oprávnění pro daný kredit pro partnery](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2).

## <a name="next-steps"></a>Další kroky

- [Odvolání a odvolání oprávnění správce pro předplatná Azure CSP](revoke-reinstate-csp.md)

- [Získaný kredit partnerů – přehled](partner-earned-credit.md)

- [Získaný kredit partnerů pro spravované služby](partner-earned-credit-explanation.md)