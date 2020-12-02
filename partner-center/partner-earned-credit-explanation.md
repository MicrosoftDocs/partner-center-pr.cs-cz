---
title: Získaný kredit partnerů pro spravované služby
ms.topic: article
ms.date: 11/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Seznamte se s tím, jak se počítá a hradí Microsoft partnerd Credit (PEC) pro spravované služby a jak zajistit, abyste měli nárok na to.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 97af446c4021e9785833374131eee2f08431b5fe
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/01/2020
ms.locfileid: "96474304"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>Principy výpočtu a vyplácení kreditu získaného partnerem

**Příslušné role**

- Globální správce
- Správce uživatelů
- Agent správce
- Správce fakturace
- Agent prodeje

Získaný kredit partnerů pro spravované služby (PEC) rozpoznává a vyměňuje partnery, kteří mají nepřetržitou provozní kontrolu a správu částí, nebo celé prostředí Azure svých zákazníků. Ve výchozím nastavení je ve zprostředkovateli CSP udělena potřebná přístupová práva k předplatnému zákazníka, což jim umožňuje provádět 24 × 7 provozní správu a kontrolu nad prostředky v rámci předplatného. Další způsoby, jak zákazník může zřídit přístup pro transakčního partnera, je popsaný v následující části. Měsíční fakturovaná částka nezahrnuje kredit získaný partnerem. Partneři můžou zobrazit podrobnosti o řadiči PEC na jejich měsíčním souboru rekognoskaci. Další způsoby, jak může zákazník zřídit přístup pro transakčního partnera, najdete [v článku Správa předplatných a prostředků v plánu Azure](azure-plan-manage.md).

Také číst [obnovit oprávnění správce pro předplatná Azure CSP](revoke-reinstate-csp.md)

## <a name="important-eligibility-and-calculation-information"></a>Důležité informace o způsobilosti a výpočtech

- Partner by měl mít aktivní smlouvu MPN a platnou roli RBAC, aby získal získaný kredit pro prostředky Azure, které spravují. 

- V případě nepřímých zprostředkovatelů a jejich nepřímých prodejců budou mít nepřímý poskytovatel nárok na PEC, pokud buď nepřímý poskytovatel, nebo nepřímý prodejce nebo obojí mají nepřetržitou provozní kontrolu a správu prostředků Azure zákazníka v CSP.

- K účtované (Fakturovatelné) spotřebě na Azure majetku v CSP spravovaném partnerem se přidruží služba PEC. K dispozici je PEC jenom partnerům v CSP, které účtuje Microsoft (nepřímý poskytovatel a partner poskytující přímý přístup k fakturaci). 

- Opravňující služby: získaný partnerský kredit se vztahuje na služby uvedené ve **cenách Azure plánu** , které mohou partneři exportovat na stránce s [cenami plánu Azure](https://partner.microsoft.com/commerce/sales) . 

- Nezpůsobilé služby: získaný kredit pro partnery je *_* nepoužit pro_* následující:
    - Rezervace plánu Azure
    - Produkty třetích stran identifikované jako *třetí strana** ve **sloupci značky** ceny spotřeby plánu Azure    
    - Produkty v ceníku webu Marketplace
   - [Virtual Machines na místě Azure](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- PEC se počítá denně a je možné ji zobrazit v souboru denního využití a v souboru rekognoskaci pro měsíční fakturu. Partner (nepřímý poskytovatel nebo nepřímý prodejce) musí mít přístup k celému dni (nepřetržitě), aby mohl získat PEC. Na spravovaných prostředcích Azure se každý den počítá PEC. Maximální počet řadičů PEC pro dané fakturační období (měsíc) je 15%. Partneři uchovávají trvalý privilegovaný přístup v průběhu měsíce (rozsah přístupu) a u všech oprávněných prostředků (rozsah přístupu) získají úplné PEC o 15%. Snížení rozsahu a rozpětí rozpětí bude mít za měsíc nižší sazbu PEC. Denní hodnocený soubor využití se denně zobrazuje na prostředku Azure, ať už se používá PEC nebo ne. Partneři taky můžou zaregistrovat výstrahy a zjistit, jestli existují změny trvalého privilegovaného přístupu.

- Řadič PEC se získal na úrovni prostředků Azure. Pokud má partner platný přístup v rámci předplatného nebo na úrovni skupiny prostředků, bude každý prostředek, který má role až k vyšší entitě, získávat řadiče PEC.  

- Podrobnosti o řadičích PEC budou také k dispozici ve [službě Azure cost management](/azure/cost-management-billing/costs/get-started-partners) .

## <a name="azure-cost-management"></a>Azure Cost Management

Azure Cost Management (ACM) s využitím analýzy nákladů umožňuje jako partnera zobrazit náklady, které dostaly výhody PEC.  

1. V [Azure Portal](https://portal.azure.com)se přihlaste ke svému partnerskému tenantovi a vyberte **cost management + fakturace**.

2. Vybrat **správu nákladů**

3. Vybrat **analýzu nákladů**

   V zobrazení analýza nákladů se zobrazí náklady na fakturační účet pro všechny služby zakoupené a spotřebované v cenách, které platíte společnosti Microsoft.

4. V rozevíracím seznamu v rozevíracím grafu vyberte **PartnerEarnedCreditApplied** , aby se zobrazily náklady s použitím pec. Pokud má vlastnost **PartnerEarnedCreditApplied** hodnotu true, mají přidružené náklady nárok na zvýhodněný kredit získaný partnerem. 

Pokud má vlastnost PartnerEarnedCreditApplied hodnotu false, přidružené náklady nevyhověly požadovanému nároku na kredit nebo zakoupená služba nemá nárok na kredit získaný partnerem.

>[!NOTE] 
>Obvykle se používání služeb v **cost management** zobrazuje za 8-24 hodin a KREDITy pec se zobrazí během 48 hodin od doby přístupu v Azure cost management.

5. Můžete také seskupit podle a filtrovat pomocí vlastnosti **PartnerEarnedCreditApplied** pomocí **Group by a přidat** funkce filtru pro přechod k podrobnostem o nákladech, které mají pec a náklady bez použití primárního řadiče PEC.

## <a name="next-steps"></a>Další kroky

- [Získaný kredit partnerů – přehled](partner-earned-credit.md)

- Podrobné příklady výpočtů vydaných kreditů pro partnery jsou umístěné na ceníku, ke kterému se můžete dostat prostřednictvím řídicího panelu partnerského centra (vyžaduje se přihlášení).

- [Přejít na Azure Plan – Začínáme](azure-plan-get-started.md)

- [Správa předplatných a prostředků v rámci plánu Azure](azure-plan-manage.md)

- [Odvolat nebo znovu nastavovat oprávnění správce pro předplatná Azure CSP](revoke-reinstate-csp.md)
