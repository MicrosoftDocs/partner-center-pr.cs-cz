---
title: Správa produktů z marketplace & nabídek
ms.topic: how-to
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Pomocí Partnerské centrum zjistěte, jak mohou poskytovatelé Cloud Solution Providers spravovat nabídky isv třetích stran zakoupené pro zákazníky z komerčního marketplace.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e1bb2752dad5325478496c83fc368943780d8afb
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147900"
---
# <a name="manage-commercial-marketplace-products-and-offers-for-your-customers"></a>Správa produktů a nabídek komerčního marketplace pro vaše zákazníky


**Odpovídající role:** Globální správce | Agent pro správu

Partneři v programu Cloud Solution Provider (CSP) mohou pomocí portálu Partnerské centrum nakupovat řadu nabídek SAAS nebo předplatných ISV pro své zákazníky z komerčního marketplace. Po zakoupení nabídky můžete nabídku spravovat různými způsoby.

## <a name="view-or-edit-a-subscription"></a>Zobrazení nebo úprava předplatného

Po zakoupení předplatného od vydavatele isv jiného výrobce softwaru ho můžete zkontrolovat nebo upravit následujícím způsobem:

1. Přihlaste se k Partnerské centrum [a](https://partner.microsoft.com/dashboard) **pak** v levé navigační nabídce vyberte Zákazníci.

2. Vyberte příslušného zákazníka a pak vyberte **Předplatná.** Zobrazí se seznam všech předplatných založených na licencích, která jste pro zákazníka zakoupili.

3. Ve **sloupci Předplatné** vyberte předplatné, které chcete zobrazit nebo upravit. Získáte tak další informace o nastavení nebo zřízení nabídky. (Pokud je u nabídky potřeba provést další akci, může se také ve sloupci Stav zobrazit stav "Action Needed" (Potřebná akce). To může být také doplněno odkazem na web vydavatele ISV.)

4. Po výběru předplatného, které chcete zobrazit nebo upravit, vám stránka s podrobnostmi o předplatném umožní upravit předplatné a dělat věci jako:

    - Změna přezdívky předplatného

    - Přidání nebo snížení počtu licencí v předplatném

    - Zrušení předplatného

    - Vypnutí automatického prodloužení platnosti

    - Přidat nepřímý prodejce ID MPN, pokud je k dispozici

> [!NOTE]
> Před provedením některých změn v předplatném, jako je zrušení odběru, možná budete muset provést některé kroky definované vydavatelem ISV.

## <a name="assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer"></a>Přiřazení licencí a Aktivace předplatného jménem zákazníka

Když si koupíte nabídku software jako službu (SaaS) poskytovanou vydavatelem nezávislého výrobce softwaru (ISV) na komerčním tržišti, vydavatel ISV pomáhá spravovat proces přiřazování licencí a aktivaci předplatného jménem vašeho zákazníka.

Vydavatel by vám měl poskytnout přizpůsobený odkaz a autorizační kód, který identifikuje konkrétní nákup.

1. Tento přizpůsobený odkaz od vydavatele ISV můžete najít několika způsoby:

   - Odkaz můžete zobrazit na stránce s potvrzením, která se zobrazí po nákupu nabídky ISV SaaS. Chcete-li najít tento odkaz na stránce, vyhledejte a vyberte možnost **Přejít na web vydavatele**.

   - Odkaz můžete zobrazit na stránce Předplatná konkrétního zákazníka. Tento odkaz na vydavatele se zobrazí na řádku přidruženém k nabídce ISV nebo k zakoupení předplatného pro zákazníka.

   - Odkaz můžete [načíst pomocí rozhraní API partnerského centra](/partner-center/develop/get-activation-link-by-order-line-item).

   > [!NOTE]
   > Pokud to chcete udělat jménem zákazníka, budete možná muset zkopírovat přizpůsobený odkaz, vložit ho do privátního prohlížeče a zadat přihlašovací údaje zákazníka.

2. Jakmile budete na webu nebo v systému vydavatele ISV, pošle vám Vydavatel informace o všech dalších krocích, které je potřeba provést k dokončení procesu nastavení zákazníka a zřízení nebo přiřazení licencí.

3. Jako partner v programu CSP, který pracuje jménem zákazníka, zodpovídáte za provádění následujících úloh:

    - Odeslat všechny požadované informace vydavateli.

    - Poslat všem požadované adrese URL přímo zákazníkovi (nebo jinak sdělit podrobnosti o tomto předplatnému vašemu zákazníkovi)

4. Po zadání požadovaných informací vydavateli bude Vydavatel zřídit a přiřadí příslušné licence. Fakturace předplatného se spustí až po těchto událostech:

    - Vydavatel ISV úspěšně přiřadil příslušné licence.

    - Vydavatel ISV potvrdil Microsoftu (prostřednictvím samostatného rozhraní API pro plnění SaaS), že nastavení účtu bylo úspěšně dokončeno.

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>Zrušení předplatného SaaS založeného na licencích od vydavatele ISV

Když se přihlásíte k odběru produktu SaaS založeného na licencích nabízeného vydavatelem ISV v rámci komerčního marketplace, máte možnost zrušit předplatné v rámci určeného období zrušení. Toto období zrušení se mění v závislosti na tom, jestli máte měsíční nebo roční předplatné. Můžete také zvolit, jestli se má předplatné automaticky obnovit.

Další informace o platnosti období zrušení, zrušení nebo automatickém prodlužování platnosti předplatného najdete v těchto tématu:

- [Zrušení předplatného](create-a-new-subscription.md#cancel-a-subscription)

- [Automatické prodloužení platnosti předplatného komerčního marketplace](create-a-new-subscription.md#choose-whether-to-automatically-renew-a-commercial-marketplace-subscription)

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>Přidání nebo odebrání licencí pro předplatné SaaS

V případě nabídek na komerčním marketplace SaaS můžete přidat nebo odebrat uživatelské licence pro předplatné zákazníka.

1. Přihlaste se k Partnerské centrum [a](https://partner.microsoft.com/dashboard) **pak** v levé navigační nabídce vyberte Zákazníci.

2. Vyberte příslušného zákazníka a pak vyberte **Předplatná.** Zobrazí se seznam všech předplatných založených na licencích, která jste pro zákazníka zakoupili.

3. Ve **sloupci Předplatné** vyberte předplatné, které chcete upravit.

4. Na stránce s podrobnostmi o předplatném vyhledejte **pole Quantity.** Tady můžete zvýšit nebo snížit počet licencí.

5. Změňte množství a pak vyberte **Submit (Odeslat).**

## <a name="manage-subscriptions-using-partner-center-apis"></a>Správa předplatných pomocí Partnerské centrum API

Pomocí rozhraní API partnerského centra můžete také provádět správu životního cyklu a spravovat faktury pro vaše předplatná. Další informace najdete v tématu [Vytvoření odběru pro produkty z komerčního tržiště](/partner-center/develop/create-subscription-azure-marketplace-products).

## <a name="next-steps"></a>Další kroky

- [Nákup nabídek pro komerční web Marketplace](csp-commercial-marketplace-purchase.md)
- [Další informace o fakturaci na komerčním webu Marketplace](csp-commercial-marketplace-billing.md)