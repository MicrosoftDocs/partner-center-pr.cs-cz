---
title: Azure Cost Management by Cloudyn pro poskytovatele CSP
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se, jak zaregistrovat webovou aplikaci v Cloudyn a používat pro ni tajný klíč v partnerském centru, abyste mohli používat aplikaci ke sledování zákaznických využití a nákladů.
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: defa691a3bc70cbda45f01cb447d89364a49e3b8
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534980"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a>Sledování využití a nákladů zákazníků Azure pomocí aplikace Azure cost management pro partnery CSP  

**Příslušné role**

- Globální správce
- Agent správce

[Získat další informace o Azure Cost Management](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>Než začnete
Než budete moci použít Azure Cost Management, ujistěte se, že splňujete následující požadavky:

- Jste partnerem v programu Cloud Solution Provider.
- Máte možnost vytvořit webovou aplikaci rozhraní API partnerského centra.

## <a name="overview"></a>Přehled

Cloudyn je webová aplikace, která umožňuje sledovat a spravovat, kolik zákazníků využívá Azure, a náklady na toto využití. Použijete ji prostřednictvím rozhraní API partnerského centra.

## <a name="register-your-web-app-in-the-partner-center"></a>Registrace webové aplikace v partnerském centru
Když zaregistrujete Azure Active Directory webovou aplikaci v partnerském centru, povolíte přístup k rozhraní API partnerského centra. 
1.  Přihlaste se k [partnerskému centru](https://partnercenter.microsoft.com/pcv/dashboard/overview) pomocí [účtu globálního správce nebo agenta správce](create-user-accounts-and-set-permissions.md).
2.  Z **partnerského centra** vyberte **Nastavení účtu** &gt; **[Správa aplikací](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.
3.  V části **Webová aplikace** klikněte na **Přidat novou webovou aplikaci**.
<br> **Poznámka**: Pokud jste dříve vytvořili webovou aplikaci, můžete přeskočit krok 3.
4.  Zkopírujte a uložte GUID **ID pro Commerce ID** a identifikátor GUID **ID aplikace** pro vaši webovou aplikaci. K používání 30denní bezplatné zkušební verze aplikace Azure cost management budete potřebovat obě ID.

## <a name="add-a-secret-key-to-your-app"></a>Přidání tajného klíče do aplikace
1. V rozevíracím seznamu vedle tlačítka **Přidat klíč** vyberte dobu trvání 1 nebo 2 roky.
2. Klikněte na **Přidat klíč**. 
3. Zkopírujte a uložte hodnotu tajného klíče. Budete ho potřebovat pro 30denní bezplatnou zkušební verzi.<br>
   > [!NOTE]  
   > Tajné klíče aplikace jako hesla mají delší datum vypršení platnosti. Uložte prosím hodnotu klíče do zabezpečeného umístění pro budoucí použití.

## <a name="next-steps"></a>Další kroky
Spusťte [30denní bezplatnou zkušební verzi](https://go.microsoft.com/fwlink/?linkid=857895).
Ke spuštění zkušební verze potřebujete následující podrobnosti:
- Přihlašovací údaje pro přihlašovací údaje partnerského centra
- Identifikátor GUID ID obchodu
- Identifikátor GUID ID aplikace
- Hodnota tajného klíče aplikace
