---
title: Zahajte přesun do plánu Azure.
description: Seznamte se s tím, co vy a vaši zákazníci potřebujete vědět o používání plánu průběžných plateb Azure, včetně prvních kroků, bezpečnostních opatření a způsobu, jak začít.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.custom: SEOAPR.20
ms.localizationpriority: High
ms.date: 12/02/2019
ms.openlocfilehash: 58feabdefb02660559c69f61190070310768b947
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149651"
---
# <a name="begin-using-pay-as-you-go-rates-with-the-azure-plan"></a>Začněte používat tarify průběžných plateb s plánem Azure.

**Příslušné role**: Agent správce | Agent prodeje


Společnost Microsoft zavedla nové prostředí pro obchod v partnerském centru.  Díky tomuto novému prostředí pro obchod získají partneři přístup ke službám Azure podle tarifů průběžných plateb pro zákazníky podle smlouvy o zákaznících Microsoftu.

Tento plán zjednodušuje možnosti nákupu – v plánu Azure můžete mít několik předplatných Azure. Už nemusíte odesílat samostatné objednávky na předplatné Azure. A v tomto novém prostředí pro obchod s Azure jsme se zarovnali s jedním globálním cenovým principem, který partnerům CSP umožní nabídnout Azure za publikované ceny.

Potřeby digitálních transformací pro naše zákazníky vyžadují nové dovednosti od partnerů. Spousta zákazníků si vyhledává, aby partneři poskytovali služby nad a po transakcích, aby jejich cloudová cesta byla plynulejší a mohla efektivně využívat služby Azure. Partneři Microsoftu hrají důležitou roli ve všech fázích životního cyklu zákazníka. Tyto druhy partnerských služeb jsou pohotové a zahrnují monitorování, zásady a správu zásad správného řízení, nastavení a konfiguraci, optimalizaci, technickou podporu a celou řadu dalších služeb. Vyžadují, aby byl partner podrobnějším pohledu zjistíte obeznámen s prostředím Azure zákazníka a měl průběžné a vhodné řízení a kontrolu nad základními prostředky, které spravují. Fakturační partneři, kteří poskytují tuto 24 × 7 cloudovou správu provozu, budou mít nárok na **kredit získaný pro partnery pro služby** , které jsou pro tuto práci spravované.

## <a name="make-sure-your-customers-have-signed-the-microsoft-customer-agreement"></a>Ujistěte se, že vaši zákazníci podepsali smlouvu o zákaznících Microsoftu.

Od 1. října 2019 je k dispozici Smlouva se zákazníkem Microsoftu, časově neomezená smlouva, která zjednodušuje a zefektivňuje nákupní prostředí zákazníků s plně digitálním procesem. Všichni zákazníci, kteří chtějí využívat nové obchodní prostředí v CSP pro Azure, musí podepsat Smlouva se zákazníkem Microsoftu.

Partneři, kteří chtějí provést transakce v rámci nového plánu Azure a vytvořit novou objednávku, by měli potvrdit souhlas zákazníka s Smlouva se zákazníkem Microsoftu pomocí řídicího panelu Partnerské centrum a rozhraní API v produkčním prostředí.

Od 1. února 2020 se existující Smlouva o službách Microsoft Cloud z programu CSP odebere. Od té doby bude u všech ostatních nabídek, včetně Microsoft 365, Dynamics 365 a existujícího Azure, vyžadováno potvrzení souhlasu partnera (ověření) přijetí nové služby Smlouva se zákazníkem Microsoftu zákazníkem. Partneři v CSP nebudou moct vytvořit pro zákazníka novou objednávku bez ověření Smlouva se zákazníkem Microsoftu.

Úplné podrobnosti najdete v tématu [Potvrzení souhlasu zákazníka s Smlouva se zákazníkem Microsoftu](confirm-customer-agreement.md)

## <a name="security-and-access-control-practices"></a>Postupy zabezpečení a řízení přístupu

Za účelem ochrany partnerů a zákazníků zavádíme sadu povinných požadavků na zabezpečení pro poradce, dodavatele Ovládací panely a partnery, kteří se účastní Cloud Solution Provider programu.

Partneři, kteří neimplementují povinné požadavky na zabezpečení, nebudou moct po vynucování těchto požadavků provádět transakce v programu Cloud Solution Provider ani spravovat tenanty zákazníků s využitím práv delegovaného správce. Právě zavádíme datum technického vynucování požadavků a na datum upozorníme partnery s podrobnými informacemi.

## <a name="actions-to-take-to-implement-mfa"></a>Akce, které je za účelem implementace MFA

Vzhledem k vysoce privilegované povaze partnera musíme zajistit, aby každý uživatel měl při každém ověření výzvu více ověřování. Toho lze dosáhnout jedním z následujících způsobů:

- Implementace Azure AD Premium a zajištění vynucení vícefaktorového ověřování (MFA) pro každého uživatele
- Implementace [výchozích hodnot zabezpečení Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- Implementace řešení třetí strany a zajištění vynucení MFA pro každého uživatele

Od 1. srpna 2019 musí všichni partneři vynucovat vícefaktorové ověřování pro všechny uživatele, včetně účtů služeb, v partnerském tenantovi. Podrobné informace o těchto požadavcích na zabezpečení najdete v požadavcích [na zabezpečení partnerů.](partner-security-requirements.md)

Microsoft doporučuje partnerům, aby RBAC vyhověli, a to podle osvědčených postupů povolených [prostřednictvím Azure Active Directory Privileged Identity Management prostředků.](/azure/active-directory/privileged-identity-management/pim-configure)

## <a name="read-more-about-the-azure-plan"></a>Další informace o plánu Azure

- [Nákup plánu Azure](purchase-azure-plan.md)

- [Porovnání nabídek Azure](compare-azure-offers.md)

- [Kredit získaný partnerem – přehled](partner-earned-credit.md)

- Výpočty kreditu získaného partnerem (PEC) a role a oprávnění, které mají nárok na získání kreditů získaných partnerem, jsou k dispozici v ceníku řídicího panelu Partnerské centrum (vyžaduje se přihlášení).

## <a name="next-steps"></a>Další kroky 

- [Způsob, jakým se určuje kredit získaný partnerem – podrobnosti](partner-earned-credit-explanation.md)
- [Vysvětlení ceníku plánu Azure](azure-plan-price-list.md)
- [Převod zákazníků na plán Azure](azure-plan-transition.md)
- [Správa předplatných a prostředků v rámci plánu Azure](azure-plan-manage.md)
- [Úplný seznam zemí/oblastí, ve kterých je plán Azure k dispozici](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x)