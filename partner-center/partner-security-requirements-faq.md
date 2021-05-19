---
title: Nejčastější dotazy k požadavkům na zabezpečení partnerů
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Nejčastější dotazy týkající se požadavků na zabezpečení partnerů – co to jsou, jak by je partneři měli implementovat a jak víte, jestli jste je splnili.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 174c56ce9bb5fb3d9d92c1ef18af73479619f4bb
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110145877"
---
# <a name="common-questions-about-partner-security-requirements"></a>Běžné dotazy týkající se požadavků na zabezpečení partnerů

**Odpovídající role:** Všichni Partnerské centrum uživatele

V tomto článku najdete odpovědi na některé běžné dotazy týkající se [požadavků na zabezpečení partnerů.](partner-security-requirements.md)

### <a name="what-are-the-partner-security-requirements-and-why-should-partners-implement-them"></a>Jaké jsou požadavky na zabezpečení partnerů a proč by je partneři měli implementovat?

Mezi naše hlavní priority patří větší a průběžná ochrana zabezpečení a ochrany osobních údajů a pomáháme partnerům chránit jejich zákazníky a tenanty. I nadále vidíme sofistikovanější a rostoucí počet útoků na zabezpečení, které souvisí především s incidenty ohrožení identity. Protože preventivní kontroly hrají klíčovou roli v celkové strategii ochrany před útoky na zabezpečení, zavedli jsme povinné požadavky na zabezpečení [v](partner-security-requirements.md) roce 2019. Všichni partneři účastnící se Cloud Solution Provider (CSP), Ovládací panely Vendors a Advisors musí implementovat požadavky na dodržování předpisů.

### <a name="what-are-the-key-timelines-and-milestones"></a>Jaké jsou klíčové časové osy a milníky?

Podmínky spojené s těmito požadavky na zabezpečení, včetně časových os a milníků, jsou součástí [Smlouva s partnerem Microsoftu](microsoft-partner-agreement.md). Tyto požadavky na zabezpečení budete muset implementovat co nejdříve, abyste měli podchycený vaši účast v programu CSP.

### <a name="what-will-happen-if-i-dont-implement-these-partner-security-requirements"></a>Co se stane, když tyto požadavky na zabezpečení partnerů neimplementuje?

Tento Smlouva s partnerem Microsoftu vyžaduje vynucení vícefaktorového ověřování pro uživatelské účty a použití zabezpečeného aplikačního modelu pro interakci s rozhraním PARTNERSKÉ CENTRUM API. 

Partneři, kteří se těmito postupy zabezpečení nevěnují, mohou ztratit svou schopnost provádět transakce v programu CSP nebo spravovat tenanty zákazníků pomocí práv delegovaného správce.

### <a name="do-the-security-requirements-apply-to-all-geographies"></a>Vztahují se požadavky na zabezpečení na všechny zeměpisné oblasti?

Ano, požadavky na zabezpečení se vztahují na všechny zeměpisné oblasti. Důrazně doporučujeme, aby všichni partneři procházeli prostřednictvím svrchovaného cloudu (vlády USA a Německa) a okamžitě přijali tyto nové požadavky na zabezpečení. Tito partneři ale momentálně nevyžadují splnění požadavků na zabezpečení. Microsoft nabídne další podrobnosti týkající se vynucování těchto požadavků na zabezpečení pro cloudy svrchovaného v budoucnu.

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>Je možné získat pro účet vyloučení?

Ne, z požadavku na vynucení vícefaktorového ověřování (MFA) není možné vyloučit žádný uživatelský účet. S ohledem na vysoce privilegovaný charakter je Partnerská smlouva Microsoftu vyžaduje, aby se pro každý uživatelský účet ve vašem partnerském tenantovi vynutilo ověřování pomocí služby Multi-Factor Authentication.

### <a name="how-do-i-know-if-i-have-met-the-partner-security-requirements"></a>Návody vědět, jestli splňujem požadavky na zabezpečení partnera?

Dokončete následující kroky:

- Musíte splnit všechny požadavky, které jsou uvedené v požadavcích na [zabezpečení partnera](partner-security-requirements.md).
- Je potřeba zajistit, aby všechny uživatelské účty ve vašem partnerském tenantovi vynutily službu Multi-Factor Authentication.

