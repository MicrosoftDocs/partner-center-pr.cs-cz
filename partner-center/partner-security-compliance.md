---
title: Stav požadavků na zabezpečení partnerů
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si o nových povinných požadavcích, které zvyšují zabezpečení pro poradce, dodavatele ovládacích panelů a partnery v programu Cloud Solution Provider.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: 1b6c2d56a0747ddf2bd1a821886e371ed698a4a1
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/22/2020
ms.locfileid: "92527323"
---
# <a name="partner-security-requirements-status---get-answers-and-check-reports-about-current-status"></a>Stav požadavků na zabezpečení partnerů – získat odpovědi a kontrolovat zprávy o aktuálním stavu

**Platí pro**

- Všichni partneři v programu Cloud Solution Provider
  - Přímá faktura
  - Nepřímý poskytovatel
  - Nepřímý prodejce
- Všichni dodavatelé ovládacích panelů
- Všechny poradce

**Příslušné uživatele**
- Všichni povolení uživatelé včetně uživatelů typu Host

Vyšší zabezpečení ochrany osobních údajů a zabezpečení je z našich nejdůležitějších priorit. Víme, že nejlepší obrana je prevence a že máme jenom silný, jako náš slabý odkaz. Proto potřebujeme, aby všichni v našem ekosystému pracovali a zajistili, že mají správné bezpečnostní ochrany. Abychom vám pomohli chránit partnery a zákazníky, zavádíme sadu povinných požadavků na zabezpečení pro poradce, dodavatele ovládacích panelů a partnery účastnící se programu Cloud Solution Provider.

Od 1. srpna 2019 musí všichni partneři vymáhat službu Multi-Factor Authentication pro všechny uživatele, včetně účtů služeb ve svém partnerském tenantovi. Podrobnější informace o nových zásadách zabezpečení najdete v článku [požadavky na zabezpečení partnera](partner-security-requirements.md).

Chceme zajistit, aby každý uživatel měl výzvu MFA pro každé jedno ověření. Toto prostředí je možné provést jedním z následujících způsobů:

