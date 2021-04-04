---
title: Získaný kredit partnerů pro spravované služby
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Seznamte se s tím, jak se počítá a hradí Microsoft partnerd Credit (PEC) pro spravované služby a jak zajistit, abyste měli nárok na to.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 022e7aabd0d850660f8236dce9a4fab9069af01b
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/31/2021
ms.locfileid: "106087123"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>Principy výpočtu a vyplácení kreditu získaného partnerem

**Příslušné role**

- Globální správce
- Správce správy uživatelů
- Agent správce
- Správce fakturace
- Agent prodeje

Získaný kredit partnerů pro spravované služby (PEC) rozpoznává a vyměňuje partnery, kteří mají nepřetržitou provozní kontrolu a správu částí, nebo celé prostředí Azure svých zákazníků. Ve výchozím nastavení je ve zprostředkovateli CSP udělena potřebná přístupová práva k předplatnému zákazníka, což jim umožňuje provádět 24 × 7 provozní správu a kontrolu nad prostředky v rámci předplatného. Další způsoby, jak můžou zákazníci zřídit přístup k transakčním partnerům, jsou popsány v následující části. Částka měsíční faktury je netto kredit získaný prostřednictvím partnerského serveru. Partneři můžou zobrazit podrobnosti o řadiči PEC na jejich měsíčním souboru rekognoskaci. Další způsoby, jak může zákazník zřídit přístup pro transakčního partnera, najdete [v článku Správa předplatných a prostředků v plánu Azure](azure-plan-manage.md).

Také číst [obnovit oprávnění správce pro předplatná Azure CSP](revoke-reinstate-csp.md)

## <a name="eligibility"></a>Vznik

Pro získání partnerského kreditu pro partnery (PEC) platí následující požadavky: 

- Pro získání realizovaného kreditu za prostředky Azure, které spravujete, musíte mít aktivní smlouvu MPN a platnou roli řízení přístupu na základě role (RBAC).

- Musíte mít nepřetržitou provozní kontrolu a správu prostředků Azure zákazníka v CSP. To znamená, že musíte mít oprávnění správce v předplatném Azure zákazníka, skupině prostředků Azure a prostředku Azure. V případě nepřímých zprostředkovatelů a jejich nepřímých prodejců budou mít nepřímý poskytovatel nárok na PEC, pokud je tento operační řízení buď nepřímým poskytovatelem, nebo nepřímým prodejcem. Další informace najdete v tématu obnovení [oprávnění správce pro odběry CSP Azure](./revoke-reinstate-csp.md).

- Kromě výše uvedených požadavků platí, že PEC se dá použít jenom pro služby uvedené v cenách Azure Plan spotřebování, které můžete exportovat na stránce s [cenami plánu Azure](https://partner.microsoft.com/commerce/sales) .

- PEC se **nevztahuje** na tyto služby:
    - Rezervace plánu Azure
    - Produkty třetích stran identifikované jako třetí strana ve sloupci značky ceny spotřeby plánu Azure
    - Produkty v ceníku webu Marketplace
    - [Virtual Machines na místě Azure](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- Řadič PEC se získal na úrovni prostředků Azure. Pokud máte platný přístup buď na úrovni předplatného nebo skupiny prostředků, bude každý prostředek, který se zahrne do vyšší entity, získat PEC.

- Podrobnosti o řadičích PEC jsou k dispozici také na stránce [Azure cost management](/azure/cost-management-billing/costs/get-started-partners) .

### <a name="calculation"></a>Výpočet

PEC se počítá denně a je možné ji zobrazit v souboru denního využití a v souboru rekognoskaci pro měsíční fakturu. Partner (nepřímý poskytovatel nebo nepřímý prodejce) musí mít přístup k celému dni (nepřetržitě), aby mohl získat PEC. Na spravovaných prostředcích Azure se každý den počítá PEC. Partneři uchovávají trvalý privilegovaný přístup v průběhu měsíce (rozsah přístupu) a u všech oprávněných prostředků (rozsah přístupu) získají úplný řadič PEC. Snížení rozsahu a rozpětí rozpětí bude mít za měsíc nižší sazbu PEC. Denní hodnocený soubor využití se denně zobrazuje na základě prostředku Azure, ať už se používá nebo ne. Partneři taky můžou zaregistrovat výstrahy a monitorovat změny trvalého privilegovaného přístupu.

## <a name="azure-cost-management"></a>Správa nákladů v Azure

Azure Cost Management (ACM) s využitím analýzy nákladů umožňuje jako partnera zobrazit náklady, které dostaly výhody PEC.  

1. V [Azure Portal](https://portal.azure.com)se přihlaste ke svému partnerskému tenantovi a vyberte **cost management + fakturace**.

2. Vybrat **správu nákladů**

3. Vybrat **analýzu nákladů**

   V zobrazení analýza nákladů se zobrazí náklady na fakturační účet pro všechny služby zakoupené a spotřebované v cenách, které platíte společnosti Microsoft.

4. V rozevíracím seznamu v kontingenčním grafu vyberte **PartnerEarnedCreditApplied** , aby se zobrazily náklady s použitím pec. Pokud má vlastnost **PartnerEarnedCreditApplied** hodnotu true, mají přidružené náklady nárok na zvýhodněný kredit získaný partnerem. 

   Pokud má vlastnost PartnerEarnedCreditApplied hodnotu false, přidružené náklady nevyhověly požadovanému nároku na kredit nebo zakoupená služba nemá nárok na kredit získaný partnerem.

   >[!NOTE] 
   >Obvykle se používání služeb v **cost management** zobrazuje za 8-24 hodin a KREDITy pec se zobrazí během 48 hodin od doby přístupu v Azure cost management.

5. Můžete také seskupit podle a filtrovat pomocí vlastnosti **PartnerEarnedCreditApplied** pomocí **Group by a přidat** funkce filtru pro přechod k podrobnostem o nákladech, které mají pec a náklady bez použití primárního řadiče PEC.

## <a name="next-steps"></a>Další kroky

- [Získaný kredit partnerů – přehled](partner-earned-credit.md)

- Podrobné příklady výpočtů vydaných kreditů partnerů najdete v ceníku, ke kterému se můžete dostat prostřednictvím řídicího panelu partnerského centra (vyžaduje se přihlášení).

- [Přejít na Azure Plan – Začínáme](azure-plan-get-started.md)

- [Správa předplatných a prostředků v rámci plánu Azure](azure-plan-manage.md)

- [Odvolat nebo obnovit oprávnění správce pro předplatná Azure CSP](revoke-reinstate-csp.md)
