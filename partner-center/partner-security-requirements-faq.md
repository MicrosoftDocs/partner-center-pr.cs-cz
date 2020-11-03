---
title: Nejčastější dotazy k požadavkům na zabezpečení partnerů
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Nejčastější dotazy týkající se požadavků na zabezpečení partnerů – co jsou, jak je chtějí partneři implementovat a jak zjistit, jestli jste je splnili.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9f60b6e2624bd4f9020181a936842bdb46db8aa9
ms.sourcegitcommit: 98f5eebe7d08ba214ed5a078f1ac770439e41eb7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/31/2020
ms.locfileid: "93133044"
---
# <a name="common-questions-about-partner-security-requirements"></a>Běžné otázky týkající se požadavků na zabezpečení partnerů

**Platí pro**

- Partnerské centrum

**Příslušné uživatele**

- Všichni povolení uživatelé včetně uživatelů typu Host


Tento článek obsahuje odpovědi na některé běžné dotazy týkající se [požadavků na zabezpečení partnera](partner-security-requirements.md).

### <a name="what-are-the-partner-security-requirements-and-why-should-partners-implement-them"></a>Jaké jsou požadavky na zabezpečení partnerů a proč by se měly jejich partneři implementovat?

Vyšší a nepřetržité zabezpečení a ochrana osobních údajů jsou z našich nejdůležitějších priorit a budeme dál pomáhat partnerům chránit své zákazníky a klienty. Dál se podrobněji prodlužuje a zvyšuje počet útoků zabezpečení, které jsou primárně spojené s incidenty ohrožení bezpečnosti identity. Protože preventivní kontroly hrají klíčovou roli v celkové strategii obrany, aby vzdoruje bezpečnostní útoky, představili jsme v 2019 [požadavky na zabezpečení](partner-security-requirements.md) . Všichni partneři účastnící se programu Cloud Solution Provider (CSP), prodejci ovládacích panelů a poradci musí implementovat požadavky, aby zůstaly v souladu.

### <a name="what-are-the-key-timelines-and-milestones"></a>Jaké jsou klíčové časové osy a milníky?

Podmínky spojené s těmito požadavky na zabezpečení, včetně časových os a milníků, jsou součástí [smlouvy Microsoft Partner Agreement](microsoft-partner-agreement.md). Tyto požadavky na zabezpečení bude nutné co nejdříve implementovat, aby bylo možné v programu CSP v souladu s vaší účastí.

### <a name="what-will-happen-if-i-dont-implement-these-partner-security-requirements"></a>Co se stane, když tyto požadavky na zabezpečení těchto partnerů neimplementujem?

Partnerská smlouva Microsoftu vyžaduje, abyste vynutili službu Multi-Factor Authentication pro uživatelské účty a přijali zabezpečený aplikační model pro interakci s rozhraním API partnerského centra. 

Partneři, kteří tyto postupy zabezpečení nedodržují, mohou ztratit svou schopnost pracovat v programu CSP nebo spravovat klienty zákazníka pomocí oprávnění delegovat správce.

### <a name="do-the-security-requirements-apply-to-all-geographies"></a>Platí požadavky na zabezpečení u všech geografických oblastí?

Ano, požadavky na zabezpečení platí pro všechna geografická pole. Důrazně doporučujeme, aby všichni partneři procházeli prostřednictvím svrchovaného cloudu (vlády USA a Německa) a okamžitě přijali tyto nové požadavky na zabezpečení. Tito partneři ale momentálně nevyžadují splnění požadavků na zabezpečení. Microsoft nabídne další podrobnosti týkající se vynucování těchto požadavků na zabezpečení pro cloudy svrchovaného v budoucnu.

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>Je možné získat pro účet vyloučení?

Ne, z požadavku na vynucení vícefaktorového ověřování (MFA) není možné vyloučit žádný uživatelský účet. S ohledem na vysoce privilegovaný charakter je Partnerská smlouva Microsoftu vyžaduje, aby se pro každý uživatelský účet ve vašem partnerském tenantovi vynutilo ověřování pomocí služby Multi-Factor Authentication.