- Implementace Azure AD Premium, aby se zajistilo, že se pro každého uživatele vynutilo vícefaktorové ověřování.
- Implementace [výchozích hodnot zabezpečení Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- Implementace řešení třetí strany, aby se zajistilo, že se MFA pro každého uživatele vynutilo.

## <a name="partner-security-requirements-status"></a>Stav požadavků na zabezpečení partnerů

Tato sestava vám může pomáhat s ověřením stavu požadavků na zabezpečení tím, že poskytuje způsob, jak zjistit, kde může být krátká. Sledování se pravidelně aktualizuje.

>[!NOTE]
>Zpráva o stavu požadavků na zabezpečení partnerů je podporovaná jenom v partnerském centru. Není k dispozici v Microsoft Cloud pro státní správu USA ani pro Microsoft Cloud Německo. Důrazně doporučujeme, aby všichni partneři, kteří v rámci svrchovaného cloudu (21Vianet, státní správa USA a Německo) přijali tyto nové požadavky na zabezpečení hned. Tito partneři ale nemusejí splňovat nové požadavky na zabezpečení, které platí od 1. srpna 2019. Microsoft nabídne další podrobnosti týkající se vynucování těchto požadavků na zabezpečení pro cloudy svrchovaného v budoucnu.

## <a name="multi-factor-authentication-mfa-report"></a>Sestava Multi-Factor Authentication ("MFA")

Sestava pro partnerský server v partnerském centru nabízí přehledy o implementaci MFA partnerských serverů tím, že poskytuje dva typy metrik založené na aktivitách konfigurace MFA a partnerského centra tenanta CSP: 

### <a name="mfa-configuration-on-a-csp-tenant"></a>Konfigurace MFA na tenantovi CSP

Tato metrika souvisí s konfigurací MFA v tenantovi CSP, který se každý den zachycuje a nahlásil. Měří procento povolených uživatelských účtů s vyvynucované MFA pomocí kterékoli z těchto [možností MFA](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started). Například:

- Contoso je partner CSP s 110 uživatelskými účty v tenantovi, 10 z těchto uživatelských účtů je zakázané. 
- Z dalších 100 uživatelských účtů, 90 se vynutilo MFA pomocí zadaných [možností MFA](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started). Metrika proto zobrazuje 90%. 

### <a name="partner-center-activities-with-mfa"></a>Aktivity partnerského centra s MFA

Pokaždé, když se vaši zaměstnanci přihlásí do partnerského centra, aby mohli pracovat nebo, prostřednictvím rozhraní API, získávat nebo odesílat data prostřednictvím partnerského centra, jejich stav zabezpečení je výzva a sledování. V rámci sledování stavu zabezpečení jsou také zahrnuty aplikace a aplikace dodavatele ovládacích panelů. Zobrazený stav je během posledních sedmi dnů.

#### <a name="mfa-verification-completed-by-users"></a>Ověřování MFA bylo dokončeno uživateli

Tato metrika se vztahuje k aktivitám v rámci řídicího panelu partnerského centra. Měří procentuální podíl operací provedených uživateli, kteří dokončili ověřování MFA. Například:

- Contoso je partner CSP se dvěma agenty pro správu, Jana a Jan.
- První den, Jana přihlášený k řídicímu panelu partnerského centra bez ověřování MFA a provedl tři operace.
- Druhý den se Jan přihlásil k řídicímu panelu partnerského centra bez ověřování MFA a provedl pět operací.
- Třetí den jste přihlásili do řídicího panelu partnerského centra pomocí ověřování MFA a provedli dvě operace.
- V žádném ze zbývajících čtyř dnů nebyly žádné operace provedené žádným agentem.
- Z 10 operací provedených v rámci 7 dnů byly dva uživatele s ověřováním MFA. Metrika proto zobrazuje 20%.

Pokud chcete zjistit, který uživatel se přihlásil k řídicímu panelu partnerského centra bez ověřování MFA a kdy se v okně generování sestav čas poslední návštěvy používá, můžete použít **požadavky na portál souborů bez MFA** .

#### <a name="appuser-authentication"></a>Ověřování aplikací a uživatelů

Tato metrika se vztahuje k použití požadavků rozhraní API partnerského centra provedených pomocí ověřování aplikací a uživatelů. Měří procento požadavků rozhraní API provedených pomocí přístupového tokenu s deklarací MFA. Například:

- Fabrikam je partner CSP a má aplikaci CSP, která používá kombinaci ověřování typu aplikace + uživatel a metody ověřování pouze aplikací.
- První den aplikace vytvořila tři požadavky rozhraní API, které byly zajištěny přístupovým tokenem získaným prostřednictvím metody ověřování pomocí aplikace + uživatel bez ověřování MFA.
- Druhý den aplikace provedla pět požadavků rozhraní API, které byly zajištěny přístupovým tokenem získaným pomocí ověřování pouze pro aplikace.
- Třetí den aplikace vytvořila dvě požadavky rozhraní API, které byly zajištěny přístupovým tokenem získaným pomocí metody ověřování pomocí aplikace + uživatel s ověřováním MFA.
- V žádném ze zbývajících čtyř dnů nebyly žádné operace provedené žádným agentem.
- Pět požadavků rozhraní API za druhý den, které byly zajištěny přístupovým tokenem získaným pomocí ověřování pouze pro aplikace, je z metriky vynecháno, protože nevyužívá přihlašovací údaje uživatele. Z zbylých pěti operací byly dva z nich zajištěny přístupovým tokenem získaným pomocí ověřování MFA. Metrika proto zobrazuje 40%.

Pokud chcete pochopit, které aplikace a aktivity uživatelů mají za následek, že v této metrikě nejsou 100%, použijte soubory:

- **Souhrn požadavků rozhraní API** pro pochopení celkového stavu MFA podle aplikace
- **Všechny požadavky rozhraní API** pro pochopení podrobností jednotlivých požadavků rozhraní API provedených uživateli vašeho tenanta je výsledkem omezení na maximum 10 000 nejnovějších žádostí o lepší stahování.

## <a name="what-should-i-do-if-the-metrics-under-mfa-report-arent-100"></a>Co mám dělat, pokud metriky v sestavě MFA nejsou 100%

Je možné, že metriky ve zprávě partnerského centra MFA nemůžou být 100% pro partnery, kteří implementovali MFA. Tady je několik faktorů, které je potřeba vzít v úvahu.

> [!NOTE]
> Budete muset spolupracovat s někým z vaší organizace, který je obeznámen se správou identit a MFA pro vašeho partnerského tenanta.

### <a name="have-you-implemented-mfa-for-your-partner-tenant"></a>Implementovali jste MFA pro vašeho partnerského tenanta?

V takovém případě je nutné nejprve implementovat vícefaktorové ověřování pro partnerský tenant. Podrobnosti o tom, jak implementovat MFA, najdete v článku [požadavky na zabezpečení partnera](partner-security-requirements.md).

### <a name="have-you-only-recently-completed-mfa-implementation"></a>Dokončili jste jenom poslední implementaci MFA?

Metrika se počítá každý den a bere v úvahu operace provedené během posledních sedmi dnů. Pokud jste pro partnerský tenant nedávno dokončili implementaci MFA, metriky nemusí být 100%.

### <a name="have-some-user-accounts-been-excluded-from-mfa-implementation"></a>Byly některé uživatelské účty vyloučené z implementace MFA?

Zjistěte, jestli vaše aktuální implementace MFA pokrývá všechny uživatelské účty nebo jenom některé. Některá řešení MFA jsou založená na zásadách a podporují vyloučení uživatelů, zatímco jiné můžou vyžadovat, abyste výslovně povolili vícefaktorové ověřování pro jednotlivé uživatele. Ověřte, že jste nevyloučili žádného uživatele z aktuální implementace MFA. Jakýkoli uživatelský účet, který je vyloučený a přihlásí se k partnerskému centru k provedení jakékoli aktivity související s CSP, může způsobit, že metriky nebudou 100%.

### <a name="is-mfa-only-required-when-certain-conditions-are-met"></a>Vyžaduje se MFA jenom v případě, že jsou splněné určité podmínky?

Zjistěte, jestli vaše aktuální implementace jenom MFA jenom jenom jenom za určitých podmínek. Některá řešení MFA poskytují flexibilitu, která vynutila MFA jenom při splnění určitých podmínek. Uživatel například přistupuje z neznámého zařízení nebo neznámého umístění. Uživatel, který je povolen pro MFA, ale není nutný k dokončení ověřování MFA při přístupu k partnerskému centru, může způsobit, že metriky nebudou 100%.

>[!NOTE]
>Pro partnery, kteří implementovali MFA pomocí výchozích hodnot zabezpečení Azure AD, je důležité si uvědomit, že služba Multi-Factor Authentication pro uživatele bez oprávnění správce se vynutila na základě rizika. Uživatelům se zobrazí výzva k MFA jenom během pokusů o rizikové přihlašování (třeba když se uživatel přihlásí z jiného místa). Kromě toho budou mít uživatelé až 14 dnů k registraci pro MFA. Uživatelům, kteří po dobu 14 dnů nedokončili registraci MFA, nebude pro ověřování MFA nahlášena žádná výzva. Proto je očekáváno, že metriky nemůžou být 100% pro partnery, kteří implementovali MFA pomocí výchozích hodnot zabezpečení Azure AD.

### <a name="are-you-using-third-party-mfa-solution"></a>Používáte řešení MFA od jiného výrobce?

Pokud používáte řešení MFA od jiného výrobce, zjistěte, jak ho Integrujte s Azure AD. Obecně existují dvě metody, včetně federace a vlastní ovládací prvky:

* **Federace identit** – když Azure AD obdrží požadavek na ověření, Azure AD přesměruje uživatele na federovaného zprostředkovatele identity pro ověřování. Po úspěšném ověření bude federovaný zprostředkovatel identit přesměrovat uživatele zpátky do služby Azure AD společně s tokenem SAML. Aby služba Azure AD rozpoznala, že při ověřování pro federovaného poskytovatele identity dokončila ověřování MFA, musí token SAML zahrnovat deklaraci *authenticationmethodsreferences* (s hodnotou *multipleauthn* ). Ověřte, zda zprostředkovatel federovaných identit podporuje vydávání takových deklarací identity. Pokud ano, ověřte, jestli je to tak, aby to provedla Konfigurace federovaného zprostředkovatele identity. Pokud chybí deklarace identity, Azure AD (a tudíž Partnerská centra) neví, že uživatel dokončil ověřování MFA a chybějící deklarace identity může způsobit, že metrika nebude 100%.

* **Vlastní ovládací prvek** – vlastní ovládací prvek Azure AD se nedá použít k určení toho, jestli uživatel dokončil ověřování MFA prostřednictvím řešení MFA třetí strany. V důsledku toho se všechny uživatele, kteří dokončili ověřování MFA prostřednictvím vlastního ovládacího prvku, budou vždycky zobrazovat do služby Azure AD (a v centru partnerských Center), protože neprošlé ověřováním MFA. Pokud je to možné, doporučujeme, abyste při integraci se službou Azure AD přepnuli na používání federace identit na rozdíl od vlastního řízení.

### <a name="identify-which-users-have-logged-into-partner-center-without-mfa"></a>Určení uživatelů přihlášených k partnerskému centru bez MFA

Může být užitečné určit, kteří uživatelé se přihlašují do partnerského centra bez ověřování MFA, a ověřit je proti vaší aktuální implementaci MFA. Pomocí [sestavy přihlášení k Azure AD](/azure/active-directory/reports-monitoring/concept-sign-ins) můžete zjistit, jestli uživatel dokončil ověřování MFA nebo ne. Sestava přihlášení k Azure AD je aktuálně dostupná jenom pro partnery, kteří se přihlásili k odběru Azure AD Premium nebo jakékoli SKU O365, což zahrnuje Azure AD Premium (například EMS).

## <a name="next-steps"></a>Další kroky

- [Komunita skupinových pokynů k zabezpečení partnerského centra](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [Požadavky na zabezpečení partnerského centra](partner-security-requirements.md)
- [Nejčastější dotazy k požadavkům na zabezpečení partnerského centra](partner-security-requirements-faq.md)