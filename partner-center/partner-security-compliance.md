---
title: Zpráva o stavu požadavků na zabezpečení
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si, jak ověřit požadavky na zabezpečení v sestavě stav požadavků zabezpečení a sestavy MFA partnerského centra.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: e9ff61b34a9154cf305efbb42147e99b9579a17f
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686275"
---
# <a name="security-requirements-status-report"></a>Zpráva o stavu požadavků na zabezpečení

**Příslušné role**

- Správce CPV
- Globální správce

Tento článek popisuje zprávu o stavu požadavků na zabezpečení v partnerském centru. Tato sestava poskytuje metriky týkající se dodržování [požadavků na zabezpečení partnerů](partner-security-requirements.md) pro službu Multi-Factor Authentication (MFA) pro uživatele v partnerském tenantovi.

Přístup k této sestavě v [partnerském centru](https://partner.microsoft.com/dashboard)získáte tak, že přejdete na **Nastavení**  >  **účet nastavení**  >  **stav požadavky zabezpečení**. Sestava je denně aktualizována a odráží přihlašovací údaje za posledních sedm dní.

>[!NOTE]
>Zpráva o stavu požadavků zabezpečení je podporována pouze v partnerském centru. Není k dispozici v Microsoft Cloud pro státní správu USA ani pro Microsoft Cloud Německo. Důrazně doporučujeme, aby všichni partneři, kteří v rámci svrchovaného cloudu (USA a Německo) přijali tyto nové požadavky na zabezpečení okamžitě. Tito partneři ale v tuto chvíli nemusejí splňovat nové požadavky na zabezpečení. Microsoft nabídne další podrobnosti týkající se vynucování těchto požadavků na zabezpečení pro cloudy svrchovaného v budoucnu.

## <a name="security-status-metrics"></a>Metriky stavu zabezpečení

Zpráva o stavu požadavků na zabezpečení nabízí přehledy o implementaci MFA s partnerskými servery a poskytuje metriky pro konfiguraci MFA a aktivity partnerského centra u partnerských tenantů. Následující části podrobně popisují tyto metriky.

### <a name="mfa-configuration-on-a-partner-tenant"></a>Konfigurace MFA na partnerském tenantovi

**Procentuální podíl povolených uživatelských účtů s vyvynucovaném ověřováním MFA pomocí možností uvedených tady:** zobrazuje procento povolených uživatelských účtů na partnerském tenantovi, u kterých je vícefaktorové ověřování vynucované. K dosažení dodržování předpisů můžete použít jednu z těchto [možností vícefaktorového ověřování](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) . Tato data se zachytová a hlásí každý den. Například:

- Contoso je partner CSP se 110 uživatelskými účty v tenantovi a 10 z těchto uživatelských účtů je zakázaných. 
- Ze zbývajících 100 uživatelských účtů se více než 90 vynucuje pomocí [poskytnutých možností MFA.](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) Metrika proto zobrazuje 90 %. 

### <a name="partner-center-requests-with-mfa"></a>Partnerské centrum žádostí s více ověřováním

Pokaždé, když se Partnerské centrum k pracovnímu nebo prostřednictvím rozhraní API pokaždé, když se zaměstnanci přihlásí nebo odesílají data přes Partnerské centrum, je jejich stav zabezpečení zpochybněn a sledován. Součástí sledování stavu zabezpečení jsou také vaše aplikace a všechny aplikace dodavatelů ovládacích panelů. Tato data se zobrazují v metrikách v části **Percentage of requests to Partnerské centrum with MFA**(Procento požadavků na více než více ověřování) a odpovídají posledním sedmi dnům.

#### <a name="dashboard-mfa-verification"></a>Ověření MFA řídicího panelu

Metrika **Prostřednictvím Partnerské centrum Portal** souvisí s aktivitami v rámci Partnerské centrum řídicího panelu. Měří procento operací provedených uživateli, kteří dokončili ověřování MFA. Například:

- Contoso je partner CSP se dvěma agenty pro správu– Janou a Janem.
- První den se Jana přihlásila k řídicímu panelu Partnerské centrum bez ověření MFA a 3 operace.
- Druhý den se Jan přihlásil k řídicímu panelu Partnerské centrum ověřování MFA a provedl pět operací.
- Třetí den se Jana přihlásila k řídicímu panelu Partnerské centrum více ověřováním a 2 operacemi.
- Ve zbývajících čtyřech dnech žádný agent nesnídá žádné operace.
- Z 10 operací provedených v sedmidenním okně byly dvě provedeny uživatelem s ověřováním MFA. Metrika proto zobrazuje 20 %.

Pomocí souboru Požadavky portálu bez **MFA** můžete pochopit, který uživatel se přihlásil k řídicímu panelu Partnerské centrum bez nutnosti ověření MFA Partnerské centrum čas poslední návštěvy během okna vytváření sestav.

#### <a name="appuser-mfa-verification"></a>Ověřování MFA aplikace a uživatele

Metrika prostřednictvím **rozhraní API nebo sady SDK** souvisí s ověřováním aplikací a uživatelů prostřednictvím Partnerské centrum rozhraní API. Měří procento požadavků rozhraní API provedených pomocí přístupového tokenu s deklarací identity MFA. Například:

- Společnost Fabrikam je partner CSP a má aplikaci CSP, která využívá kombinaci metod ověřování aplikací a uživatelů a ověřování pouze pro aplikace.
- První den aplikace učinila tři požadavky rozhraní API, které byly podchyceny přístupový token získaný prostřednictvím metody ověřování aplikace a uživatele bez ověření MFA.
- Druhý den aplikace učinila pět požadavků rozhraní API, které byly podchyceny přístupový token získaným pomocí ověřování pouze pomocí aplikace.
- Třetí den aplikace učinila dvě žádosti rozhraní API, které byly podchyceny přístupový token získaný pomocí metody ověřování aplikace a uživatele s ověřováním MFA.
- Ve zbývajících čtyřech dnech žádný agent nesnídá žádné operace.
- Pět požadavků rozhraní API druhý den, které byly podchyceny přístupový token získaný prostřednictvím ověřování pouze pomocí aplikace, se z metriky vynecháno, protože nevyuděluje přihlašovací údaje uživatele. Ze zbývajících pěti operací byly dvě z nich podchyceny přístupový token získaný ověřením MFA. Metrika proto zobrazuje 40 %.

Pokud chcete pochopit, jaké aktivity aplikací a uživatelů mají za výsledek u této metriky 100 %, použijte soubory:

- **Souhrn požadavků rozhraní API** pro pochopení celkového stavu MFA podle aplikace
- **Všechny požadavky rozhraní API,** aby porozuměli podrobnostem o jednotlivých požadavcích rozhraní API provedených uživateli vašeho tenanta, je výsledek omezen na maximálně 10 000 nejnovějších požadavků pro lepší stahování.

## <a name="actions-for-mfa-status-below-100"></a>Akce pro stav MFA nižší než 100 %

Někteří partneři, kteří implementovali více než 100% metriky sestavy, můžou vidět. Pokud chcete pochopit, proč, tady je několik faktorů, které byste měli zvážit.

> [!NOTE]
> Budete muset spolupracovat s někým z vaší organizace, který zná správu identit a implementaci MFA pro vašeho partnerského tenanta.

### <a name="implemented-mfa-for-your-partner-tenant"></a>Implementace MFA pro partnerského tenanta

Abyste dosáhli dodržování předpisů, musíte pro svého partnerského tenanta implementovat MFA. Podrobnosti o tom, jak implementovat MFA, najdete v tématu [požadavky na zabezpečení při používání rozhraní API partnerského centra nebo partnerského centra](partner-security-requirements.md).

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

* **Federace identit** – Když Azure AD obdrží žádost o ověření, Azure AD přesměruje uživatele k ověření na zprostředkovatele federované identity. Po úspěšném ověření přesměruje zprostředkovatel federované identity uživatele zpět do Azure AD spolu s tokenem SAML. Aby služba Azure AD při ověřování u federovaného zprostředkovatele identity rozpoznala, že uživatel dokončil ověření MFA, musí token SAML obsahovat deklaraci identity *authenticationmethodsreferences* (s hodnotou *multipleauthn).* Zkontrolujte, jestli federovaný zprostředkovatel identity podporuje vystavování takové deklarace identity. Pokud ano, zkontrolujte, jestli je k tomu nakonfigurovaný zprostředkovatel federované identity. Pokud deklarace identity chybí, Azure AD (a tedy Partnerské centrum) nebude vědět, že uživatel dokončil vícekoncerové ověřování a chybějící deklarace identity může způsobit, že metrika nebude 100 %.

* **Vlastní ovládací** prvek – Vlastní ovládací prvek Azure AD není možné použít k identifikaci, jestli uživatel dokončil ověření MFA prostřednictvím řešení MFA třetí strany. V důsledku toho se každý uživatel, který dokončil ověření MFA prostřednictvím vlastního ovládacího prvku, vždy zobrazí službě Azure AD (a zase Partnerské centrum) jako uživatel, který ještě neskončil ověření MFA. Pokud je to možné, doporučujeme při integraci se službou Azure AD přepnout na používání federace identit místo na vlastní řízení.

### <a name="identify-which-users-have-signed-in-to-partner-center-without-mfa"></a>Identifikace uživatelů, kteří se přihlásili k Partnerské centrum bez MFA

Může být užitečné zjistit, kteří uživatelé se přihlašují k Partnerské centrum ověřování MFA, a ověřit je v aktuální implementaci MFA. Pomocí sestavy [přihlášení k Azure AD](/azure/active-directory/reports-monitoring/concept-sign-ins) můžete zjistit, jestli uživatel dokončil nebo ne. Sestava přihlašování k Azure AD je v současné době dostupná jenom pro partnery, kteří si předplatili Azure AD Premium nebo jakoukoli skladové prostředky O365, která zahrnuje Azure AD Premium (například EMS).

## <a name="next-steps"></a>Další kroky

- [Partnerské centrum komunity skupin bezpečnostních pokynů](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [Požadavky na zabezpečení Partnerského centra](partner-security-requirements.md)
- [Partnerské centrum požadavky na zabezpečení](partner-security-requirements-faq.md)
