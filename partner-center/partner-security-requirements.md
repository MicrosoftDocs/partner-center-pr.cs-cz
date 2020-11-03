---
title: Požadavky na zabezpečení partnerů
ms.topic: article
ms.date: 10/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zavádí požadavky partnerů na povolení vícefaktorového ověřování (MFA) a přijímá rozhraní zabezpečeného modelu aplikace.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c92e8c9a9a08582d89ef478a4600f737a548b787
ms.sourcegitcommit: 2847efac28d3bff24ed37cdfaa88ff4be06705c8
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/27/2020
ms.locfileid: "92680394"
---
# <a name="partner-security-requirements-for-partners-using-partner-center-or-partner-center-apis"></a>Požadavky na zabezpečení partnerů pro partnery pomocí partnerských Center nebo rozhraní API partnerského centra

**Platí pro**

- Všichni partneři v programu Cloud Solution Provider
  - Přímá faktura
  - Nepřímý poskytovatel
  - Nepřímý prodejce
- Všichni dodavatelé ovládacích panelů
- Všechny poradce

**Příslušné uživatele**

- Všichni povolení uživatelé včetně uživatelů typu Host

Vyšší zabezpečení ochrany osobních údajů a zabezpečení je z našich nejdůležitějších priorit. Víme, že nejlepší obrana je prevence a že máme jenom silný, jako náš slabý odkaz. Proto potřebujeme, aby všichni v našem ekosystému pracovali a zajistili správné fungování ochrany zabezpečení. Abychom vám pomohli chránit partnery a zákazníky, zavádíme sadu povinných požadavků na zabezpečení pro poradce, dodavatele ovládacích panelů a partnery účastnící se programu Cloud Solution Provider.

## <a name="overview"></a>Přehled

Partneři jsou povinni vymáhat službu Multi-Factor Authentication pro všechny uživatelské účty ve svém partnerském tenantovi. Podmínky spojené s partnerskými požadavky na zabezpečení byly přidány do smlouvy o partnerovi společnosti Microsoft. V souvislosti s poradci budou stejné smluvní požadavky zavedeny.

Partneři, kteří neimplementují povinné požadavky na zabezpečení, nebudou moci pracovat v programu Cloud Solution Provider ani spravovat klienty, kteří využívají delegovaná oprávnění správce, jakmile budou tyto požadavky vynutily. Kromě toho mohou partneři, kteří neimplementují požadavky na zabezpečení, zapojovat své účasti v ohrožených programech.  

Abychom vám a vašim zákazníkům chránili, je potřeba, aby partneři okamžitě provedli následující akce:  

1. **Povolte Multi-Factor Authentication (MFA) pro všechny uživatelské účty ve vašem partnerském tenantovi** . Všechny uživatelské účty ve vašich partnerských klientech musí být vyhodnoceny službou Multi-Factor Authentication (MFA) při přihlašování k komerčním cloudovým službám Microsoftu nebo při jejich transakčním programu prostřednictvím partnerského centra nebo prostřednictvím rozhraní API.

2. **Přijímají rozhraní zabezpečeného modelu aplikace** . Přijímají rozhraní zabezpečeného modelu aplikace. Všichni partneři integrující s rozhraním API partnerského centra musí pro všechny aplikace a modely ověřování uživatelů přijmout rozhraní API pro zabezpečení aplikačního modelu.

    > [!IMPORTANT]
    > Důrazně doporučujeme, aby partneři implementovali zabezpečený aplikační model pro integraci s rozhraním API Microsoftu, jako je například Azure Resource Manager, Microsoft Graph nebo využití automatizace, jako je například prostředí PowerShell s použitím přihlašovacích údajů uživatele, aby se předešlo jakémukoli narušení při vymáhání MFA.

Povolení Multi-Factor Authentication (MFA) a přijetí rozhraní Secure Application model Service Framework vám pomůže ochránit infrastrukturu a chránit zákaznická data před potenciálními bezpečnostními riziky, jako je identifikace krádeže nebo jiné incidenty podvodů.  

