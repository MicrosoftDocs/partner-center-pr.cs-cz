---
title: Nákup nabídek pro komerční web Marketplace
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si, jak partneři programu CSP můžou použít tržiště partnerského centra k nákupu SaaS nabídek od nezávislých dodavatelů softwaru (ISV).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3f5cf4895fa4d66c65215989d808a1dd18ef9064
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147849"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>Nákup produktů z komerčního tržiště pro vaše zákazníky v partnerském centru


**Příslušné role**: globální správce | Agent správce

Jako partner v programu Cloud Solution Provider (CSP) můžete pomocí komerčního tržiště koupit předplatné pro zákazníky na určité produkty SaaS (software jako služba), které nabízí nezávislí dodavatelé softwaru (ISV).

Díky nabídce předplatným ISV SaaS vašim zákazníkům můžete lépe odlišit své podnikání. Zákazníkům můžete také poskytnout přístup k softwarovým balíčkům, které řeší jejich konkrétní obchodní potřeby. Licence a odběry pro tyto produkty SaaS z webu Marketplace od vydavatelů ISV můžete spravovat stejným způsobem jako vy při správě licencí a předplatných pro produkty Microsoftu.

Můžete si koupit buď odběry SaaS **založené na licencích** , nebo předplatné **založené na využití** . Další informace o rozdílu mezi účtováním na základě licencí a na základě využití najdete v tématu [základy fakturace](billing-basics.md).

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a>Nákup SaaS předplatných na základě licencí a vyměřených předplatných v partnerském centru

Zakoupíte si předplatné pro produkty založené na licenci nebo SaaS, které nabízí vydavatelé ISV, pomocí stejného procesu, který používáte k nákupu předplatných pro produkty Microsoftu.

Pokud si chcete koupit předplatné SaaS na základě licence nebo účtované podle objemu dat v partnerském centru, přečtěte si téma [Vytvoření, pozastavení nebo zrušení zákaznických předplatných](create-a-new-subscription.md#create-a-new-subscription).

[Rozhraní API partnerského centra](/partner-center/develop/) můžete použít také k vytváření předplatných komerčního tržiště pro vaše zákazníky. (Další informace o používání rozhraní API partnerského centra najdete v tématu [Vytvoření odběru pro produkty z komerčního tržiště](/partner-center/develop/create-subscription-azure-marketplace-products).)

>[!IMPORTANT]
> Jako partner v programu CSP si můžete koupit předplatné SaaS **založené na licencích** nebo **účtované podle objemu** od vydavatelů ISV v partnerském centru. To znamená, že si můžete zakoupit jakoukoli **nabídku** **SaaS** založenou na [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) licencích nebo na základě měření, kterou vám vydavatel ISV nabízí, včetně výhradních nabídek, ke kterým máte přístup. Pokud chcete nakupovat nebo spravovat jiné nabídky na komerčním marketplace od isv (například nabídky založené na využití zahrnující aplikace Azure, kontejnery nebo virtuální počítače), musíte přejít na [web Azure Portal](https://portal.azure.com/).

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a>Nákup předplatných založených na využití v Azure Portal

Na rozdíl od předplatných SaaS založených na licencích od vydavatelů ISV třetích stran vyžadují předplatná založená na využití nejprve od zákazníka předplatné Azure. Fakturace za komerční marketplace spadá prostředky na základě využití do předplatného Azure zákazníka. Jakmile má zákazník předplatné Azure, partner v programu CSP může podle těchto kroků zakoupit předplatné komerčního marketplace:

1. Přihlaste se Partnerské centrum [řídicího panelu a](https://partner.microsoft.com/dashboard) **pak** v nabídce vlevo vyberte Zákazníci.

2. Vyberte konkrétního zákazníka a pak vyberte **Předplatná.**  

3. V části **Předplatná založená na využití** vyberte **Všechny prostředky**. Tím se dostat na portál pro správu Azure.

4. Na portálu pro správu Azure **v** nabídce vlevo vyberte Vytvořit prostředek.

5. V **horní části** seznamu Azure Marketplace zobrazit vše.

6. Pokud chcete seznam zúžit, použijte filtry v horní části seznamu Marketplace. Můžete například vybrat **Microsoft**  nebo Partnera  z rozevíracího seznamu Vydavatel a zobrazit pouze nabídky od Microsoftu nebo nabídky od vydavatele ISV.

7. Zvolte konkrétní nabídku a pak vyberte **Vytvořit.**

## <a name="next-steps"></a>Další kroky

- [Správa nabídek komerčního marketplace](csp-commercial-marketplace-purchase.md)