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
ms.openlocfilehash: 673728ad03d6617fa60ba4119f0ebbbaaa4ce328
ms.sourcegitcommit: 98f5eebe7d08ba214ed5a078f1ac770439e41eb7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/31/2020
ms.locfileid: "93132959"
---
# <a name="security-requirements-status-report"></a>Zpráva o stavu požadavků na zabezpečení

**Platí pro**

- Všichni partneři v programu Cloud Solution Provider
- Všichni dodavatelé ovládacích panelů
- Všechny poradce

**Příslušné uživatele**
- Všichni povolení uživatelé včetně uživatelů typu Host

Tento článek popisuje zprávu o stavu požadavků na zabezpečení v partnerském centru. Tato sestava poskytuje metriky o dodržování [požadavků na zabezpečení partnerů](partner-security-requirements.md) pro službu Multi-Factor Authentication (MFA) pro uživatele v partnerském tenantovi.

Přístup k této sestavě v [partnerském centru](https://partner.microsoft.com/dashboard)získáte tak, že přejdete na **Nastavení**  >  **partner nastavení**  >  **stav požadavky zabezpečení** . Sestava se denně aktualizuje a odráží přihlašovací údaje za posledních sedm dní.

>[!NOTE]
>Zpráva o stavu požadavků zabezpečení je podporována pouze v partnerském centru. Není k dispozici v Microsoft Cloud pro státní správu USA ani pro Microsoft Cloud Německo. Důrazně doporučujeme, aby všichni partneři, kteří v rámci svrchovaného cloudu (USA a Německo) přijali tyto nové požadavky na zabezpečení okamžitě. Tito partneři ale v tuto chvíli nemusejí splňovat nové požadavky na zabezpečení. Microsoft nabídne další podrobnosti týkající se vynucování těchto požadavků na zabezpečení pro cloudy svrchovaného v budoucnu.

## <a name="security-status-metrics"></a>Metriky stavu zabezpečení

Zpráva o stavu požadavků na zabezpečení nabízí přehledy o implementaci MFA s partnerskými servery a poskytuje metriky pro konfiguraci MFA a aktivity partnerského centra u partnerských tenantů. Následující části podrobně popisují tyto metriky.

### <a name="mfa-configuration-on-a-partner-tenant"></a>Konfigurace MFA na partnerském tenantovi

**Procentuální podíl povolených uživatelských účtů s vyvynucovaném ověřováním MFA pomocí možností uvedených tady:** zobrazuje procento povolených uživatelských účtů na partnerském tenantovi, u kterých je vícefaktorové ověřování vynucované. K dosažení dodržování předpisů můžete použít jednu z těchto [možností vícefaktorového ověřování](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) . Tato data se zaznamenávají a nahlásí každý den. Například:

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
- Z 10 operací provedených v rámci 7 dnů byly dva uživatele s ověřováním MFA. Metrika proto zobrazuje 20%.

Pokud chcete zjistit, který uživatel se přihlásil k řídicímu panelu partnerského centra bez ověřování MFA a kdy se v okně generování sestav čas poslední návštěvy používá, můžete použít **požadavky na portál souborů bez MFA** .

#### <a name="appuser-mfa-verification"></a>Ověřování MFA aplikace a uživatele

Metrika **prostřednictvím rozhraní API nebo sady SDK** se v rámci požadavků na rozhraní API partnerského centra vztahuje k ověřování aplikací a uživatelů. Měří procento požadavků rozhraní API provedených pomocí přístupového tokenu s deklarací MFA. Například:

- Fabrikam je partner CSP a má aplikaci CSP, která používá kombinaci ověřování typu aplikace + uživatel a metody ověřování pouze aplikací.
- První den aplikace vytvořila tři požadavky rozhraní API, které byly zajištěny přístupovým tokenem získaným prostřednictvím metody ověřování pomocí aplikace + uživatel bez ověřování MFA.
- Druhý den aplikace provedla pět požadavků rozhraní API, které byly zajištěny přístupovým tokenem získaným pomocí ověřování pouze pro aplikace.
- Třetí den aplikace vytvořila dvě požadavky rozhraní API, které byly zajištěny přístupovým tokenem získaným pomocí metody ověřování pomocí aplikace + uživatel s ověřováním MFA.
- V žádném ze zbývajících čtyř dnů nebyly žádné operace provedené žádným agentem.
- Pět požadavků rozhraní API za druhý den, které byly zajištěny přístupovým tokenem získaným pomocí ověřování pouze pro aplikace, je z metriky vynecháno, protože nevyužívá přihlašovací údaje uživatele. Z zbylých pěti operací byly dva z nich zajištěny přístupovým tokenem získaným pomocí ověřování MFA. Metrika proto zobrazuje 40%.

Pokud chcete pochopit, které aplikace a aktivity uživatelů mají za následek, že v této metrikě nejsou 100%, použijte soubory:

- **Souhrn požadavků rozhraní API** pro pochopení celkového stavu MFA podle aplikace
- **Všechny požadavky rozhraní API** pro pochopení podrobností jednotlivých požadavků rozhraní API provedených uživateli vašeho tenanta je výsledkem omezení na maximum 10 000 nejnovějších žádostí o lepší stahování.

## <a name="actions-for-mfa-status-below-100"></a>Akce pro stav vícefaktorového ověřování pod 100%

Někteří partneři, kteří implementovali MFA, můžou zobrazit metriky sestav pod 100%. Tady je několik faktorů, které je potřeba vzít v úvahu.

> [!NOTE]
> Budete muset spolupracovat s někým z vaší organizace, který je obeznámen se správou identit a MFA pro vašeho partnerského tenanta.

### <a name="implemented-mfa-for-your-partner-tenant"></a>Implementované MFA pro vašeho partnerského tenanta

Aby bylo možné dosáhnout dodržování předpisů, je nutné implementovat MFA pro vašeho partnerského tenanta. Podrobnosti o tom, jak implementovat MFA, najdete v tématu [požadavky na zabezpečení při používání rozhraní API partnerského centra nebo partnerského centra](partner-security-requirements.md).

>[!NOTE]
> Metrika vícefaktorového ověřování se počítá každý den a bere v úvahu operace prováděné za posledních sedm dnů. Pokud jste pro partnerský tenant nedávno dokončili implementaci MFA, metriky ještě nemusí zobrazovat 100%.

### <a name="verify-mfa-on-all-user-accounts"></a>Ověření MFA u všech uživatelských účtů

Zjistěte, jestli vaše aktuální implementace MFA pokrývá všechny uživatelské účty nebo jenom některé. Některá řešení MFA jsou založená na zásadách a podporují vyloučení uživatelů, zatímco jiné můžou vyžadovat, abyste výslovně povolili vícefaktorové ověřování pro jednotlivé uživatele. Ověřte, že jste nevyloučili žádného uživatele z aktuální implementace MFA. Jakýkoli uživatelský účet, který je vyloučený a přihlásí se k partnerskému centru, aby mohl provádět jakékoli aktivity CSP, které souvisejí s poradcem, může způsobit, že metriky nebudou 100%.

### <a name="review-your-mfa-conditions"></a>Kontrola podmínek vícefaktorového ověřování

Zjistěte, jestli vaše aktuální implementace jenom MFA jenom jenom jenom za určitých podmínek. Některá řešení MFA poskytují flexibilitu, která vynutila MFA jenom při splnění určitých podmínek. Uživatel například přistupuje z neznámého zařízení nebo neznámého umístění. Uživatel, který je povolen pro MFA, ale není nutný k dokončení ověřování MFA při přístupu k partnerskému centru, může způsobit, že metriky nebudou 100%.

>[!NOTE]
>Pro partnery, kteří implementovali MFA pomocí výchozích hodnot zabezpečení Azure AD, je důležité si uvědomit, že služba Multi-Factor Authentication pro uživatele bez oprávnění správce se vynutila na základě rizika. Uživatelům se zobrazí výzva k MFA jenom během pokusů o rizikové přihlašování (třeba když se uživatel přihlásí z jiného místa). Kromě toho budou mít uživatelé až 14 dnů k registraci pro MFA. Uživatelům, kteří po dobu 14 dnů nedokončili registraci MFA, nebude pro ověřování MFA nahlášena žádná výzva. Proto je očekáváno, že metriky nemůžou být 100% pro partnery, kteří implementovali MFA pomocí výchozích hodnot zabezpečení Azure AD.

### <a name="review-third-party-mfa-configurations"></a>Kontrola konfigurací vícefaktorového ověřování třetích stran

Pokud používáte řešení MFA od jiného výrobce, zjistěte, jak ho Integrujte s Azure AD. Obecně existují dvě metody, včetně federace a vlastní ovládací prvky:

* **Federace identit** – když Azure AD obdrží požadavek na ověření, Azure AD přesměruje uživatele na federovaného zprostředkovatele identity pro ověřování. Po úspěšném ověření bude federovaný zprostředkovatel identit přesměrovat uživatele zpátky do služby Azure AD společně s tokenem SAML. Aby služba Azure AD rozpoznala, že při ověřování pro federovaného poskytovatele identity dokončila ověřování MFA, musí token SAML zahrnovat deklaraci *authenticationmethodsreferences* (s hodnotou *multipleauthn* ). Ověřte, zda zprostředkovatel federovaných identit podporuje vydávání takových deklarací identity. Pokud ano, ověřte, jestli je to tak, aby to provedla Konfigurace federovaného zprostředkovatele identity. Pokud chybí deklarace identity, Azure AD (a tudíž Partnerská centra) neví, že uživatel dokončil ověřování MFA a chybějící deklarace identity může způsobit, že metrika nebude 100%.

* **Vlastní ovládací prvek** – vlastní ovládací prvek Azure AD se nedá použít k určení toho, jestli uživatel dokončil ověřování MFA prostřednictvím řešení MFA třetí strany. V důsledku toho se všechny uživatele, kteří dokončili ověřování MFA prostřednictvím vlastního ovládacího prvku, budou vždycky zobrazovat do služby Azure AD (a v centru partnerských Center), protože neprošlé ověřováním MFA. Pokud je to možné, doporučujeme, abyste při integraci se službou Azure AD přepnuli na používání federace identit na rozdíl od vlastního řízení.

### <a name="identify-which-users-have-signed-in-to-partner-center-without-mfa"></a>Určení uživatelů přihlášených k partnerskému centru bez MFA

Může být užitečné určit, kteří uživatelé se přihlašují do partnerského centra bez ověřování MFA, a ověřit je proti vaší aktuální implementaci MFA. Pomocí [sestavy přihlášení k Azure AD](/azure/active-directory/reports-monitoring/concept-sign-ins) můžete zjistit, jestli uživatel dokončil ověřování MFA nebo ne. Sestava přihlášení k Azure AD je aktuálně dostupná jenom pro partnery, kteří se přihlásili k odběru Azure AD Premium nebo jakékoli SKU O365, což zahrnuje Azure AD Premium (například EMS).

## <a name="next-steps"></a>Další kroky

- [Komunita skupinových pokynů k zabezpečení partnerského centra](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [Požadavky na zabezpečení Partnerského centra](partner-security-requirements.md)
- [Nejčastější dotazy k požadavkům na zabezpečení partnerského centra](partner-security-requirements-faq.md)