Abychom vám pomohli identifikovat klíčové oblasti, kde můžete provádět akce, poskytujeme [zprávu o stavu požadavků na zabezpečení](https://partner.microsoft.com/commerce/security/compliance) , která je k dispozici prostřednictvím partnerského centra.

Další informace o zprávě o stavu najdete v tématu [stav požadavků na zabezpečení partnerů](partner-security-compliance.md).

## <a name="required-actions"></a>Požadované akce

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>Jaké jsou klíčové akce, které je potřeba provést, aby se splnily požadavky?

Všichni partneři v programu CSP (přímá fakturace, nepřímý poskytovatel a nepřímý prodejce), poradci a dodavatelé ovládacích panelů musí splňovat požadavky.

1. **Vymáhat MFA pro všechny uživatele**

    Všichni partneři v programu CSP, poradci a v Ovládacích panelech musí vymáhat MFA pro všechny uživatele v partnerském tenantovi.

    Další rozhodnutí:

    - Neposkytovatelé nepřímých zprostředkovatelů potřebují spolupracovat s nepřímými prodejci, kteří se dostanou do partnerského centra, pokud je ještě neudělali, a nepodporují jejich prodejce, aby splnili požadavky.
    - Azure MFA je zdarma k dispozici všem uživatelům v partnerském tenantovi prostřednictvím výchozího nastavení zabezpečení Azure AD s jedinou metodou ověřování ověřovací aplikace, která podporuje jednorázová hesla podle času (TOTP).
    - Další metody ověřování jsou k dispozici prostřednictvím [skladových Azure Active Directory Premium,](/azure/active-directory/fundamentals/active-directory-get-started-premium) pokud jsou požadovány jiné metody, jako je telefonní hovor nebo textová zpráva.
    - Partneři mohou při přístupu ke komerčním cloudovým službám Microsoftu také pro každý účet použít řešení MFA třetí strany.

2. **Přijetí Model zapezpečených aplikací architektury**

    Všichni partneři, kteří vyvinuli vlastní integraci pomocí libovolných rozhraní API (například Azure Resource Manager, Microsoft Graph, Partnerské centrum API atd.) nebo implementovali vlastní automatizaci pomocí nástrojů, jako je PowerShell, budou muset přijmout rozhraní [Model zapezpečených aplikací](/partner-center/develop/enable-secure-app-model) pro integraci s cloudovými službami Microsoftu. Pokud to není možné, může dojít k přerušení kvůli nasazení MFA. Následující zdroje obsahují přehled a pokyny týkající se osvojování modelu.

    - [Model zapezpečených aplikací přehledu](/partner-center/develop/enable-secure-app-model)
    - [Partnerské centrum: Model zapezpečených aplikací průvodce](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [Partneři v programu CSP: Vzorový kód .NET pro povolení Model zapezpečených aplikací](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
    - [Partneři v programu CSP: Vzorový kód Java pro povolení Model zapezpečených aplikací](/samples/microsoft/partner-center-java-samples/secure-app-model/)
    - [Partnerské centrum ověřování dokumentu](/partner-center/develop/partner-center-authentication)
    - [Partnerské centrum vícefaktorového ověřování (MFA) PowerShellu](/powershell/partnercenter/multi-factor-auth)

    Pokud používáte ovládací panel týkající se přijetí této architektury, obraťte se na Model zapezpečených aplikací dodavatele.

    Dodavatelé ovládacích panelů musí [tento](enroll-as-cpv.md) požadavek Partnerské centrum jako dodavatele ovládacích panelů a začít tento požadavek okamžitě implementovat. Projděte si [následující Partnerské centrum: Model zapezpečených aplikací framework](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Dodavatelé ovládacích panelů musí místo přihlašovacích údajů přijmout a spravovat souhlas partnerů CSP a vymazat přihlašovací údaje všech stávajících partnerů CSP.

## <a name="multi-factor-authentication"></a>Ověřování pomocí služby Multi-Factor Authentication

### <a name="what-is-multi-factor-authentication-mfa"></a>Co je vícefaktorové ověřování (MFA)?

MFA je bezpečnostní mechanismus pro ověřování jednotlivců prostřednictvím více než jednoho vyžadovaného postupu zabezpečení a ověření. Funguje tak, že vyžaduje dvě nebo více následujících metod ověřování:

- Něco, co znáte (obvykle heslo)
- Něco, co máte (důvěryhodné zařízení, které není jednoduše duplikováno, jako je telefon)
- Něco, co používáte (biometrika)

### <a name="what-is-the-cost-of-enabling-mfa"></a>Jaké jsou náklady na povolení MFA?

Microsoft v rámci implementace výchozích hodnot zabezpečení Azure AD poskytuje bezplatně vícefaktorové ověřování. Jediná možnost ověření, která je dostupná v této verzi MFA, je ověřovací aplikace. Pokud je vyžadován telefonní hovor nebo zpráva SMS, bude nutné zakoupit licenci [Azure Active Directory Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium) . Alternativně můžete využít řešení jiného výrobce k poskytnutí MFA pro každého uživatele v partnerském tenantovi – v tomto případě je to vaše zodpovědnost za to, abyste zajistili, že se vaše řešení MFA vynutilo a že budete dodržovat předpisy.

### <a name="what-actions-do-i-need-to-take-if-i-already-have-an-mfa-solution"></a>Jaké akce je potřeba provést, když už mám řešení MFA?

Pomocí těchto požadavků na zabezpečení se uživatelé v partnerském tenantovi budou muset při přístupu k komerčním cloudovým službám Microsoftu ověřit pomocí VÍCEFAKTOROVÉHO ověřování. K splnění těchto požadavků lze použít řešení třetích stran. Microsoft už neposkytuje ověřovací testování pro nezávislé zprostředkovatele identity kvůli kompatibilitě s Azure Active Directory. Informace o tom, jak testovat svůj produkt pro interoperabilitu, najdete v těchto [pokynech](https://www.microsoft.com/download/details.aspx?id=56843).

> [!IMPORTANT]
> Pokud používáte řešení třetí strany, je důležité ověřit, že řešení vydává deklaraci identity AMR (Authentication Method reference), která zahrnuje hodnotu MFA. Podrobnosti o tom, jak ověřit, že řešení třetí strany vydávají očekávanou deklaraci identity, najdete v tématu [testování požadavků na zabezpečení partnera](/powershell/partnercenter/test-partner-security-requirements) .

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>Používám několik partnerských tenantů pro Transact. Musím pro ně implementovat MFA?

Ano, budete muset vymáhat MFA pro každého tenanta Azure Active Directory přidruženého k programu CSP nebo programu poradce. Pokud si chcete Azure Active Directory Premium licenci, musíte si Azure Active Directory licenci pro uživatele v každém Azure Active Directory tenantovi. 

### <a name="does-each-user-account-in-my-partner-tenant-need-to-have-mfa-enforced"></a>Musí se pro každý uživatelský účet v partnerském tenantovi vynucovat více ověřování?

Ano, každý uživatel bude muset vynucovat více ověřování. Pokud ale používáte výchozí nastavení zabezpečení Azure AD, nevyžaduje se žádná další akce, protože tato funkce vynucuje MFA pro všechny uživatelské účty. Povolení výchozích hodnot zabezpečení je bezplatný a snadný způsob, jak zajistit, aby vaše uživatelské účty byly kompatibilní s více ověřováním a nebyly ovlivněny při vynucení více ověřování.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Jsem partner Microsoftu s přímým vyúčtováním. Co musím udělat?

Partneři s přímým vyúčtováním Cloud Solution Provider musí více ověřování vynutit pro každého uživatele ve svém partnerském tenantovi.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-enable-mfa"></a>Jsem nepřímý prodejce a provádím transakce jenom přes distributora. Musím ještě povolit MFA?

Všichni nepřímí prodejci musí vynutit více ověřování pro každého uživatele ve svém partnerském tenantovi. Nepřímý prodejce musí povolit MFA.

### <a name="i-dont-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>Rozhraní API pro Partnerské centrum. Musím ještě implementovat MFA?

Ano, tento požadavek na zabezpečení je pro všechny uživatele, včetně uživatelů s rolí správce partnera a koncových uživatelů v partnerském tenantovi.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Kteří dodavatelé třetích stran poskytují řešení MFA kompatibilní s Azure Active Directory?

Při prověrce dodavatelů a řešení MFA musí partneři zajistit, aby řešení, které si zvolí, bylo kompatibilní s Azure Active Directory.

Společnost Microsoft už pro nezávislé zprostředkovatele identity poskytuje ověřovací testování pro zajištění kompatibility s Azure Active Directory. Pokud chcete otestovat svůj produkt z oblasti interoperability, přečtěte si tyto [pokyny.](https://www.microsoft.com/download/details.aspx?id=56843)

Další informace najdete v seznamu kompatibility [federace Azure AD.](/azure/active-directory/hybrid/how-to-connect-fed-compatibility)

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>Jak můžu otestovat MFA v našem sandboxu pro integraci?

Měla by být povolená funkce výchozí hodnoty zabezpečení Azure AD nebo taky můžete použít řešení třetí strany, které používá federaci.

### <a name="will-enabling-mfa-affect-how-i-interact-with-my-customers-tenant"></a>Povolí MFA možnost pracovat s tenant mého zákazníka?

No. Splnění těchto požadavků na zabezpečení nebude mít vliv na způsob správy vašich zákazníků. Schopnost provádět delegované operace správy nebude přerušena.

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>Vztahují se na zákazníky požadavky na zabezpečení partnerů?

Ne, není nutné vymáhat MFA pro každého uživatele v klientech Azure AD vašeho zákazníka. Doporučuje se ale spolupracovat s jednotlivými zákazníky a určit, jak nejlépe chránit své uživatele.

### <a name="can-any-user-be-excluded-from-the-mfa-requirement"></a>Může být libovolný uživatel vyloučený z požadavku MFA?

Ne. u každého uživatele, včetně účtů služeb, se v partnerském tenantovi bude vyžadovat ověření pomocí MFA.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>Vztahují se požadavky na zabezpečení partnera na izolovaný prostor integrace?

Ano, partnerské požadavky na zabezpečení se vztahují na izolovaný prostor integrace. To znamená, že budete muset implementovat vhodné řešení MFA pro uživatele v tenantovi izolovaného prostoru (sandbox) Integration. Doporučujeme, abyste implementovali výchozí nastavení zabezpečení Azure AD, které poskytuje MFA.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Návody nakonfigurovat účet pro nouzový přístup (break)?

Doporučuje se vytvořit jeden nebo dva účty pro nouzový přístup, aby se zabránilo neúmyslnému uzamčení vašeho tenanta Azure AD. S ohledem na požadavky na zabezpečení partnerů je potřeba, aby se každý uživatel ověřoval pomocí vícefaktorového ověřování. Tento požadavek znamená, že budete muset změnit definici účtu pro nouzový přístup. Může to být účet, který používá řešení pro vícefaktorové ověřování od jiného výrobce.

### <a name="is-active-directory-federation-service-adfs-required-if-i-am-using-a-third-party-solution"></a>Vyžaduje se služba Active Directory služba FS (Federation Service) (ADFS), když používám řešení třetí strany?

Ne, pokud používáte řešení třetí strany, není nutné mít službu Active Directory služba FS (Federation Service) (ADFS). Doporučujeme spolupracovat s dodavatelem řešení, abyste zjistili, jaké jsou požadavky na jejich řešení.

### <a name="is-it-a-requirement-to-enable-azure-ad-security-defaults"></a>Je nutné povolit výchozí nastavení zabezpečení Azure AD?

Ne, výchozí nastavení zabezpečení Azure AD není nutné povolovat.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>Je možné použít podmíněný přístup ke splnění požadavku MFA?

Ano, podmíněný přístup můžete použít k vynucení MFA pro každého uživatele, včetně účtů služeb, ve vašem partnerském tenantovi. Vzhledem k vysoce privilegované povaze partnera ale musíme zajistit, aby každý uživatel měl pro každé ověření výzvu MFA. To znamená, že nebudete moct použít funkci podmíněného přístupu, která obchází požadavek na MFA.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Budou požadavky na zabezpečení partnerů Azure AD Connect budou mít vliv na účet služby používaný tímto účtem?

Ne, na účet služby, který Azure AD Connect, nebudou mít vliv požadavky na zabezpečení partnerů. Pokud nastane problém s Azure AD Connect v důsledku vynucování MFA, otevřete žádost o technickou podporu s podporou Microsoftu.

## <a name="secure-application-model"></a>Model zapezpečených aplikací

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>Kdo by měl přijmout zabezpečený aplikační model, aby splňoval požadavky?

Microsoft představuje zabezpečenou a škálovatelnou rozhraní pro ověřování partnerů Cloud Solution Provider (CSP) a Ovládací panely dodavatelů Ovládací panely (CPV), která používá vícefaktorové ověřování. Další informace najdete v Model zapezpečených aplikací [příručce](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Všichni partneři, kteří vyvinuli vlastní integraci pomocí libovolných rozhraní API (například Azure Resource Manager, Microsoft Graph, Partnerské centrum API atd.) nebo implementovali vlastní automatizaci pomocí nástrojů, jako je PowerShell, budou muset přijmout rozhraní [Model zapezpečených aplikací](/partner-center/develop/enable-secure-app-model) pro integraci s cloudovými službami Microsoftu.

### <a name="what-is-the-secure-application-model"></a>Co je Model zapezpečených aplikací?

Microsoft představuje zabezpečenou a škálovatelnou rozhraní pro ověřování partnerů Cloud Solution Provider (CSP) a dodavatelů Ovládací panely (CPV), kteří využívají vícefaktorové ověřování. Další informace [Model zapezpečených aplikací v](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) průvodci instalací.  

### <a name="how-do-i-implement-the-secure-application-model"></a>Návody implementovat zabezpečený aplikační model?

Všechny partnery, kteří vyvinuli vlastní integraci pomocí libovolných rozhraní API (například Azure Resource Manager, Microsoft Graph, rozhraní API partnerského centra atd.) nebo implementovali vlastní automatizaci pomocí nástrojů, jako je PowerShell, budou muset pro integraci s cloudovou službou Microsoftu přijmout [rozhraní zabezpečeného modelu aplikace](/partner-center/develop/enable-secure-app-model) . V důsledku tohoto selhání může dojít k přerušení kvůli nasazení MFA. Následující zdroje poskytují přehled a pokyny týkající se toho, jak model přijmout.

- [Přehled zabezpečení aplikačního modelu](/partner-center/develop/enable-secure-app-model)
- [Partner Center: Průvodce zabezpečeným modelem aplikace](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partneři v programu CSP: ukázkový kód .NET pro povolení zabezpečení aplikačního modelu](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partneři v programu CSP: vzorový kód Java pro povolení modelu zabezpečené aplikace](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Ověřovací dokument partnerského centra](/partner-center/develop/partner-center-authentication)
- [Dokument Multi-Factor Authentication PowerShellu pro partnerský Center](/powershell/partnercenter/multi-factor-auth)

Pokud používáte ovládací panely, budete se muset obrátit na dodavatele, který se týká přijetí rozhraní zabezpečeného aplikačního modelu.

Dodavatelům ovládacího [panelu se musí zapojit do](enroll-as-cpv.md) partnerského centra jako dodavatel řídicích panelů a okamžitě zahájit implementaci tohoto požadavku. Přečtěte si téma [partner Center: Secure Application Modeling Framework](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Dodavatelé ovládacích panelů musí místo přihlašovacích údajů přijmout a spravovat souhlas partnerů CSP, a vyprázdnit všechny existující přihlašovací údaje partnerů CSP.

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>Musí být zabezpečený aplikační model implementovaný jenom pro rozhraní API nebo sadu SDK pro partnerské Centrum?

Když vynucujete vícefaktorové ověřování pro všechny uživatelské účty, bude to mít vliv na automatizaci nebo integraci, které mají být spuštěny neinteraktivně. I když požadavky na zabezpečení partnera vyžadují, abyste povolili zabezpečený aplikační model pro rozhraní API partnerského centra, dá se použít k vyřešení potřeby pro druhý faktor ověřování s automatizací a integrací.

>[!Note] 
>Prostředky, ke kterým se přistupuje, budou potřebovat podporu ověřování pomocí přístupových tokenů.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>Používám automatizační nástroje, jako je PowerShell. Návody implementovat Model zapezpečených aplikací?

Pokud má vaše automatizace běžet neinteraktivně a při ověřování se spoléhá na přihlašovací údaje uživatele, budete muset implementovat rozhraní Model zapezpečených aplikací. Viz [Model zapezpečených aplikací | Partnerské centrum pokyny k](/powershell/partnercenter/multi-factor-auth) implementaci této architektury v PowerShellu.  

>[!Note] 
>Ne všechny automatizační nástroje umožňují ověřování pomocí přístupových tokenů. Pokud potřebujete pomoc s [pochopením, jaké změny je potřeba provést, Partnerské centrum](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) ve skupině s pokyny k zabezpečení, získejte zprávu. 

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>Jaké přihlašovací údaje uživatele má správce aplikace zadat při provádění procesu souhlasu?

Doporučujeme použít účet služby, který má přiřazená nejméně privilegovaná oprávnění. Pokud jde o rozhraní API Partnerské centrum, měli byste použít účet, který byl přiřazený k roli Agent prodeje nebo Agent správy.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>Proč by správce aplikace neměl při provádění procesu souhlasu poskytnout přihlašovací údaje uživatele globálního správce?

Osvědčeným postupem je používat identitu s nejmenšími oprávněními.  Tím se sníží riziko. Nedoporučujeme používat účet, který má oprávnění globálního správce, protože by poskytoval více oprávnění, než je potřeba.

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>Jsem partner CSP. Návody, jestli můj dodavatel Ovládací panely (CPV) pracuje na implementaci řešení, nebo ne?

V případě partnerů, kteří k transakcím v programu Cloud Solution Provider (CSP) používají řešení CPV (Ovládací panely Vendor), zodpovídáte za konzultace s vaším CPV.

### <a name="who-is-a-control-panel-vendor-cpv"></a>Kdo je Ovládací panely (CPV)?

Dodavatel Ovládací panely softwaru je nezávislý dodavatel softwaru, který vyvíjí aplikace pro použití partnery CSP pro integraci s Partnerské centrum API. Dodavatel Ovládací panely není partner CSP s přímým přístupem k řídicímu panelu nebo Partnerské centrum rozhraní API. Podrobný popis najdete v příručce Partnerské centrum: Secure Applications Model (Model [zabezpečených aplikací).](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)

### <a name="i-am-a-cpv-how-do-i-enroll"></a>Jsem CPV. Návody zaregistrovat?

Pokud se chcete zaregistrovat jako dodavatel ovládacího panelu (CPV), postupujte podle pokynů uvedených [tady](enroll-as-cpv.md).

CPVs musí kontaktovat [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) odkaz pro registraci a poskytnout sponzorovi zaměstnance Microsoftu, který má obchodní vztah s CPV nebo ví, že jejich podnikání. Například partner Development Manager (PDM).

Jakmile se zaregistrujete do partnerského centra a zaregistrujete své aplikace, budete mít přístup k rozhraním API partnerského centra. Pokud jste nový CPV, obdržíte informace o izolovaném prostoru prostřednictvím oznámení partnerského centra. Po dokončení registrace jako Microsoft CPV a přijetí smlouvy CPV můžete:

1. Spravujte aplikaci pro více tenantů (přidejte aplikace do Azure Portal a zaregistrujte a zrušte registraci aplikací v partnerském centru).

   >[!Note]
   >CPVs musí zaregistrovat své aplikace v partnerském centru, aby bylo možné získat autorizaci pro rozhraní API partnerského centra. Přidání aplikací do samotného Azure Portal neautorizuje aplikace CPV pro rozhraní API partnerského centra.

1. Umožňuje zobrazit a spravovat váš profil CPV.

1. Umožňuje zobrazit a spravovat uživatele, kteří potřebují přístup k možnostem CPV. CPV může mít jenom globálního správce role.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>Používám sadu SDK partnerského centra. Bude sada SDK automaticky přijímají zabezpečený aplikační model?

Ne, budete muset postupovat podle pokynů uvedených v [Průvodci zabezpečeným modelem aplikace](https://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-dont-have-mfa-enabled"></a>Můžu pro zabezpečený model aplikace vygenerovat obnovovací token s účty, u kterých není povolený MFA?

Ano, obnovovací token se dá vygenerovat pomocí účtu, který nemá vyměnitelnou MFA. Mělo by se to ale vyhnout. Jakýkoli token vygenerovaný pomocí účtu, který nemá povolený MFA, nebude mít přístup k prostředkům z důvodu vícefaktorového ověřování.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>Jak má moje aplikace získat přístupový token, pokud povolujem MFA?

Budete muset postupovat podle [Průvodce zabezpečeným modelem aplikace](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) , který poskytuje podrobné informace o tom, jak to udělat, a přitom splnit nové požadavky na zabezpečení. Vzorový kód .NET [sem](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) můžete [najít zde a](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)ukázkový kód Java.

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>V rámci CPV se vytvoří aplikace služby Azure AD v tenantovi CPV nebo tenantovi partnera CSP?

CPV bude muset vytvořit aplikaci Azure Active Directory v tenantovi přidruženém k jejich registraci jako CPV.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>Jsem CSP, který používá pouze ověřování aplikace. Potřebuji udělat nějaké změny?

Ověřování pouze aplikace není ovlivněno, protože přihlašovací údaje uživatele nejsou používány k vyžádání přístupového tokenu. Pokud jsou sdíleny přihlašovací údaje uživatele, musí dodavatelé ovládacích panelů (CPVs) přijmout rozhraní [zabezpečeného modelu aplikace](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) a vyprázdnit všechny existující partnerské přihlašovací údaje.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>V rámci CPV můžu pro získání přístupových tokenů využít styl ověřování pouze aplikace?

Ne, partneři na řídicí panely nemohou použít styl ověřování pouze aplikace k vyžádání přístupových tokenů jménem partnera. Měly by implementovat zabezpečený model aplikace, který využívá styl ověřování aplikace a uživatele.

## <a name="technical-enforcement"></a>Technická vynucování

### <a name="what-is-the-activation-of-security-safeguards"></a>Jaká je aktivace ochrany zabezpečení?

Všichni partneři účastnící se programu Cloud Solution Provider (CSP), prodejci ovládacích panelů (CPVs) a poradci by měli implementovat povinné bezpečnostní požadavky, aby zůstaly v souladu.

Aby bylo možné zajistit dodatečnou ochranu, společnost Microsoft začala aktivovat ochranu zabezpečení, která pomáhá partnerům zabezpečit své klienty a jejich zákazníky pomocí ověřování vícefaktorového ověřování mandating (MFA), aby se zabránilo neoprávněnému přístupu.  

Úspěšně jsme dokončili aktivaci funkcí ADMINISTRATE (admin-on-of) pro všechny partnerské klienty. Pokud chceme dále chránit partnery a zákazníky a cílí na Q2 CY2020, zahájíme aktivaci pro transakce Partnerské centrum v CSP a pomůžeme partnerům chránit jejich firmy a zákazníky před incidenty souvisejícími s krádeží identity.

Další informace najdete na stránce o tom, jak u svého partnerského tenanta zažádá o vícefaktorové ověřování [(MFA).](partner-security-requirements-mandating-mfa.md)

### <a name="i-am-using-a-third-party-mfa-solution-and-i-am-being-blocked-what-should-i-do"></a>Používám řešení MFA třetí strany a blokuje mě to. Co mám dělat?

Aby se ověřilo, že účet, který přistupuje k prostředkům, byl vyzýván k vícefaktorovému ověřování, budeme kontrolovat deklaraci identity odkazu [na](https://tools.ietf.org/html/rfc8176) metodu ověřování a uvidíme, jestli je uvedené vícefaktorové ověřování. Některá řešení třetích stran tuto deklaraci identity nevydá nebo nezahrnují hodnotu MFA. Pokud deklarace identity chybí nebo pokud není uvedená hodnota MFA, neexistuje způsob, jak zjistit, jestli byl ověřený účet vyzývat k vícefaktorové ověřování. Budete muset ve svém řešení třetí strany spolupracovat s dodavatelem, abyste zjistili, jaké akce je potřeba udělat, aby řešení vydanou deklaraci identity odkazu na metodu ověřování vydanou v tomto řešení.

Pokud [si nejste jistí,](/powershell/partnercenter/test-partner-security-requirements) jestli řešení třetí strany vydává očekávanou deklaraci identity, podívejte se na část Testování požadavků na zabezpečení partnera.

### <a name="mfa-is-blocking-me-from-supporting-my-customer-using-aobo-what-should-i-do"></a>MFA mi brání v podpoře zákazníků pomocí AOBO. Co mám dělat?

Technické vynucování požadavků na zabezpečení partnerů se bude kontrolovat, jestli ověřený účet nebyl vyzývat k vícefaktorové ověřování. Pokud účet ještě není, budete přesměrováni na přihlašovací stránku a budete vyzváni k novému ověření. Další informace a pokyny najdete v této dokumentaci k tomu, jak se vícefaktorové ověřování [(MFA)](partner-security-requirements-mandating-mfa.md#partner-delegated-administration) odvážit od partnerského tenanta. Ve scénáři, kdy vaše doména není federovaná, se po úspěšném ověření zobrazí výzva k nastavení vícefaktorového ověřování. Po dokončení budete moct spravovat své zákazníky pomocí funkce AOBO. Ve scénáři, kdy je vaše doména federovaná, budete muset zajistit, aby účet byl vyzýván k vícefaktorové ověřování.

## <a name="security-defaults-transition"></a>Přechod výchozích hodnot zabezpečení

### <a name="how-can-i-transition-from-baseline-policies-to-security-defaults-or-other-mfa-solutions"></a>Jak můžu přejít ze základních zásad na výchozí nastavení zabezpečení nebo jiná řešení MFA?

Azure Active Directory (Azure [AD)](/azure/active-directory/fundamentals/whats-new#replacement-of-baseline-policies-with-security-defaults) se odebraly základní zásady a nahradily se "výchozími nastaveními zabezpečení", komplexnější sadu zásad ochrany pro vás a vaše zákazníky. [Výchozí nastavení zabezpečení pomáhá](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) chránit vaši organizaci před útoky na zabezpečení souvisejícími s krádeží identity.

Vaše implementace vícefaktorového ověřování (MFA) se odebere z důvodu vyřazení základních zásad, pokud jste nesnížedli základní zásady na výchozí zásady zabezpečení nebo jiné možnosti implementace vícefaktorového [ověřování.](partner-security-requirements.md#implementing-multi-factor-authentication) Všichni uživatelé ve vašich partnerských tenantech provádějících operace chráněné více ověřováním budou požádáni o dokončení více ověřování. Podrobnější pokyny najdete [tady.](partner-security-requirements-mandating-mfa.md)
Pokud chcete dodržovat předpisy a minimalizovat přerušení služeb, udělejte jednu z následujících akcí:

- Přechod na výchozí nastavení zabezpečení
    - Jednou z možností, které partneři mohou zvolit pro implementaci MFA, jsou zásady výchozích hodnot zabezpečení. Nabízí základní úroveň zabezpečení, která je povolená bez dalších nákladů.
    - Zjistěte, jak ve vaší organizaci povolit MFA pomocí Azure AD, a přečtěte si důležité informace o výchozích [bezpečnostních klíčích.](partner-security-requirements.md#security-defaults)
    - Pokud vyhovuje vašim obchodním potřebám, povolte výchozí zásady zabezpečení.
- Přechod na podmíněný přístup
    - Pokud výchozí zásady zabezpečení vašim potřebám nepomáhou, povolte Podmíněný přístup. Další informace najdete v dokumentaci k podmíněnému přístupu Azure AD.

## <a name="key-resources"></a>Klíčové prostředky

### <a name="how-to-get-started"></a>Jak začít

- [Požadavky na zabezpečení partnerů:](partner-security-requirements.md)Podrobný průvodce .
- Své dotazy a připomínky nasměrovat na [tuto Partnerské centrum Security Guidance Group](https://aka.ms/MPCSecurityGuidance).
- Zúčastněte se nadcházejících partnerských kanceláří a webináře. Podrobné informace o [plánu a prostředcích najdete tady](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance).

### <a name="resources-for-adopting-secure-application-model"></a>Prostředky pro přijetí zabezpečeného modelu aplikace

- [Přehled zabezpečení aplikačního modelu](/partner-center/develop/enable-secure-app-model)
- [Partner Center: Průvodce zabezpečeným modelem aplikace](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partneři v programu CSP: ukázkový kód .NET pro povolení zabezpečení aplikačního modelu](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partneři v programu CSP: vzorový kód Java pro povolení modelu zabezpečené aplikace](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Ověřovací dokument partnerského centra](/partner-center/develop/partner-center-authentication)
- [Dokument Multi-Factor Authentication PowerShellu pro partnerský Center](/powershell/partnercenter/multi-factor-auth)

## <a name="support"></a>Podpora

### <a name="where-can-i-get-support"></a>Kde můžu získat podporu?

Pokud máte k dispozici prostředky podpory, které splňují požadavky na zabezpečení, obraťte se na správce účtu služby, pokud máte pokročilou podporu pro partnery (ASfP). Pokud chcete získat smlouvu Premier Support pro partnery (smlouvou psfp můžou), obraťte se na správce účtů služeb a správce technického účtu.

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>Návody získat technické informace a podporu pro pomoc při přijímání rozhraní zabezpečeného modelu aplikace?

Možnosti technické podpory pro Azure Active Directory jsou dostupné prostřednictvím výhod programu MPN. Partneři s přístupem k aktivnímu předplatnému ASfP nebo smlouvou psfp můžou mohou spolupracovat se svým přidruženým správcem účtů (SAM/TAM), aby nejlépe pochopily dostupné možnosti.

### <a name="how-do-i-contact-support-if-ive-lost-access-to-partner-center"></a>Návody kontaktujte podporu, pokud ztratili přístup k partnerskému centru?

Pokud ztratíte přístup kvůli problému MFA, kontaktujte globálního správce vašeho tenanta. Vaše interní IT oddělení vám bude moct říct, kdo je vaším globálním správcem. 

Pokud jste zapomněli heslo, [nemůžete se přihlásit](unable-to-sign-in.md) a získat nápovědu.

### <a name="where-can-i-find-more-information-about-common-technical-issues"></a>Kde najdu Další informace o běžných technických problémech?

Informace o běžných technických problémech najdete v části [požadavky na zabezpečení partnerů pro partnery pomocí partnerských rozhraní API partnerského centra nebo partnerského centra](partner-security-requirements.md) .