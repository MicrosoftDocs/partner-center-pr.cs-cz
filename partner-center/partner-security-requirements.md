---
title: Požadavky na zabezpečení partnerů
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zavádí požadavky na zabezpečení partnerů pro povolení vícefaktorového ověřování (MFA) a zajištění architektury zabezpečeného aplikačního modelu.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 351d0715645b6e43607279393cdc376d898a7f54
ms.sourcegitcommit: 98f5eebe7d08ba214ed5a078f1ac770439e41eb7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/31/2020
ms.locfileid: "93132973"
---
# <a name="security-requirements-for-using-partner-center-or-partner-center-apis"></a>Požadavky na zabezpečení pro používání partnerských Center nebo rozhraní API partnerského centra

**Platí pro**

- Všichni partneři v programu Cloud Solution Provider
- Všichni dodavatelé ovládacích panelů
- Všechny poradce

**Příslušné uživatele**

- Všichni povolení uživatelé včetně uživatelů typu Host

Tento článek vysvětluje povinné požadavky na zabezpečení pro poradce, výrobce ovládacích panelů a partnery účastnící se programu Cloud Solution Provider a také možnosti ověřování a další informace o zabezpečení. Ochrana osobních údajů a zabezpečení je z našich nejdůležitějších priorit. Víme, že nejlepší obrana je prevence a že máme jenom silný, jako náš slabý odkaz. Proto potřebujeme, aby všichni v našem ekosystému pracovali a zajistili správné fungování ochrany zabezpečení.

## <a name="mandatory-security-requirements"></a>Povinné požadavky na zabezpečení

Partneři, kteří neimplementují povinné požadavky na zabezpečení, nebudou moci pracovat v programu Cloud Solution Provider ani spravovat klienty zákazníka, kteří využívají delegovaná práva správce. Kromě toho mohou partneři, kteří neimplementují požadavky na zabezpečení, zapojovat své účasti v ohrožených programech. Podmínky spojené s partnerskými požadavky na zabezpečení byly přidány do smlouvy o partnerovi společnosti Microsoft. V souvislosti s poradci budou stejné smluvní požadavky zavedeny.

Abychom vám a vašim zákazníkům chránili, je potřeba, aby partneři okamžitě provedli následující akce:  

1. **Povolte službu Multi-Factor Authentication (MFA) pro všechny uživatelské účty ve vašem partnerském tenantovi** . U všech uživatelských účtů ve vašich partnerských klientech musíte vymáhat MFA. Pokud se uživatelé přihlásí k komerčním cloudovým službám Microsoftu nebo když budou v programu Cloud Solution Provider prostřednictvím partnerského centra nebo přes rozhraní API, musí je vyvolávat ověřování MFA.

2. **Přijímají rozhraní zabezpečeného modelu aplikace** . Všichni partneři integrující s rozhraními API partnerského centra musí pro všechny aplikace a modely ověřování uživatelů přijmout rozhraní [Secure Application model](/partner-center/develop/enable-secure-app-model) .

    > [!IMPORTANT]
    > Důrazně doporučujeme, aby partneři implementovali zabezpečený aplikační model pro integraci s rozhraním Microsoft API, jako je Azure Resource Manager nebo Microsoft Graph, nebo když využíváte automatizaci, jako je například PowerShell s použitím přihlašovacích údajů uživatele, abyste se vyhnuli jakémukoli narušení při vymáhání MFA.

Tyto požadavky na zabezpečení vám pomůžou ochránit infrastrukturu a chránit data vašich zákazníků před potenciálními bezpečnostními riziky, jako je identifikace krádeže nebo jiné incidenty v podvodu.  

## <a name="implementing-multi-factor-authentication"></a>Implementace Multi-Factor Authentication

Abyste vyhověli požadavkům na zabezpečení partnerů, musíte implementovat a vymáhat MFA pro každý uživatelský účet v partnerském tenantovi. Můžete to udělat jedním z následujících způsobů:

