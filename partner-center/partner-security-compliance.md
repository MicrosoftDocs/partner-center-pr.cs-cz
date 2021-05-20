---
title: Sestava stavu požadavků na zabezpečení
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak zkontrolovat dodržování požadavků na zabezpečení pomocí sestavy stavu požadavků na zabezpečení a Partnerské centrum MFA.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: c9bba02744d466741d7625b1624995084c0a3492
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152558"
---
# <a name="security-requirements-status-report"></a>Sestava stavu požadavků na zabezpečení

**Odpovídající role:** Správce CPV | Globální správce

Tento článek vysvětluje sestavu stavu požadavků na zabezpečení v Partnerské centrum. Tato sestava poskytuje metriky [](partner-security-requirements.md) týkající se dodržování požadavků na zabezpečení partnerů pro vícefaktorové ověřování (MFA) pro uživatele ve vašem partnerském tenantovi.

Pokud chcete získat přístup k [této sestavě Partnerské centrum](https://partner.microsoft.com/dashboard), přejděte na **Nastavení** Nastavení  >  **Nastavení účtu** Stav požadavků na  >  **zabezpečení.** Sestava se aktualizuje každý den a bude odrážet přihlašovací data z posledních sedmi dnů.

>[!NOTE]
>Sestava stavu požadavků na zabezpečení je podporována pouze v Partnerské centrum. Není k dispozici ve službě Microsoft Cloud for US Government Microsoft Cloud Germany. Důrazně doporučujeme, aby všichni partneři, kteří provádí transakce prostřednictvím suverénního cloudu (státní správa USA a Německo), přijali tyto nové požadavky na zabezpečení okamžitě. Tito partneři se ale v současné době ke splnění nových požadavků na zabezpečení nepožaduje. Microsoft v budoucnu poskytne další podrobnosti týkající se vynucování těchto požadavků na zabezpečení pro suverénní cloudy.

## <a name="security-status-metrics"></a>Metriky stavu zabezpečení

Sestava stavu požadavků na zabezpečení nabízí přehled o implementaci partnerského MFA a poskytuje metriky o konfiguraci MFA a Partnerské centrum aktivitách v partnerských tenantech. V následujících částech jsou tyto metriky podrobněji vysvětleny.

### <a name="mfa-configuration-on-a-partner-tenant"></a>Konfigurace MFA v partnerském tenantovi

Metrika Procento povolených uživatelských účtů s vynucením MFA pomocí možností uvedených **tady:** Zobrazuje procento povolených uživatelských účtů ve vašem partnerském tenantovi, které vynucuje více ověřování. K zajištění dodržování předpisů můžete použít jednu z těchto [možností MFA.](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) Tato data se zachytová a hlásí každý den. Například:

- Contoso je partner CSP s 110 uživatelskými účty v tenantovi, 10 z těchto uživatelských účtů je zakázané. 
- Z dalších 100 uživatelských účtů, 90 se vynutilo MFA pomocí zadaných [možností MFA](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started). Metrika proto zobrazuje 90%. 

### <a name="partner-center-requests-with-mfa"></a>Žádosti partnerského centra s MFA

Pokaždé, když se vaši zaměstnanci přihlásí do partnerského centra, aby mohli pracovat nebo, prostřednictvím rozhraní API, získávat nebo odesílat data prostřednictvím partnerského centra, jejich stav zabezpečení je výzva a sledování. Je také součástí zabezpečení – sledování stavu jsou vaše aplikace a libovolné aplikace od dodavatele ovládacích panelů. Tato data se zobrazují v metrikách v **procentech požadavků do partnerského centra s MFA** a zobrazují se v posledních sedmi dnech.

#### <a name="dashboard-mfa-verification"></a>Ověření MFA řídicího panelu

Metrika **prostřednictvím portálu partnerského centra** souvisí s aktivitami v řídicím panelu partnerského centra. Měří procentuální podíl operací provedených uživateli, kteří dokončili ověřování MFA. Například:

- Contoso je partner CSP se dvěma agenty pro správu, Jana a Jan.
- První den, Jana přihlášený k řídicímu panelu partnerského centra bez ověřování MFA a provedl tři operace.
- Druhý den se Jan přihlásil k řídicímu panelu partnerského centra bez ověřování MFA a provedl pět operací.
- Třetí den jste přihlásili do řídicího panelu partnerského centra pomocí ověřování MFA a provedli dvě operace.
- V žádném ze zbývajících čtyř dnů nebyly žádné operace provedené žádným agentem.
- Po 10 operacích provedených v sedmi dnech se uživateli provedlo ověřování MFA. Metrika proto zobrazuje 20%.

Pokud chcete zjistit, který uživatel se přihlásil k řídicímu panelu partnerského centra bez ověřování MFA a kdy se v okně generování sestav čas poslední návštěvy používá, můžete použít **požadavky na portál souborů bez MFA** .

#### <a name="appuser-mfa-verification"></a>Ověřování MFA aplikace a uživatele

Metrika **prostřednictvím rozhraní API nebo sady SDK** se v rámci požadavků na rozhraní API partnerského centra vztahuje k ověřování aplikací a uživatelů. Měří procento požadavků rozhraní API provedených pomocí přístupového tokenu s deklarací identity MFA. Například:

- Společnost Fabrikam je partner CSP a má aplikaci CSP, která používá kombinaci metod ověřování aplikací a uživatelů a ověřování pouze pro aplikace.
- První den aplikace učinila tři požadavky rozhraní API, které byly podchyceny přístupový token získaný prostřednictvím metody ověřování aplikace a uživatele bez ověření MFA.
- Druhý den aplikace učinila pět požadavků rozhraní API, které byly podchyceny přístupový token získaným pomocí ověřování pouze pomocí aplikace.
- Třetí den aplikace učinila dvě žádosti rozhraní API, které byly podchyceny přístupový token získaný pomocí metody ověřování aplikace a uživatele s ověřováním MFA.
- Žádný agent ve zbývajících čtyřech dnech nesnídá žádné operace.
- Pět požadavků rozhraní API druhý den, které byly podchyceny přístupový token získaný prostřednictvím ověřování pouze pomocí aplikace, se z metriky vynecháno, protože nevyuděluje přihlašovací údaje uživatele. Ze zbývajících pěti operací byly dvě z nich zálohovány pomocí přístupového tokenu získaného ověřením MFA. Metrika proto zobrazuje 40 %.

Pokud chcete pochopit, jaké aktivity aplikací a uživatelů mají za výsledek u této metriky 100 %, použijte soubory:

- **Souhrn požadavků rozhraní API** pro pochopení celkového stavu MFA podle aplikace
- **Všechny požadavky rozhraní API,** aby porozuměli podrobnostem o jednotlivých požadavcích rozhraní API provedených uživateli vašeho tenanta, je výsledek omezen na maximálně 10 000 nejnovějších požadavků pro lepší stahování.

## <a name="actions-for-mfa-status-below-100"></a>Akce pro stav MFA nižší než 100 %

Někteří partneři, kteří implementovali více než 100% metriky sestavy, můžou vidět. Pokud chcete pochopit, proč, tady je několik faktorů, které byste měli zvážit.

> [!NOTE]
> Budete muset spolupracovat s někým z vaší organizace, který zná správu identit a implementaci MFA pro vašeho partnerského tenanta.

### <a name="implemented-mfa-for-your-partner-tenant"></a>Implementace MFA pro partnerského tenanta

Abyste dosáhli dodržování předpisů, musíte implementovat MFA pro vašeho partnerského tenanta. Podrobnosti o tom, jak implementovat MFA, najdete v tématu [požadavky na zabezpečení při používání rozhraní API partnerského centra nebo partnerského centra](partner-security-requirements.md).

>[!NOTE]
> Metrika vícefaktorového ověřování se počítá každý den a bere v úvahu operace prováděné za posledních sedm dnů. Pokud jste pro partnerský tenant nedávno dokončili implementaci MFA, metriky ještě nemusí zobrazovat 100%.

### <a name="verify-mfa-on-all-user-accounts"></a>Ověření MFA u všech uživatelských účtů

Zjistěte, jestli vaše aktuální implementace MFA pokrývá všechny uživatelské účty nebo jenom některé. Některá řešení MFA jsou založená na zásadách a podporují vyloučení uživatelů, zatímco jiné můžou vyžadovat, abyste výslovně povolili vícefaktorové ověřování pro jednotlivé uživatele. Ověřte, že jste nevyloučili žádného uživatele z aktuální implementace MFA. Jakýkoli uživatelský účet, který je vyloučený a přihlásí se k partnerskému centru, aby mohl provádět jakékoli aktivity CSP, které souvisejí s poradcem, může způsobit, že metriky nebudou 100%.

### <a name="review-your-mfa-conditions"></a>Kontrola podmínek vícefaktorového ověřování

Zjistěte, jestli vaše aktuální implementace jenom MFA jenom jenom jenom za určitých podmínek. Některá řešení MFA poskytují flexibilitu, která vynutila MFA jenom při splnění určitých podmínek. Uživatel například přistupuje z neznámého zařízení nebo neznámého umístění. Uživatel, který je povolen pro MFA, ale není nutný k dokončení ověřování MFA při přístupu k partnerskému centru, může způsobit, že metriky nebudou 100%.

>[!NOTE]
>Pro partnery, kteří implementovali MFA pomocí výchozích hodnot zabezpečení Azure AD, je důležité si uvědomit, že služba Multi-Factor Authentication pro uživatele bez oprávnění správce se vynutila na základě rizika. Uživatelům se zobrazí výzva k MFA jenom během pokusů o rizikové přihlašování (třeba když se uživatel přihlásí z jiného místa). Kromě toho budou mít uživatelé až 14 dnů k registraci pro MFA. Uživatelům, kteří po dobu 14 dnů nedokončili registraci MFA, nebude pro ověřování MFA nahlášena žádná výzva. Proto je očekáváno, že metriky nemůžou být 100% pro partnery, kteří implementovali MFA pomocí výchozích hodnot zabezpečení Azure AD.

### <a name="review-third-party-mfa-configurations"></a>Kontrola konfigurací vícefaktorového ověřování třetích stran

Pokud používáte řešení MFA třetí strany, zjistěte, jak ho integrujete s Azure AD. Obecně existují dvě metody, včetně federace a vlastních ovládacích prvků:

* **Federace identit** – Když Azure AD obdrží žádost o ověření, přesměruje Azure AD uživatele k ověření na zprostředkovatele federované identity. Po úspěšném ověření přesměruje zprostředkovatel federované identity uživatele zpět do Azure AD spolu s tokenem SAML. Aby služba Azure AD při ověřování u federovaného zprostředkovatele identity rozpoznala, že uživatel dokončil ověření MFA, musí token SAML obsahovat deklaraci identity *authenticationmethodsreferences* (s hodnotou *multipleauthn).* Zkontrolujte, jestli federovaný zprostředkovatel identity podporuje vystavování takové deklarace identity. Pokud ano, zkontrolujte, jestli je k tomu nakonfigurovaný zprostředkovatel federované identity. Pokud deklarace identity chybí, Azure AD (a tedy Partnerské centrum) nebude vědět, že uživatel dokončil ověření MFA a chybějící deklarace identity může způsobit, že metrika nebude 100 %.

* **Vlastní ovládací** prvek – Vlastní ovládací prvek Azure AD není možné použít k identifikaci, jestli uživatel dokončil ověření MFA prostřednictvím řešení MFA třetí strany. V důsledku toho se každý uživatel, který dokončil ověření MFA prostřednictvím vlastního ovládacího prvku, vždy zobrazí službě Azure AD (a zase Partnerské centrum), jako by neskončil ověření MFA. Pokud je to možné, doporučujeme při integraci se službou Azure AD přepnout na používání federace identit místo na vlastní řízení.

### <a name="identify-which-users-have-signed-in-to-partner-center-without-mfa"></a>Identifikace uživatelů, kteří se přihlásili k Partnerské centrum bez MFA

Může být užitečné zjistit, kteří uživatelé se přihlašují k Partnerské centrum ověřování MFA, a ověřit je v aktuální implementaci MFA. Pomocí sestavy [přihlášení k Azure AD](/azure/active-directory/reports-monitoring/concept-sign-ins) můžete zjistit, jestli uživatel dokončil nebo ne. Sestava přihlášení k Azure AD je aktuálně dostupná jenom pro partnery, kteří se přihlásili k odběru Azure AD Premium nebo jakékoli SKU O365, což zahrnuje Azure AD Premium (například EMS).

## <a name="next-steps"></a>Další kroky

- [Komunita skupinových pokynů k zabezpečení partnerského centra](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [Požadavky na zabezpečení Partnerského centra](partner-security-requirements.md)
- [Nejčastější dotazy k požadavkům na zabezpečení partnerského centra](partner-security-requirements-faq.md)