### <a name="how-do-i-know-if-i-have-met-the-partner-security-requirements"></a>Návody vědět, jestli splňujem požadavky na zabezpečení partnera?

Je nutné provést následující kroky:

- Musíte splnit všechny požadavky, které jsou uvedené v požadavcích na [zabezpečení partnera](partner-security-requirements.md).
- Je potřeba zajistit, aby všechny uživatelské účty ve vašem partnerském tenantovi vynutily službu Multi-Factor Authentication.

Abychom vám pomohli identifikovat klíčové oblasti, kde můžete provádět akce, poskytujeme [zprávu o stavu požadavků na zabezpečení](https://partner.microsoft.com/commerce/security/compliance) , která je k dispozici prostřednictvím partnerského centra.

Další informace o zprávě o stavu najdete v tématu [stav požadavků na zabezpečení partnerů](partner-security-compliance.md) .

## <a name="required-actions"></a>Požadované akce

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>Jaké jsou klíčové akce, které je potřeba provést, aby se splnily požadavky?

Všichni partneři v programu CSP (přímá fakturace, nepřímý poskytovatel a nepřímý prodejce), poradci a dodavatelé ovládacích panelů musí splňovat požadavky.

1. **Vymáhat MFA pro všechny uživatele**

    Všichni partneři v programu CSP, poradci a v Ovládacích panelech musí vymáhat MFA pro všechny uživatele v partnerském tenantovi.

    Další rozhodnutí:

    - Neposkytovatelé nepřímých zprostředkovatelů potřebují spolupracovat s nepřímými prodejci, kteří se dostanou do partnerského centra, pokud je ještě neudělali, a nepodporují jejich prodejce, aby splnili požadavky.
    - Azure MFA se zpřístupňuje všem uživatelům v partnerském tenantovi bez jakýchkoli nákladů prostřednictvím výchozích hodnot zabezpečení Azure AD s jedinou metodou ověření aplikace ověřovatele, která podporuje časová hesla založená na čase (TOTP).
    - Další metody ověřování jsou dostupné prostřednictvím [Azure Active Directory Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium) SKU, pokud potřebujete jiné metody, jako je třeba telefonní hovor nebo textová zpráva.
    - Při přístupu k komerčním cloudovým službám Microsoftu můžou pro každý účet využít také řešení MFA od jiného výrobce.

2. **Přijmout rozhraní zabezpečeného modelu aplikace**

    Všechny partnery, kteří vyvinuli vlastní integraci pomocí libovolných rozhraní API (například Azure Resource Manager, Microsoft Graph, rozhraní API partnerského centra atd.) nebo implementovali vlastní automatizaci pomocí nástrojů, jako je PowerShell, budou muset pro integraci s cloudovou službou Microsoftu přijmout [rozhraní zabezpečeného modelu aplikace](/partner-center/develop/enable-secure-app-model) . V důsledku tohoto selhání může dojít k přerušení kvůli nasazení MFA. Následující zdroje poskytují přehled a pokyny týkající se toho, jak model přijmout.

    - [Přehled zabezpečení aplikačního modelu](/partner-center/develop/enable-secure-app-model)
    - [Partner Center: Průvodce zabezpečeným modelem aplikace](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [Partneři v programu CSP: ukázkový kód .NET pro povolení zabezpečení aplikačního modelu](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
    - [Partneři v programu CSP: vzorový kód Java pro povolení modelu zabezpečené aplikace](/samples/microsoft/partner-center-java-samples/secure-app-model/)
    - [Ověřovací dokument partnerského centra](/partner-center/develop/partner-center-authentication)
    - [Dokument Multi-Factor Authentication PowerShellu pro partnerský Center](/powershell/partnercenter/multi-factor-auth)

    Pokud používáte ovládací panely, které se týkají přijetí rozhraní zabezpečeného aplikačního modelu, obraťte se na dodavatele.

    Dodavatelům ovládacího [panelu se musí zapojit do](enroll-as-cpv.md) partnerského centra jako dodavatel řídicích panelů a okamžitě zahájit implementaci tohoto požadavku. Přečtěte si téma [partner Center: Secure Application Modeling Framework](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Dodavatelé ovládacích panelů musí místo přihlašovacích údajů přijmout a spravovat souhlas partnerů CSP, a vyprázdnit všechny existující přihlašovací údaje partnerů CSP.

## <a name="multi-factor-authentication"></a>Ověřování pomocí služby Multi-Factor Authentication

### <a name="what-is-multi-factor-authentication-mfa"></a>Co je Multi-Factor Authentication (MFA)?

MFA je bezpečnostní mechanismus, při kterém se jednotlivci ověřují prostřednictvím více než jednoho vyžadovaného postupu zabezpečení a ověření. Funguje tak, že vyžaduje dvě nebo více následujících metod ověřování:

- Něco, co znáte (obvykle heslo)
- Něco, co máte (důvěryhodné zařízení, které není jednoduše duplikováno, jako je telefon)
- Něco, co používáte (biometrika)

### <a name="what-is-the-cost-of-enabling-mfa"></a>Jaké jsou náklady na povolení MFA?

Microsoft v rámci implementace výchozích hodnot zabezpečení Azure AD poskytuje bezplatně vícefaktorové ověřování. Jediná možnost ověřování dostupná prostřednictvím této verze MFA je ověřovací aplikace. Pokud je vyžadován telefonní hovor nebo zpráva SMS, bude nutné zakoupit licenci [Azure Active Directory Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium) . Alternativně můžete využít řešení jiného výrobce k poskytnutí MFA pro každého uživatele v partnerském tenantovi – v tomto případě je to vaše zodpovědnost za to, abyste zajistili, že se vaše řešení MFA vynutilo a že budete dodržovat předpisy.

### <a name="what-actions-do-i-need-to-take-if-i-already-have-an-mfa-solution"></a>Jaké akce je potřeba provést, když už mám řešení MFA?

Pomocí těchto požadavků na zabezpečení se uživatelé v partnerském tenantovi budou muset při přístupu k komerčním cloudovým službám Microsoftu ověřit pomocí VÍCEFAKTOROVÉHO ověřování. K splnění těchto požadavků lze použít řešení třetích stran. Microsoft už neposkytuje ověřovací testování pro nezávislé zprostředkovatele identity kvůli kompatibilitě s Azure Active Directory. Informace o tom, jak testovat svůj produkt pro interoperabilitu, najdete v těchto [pokynech](https://www.microsoft.com/download/details.aspx?id=56843).

> [!IMPORTANT]
> Pokud používáte řešení třetí strany, je důležité ověřit, že řešení vydává deklaraci identity AMR (Authentication Method reference), která zahrnuje hodnotu MFA. Podrobnosti o tom, jak ověřit, že řešení třetí strany vydávají očekávanou deklaraci identity, najdete v tématu [testování požadavků na zabezpečení partnera](/powershell/partnercenter/test-partner-security-requirements) .

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>Používám několik partnerských tenantů pro Transact. Musím pro ně implementovat MFA?

Ano, budete muset vymáhat MFA pro každého tenanta Azure Active Directory přidruženého k programu CSP nebo programu poradce. Pokud si chcete koupit licenci Azure Active Directory Premium, musíte pro uživatele v každém klientovi Azure Active Directory zakoupit licenci Azure Active Directory. 

### <a name="does-each-user-account-in-my-partner-tenant-need-to-have-mfa-enforced"></a>Musí mít každý uživatelský účet v partnerském tenantovi vymáhání MFA?

Ano, u každého uživatele bude nutné vyhovět MFA. Pokud ale používáte výchozí hodnoty zabezpečení Azure AD, není nutná žádná další akce, protože tato funkce vynutila MFA pro všechny uživatelské účty. Povolení výchozích hodnot zabezpečení je bezplatný a snadný způsob, jak zajistit, aby byly uživatelské účty kompatibilní s MFA a neovlivnily se při vymáhání MFA.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Jsem přímým účtováným partnerem Microsoftu. Co musím udělat?

Partneři poskytovatele cloudových řešení pro přímé faktury musí vymáhat MFA pro každého uživatele v partnerském tenantovi.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-enable-mfa"></a>Jsem nepřímým prodejcem a jenom v případě, že je distributor. Musím pořád povolit MFA?

Všem nepřímým prodejcům se vyžaduje, aby vynutil MFA pro každého uživatele v partnerském tenantovi. Nepřímý prodejce musí povolit vícefaktorové ověřování.

### <a name="i-dont-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>Nepoužívám rozhraní API partnerského centra. Je stále potřeba implementovat MFA?

Ano, tento požadavek zabezpečení je pro všechny uživatele, včetně uživatelů partnerského správce a koncových uživatelů v partnerském tenantovi.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Kteří dodavatelé třetích stran poskytují řešení MFA kompatibilní s Azure Active Directory?

Při kontrole dodavatelů a řešení MFA musí partneři zajistit, aby zvolené řešení bylo kompatibilní s Azure Active Directory.

Microsoft už neposkytuje ověřovací testování pro nezávislé zprostředkovatele identity kvůli kompatibilitě s Azure Active Directory. Pokud chcete svůj produkt testovat pro interoperabilitu, přečtěte si tyto [pokyny](https://www.microsoft.com/download/details.aspx?id=56843).

Další informace najdete v [seznamu Kompatibilita federace služby Azure AD](/azure/active-directory/hybrid/how-to-connect-fed-compatibility).

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>Jak můžu otestovat vícefaktorové ověřování v naší karanténě pro integraci?

Funkce Azure AD Security Defaults by měla být povolená nebo taky můžete využít řešení třetích stran, které využívá federaci.

### <a name="will-enabling-mfa-affect-how-i-interact-with-my-customers-tenant"></a>Povolí MFA možnost pracovat s tenant mého zákazníka?

Ne. Splnění těchto požadavků na zabezpečení nebude mít vliv na způsob správy vašich zákazníků. Schopnost provádět delegované operace správy nebude přerušena.

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>Vztahují se na zákazníky požadavky na zabezpečení partnerů?

Ne, není nutné vymáhat MFA pro každého uživatele v klientech Azure AD vašeho zákazníka. Doporučuje se ale spolupracovat s jednotlivými zákazníky a určit, jak nejlépe chránit své uživatele.

### <a name="can-any-user-be-excluded-from-the-mfa-requirement"></a>Může být libovolný uživatel vyloučený z požadavku MFA?

Ne. u každého uživatele, včetně účtů služeb, se v partnerském tenantovi bude vyžadovat ověření pomocí MFA.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>Vztahují se požadavky na zabezpečení partnera na izolovaný prostor integrace?

Ano, partnerské požadavky na zabezpečení se vztahují na izolovaný prostor integrace. To znamená, že budete muset implementovat vhodné řešení MFA pro uživatele v tenantovi izolovaného prostoru (sandbox) Integration. Doporučujeme, abyste implementovali výchozí nastavení zabezpečení Azure AD, které poskytuje MFA.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Návody nakonfigurovat účet pro nouzový přístup (break)?

Doporučuje se vytvořit jeden nebo dva účty pro nouzový přístup, aby se zabránilo neúmyslnému uzamčení vašeho tenanta Azure AD. S ohledem na požadavky na zabezpečení partnerů je potřeba, aby se každý uživatel ověřoval pomocí vícefaktorového ověřování. Tento požadavek znamená, že budete muset změnit definici účtu pro nouzový přístup. Může to být účet, který využívá řešení pro MFA od jiného výrobce.

### <a name="is-active-directory-federation-service-adfs-required-if-i-am-using-a-third-party-solution"></a>Vyžaduje se služba Active Directory služba FS (Federation Service) (ADFS), když používám řešení třetí strany?

Ne, pokud používáte řešení třetí strany, není nutné mít službu Active Directory služba FS (Federation Service) (ADFS). Doporučujeme, abyste spolupracovali s dodavatelem řešení a určili, jaké jsou požadavky na jejich řešení.

### <a name="is-it-a-requirement-to-enable-azure-ad-security-defaults"></a>Je požadavek na povolení výchozích hodnot zabezpečení Azure AD?

Ne, není nutné povolit výchozí nastavení zabezpečení služby Azure AD.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>Dá se podmíněný přístup použít ke splnění požadavku MFA?

Ano, podmíněný přístup můžete použít k vymáhání MFA pro každého uživatele, včetně účtů služeb ve vašem partnerském tenantovi. Vzhledem k tomu, že s vysokou mírou privilegované povahy je ale partner, potřebujeme zajistit, aby každý uživatel měl výzvu MFA pro každé samostatné ověřování. To znamená, že nebudete moci využívat funkci podmíněného přístupu, která obchází požadavek MFA.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Bude účet služby, který používá Azure AD Connect, ovlivněn požadavky na zabezpečení partnera?

Ne, účet služby, který používá Azure AD Connect, nebude ovlivněn požadavky na zabezpečení partnera. Pokud dojde k potížím s Azure AD Connect jako výsledek vynucování MFA, otevřete žádost o technickou podporu s podporou Microsoftu.

## <a name="secure-application-model"></a>Model zabezpečené aplikace

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>Kdo by měl přijmout zabezpečený aplikační model pro splnění požadavků?

Společnost Microsoft zavádí zabezpečenou, škálovatelnou architekturu pro ověřování partnerů CSP (Cloud Solution Provider) a dodavatelů ovládacích panelů (CPV), které využívají Multi-Factor Authentication. Další informace najdete v [Průvodci zabezpečeným modelem aplikace](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) . Všechny partnery, kteří vyvinuli vlastní integraci pomocí libovolných rozhraní API (například Azure Resource Manager, Microsoft Graph, rozhraní API partnerského centra atd.) nebo implementovali vlastní automatizaci pomocí nástrojů, jako je PowerShell, budou muset pro integraci s cloudovou službou Microsoftu přijmout [rozhraní zabezpečeného modelu aplikace](/partner-center/develop/enable-secure-app-model) .

### <a name="what-is-the-secure-application-model"></a>Jaký je model zabezpečené aplikace?

Společnost Microsoft zavádí zabezpečenou, škálovatelnou architekturu pro ověřování partnerů CSP (Cloud Solution Provider) a dodavatelů ovládacích panelů (CPV), které využívají Multi-Factor Authentication. Další informace najdete v [Průvodci zabezpečeným modelem aplikace](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) .  

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

Když vynucujete vícefaktorové ověřování pro všechny uživatelské účty, bude to mít vliv na automatizaci nebo integraci, které mají být spuštěny neinteraktivně. I když požadavky na zabezpečení partnera vyžadují, abyste povolili zabezpečený aplikační model pro rozhraní API partnerského centra, dá se využít k vyřešení potřeby pro druhý faktor ověřování s automatizací a integrací.

>[!Note] 
>Prostředky, ke kterým se přistupuje, budou potřebovat podporu ověřování pomocí přístupových tokenů.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>Používám nástroje pro automatizaci, jako je PowerShell. Návody implementovat zabezpečený aplikační model?

Pokud má vaše automatizace běžet neinteraktivně a závisí na přihlašovacích údajích uživatele k ověřování, bude nutné implementovat zabezpečený model aplikace. Viz [zabezpečený model aplikace | ](/powershell/partnercenter/multi-factor-auth) Informace o tom, jak implementovat tuto architekturu, najdete v centru partnerů prostředí PowerShell.  

>[!Note] 
>Ne všechny nástroje pro automatizaci poskytují možnost ověřování pomocí přístupových tokenů. Pokud potřebujete pomoc s porozuměním, co je potřeba udělat, vystavte zprávu ve skupině [doprovodné materiály zabezpečení partnerského centra](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) . 

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>Jaké přihlašovací údaje uživatele by měl správce aplikace poskytnout při provádění procesu souhlasu?

Doporučuje se použít účet služby, kterému byla přiřazena nejméně privilegovaná oprávnění. S ohledem na rozhraní API partnerského centra byste měli použít účet, který byl buď přiřazený k roli agenta prodeje nebo agentů pro správu.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>Proč by správce aplikace při provádění procesu souhlasu neposkytoval globální přihlašovací údaje uživatele?

Osvědčeným postupem je použití identity s nejnižšími oprávněními.  Tím se sníží riziko. Nedoporučujeme používat účet, který má oprávnění globálního správce, protože by poskytoval více oprávnění, než je potřeba.

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>Jsem partner CSP. Návody o tom, jestli můj dodavatel ovládacího panelu (CPV) pracuje na implementaci řešení nebo ne?

Pro partnery, kteří používají v programu Cloud Solution Provider (CSP) řešení pro transakce, je vaším zodpovědností, abyste se mohli obrátit na CPV.

### <a name="who-is-a-control-panel-vendor-cpv"></a>Kdo je to dodavatel ovládacího panelu (CPV)?

Dodavatel ovládacího panelu je nezávislý dodavatel softwaru, který vyvíjí aplikace pro použití partnery CSP při integraci s rozhraními API partnerského centra. Dodavatel ovládacího panelu není partnerem CSP s přímým přístupem k řídicímu panelu nebo rozhraním API partnerského centra. Podrobný popis je k dispozici v rámci [služby partner Center: Průvodce modelem zabezpečených aplikací](https://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="i-am-a-cpv-how-do-i-enroll"></a>Jsem CPV. Návody zaregistrovat?

Pokud se chcete zaregistrovat jako dodavatel ovládacího panelu (CPV), postupujte podle pokynů uvedených [tady](enroll-as-cpv.md).

CPVs musí kontaktovat [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) odkaz pro registraci a poskytnout sponzorovi zaměstnance Microsoftu, který má obchodní vztah s CPV nebo ví, že jejich podnikání. Například partner Development Manager (PDM).

Jakmile se zaregistrujete do partnerského centra a zaregistrujete své aplikace, budete mít přístup k rozhraním API partnerského centra. Pokud jste nový CPV, obdržíte informace o izolovaném prostoru prostřednictvím oznámení partnerského centra. Po dokončení registrace jako Microsoft CPV a přijetí smlouvy CPV můžete:

1. Spravujte aplikaci pro více tenantů (přidejte aplikace do Azure Portal, zaregistrujte a zrušte registraci aplikací v partnerském centru).

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

Úspěšně jsme dokončili aktivaci funkcí ADMINISTRATE (admin-on-of) pro všechny partnerské klienty. Abychom vám pomohli chránit partnery a zákazníky, zahájíme aktivaci transakcí partnerského centra ve zprostředkovateli CSP, což pomáhá partnerům chránit své firmy a zákazníky před incidenty souvisejícími s krádeží identity.

Další informace najdete na stránce [pro partnerský tenant na webu Mandating Multi-Factor Authentication (MFA)](partner-security-requirements-mandating-mfa.md) .

### <a name="i-am-using-a-third-party-mfa-solution-and-i-am-being-blocked-what-should-i-do"></a>Používám řešení MFA od jiného výrobce, které jsem zablokovaný, co mám dělat?

Pokud chcete ověřit, jestli je pro službu Multi-Factor Authentication prověřený účet přistupující k prostředkům, provedeme kontrolu deklarace [referencí na metodu ověřování](https://tools.ietf.org/html/rfc8176) , abyste zjistili, jestli je MFA uvedená. Některá řešení třetí strany nedávají tuto deklaraci identity nebo neobsahují hodnotu MFA. Pokud chybí deklarace identity nebo pokud hodnota MFA není uvedená, neexistuje žádný způsob, jak určit, jestli byl ověřený účet pro službu Multi-Factor Authentication napaden. Aby bylo možné určit, jaké akce je třeba provést, bude nutné, abyste spolupracovali s dodavatelem pro vaše řešení třetích stran.

Pokud si nejste jistí, jestli vaše řešení třetí strany vydává očekávanou deklaraci identity, podívejte [se na téma testování požadavků na zabezpečení partnera](/powershell/partnercenter/test-partner-security-requirements) .

### <a name="mfa-is-blocking-me-from-supporting-my-customer-using-aobo-what-should-i-do"></a>Vícefaktorové ověřování brání podpoře mého zákazníka pomocí ADMINISTRATE, co mám dělat?

Technické vynucování požadavků na zabezpečení partnera se ověří, pokud byl ověřený účet ověřen pro službu Multi-Factor Authentication. Pokud účet není, budete přesměrováni na přihlašovací stránku a zobrazí se výzva k ověření znovu. Přečtěte si další zkušenosti a pokyny v tomto [Mandating Multi-Factor Authentication (MFA) pro vaši dokumentaci k partner partnerovi](partner-security-requirements-mandating-mfa.md#partner-delegated-administration) . V případě, že vaše doména není federované, po úspěšném ověření se zobrazí výzva k nastavení služby Multi-Factor Authentication. Až to bude hotové, budete moct zákazníky spravovat pomocí ADMINISTRATE. V případě, kdy je vaše doména federované, musíte zajistit, aby byl účet využíván pro službu Multi-Factor Authentication.

## <a name="security-defaults-transition"></a>Přechod výchozích hodnot zabezpečení

### <a name="how-can-i-transition-from-baseline-policies-to-security-defaults-or-other-mfa-solutions"></a>Jak můžu přejít ze základních zásad na výchozí hodnoty zabezpečení nebo jiná řešení MFA?

Zásady "základní hodnoty" Azure Active Directory (Azure AD) [se odstraňují a nahrazují](/azure/active-directory/fundamentals/whats-new#replacement-of-baseline-policies-with-security-defaults) "výchozím nastavením zabezpečení", ucelenou sadou zásad ochrany pro vás a vaše zákazníky. [Výchozí nastavení zabezpečení](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) vám může přispět k ochraně vaší organizace před útoky zabezpečení souvisejícími s krádeží identity.

Implementace služby Multi-Factor Authentication (MFA) bude odebrána z důvodu vyřazení zásad standardních hodnot v případě, že jste nepřešli ze základních zásad na zásadu výchozích hodnot zabezpečení nebo [jiné možnosti implementace MFA](partner-security-requirements.md#implementing-multi-factor-authentication). Všichni uživatelé v partnerských klientech provádějících operace chráněné MFA budou požádáni o dokončení ověřování MFA. Přečtěte si podrobnější pokyny [zde](partner-security-requirements-mandating-mfa.md).
Chcete-li zachovat dodržování předpisů a minimalizovat přerušení, proveďte jednu z následujících akcí:

- Přechod na výchozí hodnoty zabezpečení
    - Zásada výchozích hodnot zabezpečení je jednou z možností, které můžou partneři vybrat k implementaci MFA. Nabízí základní úroveň zabezpečení, která je povolená bez dalších poplatků.
    - Naučte se, jak ve vaší organizaci povolit vícefaktorové ověřování pomocí Azure AD, a přečtěte si [klíčové důležité informace o zabezpečení](partner-security-requirements.md#security-defaults).
    - Pokud vyhovuje vašim obchodním potřebám, povolte zásady výchozího nastavení zabezpečení.
- Přechod na podmíněný přístup
    - Pokud zásady výchozích hodnot zabezpečení neodpovídají vašim potřebám, povolte podmíněný přístup. Další informace najdete v dokumentaci k podmíněnému přístupu ke službě Azure AD.

## <a name="key-resources"></a>Klíčové prostředky

### <a name="how-to-get-started"></a>Jak začít

- [Požadavky na zabezpečení partnera: podrobný průvodce](partner-security-requirements.md).
- Nasměrujte své dotazy a zpětnou vazbu do této [skupiny pokynů pro zabezpečení partnera](https://aka.ms/MPCSecurityGuidance).
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