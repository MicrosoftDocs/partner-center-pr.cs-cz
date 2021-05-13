---
title: Přesun z centra členství v partnerovi
ms.topic: article
ms.date: 06/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si užitečné informace a nejčastější dotazy před přesunem firmy z partnerského centra členství do partnerského centra.
author: parthpandyamsft
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 7f533240d5236f03fe277d4c6dfa02ed1c58b63c
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855008"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Příprava na přesun z partnerského centra členství (PMC) do partnerského centra

**Příslušné role**: globální správce | Správce správy uživatelů | Prodejní agent | Agent správce

Přesouváme správu členství z partnerského centra členství (PMC) do partnerského centra – jediné místo pro správu vašeho obchodního vztahu s Microsoftem. Chceme, aby váš přesun do partnerského centra byl co nejefektivnější a co nejjednodušší. Identifikovali jsme některé oblasti, ve kterých se partnerské Centrum liší od PMC, a myslíme si, že před tím, než ho přesunete, bude pro ně potřeba pochopit a připravit.

## <a name="account-and-identity-setup"></a>Nastavení účtu a identity

V následujícím seznamu najdete odpovědi na běžné otázky týkající se nastavení účtu a identity.

### <a name="what-is-an-azure-active-directory-azure-ad-work-account"></a>Co je pracovní účet Azure Active Directory (Azure AD)?

Pracovní účet Azure je vyhrazená a izolovaná virtuální reprezentace vaší společnosti ve veřejném cloudu Azure, která se vytvoří po přihlášení k odběru cloudové služby Microsoftu, jako je Azure, Microsoft Intune nebo Office 365.

Váš pracovní účet je hostitelem uživatelů Azure AD a informací o nich – jejich e-maily, hesla, data profilu, oprávnění atd. Pracovní účet obsahuje také skupiny, aplikace a další informace, které se týkají společnosti a jejího zabezpečení. 

Pracovní e-mail je součástí tenanta Azure Active Directory. Pokud chcete mít účet v partnerském centru, musíte mít tenanta AAD. Pokud chcete získat další informace o Azure Active Directory, přečtěte si téma [Vytvoření adresáře ve službě Azure AD](/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).

V partnerském centru použijete pracovní e-mail k přihlášení k vašemu účtu, ne k vašemu osobnímu e-mailu.

- Váš pracovní účet: john@contoso.com
- Váš osobní účet: John@outlook.com

### <a name="what-account-should-you-sign-into-partner-center-with-if-you-have-an-aad-tenant-with-microsoft-for-office-365-for-example-and-you-also-have-a-tenant-for-your-csp-business"></a>Jaký účet by měl být přihlášený k partnerskému centru s tím, že máte tenanta služby AAD s Microsoftem (například pro Office 365) a také máte tenanta pro podnikání vašeho poskytovatele CSP?

Můžete se přihlásit k Partnerské centrum pomocí účtu CSP nebo pracovního e-mailového účtu MPN. Pokud se rozhodnete přihlásit pomocí pracovního e-mailu CSP, v levém navigačním panelu na řídicím panelu se zobrazí informace o programu MPN i CSP. Pokud se přihlásíte pomocí pracovního e-mailu tenanta Azure AD MPN, zobrazí se pouze informace o programu MPN. 

### <a name="if-you-dont-want-to-use-your-existing-office-365-azure-ad-tenant-for-partner-center-you-can-create-a-new-tenant-prior-to-migrating-from-pmc"></a>Pokud nechcete používat stávajícího tenanta Azure AD Office 365 pro Partnerské centrum, můžete před migrací z PMC vytvořit nového tenanta.

