---
title: Vynucení limitu kreditu
ms.topic: how-to
ms.date: 05/11/2021
description: Přečtěte si o kreditním limitu a o tom, jak se počítá. Obsahuje nejčastější dotazy.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: da3fc23a51cc70eec91a304f14189eb191c71339
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148104"
---
# <a name="credit-limit-enforcement-cle"></a>Vynucení limitu kreditu (CLE)

**Příslušné role**: správce fakturace

## <a name="your-credit-limit-and-how-it-works"></a>Limit kreditu a jak to funguje

Vaše kreditní omezení je maximální částka (v amerických dolarech), kterou můžete jako partner zaplatit za nákup produktů nebo předplatných v partnerském centru. Pokud překročíte úvěrový limit, nebudete moct vytvářet nové nákupy, dokud neproběhne dostatečná platba. Stávající předplatná budou bez přerušení pokračovat.

Úvěrový limit se vztahuje na nabídky v plánu Azure, rezervacích Azure, softwaru, Marketplace, Azure 145 P, Office a Dynamics Products. Limity úvěru se nevztahují na obnovení a průběžnou spotřebu.

Vaše kreditní limit přiřadíme na úrovni tenanta během období připojování. Založíme ji na vaše předpovědi pro tržby, nákup prowess a historii plateb. K výpočtu dostupného zůstatku použijeme následující vzorec:

**[Limit úvěru – (příchozí nákup + nedokončené faktury + neúčtované poplatky – přeplatek)]**

## <a name="frequently-asked-questions"></a>Nejčastější dotazy

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a>Je můj limit kreditu nastavený na tenantovi nebo na globální úrovni?

Úroveň tenanta. Předpokládejme například, že pracujete v USA, Kanadě a Japonsku. Pokud má kanadský tenant limit úvěru, pak tento tenant obdrží oznámení o tom, že se pokusí koupit v partnerském centru. Ostatní klienti nebudou ovlivněni. 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a>Pokud překročím svůj úvěrový limit, můžu pokračovat ve obsluhování stávajících zákazníků a předplatných s úplným přístupem?

Ano. Stávající předplatná vašich zákazníků budou bez přerušení pokračovat. Nemůžete ale koupit nové předplatné pro vaše zákazníky.

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a>Vztahuje se CLE na přímé i nepřímých poskytovatelů faktur?

Ano, platí pro obojí.

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a>Kdy se po odeslání platby má účet obnovit, kdy si můžu koupit další předplatné? 

Během 24 hodin platby byste měli být schopni pokračovat v nákupu, a to za předpokladu, že společnost Microsoft obdržela všechny požadavky, aby bylo možné pokračovat v procesu kontroly kreditu.

### <a name="how-can-i-check-my-credit-limit"></a>Jak si můžu ověřit úvěrový limit?

Kontaktujte, pokud [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) chcete zobrazit úvěrový limit a získat informace o nedávném nákupu.

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a>Mají se faktury v počtu sporů s limitem úvěru?

Ano. Můžete však kontaktovat společnost Microsoft [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) a vyřešit problém.

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a>Jak brzy uslyším, když zapisujem ucmwrcsp@microsoft.com ?

Odpověď by měla být kratší než 24 hodin. 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a>Jaká kritéria Microsoft používá k nastavení úvěrového limitu pro partnery?

Váš limit kreditu určíme na základě vašich předpokládaných výnosů, nákupu prowess a historie plateb.

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a>Je limit úvěru aktuálně vyhodnocený na novém prostředí pro obchod?

Ano. Úvěrový limit se vztahuje na všechny programy a produkty CSP v partnerském centru.

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a>Kdo obdrží oznámení, když se moje organizace blíží limitu úvěru?

Oznámení o závazku finančního účtu vaší organizace by mělo obdržet oznámení.

## <a name="next-steps"></a>Další kroky

[Základní informace o fakturaci](./billing-basics.md)