- Implementujte [výchozí hodnoty zabezpečení Azure Active Directory (Azure AD)](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults). Další informace najdete v [Další části](#security-defaults).

- Zakupte Azure Active Directory Premium pro každý uživatelský účet. Další informace najdete v tématu [Plánování nasazení služby Azure Multi-Factor Authentication](/azure/active-directory/authentication/howto-mfa-getstarted).

- Pomocí řešení třetí strany vyvynuťte MFA pro každý uživatelský účet ve vašem partnerském tenantovi. Chcete-li zajistit, aby řešení poskytovalo očekávané řešení, přečtěte si téma [jak se vynutily požadavky na zabezpečení](#how-the-requirements-are-enforced).

> [!NOTE]
> I když se vícefaktorové ověřování pro svrchovaný Cloud (státní správu a Německo) nevyžaduje pro službu Multi-Factor Authentication, důrazně doporučujeme, abyste přijali tyto požadavky na zabezpečení.

### <a name="security-defaults"></a>Výchozí nastavení zabezpečení

Jedna z možností, které mohou partneři vybrat k implementaci požadavků MFA, je povolit výchozí nastavení zabezpečení ve službě Azure AD. Výchozí nastavení zabezpečení nabízí základní úroveň zabezpečení bez dalších poplatků. Než povolíte výchozí nastavení zabezpečení, přečtěte si, jak povolit vícefaktorové ověřování pro vaši organizaci pomocí Azure AD a klíčová doporučení níže.

- Partneři, kteří již přijali základní zásady, musí provést akci přechodu na výchozí nastavení zabezpečení.

- Výchozími hodnotami zabezpečení jsou obecné náhrady základní dostupnosti zásad směrného plánu Preview. Jakmile partner povolí výchozí nastavení zabezpečení, již nebude moci povolit základní zásady.

- V případě výchozích hodnot zabezpečení budou všechny zásady povoleny najednou.

- Pro partnery, kteří používají [podmíněný přístup](/azure/active-directory/conditional-access/concept-conditional-access-policy-common), nebudou [výchozí hodnoty zabezpečení k dispozici](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults).

- V tuto chvíli neblokujeme starší verze ověřování. Vzhledem k neúspěšným pokusům o přihlášení pomocí staršího ověřování ale partneři doporučujeme přesunout se z těchto starších protokolů, protože většina událostí týkajících se napadených identit nabývá od pokusů o přihlášení.

- Z výchozího nastavení zabezpečení je vyloučený účet Azure AD Connect synchronizace.

Podrobné informace najdete v tématu [přehled Multi-Factor Authentication Azure pro vaši organizaci](/azure/active-directory/authentication/concept-mfa-get-started) a o [tom, co jsou to výchozí zabezpečení?](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

> [!NOTE]
> Výchozím nastavením zabezpečení služby Azure AD je vývoj zásad ochrany základní úrovně zjednodušený. Pokud jste již povolili zásady ochrany základní úrovně, důrazně doporučujeme povolit [výchozí nastavení zabezpečení](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

## <a name="implementation-considerations"></a>Důležité informace o implementaci

Vzhledem k tomu, že se tyto požadavky vztahují na všechny uživatelské účty v partnerském tenantovi, je potřeba zvážit několik věcí, abyste zajistili hladké nasazení. Identifikujte například uživatelské účty ve službě Azure AD, které nemůžou provádět MFA, a také aplikace a zařízení ve vaší organizaci, které nepodporují moderní ověřování.

Před provedením jakékoli akce doporučujeme, abyste dokončili následující ověřování. 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Máte aplikaci nebo zařízení, které nepodporuje použití moderního ověřování?

Když využijete MFA, budou starší verze ověřování používat protokoly, jako jsou IMAP, POP3, SMTP atd., budou blokované, protože nepodporují MFA. Pro vyřešení tohoto omezení použijte funkci [hesla aplikací](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) , abyste zajistili, že se aplikace nebo zařízení bude i nadále ověřovat. Přečtěte si téma [požadavky na používání hesel aplikací](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) k určení, jestli se dají použít ve vašem prostředí.

#### <a name="do-you-have-office-365-users-with-licenses-associated-with-your-partner-tenant"></a>Máte uživatelé Office 365 s licencemi přidruženými k Vašemu partnerskému tenantovi?

Před implementací nějakého řešení doporučujeme určit, jakou verzi systém Microsoft Office uživatelé ve vašem partnerském tenantovi používají. Může se stát, že uživatelé budou mít problémy s připojením k aplikacím, jako je Outlook. Před vynucováním MFA je důležité, abyste měli jistotu, že používáte Outlook 2013 SP1 nebo novější a že má vaše organizace povolené moderní ověřování. Další informace najdete v tématu [Povolení moderního ověřování v systému Exchange Online](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online). 

Pokud chcete povolit moderní ověřování pro zařízení s Windows, která mají nainstalované systém Microsoft Office 2013, budete muset vytvořit dva klíče registru. Viz [Povolení moderního ověřování pro Office 2013 na zařízeních s Windows](/office365/admin/security-and-compliance/enable-modern-authentication).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Brání některý z uživatelů, aby při práci používal jejich mobilní zařízení?

Je důležité identifikovat všechny podnikové zásady, které uživatelům brání v používání mobilních zařízení při práci, protože budou mít vliv na to, jaké řešení MFA implementujete. Existují řešení, jako je třeba ta, která je poskytována prostřednictvím implementace [výchozích hodnot zabezpečení Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults), která povoluje použití ověřovací aplikace jenom k ověření. Pokud má vaše organizace zásady prevence používání mobilních zařízení, vezměte v úvahu jednu z následujících možností:

- Nasaďte čas založený na hesle (TOTP) založeném na čase, který může běžet v zabezpečeném systému.

- Implementujte řešení třetí strany, které vynutilo MFA pro každý uživatelský účet v partnerském tenantovi, který poskytuje nejvhodnější možnost ověřování.

- Zakupte licence [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) pro ovlivněné uživatele.

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>Jakou automatizaci nebo integraci potřebujete k ověřování využít přihlašovací údaje uživatele?

Vzhledem k tomu, že vynutili VÍCEFAKTOROVÉ ověřování pro každého uživatele, včetně účtů služby, ve vašem partnerském adresáři, bude to mít vliv na jakoukoli automatizaci nebo integraci, která využívá přihlašovací údaje uživatele k ověření. Proto je důležité určit, které účty se v těchto situacích používají. Podívejte se na následující seznam ukázkových aplikací nebo služeb, které je potřeba vzít v úvahu:

- Ovládací panel, který slouží ke zřízení prostředků jménem zákazníků

- Integrace s jakoukoli platformou, která se používá k fakturaci (ve vztahu k programu CSP) a podpoře vašich zákazníků

- Skripty PowerShellu, které využívají moduly AZ, AzureRM, Azure AD, MS online atd.

Výše uvedený seznam není vyčerpávající. Proto je důležité, abyste provedli kompletní posouzení jakékoli aplikace nebo služby ve vašem prostředí, která využívá přihlašovací údaje uživatele pro ověřování. Pokud chcete soupeří s požadavkem na MFA, měli byste implementovat pokyny v [rozhraní Secure Application model](/partner-center/develop/enable-secure-app-model) , kde je to možné.

## <a name="accessing-your-environment"></a>Přístup k prostředí

Chcete-li lépe pochopit, co nebo kdo se ověřuje bez výzvy pro MFA, doporučujeme zkontrolovat aktivitu přihlášení. Prostřednictvím Azure Active Directory Premium můžete využít sestavu přihlášení. Další informace o tomto tématu najdete v tématu [sestavy aktivit přihlašování na portálu Azure Active Directory](/azure/active-directory/reports-monitoring/concept-sign-ins). Pokud nemáte Azure Active Directory Premium nebo hledáte způsob, jak získat tuto přihlašovací aktivitu prostřednictvím PowerShellu, budete muset využít rutinu [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity) z modulu [portálu pro partnery v prostředí PowerShell](https://www.powershellgallery.com/packages/PartnerCenter/) .

## <a name="how-the-requirements-are-enforced"></a>Jak se vynutily požadavky

Požadavky na zabezpečení partnera vynutila služba Azure AD a v partnerském centru si můžete zkontrolovat přítomnost deklarace MFA, abyste identifikovali, že ověření MFA bylo provedeno. Od 18. listopadu 2019 společnost Microsoft aktivovala další bezpečnostní zabezpečení (dříve označované jako "technické vynucování") do partnerských tenantů.

Při aktivaci se uživatelé v partnerském tenantovi budou požádáni, aby při provádění všech operací ADMINISTRATE (správce), přístupu k portálu partnerského centra nebo volání rozhraní API partnerského centra dokončili ověřování MFA. Další informace najdete v tématu [Mandating Multi-Factor Authentication (MFA) pro vašeho partnerského tenanta](partner-security-requirements-mandating-mfa.md). 

Partneři, kteří tyto požadavky nesplnili, by měli co nejdříve implementovat tyto míry, abyste se vyhnuli jakýmkoli výpadkům v podniku. Pokud používáte výchozí nastavení zabezpečení Azure Multi-Factor Authentication nebo Azure AD, nemusíte provádět žádné další kroky.

Pokud používáte řešení MFA od jiného výrobce, je možné, že se deklarace MFA nevydá. Pokud tato deklarace identity chybí, Azure AD nebude moct zjistit, jestli je žádost o ověření ověřená MFA. Informace o tom, jak ověřit, že vaše řešení vydává očekávanou deklaraci identity, najdete v tématu [testování požadavků na zabezpečení partnera](/powershell/partnercenter/test-partner-security-requirements). 

> [!IMPORTANT]
> Pokud vaše řešení třetí strany nevydá očekávanou deklaraci identity, budete muset spolupracovat s dodavatelem, který řešení vyvinul, abyste zjistili, jaké akce by se měly provést.

## <a name="resources-and-samples"></a>Prostředky a ukázky

Informace o podpoře a ukázkovém kódu najdete v následujících zdrojích informací:

- [Komunita poradenského centra zabezpečení](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): komunitní komunita Příručka zabezpečení je online komunita, kde se můžete dozvědět o nadcházejících událostech a položit se na případné dotazy.
- [Ukázky pro Partnerský portál .NET](https://github.com/microsoft/partner-center-dotnet-samples): Toto úložiště GitHub obsahuje ukázky, vyvinuté pomocí .NET, které demonstrují, jak můžete implementovat rozhraní zabezpečeného aplikačního modelu.
- [Ukázky pro Partnerský portál Java](https://github.com/microsoft/partner-center-java-samples): Toto úložiště GitHub obsahuje ukázky, vyvinuté v jazyce Java, které demonstrují, jak můžete implementovat rozhraní zabezpečeného aplikačního modelu.
- [Prostředí PowerShell pro Partnerský portál – Multi-Factor Authentication](/powershell/partnercenter/multi-factor-auth): Tento Multi-Factor Authentication článek poskytuje podrobné informace o tom, jak implementovat rozhraní zabezpečeného modelu aplikace pomocí prostředí PowerShell.

## <a name="next-steps"></a>Další kroky

- [Mandating Multi-Factor Authentication (MFA) pro vašeho partnerského tenanta](partner-security-requirements-mandating-mfa.md)