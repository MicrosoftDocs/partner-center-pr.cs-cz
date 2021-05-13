---
title: Vynucení limitu kreditu
ms.topic: how-to
ms.date: 05/11/2021
description: Přečtěte si o limitu kreditu a o tom, jak se počítá. Zahrnuje nejčastější dotazy.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cf0d3c38b301c363a4a990db5258cf2a3f30d487
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/12/2021
ms.locfileid: "109819377"
---
# <a name="credit-limit-enforcement-cle"></a>Vynucení limitu kreditu (CLE)

**Odpovídající role**

- Správce fakturace

## <a name="your-credit-limit-and-how-it-works"></a>Váš limit kreditu a jak funguje

Váš limit kreditu je maximální částka (v USD), kterou jako partner můžete utratíte za nákup produktů nebo předplatných v Partnerské centrum. Pokud překročíte limit kreditu, nebude možné provádět nové nákupy, dokud nebude provedena dostatečná platba. Vaše stávající předplatná budou bez přerušení.

Limity kreditů se vztahují na nabídky v plánech Azure, rezervacích Azure, softwaru, Marketplace, Azure 145 P, Office a produktech Dynamics. Limity kreditů se nevztahují na prodloužení a průběžné využití.

Během období onboardingu přiřadíme váš limit kreditu na úrovni tenanta. Založit ho na vašich předpovídaných výnosech, nákupech a historii plateb. K výpočtu dostupného zůstatku pak použijeme následující vzorec:

**[Credit Limit – (Incoming Purchase + Outstanding Unpaid Invoices + Unbilled Charges – Overpayment)]**

## <a name="frequently-asked-questions"></a>Nejčastější dotazy

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a>Je limit kreditu nastavený na úrovni tenanta nebo na globální úrovni?

Úroveň tenanta. Předpokládejme například, že pracujete z USA, Kanady a Japonska. Pokud kanadský tenant dosáhne svého limitu kreditu, obdrží tento tenant oznámení, když se pokusí provést nákup v Partnerské centrum. Ostatní tenanty to nebude mít vliv. 

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
