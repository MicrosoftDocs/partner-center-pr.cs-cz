---
title: Propojit pracovní účet pro přístup k partnerskému centru
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Vytvořte pracovní účet, který propojuje vaši společnost s účtem partnerského centra. Zaměstnanci ve vaší společnosti tak mohou přistupovat k partnerskému centru.
author: vinayks
ms.author: vinayks
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 6/17/2021
ms.openlocfilehash: 69aa45de55a4356eaab1bcd4cd309feb14de9f6e
ms.sourcegitcommit: 0410e2a3f91b7e6b592cc47e7af1dfbe468c7881
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/17/2021
ms.locfileid: "112318057"
---
# <a name="create-a-work-account-that-links-your-company-to-your-partner-center-account"></a>Vytvořte pracovní účet, který propojuje vaši společnost s účtem partnerského centra.

**Příslušné role**: globální správce | Správce správy uživatelů

## <a name="why-you-need-a-work-account"></a>Proč potřebujete pracovní účet

Microsoft vyžaduje, abyste svůj pracovní účet společnosti propojíte s novým účtem partnerského centra. Odkaz umožňuje uživatelům vašeho účtu přihlásit se do partnerského centra pomocí uživatelských jmen a hesel pracovního účtu.

## <a name="the-work-account-email-address"></a>E-mailová adresa pracovního účtu

Pracovní účet nebo pracovní e-mail je e-mailová adresa, kterou vám poskytla vaše společnost. E-mail pracovního účtu je obvykle ve formátu `you@yourcompany.com` . Osobní e-mailové adresy, jako je například Hotmail, Gmail nebo Yahoo, nejsou pracovní e-maily a nelze je použít pro účet partnerského centra.

Pokud máte více než jednu platnou pracovní e-mailovou adresu, použijte tu, která je přidružená k vašemu firemnímu ústředí, nikoli k místnímu oddělení, například `contoso.com` e-mailu místo `contoso.uk` adresy.

> [!NOTE]  
> Než začnete používat stávající pracovní účet, vezměte v úvahu, kolik uživatelů v pracovním účtu bude potřebovat přístup k partnerskému centru. Pokud máte uživatele v pracovním účtu, který nebude potřebovat přístup k partnerskému centru, zvažte vytvoření nového účtu jenom pro uživatele, kteří budou potřebovat přístup k partnerskému centru.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Nejste si jistí, jestli má vaše společnost již pracovní účet?

Pokud si nejste jistí, jestli má vaše společnost pracovní účet, proveďte kontrolu pomocí těchto kroků. Pokud máte aktivní předplatné Microsoft Azure nebo Office 365, již máte pracovní účet.

1. Přihlaste se k webu [Azure Portal](https://portal.azure.com).

2. V navigační nabídce vyberte Azure Active Directory a vyberte **vlastní názvy domén**.

3. Pokud již máte pracovní účet, bude uveden název vaší domény.

Pokud vaše společnost ještě nemá pracovní účet, můžete si ji vytvořit během procesu registrace.

Diagram níže popisuje kroky pro několik typických scénářů:

- určení, jestli máte pracovní účet
- určení způsobu přihlášení k pracovnímu účtu
- určení, jestli je potřeba vytvořit nový pracovní účet

:::image type="content" source="images/onboardingAADFlow.png" lightbox="images/onboardingAADFlow.png" alt-text="Máte pracovní účet nebo ho potřebujete vytvořit?":::

Další informace o přidávání domén v Azure AD najdete v tématu [Přidání nebo přidružení domény ve službě Azure AD](/azure/active-directory/active-directory-add-domain) .

## <a name="about-microsoft-azure"></a>O Microsoft Azure

Microsoft Azure je veřejná cloudová platforma, kterou můžou společnosti používat k sestavování, nasazování a správě aplikací napříč globální sítí datových center spravovaných Microsoftem. Společnosti využívají Azure k vytváření virtuálních IT infrastruktury s virtuálními funkcemi nebo službami místo fyzických počítačů.

Když si koupíte předplatné Azure, nebudete mít v podstatě vyhrazené a zabezpečené místo ve veřejném cloudu Azure, ale nemusíte se zabývat podlahou v budově Office, která bude firemní fyzickou firmu. K vlastníkovi budovy Office je vaše společnost tenant.

Pracovní účet Azure je vyhrazená a izolovaná virtuální reprezentace vaší společnosti ve veřejném cloudu Azure, která se vytvoří po přihlášení k odběru cloudové služby Microsoftu, jako je Azure, Microsoft Intune nebo Office 365.

Váš pracovní účet je hostitelem uživatelů Azure AD a informací o nich – jejich hesla, data profilu, oprávnění atd. Pracovní účet obsahuje také skupiny, aplikace a další informace, které se týkají společnosti a jejího zabezpečení.

## <a name="next-steps"></a>Další kroky

- [Správa účtu v Partnerském centru](partner-center-account-setup.md)
- [Sledovat stav ověřování](verification-responses.md)
