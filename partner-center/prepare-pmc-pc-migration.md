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
ms.openlocfilehash: be4250864bd07e555b0eb2079c28f3dfb4920805
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/22/2020
ms.locfileid: "92527327"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Příprava na přesun z partnerského centra členství (PMC) do partnerského centra

**Příslušné role**
- Globální správce
- Správce uživatelů
- Agent prodeje
- Agent správce

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

Do partnerského centra se můžete přihlásit buď pomocí účtu CSP, nebo e-mailového účtu MPN. Pokud se rozhodnete přihlásit pomocí pracovního e-mailu CSP, v levém navigačním panelu se zobrazí informace o programu MPN i CSP. Pokud se přihlásíte pomocí pracovního e-mailu tenanta MPN Azure AD, zobrazí se jenom informace o programu MPN. 

### <a name="if-you-dont-want-to-use-your-existing-office-365-azure-ad-tenant-for-partner-center-you-can-create-a-new-tenant-prior-to-migrating-from-pmc"></a>Pokud nechcete používat stávající tenant Azure AD pro partnerské Centrum pro Office 365, můžete před migrací z PMC vytvořit nového tenanta.

Může existovat mnoho důvodů, proč nechcete použít stávajícího tenanta Azure AD k nastavení účtu partnerského centra. Než začnete s migrací do partnerského centra, můžete přejít na [Azure Portal](https://ms.portal.azure.com/#home) a vytvořit nového TENANTA Azure AD. Postupujte podle pokynů v části [Vytvoření nového tenanta v Azure Active Directory](/azure/active-directory/develop/quickstart-create-new-tenant). Pomocí nového tenanta AAD nastavte účet partnerského centra. Abyste mohli vytvořit tenanta, musíte být globálním správcem. 

### <a name="user-roles-including-guest-user-roles-in-partner-center"></a>Role uživatelů včetně rolí uživatelů typu Host v partnerském centru

Partnerské centrum má různé typy rolí v závislosti na typech práce, které je třeba provést. K dispozici jsou role, jako je například globální správce, kteří jsou rolemi Azure AD. Některé role jsou specifické pro programy, jako je program poskytovatele cloudové služby nebo motivace, a existují role, které jsou specifické pro MPN. Pokud chcete zjistit, co jsou role partnerského centra, přečtěte si téma [přiřazení rolí uživatelů a oprávnění](permissions-overview.md).

### <a name="what-happens-to-my-users-roles-when-they-move-from-pmc-to-partner-center"></a>Co se stane s rolemi uživatelů při přesunu z PMC do partnerského centra?

S výjimkou toho, že je pro uživatele programu MPN globální správce nebo primární program kontaktována osoba, která provádí migraci, ztratí všichni uživatelé v PMC své role správce. Jednotlivec, který dokončí migraci, bude muset přiřadit role v partnerském centru. Role v partnerském centru se liší od rolí v PMC. Další informace o rolích uživatelů v partnerském centru najdete [přiřazení rolí uživatelů a oprávnění] (oprávnění – overview.md a [přesunutí z PMC do partnerského centra](move-pmc-pc-map.md#user-roles) .

### <a name="whats-the-difference-between-my-company-profile-and-my-business-profile"></a>Jaký je rozdíl mezi profilem společnosti a obchodním profilem?

Váš profil společnosti obsahuje informace o vaší společnosti, které zahrnují adresy, umístění, primární kontakt, banku a daňové podrobnosti.

Vaším obchodním profilem je způsob, jakým prezentujete zákazníkům, a jedná se o marketingovou stránku, která zobrazuje vaše logo, podrobnosti o vašem firemním zaměření, odbornosti atd.

### <a name="what-does-account-consolidation-mean-for-my-account"></a>Co znamená konsolidace účtů pro můj účet?

Pokud ke migraci více účtů MPN do partnerského centra použijete stejného tenanta Azure AD, systém ho automaticky rozpozná a požádá vás, abyste si účty konsoliduji. To platí i v případě, že ke stejnému tenantovi služby Azure AD je přidruženo několik domén. 

Stále se můžete rozhodnout migrovat do partnerského centra pomocí samostatných tenantů služby AAD, ale Všimněte si, že se jedná o izolované hodnocení vašich kompetencí a dalších nákupních nákladů. Další informace o konsolidaci účtů najdete v článku konsolidace [účtů vaší společnosti](consolidate-accounts.md) .

### <a name="if-i-have-multiple-aad-tenants-and-a-single-mpn-account-is-it-possible-to-link-them-in-partner-center"></a>Pokud mám více tenantů AAD a jeden účet MPN, je možné je propojit v partnerském centru?

Ano, v partnerském centru můžete propojit několik tenantů Azure AD s jedním účtem partnerského centra.
Další informace o konsolidaci účtů najdete v článku konsolidace [účtů vaší společnosti](consolidate-accounts.md) .

### <a name="are-there-restrictions-to-adding-multiple-azure-ad-tenants-to-a-single-partner-center-account"></a>Existují omezení pro přidání více tenantů Azure AD do jednoho účtu partnerského centra?

Pokud je tenant Azure AD už přidružený k existujícímu účtu partnerského centra, nedá se přidružit k novým účtům partnerského centra pomocí funkce víceklientské architektury. Dalším způsobem, jak ho představit, je tenant Azure AD může být přidružený jenom k jednomu účtu partnerského centra, ale k účtu partnerského centra se dá přidružit víc klientů.

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Migrace členství v Microsoft Partner Network (MPN) 

Přečtěte si o běžných dotazech ohledně migrace členství v programu MPN v následujících odpovědích.

### <a name="who-can-perform-the-move-from-pmc-to-partner-center"></a>Kdo může provést přesun z PMC do partnerského centra?

Vaše společnost: globální správce MPN nebo kontakt na primární program (tyto dvě role často používá stejná osoba) může zahájit a provést přesun.

### <a name="will-the-person-completing-the-migration-become-the-primary-contact-on-the-company-legal-profile-in-partner-center"></a>Bude se osoba, která dokončení migrace stane primárním kontaktem na oficiální profil společnosti v partnerském centru?

Primární kontakt ale nemusí být nutně osoba, která má autorizaci k podepisování smluv.

### <a name="can-microsoft-migrate-my-mpn-membership-for-me"></a>Může Microsoft migrovat svoje členství v programu MPN?

Ne. Společnost Microsoft vám nemůže přesunout váš účet členství do partnerského centra. Pokud chcete zahájit proces migrace, budete muset svůj účet přesunout pomocí přihlášení k PMC pomocí svého pracovního účtu (přihlašovací údaje). Po dokončení postupu pro přesunutí účtu můžete začít spravovat členství a přiřazovat role uživatelů a oprávnění k vašemu týmu, aby mohli získat přístup k výhodám a lépe spravovat členství. 

Microsoft automaticky migruje aktuální kompetence, výhody, informace o poloze, banku a daňové informace pro pobídky a asociace MCP, včetně partnerského přístupu k partnerské škole.

### <a name="how-will-the-renewal-policy-change"></a>Jak se změní zásady obnovování?

V partnerském centru je okno obnovení od data výročí v následujících 30 dnech.

### <a name="will-our-competencies-remain-unchanged-after-we-move-to-partner-center"></a>Budou naše kompetence po přesunu do partnerského centra stále beze změny?

Ano, kompetence nebudou ovlivněny přesunem do partnerského centra. Pokud si všimnete rozporů, obraťte se na [podporu](https://partner.microsoft.com/support).

### <a name="will-my-benefits-including-cloud-benefits-technical-support-software-benefits-visual-studio-change-after-we-move"></a>Budou mé výhody (včetně výhod cloudu, technické podpory, výhod softwaru, sady Visual Studio) po přesunu změněny?

Vaše vhodné výhody se nemění. Pokud si všimnete rozporů, obraťte se na [podporu](https://partner.microsoft.com/support).

### <a name="will-our-microsoft-accounts-that-have-visual-studio-benefits-allocations-be-honored"></a>Budou se respektovat naše účty Microsoft, které mají přidělení výhod sady Visual Studio?

Ano Výhody sady Visual Studio přidělené účty spravované služby se budou respektovat a uchovávat. Po obnovení v partnerském centru budou taky zachované. Pokud ale přidělení MSA odeberete po migraci v partnerském centru, nejde ho přidat zpátky do partnerského centra.

V partnerském centru může partner přidat pracovní účty a uživatelské účty hosta, které jsou MSA ze stejného tenanta, ve kterém je partner správce MPN v tenantovi Azure AD. Pokud je partner globálním správcem ve více klientech Azure AD a všichni tito klienti jsou přidružení ke stejnému účtu partnerského centra, pak partnerovi může přidat uživatele ze všech těchto tenantů do výhod sady Visual Studio a přidělení na základě využití Azure.

I když se uživatelům typu Host dá přiřadit odběry na základě využití sady Visual Studio pomocí Správce MPN nebo globálního správce, uživatelé typu Host se nemůžou přihlásit do partnerského centra pomocí svých MSA. Uživatelé typu Host se ale můžou přihlásit k Azure a Visual Studiu a ověřit a použít jim přiřazené výhody.

### <a name="how-should-we-manage-our-mcp-associations-and-our-partner-university-access"></a>Jak bychom měli spravovat naše přidružení MCP a přístup k partnerské škole?

Neexistují žádné změny MCP přidružení, která se pohybují z PMC. Všichni noví zaměstnanci potom, co se přesunete do partnerského centra, ale budou muset být přidruženi v partnerském centru. Všechna vaše partnerská oprávnění pro stávající uživatele zůstanou, ale všichni noví zaměstnanci by měli přejít do [školicího centra](https://partner.microsoft.com/training) , kde najdete informace o tom, jak získat přístup k partnerské univerzitě.

### <a name="how-do-i-view-mcp-information-once-i-move-to-partner-center"></a>Návody zobrazit informace o MCP po přesunu do partnerského centra?

Vyberte **kompetence** z levé navigace na řídicím panelu. Na stránce **kompetence** můžete stáhnout sestavu dovedností. Sestava odbornosti zobrazí seznam uživatelů, kteří získali dovednosti vztahující se k kompetencím a programům v partnerském centru. Pokud vaši uživatelé získali dovednosti, ale tyto dovednosti nejsou důležité pro kompetence, na kterých právě pracujete, nebudou uvedené v sestavě.

### <a name="are-customer-references-used-in-partner-center"></a>Používají se v partnerském centru odkazy na zákazníky?

Ne, odkazy na zákazníky nepotřebujete, aby splňovaly požadavky na kompetenci v partnerském centru.

### <a name="will-partner-of-record-associations-move-to-partner-center"></a>Bude partnerem přidružení záznamů přesunutá do partnerského centra?

Ano, nedošlo k žádné změně partnera záznamu. Přečtěte si další informace o [propojení ID partnera s vašimi zákazníky](/azure/billing/billing-partner-admin-link-started).

### <a name="is-there-an-impact-to-incentives-because-of-the-move-to-partner-center"></a>Existuje dopad na motivaci z důvodu přesunu do partnerského centra?

Ne, nemusíte mít žádný vliv na to, jestli jste svůj účet přesunuli bez slučování míst. Pokud má vaše firma více účtů v PMC a při přesunu do partnerského centra, které se rozhodnete konsolidovat do globálního účtu, nedojde ke ztrátě informací, ale může dojít ke zpoždění v pobídkovém vyvýběru. 

Pokud nepřesunete všechny účty PMC, které byly součástí programu pobídek, můžete přestat získávat pobídky, které jsou svázané s těmito účty.

### <a name="what-are-the-incentive-roles-in-partner-center"></a>Jaké jsou role k disměně v partnerském centru?

Role rolí v partnerském centru jsou založené na umístění a zahrnují pobídky správce a pobídky uživatele. Další informace o tom, co tyto role mohou provádět, najdete v tématu [přiřazení rolí uživatelů a oprávnění](permissions-overview.md).

### <a name="can-incentives-admins-be-assigned-at-the-global-and-location-level"></a>Je možné přiřazovat správce na úrovni globálních a umístění?

Ano Můžete přiřadit správce pobídek jako správce pobídek pro všechna umístění nebo každé umístění může mít svého vlastního správce pobídek.

### <a name="can-incentives-be-paid-at-the-global-or-location-level"></a>Je možné je vyplatit na globální úrovni nebo na úrovni umístění?

Pobídky jsou vypláceny pouze na úrovni umístění.

### <a name="regarding-referrals-how-many-business-profiles-can-we-create"></a>V souvislosti s referenčními informacemi, kolik obchodních profilů můžeme vytvořit?

Vaše společnost může vytvořit tolik obchodních profilů, kolik budete potřebovat k úplnému vyjádření zájmů vaší společnosti. V každém obchodním profilu můžete seznamovat až pět umístění, jedno místo na zemi. Každý z obchodních profilů může získat referenčních seznamů pro každé z jeho umístění.

### <a name="how-will-referrals-be-assigned-what-changes-can-i-expect-for-example-if-i-have-a-global-company-in-one-market-and-locations-in-other-markets-how-will-referrals-be-assigned"></a>Jak budou odkazy přiřazeny, jaké změny je možné očekávat? Například pokud mám globální společnost na jednom trhu a umístění na jiných trzích, jak budou odkazy přiřazeny?

Odkazy jsou přiřazeny na základě parametrů hledání, které zákazník definuje. Bez ohledu na to, jestli máte jedno nebo mnoho umístění, pokud zákazníci určí požadované umístění a máte firmu, která splňuje ostatní parametry, odkaz by přešel do tohoto umístění.

### <a name="i-am-migrating-to-partner-center-from-within-russia-i-get-an-error-message-about-web-direct-how-do-i-continue-with-the-migration"></a>Migruju do partnerského centra z Ruska. Zobrazí se chybová zpráva o webu Direct. Návody pokračovat v migraci?

Pokud se zobrazí chybová zpráva, že se účastníte programu web Direct, měli byste provést následující akce:

1. Přihlaste se k portálu. Azure.com a vytvořte nového tenanta Azure AD. Další informace najdete v tématu [Vytvoření nového tenanta Azure AD](/azure/active-directory/fundamentals/active-directory-access-create-new-tenant).

2. Po vytvoření nového tenanta Azure AD ho pomocí něj migrujete z partnerského centra pro členství v partnerském centru nebo se zaregistrujete jako síť novinkou v partnerském centru.