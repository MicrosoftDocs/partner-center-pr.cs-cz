---
title: Registrace do programu CSP
titleSuffix: Microsoft Cloud for US Government - Partner Center
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Seznamte se s požadavky na program CSP pro partnery, kteří se chtějí zaregistrovat do Cloud Solution Provider programu pro Microsoft Cloud for US Government.
author: mowrim
ms.author: mowrim
ms.localizationpriority: medium
ms.custom: SEOJUNE.20
ms.date: 10/05/2020
ms.openlocfilehash: e2b206b049050efa520099d74230d8535ac93793
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147169"
---
# <a name="enroll-in-the-cloud-solution-provider-program-for-microsoft-cloud-for-us-government"></a>Registrace do Cloud Solution Provider pro Microsoft Cloud for US Government

**Platí pro:** Partnerské centrum pro Microsoft Cloud for US Government

**Odpovídající role:** Globální správce

Partneři Microsoftu teď dají cloudová řešení a služby Microsoftu americkým federálním, státním, místním a kmenovým entitám prostřednictvím Cloud Solution Provider programu (CSP) pro Microsoft Cloud for US Government.

Microsoft Cloud for US Government poskytuje privátní, vyhrazenou a izolovanou instanci služby Microsoft Azure která splňuje požadavky státní správy USA na zabezpečení dat, ochranu osobních údajů a dodržování předpisů. Aby se vaše společnost mohli programu CSP zapojit do programu CSP, musí splňovat podmínky Microsoft Cloud for US Government. Další informace najdete v tématu [Partnerské centrum pro Microsoft Cloud for US Government](partner-center-for-microsoft-us-govt-cloud.md).

## <a name="before-you-begin"></a>Než začnete

Než se budete moci zaregistrovat do programu CSP pro Microsoft Cloud for US Government, musíme ověřit, že vaše společnost splňuje požadavky na prodej organizacím státní správy USA. Před zahájením procesu registrace vyplňte formulář pro ověření cloudu [Microsoft Government,](https://azuregov.microsoft.com/csp) abychom mohli ověřit způsobilost vaší společnosti. Po ověření způsobilosti vaší společnosti vám poskytneme tenanta azure Azure Active Directory (Azure AD) specifického pro Microsoft Cloud for US Government.  

Pokud chcete vytvořit Partnerské centrum účet a zaregistrovat se v CSP pro Microsoft Cloud for US Government, budete muset zadat následující informace (tyto informace možná budete chtít před zahájením procesu registrace shromáždit):

- Přihlašovací údaje globálního správce pro nového tenanta Azure AD vaší organizace pro Microsoft Cloud for US Government
- ID účtu Microsoft Partner Network (MPN)
- Obchodní adresa v USA

> [!IMPORTANT]  
> Pokud máte v partnerském centru existující účet a chcete se zaregistrovat do CSP pro Microsoft Cloud pro státní správu USA, musíte pro státní správu USA vytvořit nový samostatný účet zvlášť.

## <a name="how-to-enroll"></a>Jak se zaregistrovat

### <a name="step-1---create-a-partner-center-account-for-microsoft-cloud-for-us-government"></a>Krok 1 – Vytvoření účtu partnerského centra pro Microsoft Cloud pro státní správu USA

1. [Sem zahájíte](https://partnercenter.microsoft.com/register/resellerusgjoinnow)proces registrace.

2. Přihlaste se pomocí přihlašovacích údajů globálního správce pro tenanta Azure AD vaší organizace pro Microsoft Cloud pro státní správu USA. Pokud vaše organizace nemá účet pro tento portál, můžete si ho vyžádat vyplněním [formuláře pro ověření cloudu pro státní správu Microsoftu](https://azuregov.microsoft.com/csp).

### <a name="step-2---apply-to-participate-in-the-cloud-solution-provider-program-for-microsoft-cloud-for-us-government"></a>Krok 2 – platí pro účast v programu Cloud Solution Provider pro Microsoft Cloud pro státní správu USA

1. Do formuláře pro zápis zadejte všechny chybějící informace, včetně ID Microsoft Partner Network a podrobností o podpoře zákazníků vaší organizace.

2. Vyberte **přijmout a pokračovat**. Kontrola vaší aplikace může trvat několik dní. Až tuto kontrolu dokončíte, pošleme vám e-mail.

   > [!IMPORTANT]
   > Když vyberete **přijmout a pokračovat**, potvrzujete, že jste oprávněni jednat jménem vaší organizace, a souhlasíte s tím, že umožníte, aby Microsoft spouštěl kontrolu kreditů na pozadí před kontrolou aplikace poskytovatele Cloud Solution Provider vaší organizace.

### <a name="step-3---sign-the-reseller-agreement-for-microsoft-cloud-for-us-government"></a>Krok 3 – podepsání smlouvy o prodejci pro Microsoft Cloud pro státní správu USA

1. Přihlaste se k partnerskému centru pro Microsoft Cloud pro státní správu USA pomocí odkazu uvedeného v e-mailu pro schválení aplikace.

2. Na stránce **smlouva** si přečtěte podmínky a pokud souhlasíte, vyberte **přijmout a pokračovat** , pokud chcete Microsoft Cloud pro státní správu USA digitálně podepsat smlouvu o prodejci. Vytvoření účtu může trvat několik hodin. Z partnerského centra se můžete odhlásit Microsoft Cloud pro státní správu USA a pak se znovu přihlásit později.

### <a name="step-4---assign-users-to-the-admin-agent-role-in-the-microsoft-azure-admin-portal-for-microsoft-cloud-for-us-government"></a>Krok 4: přiřazení uživatelů k roli agenta správce na portálu pro správu Microsoft Azure pro Microsoft Cloud pro státní správu USA

Microsoft Cloud for US Government poskytuje samostatnou instanci služby Microsoft Azure která splňuje standardy dodržování předpisů, zabezpečení a ochrany osobních údajů ze státní správy. Pokud chcete správcům povolit správu uživatelů a licencí v portál Microsoft Azure, musíte jim ručně přiřadit roli Agent pro správu.

> [!NOTE]
> Jakmile přiřadíte uživatele k roli Agent pro správu, budou mít  přístup k vašemu seznamu zákazníků na stránce Zákazníci a [přidávají nové zákazníky.](add-a-new-customer.md)

1. Přihlaste se k portálu Microsoft Azure na adrese [https://portal.azure.us/](https://portal.azure.us/) .

2. Přiřaďte roli Agent pro správu příslušným uživatelům ve vaší organizaci. K tomu je potřeba přidat tyto uživatele do integrované skupiny **AdminAgent.** Informace [o tom, jak to provést, Azure Active Directory](/azure/active-directory/active-directory-groups-members-azure-portal) v tématu Správa členů skupiny v systému .

## <a name="connect-with-us"></a>Spojte se s námi.

- Máte otázky? Pošlete nám e-mail na adresu . azgovcsp@microsoft.com

- Připojte se k nám [v Yammeru.](https://www.yammer.com/cloudpartnercommunity/#/threads/inGroup?type=in_group&feedId=11509777)

## <a name="next-steps"></a>Další kroky

- [Partnerské centrum pro Microsoft Cloud for US Government](partner-center-for-microsoft-us-govt-cloud.md)

- [Správa uživatelů a licencí v Partnerské centrum pro Microsoft Cloud for US Government](user-management-in-partner-center-for-microsoft-us-govt-cloud.md)