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
ms.openlocfilehash: 18cc5c62beaa76f6e3ade79f2f2069e0f2bd3c7e
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149600"
---
# <a name="manage-subscriptions-and-resources-under-the-azure-plan"></a>Správa předplatných a prostředků v rámci plánu Azure

**Příslušné role**: Agent správce


V tomto článku se dozvíte, jak partneři CSP můžou pomocí různých možností řízení přístupu na základě role (RBAC) získat provozní kontrolu a správu prostředků Azure zákazníka. Při převodu zákazníka na plán Azure vám standardně přiřadíte oprávnění správce v Azure (práva vlastníka předplatného prostřednictvím Správce jménem).

 > [!NOTE]
 > Oprávnění správce k předplatnému Azure může odebrat zákazník na základě předplatného, skupiny prostředků nebo úrovně zatížení. 

 Partneři můžou pomocí různých možností poskytovaných prostřednictvím funkce řízení přístupu na základě rolí (RBAC) získat nepřetržitou provozní kontrolu a správu prostředků Azure u zákazníka v CSP. 

- **Správce jménem (administrate)** – s [administrate](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO)bude mít každý uživatel s rolí agenta správce v partnerském tenantovi přístup k předplatným Azure, které vytvoříte prostřednictvím programu CSP.

- **Azure Lighthouse**: administrate neumožňuje flexibilitu vytvářet odlišné skupiny, které pracují s různými zákazníky, nebo pro skupiny nebo uživatele povolit různé role. Pomocí Azure Lighthouse můžete přiřadit různé skupiny různým zákazníkům nebo rolím. Vzhledem k tomu, že uživatelé budou mít odpovídající úroveň přístupu prostřednictvím delegované správy prostředků Azure, můžete snížit počet uživatelů, kteří mají roli agenta správce (a mít tak úplný přístup k ADMINISTRATE). To pomáhá zlepšovat zabezpečení tím, že omezuje zbytečný přístup k prostředkům vašich zákazníků. Nabízí také větší flexibilitu při správě více zákazníků ve velkém měřítku. Další informace najdete v tématu věnovaném nástroji [Azure Lighthouse a programu Cloud Solution Provider](/azure/lighthouse/concepts/cloud-solution-provider).

- Uživatelé adresáře nebo hosta nebo instanční objekty: Podrobný přístup k předplatným CSP můžete delegovat přidáním uživatelů do adresáře zákazníka nebo přidáním uživatelů typu host a přiřazením konkrétních rolí RBAC. **[](/azure/active-directory/develop/app-objects-and-service-principals)**

Microsoft doporučuje, aby uživatelé měli minimální oprávnění, která potřebují k provedení své práce, jako bezpečnostní postup. Viz [Azure Active Directory Privileged Identity Management zdroje informací.](/azure/active-directory/privileged-identity-management/pim-configure)

## <a name="link-your-partner-id-mpn-id-to-your-credentials-for-managing-customers-azure-resources"></a>Propojení ID partnera (MPN ID) s přihlašovacími údaji pro správu prostředků Azure zákazníka

Následující tabulka uvádí metody používané k přidružení ID partnera k různým možnostem přístupu RBAC.

|**Kategorie**   |**Scénář**   |**Přidružení ID MPN**|
|-----------------|:------------------------|:------------------|
|Aobo   |Přímý partner nebo nepřímý poskytovatel CSP vytvoří předplatné pro zákazníka, aby se přímý partner CSP nebo nepřímý poskytovatel vlastníkem předplatného pomocí funkce AOBO. Přímý partner nebo nepřímý poskytovatel CSP poskytují nepřímým prodejcům přístup k předplatnému pomocí AOBO.|Automatické (nevyžaduje se žádná práce partnera)|
|Azure Lighthouse|Partner vytvoří novou [nabídku spravovaných služeb na Marketplace.](/azure/lighthouse/concepts/managed-services-offers) Tato nabídka je přijata pro předplatné CSP a partner získá přístup k předplatnému CSP.|Automatické (nevyžaduje se žádná práce partnera)|
|Azure Lighthouse|Partner nasazovat [šablonu ARM](/azure/lighthouse/how-to/onboard-customer) v předplatném Azure|Partner musí přidružit ID MPN k uživateli nebo instančnímu objektu v partnerském tenantovi. Další informace najdete v [tématu Partnerské ID](/azure/billing/billing-partner-admin-link-started).|
|Uživatel adresáře nebo hosta|Partner vytvoří nového uživatele nebo instanční objekt v adresáři zákazníka a poskytne uživateli přístup k předplatnému CSP. Partner vytvoří nového uživatele nebo instanční objekt v adresáři zákazníka. Partner přidá uživatele do skupiny a poskytne této skupině přístup k předplatnému CSP.|Partner musí přidružit ID MPN k uživateli nebo instančnímu objektu v tenantovi zákazníka. Další informace najdete v [odkazu s ID partnera](/azure/billing/billing-partner-admin-link-started).|

## <a name="confirm-that-you-have-admin-access"></a>Potvrďte, že máte přístup správce.

Pro správu služeb zákazníka a přijímání realizovaných kreditů vyžadujete přístup správce. Přečtěte si [kredity získané partnerem](partner-earned-credit.md) , kde najdete podrobné informace o získaných kreditech. Máte dva způsoby, jak se ujistit, že máte oprávnění správce.

- Projděte si soubor denního využití – můžete ho určit tak, že zkontrolujete cenu za jednotku a platnou jednotkovou cenu v souboru denního využití a potvrdíte, jestli se sleva uplatňuje. Pokud obdržíte slevu, kterou jste správcem.

- Vytvoření upozornění na Azure monitor – můžete vytvořit [Upozornění](/azure/azure-monitor/platform/alerts-activity-log) protokolu aktivit Azure monitor, abyste byli informováni o tom, kdy se přístup k RBAC odebere z předplatného CSP.

### <a name="create-an-azure-monitor-alert"></a>Vytvoření výstrahy Azure monitoru

1. Vytvořit výstrahu.

   :::image type="content" source="images/azure/azurealert1.png" alt-text="Výstraha Azure":::

2. Vyberte typ akce, kterou má výstraha provést. Pokud například zadáte, že chcete e-mailem, obdržíte e-mail s upozorněním, pokud dojde k odstranění přiřazení role.

   :::image type="content" source="images/azure/azureconfigurealert2.png" alt-text="konfigurovat výstrahu":::

### <a name="aobo-removal"></a>Odebrání ADMINISTRATE

Zákazníci mohou spravovat přístup ke svým předplatným, a to tak, že v Azure Portal **Access Control** . Na kartě **přiřazení rolí** vyberte možnost **Odebrat přístup**. Pokud k tomu dojde, můžete:

- Poraďte se se zákazníkem a zjistěte, jestli je možné obnovit přístup správce.

- Použijte přístup poskytnutý prostřednictvím [řízení přístupu na základě role (RBAC)](/azure/role-based-access-control/overview).

- Použijte přístup poskytovaný prostřednictvím [Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/).

Přístup na základě role se liší od přístupu správce. Role omezte přesně to, co můžete a nemůžete dělat. Přístup správce je širší.

Pokud chcete zobrazit role, které mají nárok na získání kreditu PEC, přečtěte si informace o rolích a [oprávněních pro kredit získaný partnerem.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2)

## <a name="next-steps"></a>Další kroky

- [Odvolání a obnovení oprávnění správce pro Azure CSP předplatná](revoke-reinstate-csp.md)

- [Kredit získaný partnerem – přehled](partner-earned-credit.md)

- [Kredit získaný partnerem za spravované služby](partner-earned-credit-explanation.md)