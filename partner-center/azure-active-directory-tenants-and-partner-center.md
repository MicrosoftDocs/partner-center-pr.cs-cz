---
title: Propojení pracovního účtu pro přístup k Partnerské centrum
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Vytvořte pracovní účet, který pro propojení vaší společnosti s vaším Partnerské centrum účtem. Zaměstnanci ve vaší společnosti tak budou mít přístup k Partnerské centrum.
author: vinayks
ms.author: vinayks
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 11/25/2019
ms.openlocfilehash: a06a38ef9d96b4c2a1e95328d510eb2fd71ff0e3
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149838"
---
# <a name="create-a-work-account-that-links-your-company-to-your-partner-center-account"></a>Vytvoření pracovního účtu, který pro propojení vaší společnosti s vaším Partnerské centrum účtem

**Odpovídající role:** Globální správce | Správce správy uživatelů

## <a name="why-you-need-a-work-account"></a>Proč potřebujete pracovní účet

Microsoft vyžaduje, abyste pracovní účet vaší společnosti propojují s novým Partnerské centrum účtem. Tento odkaz umožňuje uživatelům vašeho účtu přihlásit se k Partnerské centrum pomocí uživatelských jmen a hesel svých pracovních účtů.

## <a name="the-work-account-email-address"></a>E-mailová adresa pracovního účtu

Váš pracovní účet nebo pracovní e-mail je e-mailová adresa, kterou vám poskytla vaše společnost. E-mail pracovního účtu je obvykle ve formátu `you@yourcompany.com` . Osobní e-mailové adresy, jako je Hotmail, Gmail nebo Yahoo, nejsou pracovní e-maily a nelze je použít Partnerské centrum účtu.

Pokud máte více než jednu platnou pracovní e-mailovou adresu, použijte tu, která je přidružená k ústředí společnosti, a ne oblastní oddělení, například místo adresy použijte `contoso.com` `contoso.uk` e-mail.

> [!NOTE]  
> Než se rozhodnete použít existující pracovní účet, zamyslete se nad tím, kolik uživatelů v tomto účtu bude muset Partnerské centrum. Pokud máte v účtu uživatele, kteří nebudou muset pracovat v Partnerské centrum, zvažte vytvoření nového účtu jenom pro uživatele, kteří budou potřebovat pracovat v Partnerské centrum.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Nejste si jistí, jestli už vaše společnost má pracovní účet?

Pokud si nejste jistí, jestli má vaše společnost pracovní účet, postupujte podle těchto kroků a proveďte kontrolu. Pokud máte aktivní předplatné pro Microsoft Azure nebo Office 365, už máte pracovní účet.

1. Přihlaste se na [Azure Portal](https://portal.azure.com).

2. V Azure Active Directory vyberte Název domény a pak vyberte Názvy domén.

3. Pokud už máte pracovní účet, zobrazí se váš název domény.

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