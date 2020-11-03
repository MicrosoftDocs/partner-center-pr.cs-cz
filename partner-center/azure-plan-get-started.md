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
ms.openlocfilehash: 5ad7bd7c99d7caa044877c98aac6dc5e3ce69420
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/22/2020
ms.locfileid: "92527597"
---
# <a name="begin-using-pay-as-you-go-rates-with-the-azure-plan"></a>Začněte používat tarify průběžných plateb s plánem Azure.

Společnost Microsoft zavedla nové prostředí pro obchod v partnerském centru.  Díky tomuto novému prostředí pro obchod získají partneři přístup ke službám Azure podle tarifů průběžných plateb pro zákazníky podle smlouvy o zákaznících Microsoftu.

Tento plán zjednodušuje možnosti nákupu – v plánu Azure můžete mít několik předplatných Azure. Už nemusíte odesílat samostatné objednávky na předplatné Azure. A v tomto novém prostředí pro obchod s Azure jsme se zarovnali s jedním globálním cenovým principem, který partnerům CSP umožní nabídnout Azure za publikované ceny.

Potřeby digitálních transformací pro naše zákazníky vyžadují nové dovednosti od partnerů. Spousta zákazníků si vyhledává, aby partneři poskytovali služby nad a po transakcích, aby jejich cloudová cesta byla plynulejší a mohla efektivně využívat služby Azure. Partneři Microsoftu hrají důležitou roli ve všech fázích životního cyklu zákazníka. Tyto druhy partnerských služeb jsou pohotové a zahrnují monitorování, zásady a správu zásad správného řízení, nastavení a konfiguraci, optimalizaci, technickou podporu a celou řadu dalších služeb. Vyžadují, aby byl partner podrobnějším pohledu zjistíte obeznámen s prostředím Azure zákazníka a měl průběžné a vhodné řízení a kontrolu nad základními prostředky, které spravují. Fakturační partneři, kteří poskytují tuto 24 × 7 cloudovou správu provozu, budou mít nárok na **kredit získaný pro partnery pro služby** , které jsou pro tuto práci spravované.

## <a name="make-sure-your-customers-have-signed-the-microsoft-customer-agreement"></a>Ujistěte se, že vaši zákazníci podepsali smlouvu o zákaznících Microsoftu.

Od 1. října 2019 se k dispozici smlouva o zákaznících Microsoftu, která je k dispozici a zjednodušuje a zjednodušuje možnosti nákupu zákazníků pomocí plně digitálního procesu. Všichni zákazníci, kteří chtějí využít nové prostředí pro obchodování v CSP pro Azure, musí podepsat smlouvu o zákaznících Microsoftu.

Partneři, kteří chtějí v rámci nového plánu Azure vytvořit novou objednávku, by měli potvrdit přijetí zákaznických smluv Microsoftu pomocí řídicího panelu partnerského centra a rozhraní API v produkčním prostředí.

Od 1. února 2020 se stávající smlouva Microsoft Cloud odebere z programu CSP. Od této doby bude pro všechny ostatní nabídky, včetně Microsoft 365, Dynamics 365 a stávajících Azure, vyžadováno potvrzení partnera (atestace) přijetí souhlasu se zákazníkem pro novou zákaznickou smlouvu Microsoftu. Partneři v CSP nebudou moct vytvořit novou objednávku pro zákazníka bez potvrzení smlouvy o zákaznících Microsoftu.

Úplné podrobnosti najdete v článku [potvrzení souhlasu zákazníka se smlouvou Microsoft pro zákazníky](confirm-customer-agreement.md) .

## <a name="security-and-access-control-practices"></a>Postupy řízení přístupu a zabezpečení

Abychom vám pomohli chránit partnery a zákazníky, zavádíme sadu povinných požadavků na zabezpečení pro poradce, dodavatele ovládacích panelů a partnery účastnící se programu Cloud Solution Provider.

Partneři, kteří neimplementují povinné požadavky na zabezpečení, nebudou moci pracovat v programu Cloud Solution Provider ani spravovat klienty, kteří využívají oprávnění správce delegování, jakmile budou tyto požadavky vynutily. V procesu nastavování data technického vynucování pro požadavky a upozorní partnery na datum s podrobnými informacemi.

## <a name="actions-to-take-to-implement-mfa"></a>Akce, které se mají provést při implementaci MFA

Vzhledem k tomu, že má vysoce privilegovaný charakter jako partner, potřebujeme zajistit, aby měl každý uživatel výzvu MFA pro každé samostatné ověřování. To lze provést jedním z následujících způsobů:

- Implementace Azure AD Premium a zajištění, že pro každého uživatele se vynutilo vícefaktorové ověřování (MFA)
- Implementace [výchozích hodnot zabezpečení Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- Implementace řešení třetí strany a ověření vícefaktorového ověřování pro každého uživatele

Od 1. srpna 2019 musí všichni partneři vymáhat službu Multi-Factor Authentication pro všechny uživatele, včetně účtů služeb ve svém partnerském tenantovi. Podrobné informace o těchto požadavcích na zabezpečení najdete v [požadavcích na zabezpečení partnera](partner-security-requirements.md).

Microsoft doporučuje partnerům využít usilovně RBAC, a to podle osvědčených postupů povolených prostřednictvím [Azure Active Directory Privileged identity Managementch prostředků](/azure/active-directory/privileged-identity-management/pim-configure).

## <a name="read-more-about-the-azure-plan"></a>Přečtěte si další informace o plánu Azure.

- [Nákup plánu Azure](purchase-azure-plan.md)

- [Porovnání nabídek Azure](compare-azure-offers.md)

- [Získaný kredit partnerů – přehled](partner-earned-credit.md)

- Výpočty s vydaným kreditem (PEC) a role a oprávnění, které mají nárok na získání partnerských kreditů, jsou k dispozici na základě ceníku vašeho řídicího panelu partnerského centra (vyžaduje se přihlášení).

## <a name="next-steps"></a>Další kroky 

- [Jak je určeno, jak je určen partnerský kredit – podrobnosti](partner-earned-credit-explanation.md)
- [Vysvětlení ceníku plánu Azure](azure-plan-price-list.md)
- [Převod zákazníků na plán Azure](azure-plan-transition.md)
- [Správa předplatných a prostředků v rámci plánu Azure](azure-plan-manage.md)
- [Úplný seznam zemí nebo oblastí, ve kterých je plán Azure k dispozici](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x)