K nastavení účtu služby Azure AD může dojít z mnoha důvodů, Partnerské centrum tenanta Azure AD. Než začnete s migrací na Partnerské centrum, [](https://ms.portal.azure.com/#home) přejděte do Azure Portal a vytvořte nového tenanta Azure AD. Postupujte podle pokynů v [tématu Vytvoření nového tenanta v Azure Active Directory](/azure/active-directory/develop/quickstart-create-new-tenant). Použijte nového tenanta AAD k nastavení Partnerské centrum účtu. Abyste tenanta vytvořili, musíte být globálním správcem. 

### <a name="user-roles-including-guest-user-roles-in-partner-center"></a>Role uživatelů včetně rolí uživatelů hosta v Partnerské centrum

Partnerské centrum různé typy rolí v závislosti na typech práce, které je potřeba provést. Existují role, jako je globální správce, které jsou rolemi Azure AD. Některé role jsou specifické pro programy, jako je program cloudových služeb nebo pobídky, a existují role, které jsou specifické pro MPN. Pokud chcete zjistit, jaké jsou všechny Partnerské centrum role, přečtěte si o přiřazení [rolí a oprávnění uživatelů.](permissions-overview.md)

### <a name="what-happens-to-my-users-roles-when-they-move-from-pmc-to-partner-center"></a>Co se stane s rolemi uživatelů při přechodu z PMC na Partnerské centrum?

S výjimkou kontaktu globálního správce MPN nebo primárního programu, který migraci provádí, přijde všichni uživatelé v PMC o své role správce. Jednotlivec, který migraci dokončí, bude muset přiřadit role v Partnerské centrum. Role v Partnerské centrum liší od rolí v PMC. Přečtěte si [Přiřazení uživatelských rolí a oprávnění](permissions-overview.md a [Moving from PMC to Partnerské centrum](move-pmc-pc-map.md#user-roles) for more on user roles in Partnerské centrum.

### <a name="whats-the-difference-between-my-company-profile-and-my-business-profile"></a>Jaký je rozdíl mezi profilem společnosti a obchodním profilem?

Profil vaší společnosti obsahuje informace o vaší společnosti, včetně adresy, umístění, primárního kontaktu, banky a daňových údajů.

Váš obchodní profil je způsob, jakým se prezentuje zákazníkům, a je to marketingová stránka, která zobrazuje vaše logo, podrobnosti o zaměření vaší firmy, vaše odborné znalosti atd.

### <a name="what-does-account-consolidation-mean-for-my-account"></a>Co pro můj účet znamená konsolidace účtů?

Pokud k migraci několika účtů MPN do služby Partnerské centrum použijete stejného tenanta Azure AD, systém to automaticky rozpozná a požádá vás o konsolidaci účtů. To platí i v případě, že ke stejnému tenantovi Azure AD máte přidružených více domén. 

Přesto se můžete rozhodnout migrovat na Partnerské centrum pomocí samostatných tenantů AAD, ale všimněte si, že výsledkem je izolované vyhodnocení vašich kompetencí a dalších nákladů na nákup. Další informace o konsolidaci účtů najdete v přečtěte si o [konsolidaci firemních účtů.](consolidate-accounts.md)

### <a name="if-i-have-multiple-aad-tenants-and-a-single-mpn-account-is-it-possible-to-link-them-in-partner-center"></a>Pokud mám více tenantů AAD a jeden účet MPN, je možné je propojit v Partnerské centrum?

Ano, v Partnerské centrum můžete propojit více tenantů Azure AD s jedním Partnerské centrum účtem.
Další informace o konsolidaci účtů najdete v přečtěte si o [konsolidaci firemních účtů.](consolidate-accounts.md)

### <a name="are-there-restrictions-to-adding-multiple-azure-ad-tenants-to-a-single-partner-center-account"></a>Existují omezení pro přidání více tenantů Azure AD do jednoho Partnerské centrum účtu?

Pokud už je tenant Azure AD přidružený k existujícímu účtu Partnerské centrum, není možné ho pomocí funkce více tenantů Partnerské centrum k novým účtům tenantů. Dalším způsobem, jak si to můžete myslet, je, že tenanta Azure AD je možné přidružené pouze k jednomu účtu Partnerské centrum, ale k účtu Partnerské centrum může být přidružených více tenantů.

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Microsoft Partner Network (MPN) 

Podívejte se na následující odpovědi na běžné dotazy týkající se migrace členství v programu MPN.

### <a name="who-can-perform-the-move-from-pmc-to-partner-center"></a>Kdo může provést přesun z PMC do Partnerské centrum?

Váš globální správce MPN vaší společnosti nebo primární kontakt programu (tyto dvě role často vlastní stejná osoba) může iniciovat a provést přesun.

### <a name="will-the-person-completing-the-migration-become-the-primary-contact-on-the-company-legal-profile-in-partner-center"></a>Bude se osoba, která dokončení migrace stane primárním kontaktem na oficiální profil společnosti v partnerském centru?

Primární kontakt ale nemusí být nutně osoba, která má autorizaci k podepisování smluv.

### <a name="can-microsoft-migrate-my-mpn-membership-for-me"></a>Může Microsoft migrovat svoje členství v programu MPN?

No. Společnost Microsoft vám nemůže přesunout váš účet členství do partnerského centra. Pokud chcete zahájit proces migrace, budete muset svůj účet přesunout pomocí přihlášení k PMC pomocí svého pracovního účtu (přihlašovací údaje). Po dokončení postupu pro přesunutí účtu můžete začít spravovat členství a přiřazovat role uživatelů a oprávnění k vašemu týmu, aby mohli získat přístup k výhodám a lépe spravovat členství. 

Microsoft automaticky migruje aktuální kompetence, výhody, informace o poloze, banku a daňové informace pro pobídky a asociace MCP, včetně partnerského přístupu k partnerské škole.

### <a name="how-will-the-renewal-policy-change"></a>Jak se změní zásady obnovování?

V partnerském centru je okno obnovení od data výročí v následujících 30 dnech.

### <a name="will-our-competencies-remain-unchanged-after-we-move-to-partner-center"></a>Budou naše kompetence po přesunu do partnerského centra stále beze změny?

Ano, kompetence nebudou ovlivněny přesunem do partnerského centra. Pokud si všimnete rozporů, obraťte se na [podporu](https://partner.microsoft.com/support).

### <a name="will-my-benefits-including-cloud-benefits-technical-support-software-benefits-visual-studio-change-after-we-move"></a>Budou mé výhody (včetně výhod cloudu, technické podpory, výhod softwaru, sady Visual Studio) po přesunu změněny?

Vaše vhodné výhody se nemění. Pokud si všimnete rozporů, obraťte se na [podporu](https://partner.microsoft.com/support).

### <a name="will-our-microsoft-accounts-that-have-visual-studio-benefits-allocations-be-honored"></a>Budou se respektovat naše účty Microsoft, které mají přidělení výhod sady Visual Studio?

Ano. Výhody sady Visual Studio přidělené účty spravované služby se budou respektovat a uchovávat. Po obnovení v partnerském centru budou taky zachované. Pokud ale přidělení MSA odeberete po migraci v partnerském centru, nejde ho přidat zpátky do partnerského centra.

V partnerském centru může partner přidat pracovní účty a uživatelské účty hosta, které jsou MSA ze stejného tenanta, ve kterém je partner správce MPN v tenantovi Azure AD. Pokud je partner globálním správcem ve více tenantech Azure AD a všechny tyto tenanty jsou přidružené ke stejnému účtu Partnerské centrum, pak partner může přidávat uživatele mezi všechny tyto tenanty do výhod Visual Studio a přidělování na základě využití Azure.

I když správce MPN nebo globální správce může uživatelům guest přiřadit předplatná služby Visual Studio na základě využití, uživatelé guest se k přihlášení Partnerské centrum pomocí MSA. Uživatelé hosta se ale mohou přihlásit k Azure a Visual Studio ověřit a využít své přiřazené výhody.

### <a name="how-should-we-manage-our-mcp-associations-and-our-partner-university-access"></a>Jak bychom měli spravovat přidružení MCP a přístup k Partner University?

Přidružení MCP se od PMC nemění. Noví zaměstnanci po přechodu na Partnerské centrum ale budou muset být přidruženi v Partnerské centrum. Všechna vaše oprávnění Partner University pro stávající uživatele zůstanou, ale noví zaměstnanci by měli přejít do školicích centra, kde najdete informace o tom, jak získat přístup k Partner University. [](https://partner.microsoft.com/training)

### <a name="how-do-i-view-mcp-information-once-i-move-to-partner-center"></a>Návody informace o MCP po přechodu na Partnerské centrum?

V **levém navigačním** panelu na řídicím panelu vyberte Kompetence. Na **stránce Kompetence** si můžete stáhnout sestavu dovedností. Sestava dovedností zobrazí seznam uživatelů, kteří získali dovednosti související s kompetencemi a programy v Partnerské centrum. Pokud vaši uživatelé získali dovednosti, ale tyto dovednosti nejsou relevantní pro kompetence, na které pracujete, nebudou uvedené v sestavě.

### <a name="are-customer-references-used-in-partner-center"></a>Používají se referenční informace zákazníků v Partnerské centrum?

Ne, ke splnění požadavků na kompetence v nástroji Partnerské centrum.

### <a name="will-partner-of-record-associations-move-to-partner-center"></a>Přesunou se přidružení partnerů záznamů do Partnerské centrum?

Ano, u partnera záznamu se nic nemění. Další informace o propojení ID partnera se [zákazníky.](/azure/billing/billing-partner-admin-link-started)

### <a name="is-there-an-impact-to-incentives-because-of-the-move-to-partner-center"></a>Má přechod na nové prostředí Partnerské centrum dopad na pobídky?

Ne, pobídky nemají žádný vliv, pokud jste přesunuli svůj účet bez konsolidace umístění. Pokud má vaše firma více účtů v PMC a při přesunu do partnerského centra, které se rozhodnete konsolidovat do globálního účtu, nedojde ke ztrátě informací, ale může dojít ke zpoždění v pobídkovém vyvýběru. 

Pokud nepřesunete všechny účty PMC, které byly součástí programu pobídek, můžete přestat získávat pobídky, které jsou svázané s těmito účty.

### <a name="what-are-the-incentive-roles-in-partner-center"></a>Jaké jsou role k disměně v partnerském centru?

Role rolí v partnerském centru jsou založené na umístění a zahrnují pobídky správce a pobídky uživatele. Další informace o tom, co tyto role mohou provádět, najdete v tématu [přiřazení rolí uživatelů a oprávnění](permissions-overview.md).

### <a name="can-incentives-admins-be-assigned-at-the-global-and-location-level"></a>Je možné přiřazovat správce na úrovni globálních a umístění?

Ano. Můžete přiřadit správce pobídek jako správce pobídek pro všechna umístění nebo každé umístění může mít svého vlastního správce pobídek.

### <a name="can-incentives-be-paid-at-the-global-or-location-level"></a>Je možné je vyplatit na globální úrovni nebo na úrovni umístění?

Pobídky jsou vypláceny pouze na úrovni umístění.

### <a name="regarding-referrals-how-many-business-profiles-can-we-create"></a>V souvislosti s referenčními informacemi, kolik obchodních profilů můžeme vytvořit?

Vaše společnost může vytvořit tolik obchodních profilů, kolik budete potřebovat k úplnému vyjádření zájmů vaší společnosti. V každém obchodním profilu můžete seznamovat až pět umístění, jedno místo na zemi. Každý z obchodních profilů může získat referenčních seznamů pro každé z jeho umístění.

### <a name="how-will-referrals-be-assigned-what-changes-can-i-expect-for-example-if-i-have-a-global-company-in-one-market-and-locations-in-other-markets-how-will-referrals-be-assigned"></a>Jak budou odkazy přiřazeny, jaké změny je možné očekávat? Například pokud mám globální společnost na jednom trhu a umístění na jiných trzích, jak budou odkazy přiřazeny?

Odkazy jsou přiřazeny na základě parametrů hledání, které zákazník definuje. Bez ohledu na to, jestli máte jedno nebo mnoho umístění, pokud zákazník zadá požadované umístění a máte firmu, která splňuje ostatní parametry, odkaz by přešel do tohoto umístění.

### <a name="i-am-migrating-to-partner-center-from-within-russia-i-get-an-error-message-about-web-direct-how-do-i-continue-with-the-migration"></a>Migruju do partnerského centra z Ruska. Zobrazí se chybová zpráva o webu Direct. Návody pokračovat v migraci?

Pokud se vám zobrazí chybová zpráva, protože se účastníte programu Web Direct, měli byste provést následující kroky:

1. Přihlaste se k portálu. Azure.com a vytvořte nového tenanta Azure AD. Další informace najdete v [tématu Vytvoření nového tenanta Azure AD.](/azure/active-directory/fundamentals/active-directory-access-create-new-tenant)

2. Po vytvoření nového tenanta Azure AD ho použijte k migraci z Partner Membership Center do Partnerské centrum nebo k registraci jako nový tenant Partnerské centrum.