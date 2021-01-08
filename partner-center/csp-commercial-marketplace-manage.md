---
title: Správa produktů Marketplace & nabídek
ms.topic: how-to
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Pomocí partnerského centra se dozvíte, jak můžou poskytovatelé cloudového řešení spravovat nabídky třetích stran zakoupené pro zákazníky z komerčního tržiště.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5e6ca188aeb50cec6f847afb08be4a9d62b36984
ms.sourcegitcommit: a78dd3c532860d01867d116bfb4e2c88b84bcd25
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/08/2021
ms.locfileid: "97979672"
---
# <a name="manage-commercial-marketplace-products-and-offers-for-your-customers"></a>Správa produktů a nabídek komerčního tržiště pro vaše zákazníky


**Příslušné role**

- Globální správce
- Agent správce

Partneři v programu Cloud Solution Provider (CSP) můžou použít portál partnerského centra k nákupu mnoha nabídek SaaS ISV nebo předplatných pro své zákazníky z komerčního tržiště. Po zakoupení nabídky máte různé způsoby, jak ji spravovat.

## <a name="view-or-edit-a-subscription"></a>Zobrazit nebo upravit předplatné

Po zakoupení předplatného od jiného vydavatele ISV jiného výrobce ho můžete zkontrolovat nebo upravit následujícím způsobem:

1. Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard)partnerského centra a v levé navigační nabídce vyberte **zákazníky** .

2. Vyberte příslušného zákazníka a pak vyberte **předplatná**. Obsahuje seznam všech předplatných založených na licencích, které jste zakoupili pro zákazníka.

3. Ve sloupci **předplatné** vyberte předplatné, které chcete zobrazit nebo upravit. Získáte tak další informace o nastavení nebo zřízení nabídky. (Pokud se v nabídce vyžaduje více akcí, může se ve sloupci Stav zobrazit také stav "potřeba akce". Může se taky doprovázet odkaz na web vydavatele ISV.)

4. Po výběru předplatného, které chcete zobrazit nebo upravit, vám stránka s podrobnostmi o předplatném umožňuje upravit předplatné a dělat tyto věci:

    - Změnit přezdívku předplatného

    - Přidat nebo snížit počet licencí v předplatném

    - Zrušení předplatného

    - Vypnout automatické obnovení

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

4. Po zadání požadovaných informací vydavateli bude Vydavatel zřídit a přiřadí příslušné licence. Fakturace předplatného se spustí až po výskytu následujících událostí:

    - Vydavatel ISV úspěšně přiřadil příslušné licence.

    - Vydavatel ISV potvrdil společnost Microsoft (prostřednictvím samostatného rozhraní API pro plnění SaaS), že se nastavení účtu úspěšně dokončilo.

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>Zrušení předplatného SaaS založeného na licencích od vydavatele ISV

Když se přihlásíte k odběru produktu SaaS založeného na licencích, který nabízí Vydavatel ISV v rámci komerčního tržiště, máte možnost zrušit předplatné v rámci stanoveného období zrušení. Tato doba zrušení se mění v závislosti na tom, zda máte měsíční nebo roční předplatné. Můžete také zvolit, zda má být předplatné automaticky obnoveno.

Další informace o časových obdobích zrušení, která platí, jak zrušit nebo jak automaticky obnovit předplatné, najdete v tématech:

- [Zrušení předplatného](create-a-new-subscription.md#cancel-a-subscription)

- [Automatické obnovení předplatného komerčního tržiště](create-a-new-subscription.md#choose-whether-to-automatically-renew-a-commercial-marketplace-subscription)

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>Přidání nebo odebrání licencí pro předplatné SaaS

V případě nabídek SaaS Commercial Marketplace můžete přidat nebo odebrat uživatelské licence pro předplatné zákazníka.

1. Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard)partnerského centra a v levé navigační nabídce vyberte **zákazníky** .

2. Vyberte příslušného zákazníka a pak vyberte **předplatná**. Obsahuje seznam všech předplatných založených na licencích, které jste zakoupili pro zákazníka.

3. Ve sloupci **předplatné** vyberte předplatné, které chcete upravit.

4. Na stránce Podrobnosti předplatného vyhledejte pole **množství** . Tady můžete zvýšit nebo snížit počet licencí.

5. Změňte množství a pak vyberte **Odeslat**.

## <a name="manage-subscriptions-using-partner-center-apis"></a>Správa předplatných pomocí rozhraní API partnerského centra

Pomocí rozhraní API partnerského centra můžete také provádět správu životního cyklu a spravovat faktury pro vaše předplatná. Další informace najdete v tématu [Vytvoření odběru pro produkty z komerčního tržiště](/partner-center/develop/create-subscription-azure-marketplace-products).

## <a name="next-steps"></a>Další kroky

- [Nákup nabídek pro komerční web Marketplace](csp-commercial-marketplace-purchase.md)
- [Další informace o fakturaci na komerčním webu Marketplace](csp-commercial-marketplace-billing.md)