## <a name="actions-that-you-need-to-take"></a>Akce, které je třeba provést

Abyste vyhověli požadavkům na zabezpečení partnerů, musíte vymáhat službu Multi-Factor Authentication pro každý uživatelský účet v partnerském tenantovi. Můžete to udělat jedním z následujících způsobů:

- Implementují se [výchozí hodnoty zabezpečení Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

- Azure Active Directory Premium nákupu pro každý uživatelský účet. Další informace najdete v tématu [plánování cloudového nasazení Azure Multi-Factor Authentication](/azure/active-directory/authentication/howto-mfa-getstarted).

- Použití řešení třetí strany k vymáhání služby Multi-Factor Authentication pro každý uživatelský účet v partnerském tenantovi. Chcete-li zajistit, aby řešení poskytovalo očekávané řešení, přečtěte si téma [jak se vynutily požadavky na zabezpečení](#how-the-requirements-are-enforced).

> [!NOTE]
> I když se vícefaktorové ověřování nesmluvně nevyžaduje pro svrchovaný Cloud (21Vianet, státní správu USA a Německo), důrazně doporučujeme, abyste přijali tyto požadavky na zabezpečení.

## <a name="security-defaults"></a>Výchozí nastavení zabezpečení

Zásada výchozích hodnot zabezpečení je jednou z [možností](#actions-that-you-need-to-take) , které partneři můžou použít k implementaci vícefaktorového ověřování pro požadavky na zabezpečení v závislosti na jejich obchodních potřebách. Nabízí základní úroveň zabezpečení, která je povolená bez dalších poplatků. Než povolíte výchozí nastavení zabezpečení, přečtěte si, jak povolit vícefaktorové ověřování pro vaši organizaci pomocí Azure AD a klíčová doporučení níže.

- Základní zásady budou zůstat v následujících měsících a na konci února 2020 zastaraly cílení.

- Partneři, kteří již přijali základní zásady, musí provést akci přechodu na výchozí nastavení zabezpečení.

- Výchozími hodnotami zabezpečení jsou obecné náhrady základní dostupnosti zásad směrného plánu Preview. Jakmile partner povolí výchozí nastavení zabezpečení, již nebude moci povolit základní zásady.

- V případě výchozích hodnot zabezpečení budou všechny zásady povoleny najednou.

- Pro partnery, kteří používají [podmíněný přístup](/azure/active-directory/conditional-access/concept-conditional-access-policy-common), nebudou [výchozí hodnoty zabezpečení k dispozici](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults).

- Blokování starších verzí ověřování nebude v současnosti vynutilo pro partnery. Vzhledem k neúspěšným pokusům o přihlášení pomocí staršího ověřování ale partneři doporučujeme přesunout se z těchto starších protokolů, protože většina událostí týkajících se napadených identit nabývá od pokusů o přihlášení.

- Z výchozího nastavení zabezpečení je vyloučený účet Azure AD Connect synchronizace.

- Podrobné informace najdete v tématu [povolení Multi-Factor Authentication ve vaší organizaci](/azure/active-directory/authentication/concept-mfa-get-started) a ve [výchozím nastavení zabezpečení Azure Active Directory](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

> [!NOTE]
> Výchozím nastavením zabezpečení služby Azure AD je vývoj zásad ochrany základní úrovně zjednodušený. Pokud jste již povolili zásady ochrany základní úrovně, důrazně doporučujeme povolit výchozí nastavení zabezpečení.

Pokud chcete přejít ze základních zásad na výchozí nastavení zabezpečení, přečtěte si téma [co je výchozí nastavení zabezpečení?](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

### <a name="consideration"></a>Aspekty

Vzhledem k tomu, že se tyto požadavky vztahují na všechny uživatelské účty v partnerském tenantovi, je potřeba zvážit několik věcí, abyste zajistili hladké nasazení, včetně určení uživatelských účtů v Azure Active Directory, které nemůžou provádět vícefaktorové ověřování, a také aplikace a zařízení, které vaše organizace používá, které nepodporují moderní ověřování.

Před provedením jakékoli akce doporučujeme, abyste dokončili následující ověřování: 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Máte aplikaci nebo zařízení, které nepodporuje použití moderního ověřování?

Pokud využijete starší verzi ověřování služby Multi-Factor Authentication, budou zablokovány protokoly, jako jsou IMAP, POP3, SMTP atd., protože nepodporují službu Multi-Factor Authentication. Pro vyřešení tohoto omezení se dá použít funkce známá jako [hesla aplikací](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) , aby se zajistilo, že se aplikace nebo zařízení bude i nadále ověřovat. Pokud chcete zjistit, jestli je možné použít ve svém prostředí, Projděte si pokyny k používání hesel aplikací, které jsou popsané [tady](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) .

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>Máte uživatele, kteří používají Office 365, k dispozici prostřednictvím licencí přidružených k Vašemu partnerskému tenantovi?

Před implementací nějakého řešení doporučujeme určit, jakou verzi systém Microsoft Office uživatelé ve vašem partnerském tenantovi používají. Může se stát, že uživatelé budou mít problémy s připojením k aplikacím, jako je Outlook. Před vynucováním vícefaktorového ověřování je důležité zajistit, že se používá Outlook 2013 SP1 nebo novější a že má vaše organizace povolené moderní ověřování. Další informace najdete v tématu [Povolení moderního ověřování v systému Exchange Online](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online). 

Pokud chcete povolit moderní ověřování pro všechna zařízení s Windows, která mají nainstalovanou systém Microsoft Office 2013, budete muset vytvořit dva klíče registru. Viz [Povolení moderního ověřování pro Office 2013 na zařízeních s Windows](/office365/admin/security-and-compliance/enable-modern-authentication).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Brání některý z uživatelů, aby při práci používal jejich mobilní zařízení?

Je důležité identifikovat všechny podnikové zásady, které uživatelům brání v používání mobilních zařízení při práci, protože budou mít vliv na to, jaké řešení Multi-Factor Authentication implementujete. Existují řešení, jako je třeba ta, která je poskytována prostřednictvím implementace [výchozích hodnot zabezpečení Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults), která povoluje použití ověřovací aplikace jenom k ověření. Pokud má vaše organizace zásady prevence používání mobilních zařízení, vezměte v úvahu jednu z následujících možností:

- Nasazení TOTP aplikace založené na čase, která může běžet v zabezpečeném systému

- Implementujte řešení třetí strany, které vynutilo vícefaktorové ověřování pro každý uživatelský účet v partnerském tenantovi, který poskytuje nejvhodnější možnost ověřování.

- Nákup licencí [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) pro ovlivněné uživatele

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>Jakou automatizaci nebo integraci potřebujete k ověřování využít přihlašovací údaje uživatele?

Vzhledem k tomu, že je nutné vynutilit MFA pro každého uživatele, včetně účtů služeb, v adresáři partnerů bude ovlivněna jakákoli automatizace nebo integrace, která využívá přihlašovací údaje uživatele k ověřování. Proto je důležité zjistit, jaké účty se v těchto situacích používají. Podívejte se na následující seznam ukázkových aplikací nebo služeb, které je potřeba vzít v úvahu:

- Ovládací panel, který slouží ke zřízení prostředků jménem zákazníků

- Integrace s jakoukoli platformou, která se používá k fakturaci (ve vztahu k programu CSP) a podpoře vašich zákazníků

- Skripty PowerShellu, které využívají moduly AZ, AzureRM, Azure AD, MS online atd.

Výše uvedený seznam není vyčerpávající. Proto je důležité, abyste provedli kompletní posouzení jakékoli aplikace nebo služby ve vašem prostředí, která využívá přihlašovací údaje uživatele pro ověřování. Chcete-li soupeří s požadavkem na vícefaktorové ověřování, měli byste implementovat doprovodné materiály v [rozhraní zabezpečeného modelu aplikace](/partner-center/develop/enable-secure-app-model) , kde je to možné.

## <a name="accessing-your-environment"></a>Přístup k prostředí

Pro lepší pochopení toho, co nebo kdo se ověřuje bez výzvy k ověření služby Multi-Factor Authentication, doporučujeme zkontrolovat aktivitu přihlášení. Prostřednictvím Azure Active Directory Premium můžete využít sestavu přihlášení. Další informace o tomto tématu najdete v [sestavách aktivit přihlašování na portálu Azure Active Directory](/azure/active-directory/reports-monitoring/concept-sign-ins). Pokud nemáte Azure Active Directory Premium nebo hledáte způsob, jak získat tuto přihlašovací aktivitu prostřednictvím PowerShellu, budete muset využít rutinu [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity)  z modulu [portálu pro partnery v prostředí PowerShell](https://www.powershellgallery.com/packages/PartnerCenter/) .

## <a name="how-the-requirements-are-enforced"></a>Jak se vynutily požadavky

Požadavky na zabezpečení partnera vynutila Azure Active Directory a v centru partnerských serverů kontrolují přítomnost deklarace MFA, aby identifikovali, že bylo provedeno ověřování službou Multi-Factor Authentication. Od 18. listopadu 2019 společnost Microsoft aktivovala další bezpečnostní zabezpečení (dříve označované jako "technické vynucování") do partnerských tenantů.

Při aktivaci se uživatelé v partnerském tenantovi budou požádáni, aby při provádění všech operací s oprávněními správce (ADMINISTRATE), přístupu k portálu partnerského centra nebo volání rozhraní API partnerského centra vyžádali ověření MFA (Multi-Factor Authentication). Další podrobné informace najdete v tématu [Mandating Multi-Factor Authentication (MFA) pro vašeho partnerského tenanta](partner-security-requirements-mandating-mfa.md). 

Partneři, kteří tyto požadavky nesplnili, by měli co nejdříve implementovat tyto míry, abyste se vyhnuli jakýmkoli výpadkům v podniku. 

Pokud používáte výchozí nastavení zabezpečení Azure Multi-Factor Authentication nebo Azure AD, nemusíte provádět žádné další kroky.

Pokud používáte řešení Multi-Factor Authentication od jiného výrobce, je možné, že se deklarace MFA nevydá. Pokud tato deklarace identity chybí, Azure Active Directory nebude moct určit, jestli se žádost o ověření nastoupila službou Multi-Factor Authentication. Informace o tom, jak ověřit, že vaše řešení vydává očekávanou deklaraci identity, najdete v tématu [testování požadavků na zabezpečení partnera](/powershell/partnercenter/test-partner-security-requirements). 

> [!IMPORTANT]
> Pokud vaše řešení třetí strany nevydá očekávanou deklaraci identity, budete muset spolupracovat s dodavatelem, který řešení vyvinul, abyste zjistili, jaké akce by se měly provést.

## <a name="resources-and-support"></a>Zdroje a podpora

Informace o podpoře a ukázkovém kódu najdete v následujících zdrojích informací:

- [Komunita poradenského centra zabezpečení](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): komunitní komunita Příručka zabezpečení je online komunita, kde se můžete dozvědět o nadcházejících událostech a položit se na případné dotazy.
- [Ukázky pro Partnerský portál .NET](https://github.com/microsoft/partner-center-dotnet-samples): Toto úložiště GitHub obsahuje ukázky, vyvinuté pomocí .NET, které demonstrují, jak můžete implementovat rozhraní zabezpečeného aplikačního modelu.
- [Ukázky pro Partnerský portál Java](https://github.com/microsoft/partner-center-java-samples): Toto úložiště GitHub obsahuje ukázky, vyvinuté v jazyce Java, které demonstrují, jak můžete implementovat rozhraní zabezpečeného aplikačního modelu.
- [Prostředí PowerShell pro Partnerský portál – Multi-Factor Authentication](/powershell/partnercenter/multi-factor-auth): Tento Multi-Factor Authentication článek poskytuje podrobné informace o tom, jak implementovat rozhraní zabezpečeného modelu aplikace pomocí prostředí PowerShell.