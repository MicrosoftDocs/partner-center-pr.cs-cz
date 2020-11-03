---
title: Vyžadování vícefaktorového ověřování u partnerského tenanta
ms.topic: article
ms.date: 10/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se, jak mandating MFA pro vaše partnerské klienty pomůže zabezpečit váš přístup k zákaznickým prostředkům. Obsahuje vzorové scénáře.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 01122e81254a8e63f9bbf8d6bc3d3271accac74a
ms.sourcegitcommit: 2847efac28d3bff24ed37cdfaa88ff4be06705c8
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/27/2020
ms.locfileid: "92680404"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>Mandating Multi-Factor Authentication (MFA) pro vašeho partnerského tenanta

**Platí pro**

- Všichni partneři v programu Cloud Solution Provider
  - Přímá faktura
  - Nepřímý poskytovatel
  - Nepřímý prodejce
- Všechny poradce

**Ovlivněné role**

- Agent správce
- Agent prodeje
- Agent helpdesku
- Správce fakturace
- Globální správce

Účelem této funkce je pomáhat partnerům zabezpečit svůj přístup k zákaznickým prostředkům proti zneužití přihlašovacích údajů.
Partneři se musí vymáhat službou Multi-Factor Authentication (MFA) u všech uživatelských účtů ve svém partnerském tenantovi, včetně uživatele typu Host. Tato funkce bude pro tyto role partnerských procesů pověřena dokončením ověřování MFA v následujících oblastech:

- [Řídicí panel partnerského centra](#partner-center-dashboard)
- [Rozhraní API partnerského centra](#partner-center-api)
- [Delegovaná Správa partnera](#partner-delegated-administration)

Vyšší a nepřetržité zabezpečení a ochrana osobních údajů jsou z našich nejdůležitějších priorit a budeme dál pomáhat partnerům chránit své zákazníky a klienty. Všichni partneři účastnící se programu Cloud Solution Provider (CSP), dodavatelé ovládacích panelů (CPVs) a poradci musí implementovat požadavky na [zabezpečení partnerů](partner-security-requirements.md) , aby zůstaly v souladu.

Abychom svým firmám a zákazníkům usnadnili ochranu svých podniků a zákazníků před incidenty souvisejícími s krádeží identity, aktivovali jsme další bezpečnostní zabezpečení pro partnerské klienty, kteří můžou partnerům a zákazníkům zajistit, aby mandating ověřování vícefaktorového ověřování (MFA), aby se předešlo neoprávněnému přístupu. 

Tato dokumentace poskytuje partnerům podrobné zkušenosti a pokyny týkající se aktivace bezpečnostních zabezpečení.

## <a name="partner-center-dashboard"></a>Řídicí panel partnerského centra

Některé stránky na řídicím panelu partnerského centra budou chráněny MFA, včetně:

- Všechny stránky na kartě **zákazníci** , například všechny stránky, které jsou dostupné prostřednictvím následující adresy URL: https://partner.microsoft.com/commerce/*
- Všechny stránky na kartě **podpora > žádosti zákazníků** , například stránka přístupná v části https://partner.microsoft.com/dashboard/support/csp/customers/*
- Stránka fakturace

Pokud se pokusíte získat přístup k některým z těchto stránek a jste předtím nedokončili ověřování MFA, budete se muset udělat.

> [!NOTE]
> Jiné stránky v partnerském centru, jako je například stránka přehled, Service Health stavová stránka pro kontrolu stavu nebudou chráněny proti MFA.

Následující typy uživatelů mají autorizaci pro přístup k těmto stránkám chráněným MFA a jsou proto ovlivněny touto funkcí.


| Stránky chráněné MFA       | Agenti správce      |  Prodejní agenti     |   Agenti helpdesku     | Globální správce      |  Správce fakturace     | 
|---    |---    |---    |---    |---    |---    |
| Všechny stránky na kartě Customers      |   x    |    x   |  x     |       |       |
| Všechny stránky v rámci podpory > kartě žádosti o zákazníky     | x      |       |    x   |       |       |
| Stránka fakturace     |   x    |       |       |    x   |   x    |

## <a name="examples-showing-how-verification-works"></a>Příklady ukazující, jak funguje ověřování

K ilustraci, jak ověřování funguje, vezměte v úvahu následující dva příklady.

### <a name="example-1-partner-has-implemented-azure-ad-mfa"></a>Příklad 1: partner implementoval Azure AD MFA

1. Jana funguje pro poskytovatele CSP společnosti Contoso. Společnost Contoso implementovala MFA pro všechny své uživatele v rámci partnerského tenanta contoso s použitím služby Azure Active Directory (Azure AD) MFA.

2. Jana spustí novou relaci prohlížeče a přejde na stránku s přehledem řídicího panelu partnerského centra (která není chráněna MFA). Partnerské centrum přesměruje Jana na službu Azure AD, aby se přihlásil.

3. Vzhledem k existující instalaci Azure AD MFA pomocí společnosti Contoso je potřeba, aby se dokončilo ověřování MFA. Po úspěšném přihlášení a ověření MFA je Jana přesměrován zpět na stránku Přehled řídicího panelu partnerského centra.

4. Jana se pokusí získat přístup k jedné ze stránek chráněných MFA v partnerském centru. Vzhledem k tomu, že Jana již dokončila ověřování MFA během přihlášení, má Jana přístup na stránku chráněnou MFA, aniž by bylo nutné provést ověření MFA znovu.

### <a name="example-2-partner-has-implemented-third-party-mfa-using-identity-federation"></a>Příklad 2: partner implementoval vícefaktorové ověřování třetí strany pomocí federace identit.

1. Trent funguje pro zprostředkovatele CSP Wingtip. Společnost Wingtip implementovala vícefaktorové ověřování pro všechny své uživatele v partnerském tenantovi klienta Wingtip pomocí MFA, která je integrovaná se službou Azure AD prostřednictvím federace identit.

2. Trent spustí novou relaci prohlížeče a přejde na stránku s přehledem řídicího panelu partnerského centra (což není chráněna MFA). Partnerské centrum přesměruje Trent do služby Azure AD, aby se přihlásil.

3. Vzhledem k tomu, že společnost Wingtip má nastavení federace identit, Azure AD přesměruje Trent na federovaného zprostředkovatele identity, aby bylo možné dokončit přihlášení a ověřování MFA. Po úspěšném přihlášení a ověření MFA se Trent přesměruje zpátky na Azure AD a na stránku Přehled řídicího panelu partnerského centra.

4. Trent se snaží o přístup k jedné ze stránek chráněných MFA v partnerském centru. Vzhledem k tomu, že Trent již dokončila ověřování MFA během přihlašování, Trent má přístup ke stránce chráněné MFA, aniž by bylo nutné se znovu projít ověřováním MFA.

### <a name="example-3-partner-hasnt-implemented-mfa"></a>Příklad 3: partner neimplementoval MFA

1. Jan funguje pro zprostředkovatele CSP Fabrikam. Společnost Fabrikam neimplementovala MFA pro žádného uživatele v partnerském tenantovi Fabrikam.

2. Jan spustí novou relaci prohlížeče a přejde na stránku s přehledem řídicího panelu partnerského centra (která není chráněna MFA). Partnerské centrum přesměruje Jan na službu Azure AD, aby se přihlásil.

3. Vzhledem k tomu, že společnost Fabrikam neimplementovala MFA, nepotřebuje Jan dokončit ověřování MFA. Po úspěšném přihlášení se Jan přesměruje zpátky na stránku Přehled řídicího panelu partnerského centra.

4. Jan se pokusí získat přístup k jedné ze stránek chráněných MFA v partnerském centru. Vzhledem k tomu, že Jan nedokončil ověřování MFA, Partnerské centrum přesměruje Jan na Azure AD, aby se dokončilo ověřování MFA. Vzhledem k tomu, že se jedná o první požadavek Jan, aby bylo možné provést MFA, je pro [vícefaktorové ověřování](#mfa-registration-experience)také požádána Jan. Po úspěšné registraci MFA a ověřování MFA teď má Jan přístup na stránku chráněnou MFA.

5. Druhý den před tím, než společnost Fabrikam implementuje MFA pro libovolného uživatele, spustí novou relaci prohlížeče a přejde na stránku Přehled řídicího panelu partnerského centra (což není chráněno MFA). Partnerské centrum přesměruje Jan na službu Azure AD, aby se přihlásil bez výzvy MFA. 

6. Jan se pokusí získat přístup k jedné ze stránek chráněných MFA v partnerském centru. Vzhledem k tomu, že Jan nedokončil ověřování MFA, Partnerské centrum přesměruje Jan na Azure AD, aby se dokončilo ověřování MFA. Vzhledem k tomu, že Jan zaregistroval MFA, tak v tomto okamžiku se zobrazí pouze výzva k dokončení ověřování MFA.

> [!NOTE]
>Akce: Správce společnosti by měl implementovat MFA hned prostřednictvím kterékoli z těchto [možností](partner-security-requirements.md#actions-that-you-need-to-take) navržených partnerským centrem.

## <a name="partner-center-api"></a>Rozhraní API partnerského centra

Rozhraní API partnerského centra podporuje ověřování jenom pro aplikace a ověřování uživatelů a aplikací. 

Když se použije ověřování aplikace + uživatel, bude partnerské Centrum vyžadovat ověření MFA. Konkrétně, když Partnerská aplikace chce odeslat požadavek rozhraní API partnerskému centru, musí do autorizační hlavičky žádosti zahrnovat přístupový token. 

> [!NOTE]
>[Model zabezpečené aplikace](/partner-center/develop/enable-secure-app-model) je zabezpečená, škálovatelná architektura pro ověřování partnerů CSP a CPVs Microsoft Azure prostřednictvím architektury vícefaktorového ověřování při volání rozhraní API partnerského centra. před povolením vícefaktorového ověřování ve vašem tenantovi ji musíte implementovat. 

Když partnerské Centrum přijme požadavek rozhraní API s přístupovým tokenem získaným pomocí ověřování aplikace + uživatel, rozhraní API partnerského centra ověří přítomnost hodnoty *MFA* v deklaraci *metody ověřování (AMR)* . Pomocí dekodéru JWT můžete ověřit, zda přístupový token obsahuje očekávanou hodnotu odkaz na metodu ověřování (AMR), nebo ne:

``` csharp
{
  "aud": "https://api.partnercenter.microsoft.com",
  "iss": "https://sts.windows.net/df845f1a-7b35-40a2-ba78-6481de91f8ae/",
  "iat": 1549088552,
  "nbf": 1549088552,
  "exp": 1549092452,
  "acr": "1",
  "amr": [
    "pwd",
    "mfa"
  ],
  "appid": "23ec45a3-5127-4185-9eff-c8887839e6ab",
  "appidacr": "0",
  "family_name": "Adminagent",
  "given_name": "CSP",
  "ipaddr": "127.0.0.1",
  "name": "Adminagent CSP",
  "oid": "4988e250-5aee-482a-9136-6d269cb755c0",
  "scp": "user_impersonation",
  "tenant_region_scope": "NA",
  "tid": "df845f1a-7b35-40a2-ba78-6481de91f8ae",
  "unique_name": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "upn": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "ver": "1.0"
}
```

Pokud je hodnota přítomna, partnerským centrem se dokončí ověřování MFA a zpracuje požadavek rozhraní API. Pokud hodnota není k dispozici, rozhraní API partnerského centra žádost odmítne s následující odpovědí:

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

Když se použije ověřování App-Only, rozhraní API, která podporují ověřování App-Only, budou nepřetržitě fungovat bez nutnosti MFA.

## <a name="partner-delegated-administration"></a>Delegovaná Správa partnera

### <a name="using-service-portals"></a>Používání portálů služeb

Partnerské účty, včetně agentů pro správu a agentů helpdesku, můžou používat svá oprávnění správce delegovaná pro správu zákaznických prostředků prostřednictvím portálů Microsoft Online Services, rozhraní příkazového řádku (CLI) a rozhraní API (pomocí ověřování aplikací a uživatelů).

Při přístupu k portálům služby Microsoft Online Services pomocí delegovaných oprávnění správce (admin-on-of) za účelem správy zákaznických prostředků je mnoho z těchto portálů vyžadovat interaktivní ověření partnerského účtu se zákazníkem Azure Active Directory jako kontext ověřování – Partnerský účet je vyžadován pro přihlášení k tenantovi zákazníka.

Když Azure Active Directory obdrží takové žádosti o ověření, bude vyžadovat, aby Partnerský účet dokončil ověřování MFA. Existují dvě možná uživatelská prostředí v závislosti na tom, jestli je partnerským účtem spravovaná nebo federované identita:

- Pokud je partnerským účtem **spravovaná** identita, Azure Active Directory se uživateli zobrazí výzva k dokončení ověřování MFA. Pokud nebyl Partnerský účet pro MFA s Azure Active Directory zaregistrován, bude uživatel vyzván k [dokončení registrace MFA](#mfa-registration-experience) .

- Pokud je Partnerský účet **federované** identitou, bude prostředí závislé na tom, jak správce partnera nakonfiguroval federaci v Azure Active Directory. Při nastavování federace v Azure Active Directory může správce partnera určit, že Azure Active Directory, jestli zprostředkovatel federovaných identit podporuje vícefaktorové ověřování (MFA). Pokud ano, Azure Active Directory přesměruje uživatele na federovaného zprostředkovatele identity, aby se dokončilo ověřování MFA. V opačném případě Azure Active Directory přímo vyzve uživatele k dokončení ověřování MFA. Pokud nebyl Partnerský účet pro MFA s Azure Active Directory zaregistrován, bude uživatel vyzván k [dokončení registrace MFA](#mfa-registration-experience) .

Celkové prostředí se podobá scénáři, kdy tenant koncového zákazníka implementoval MFA pro své správce. Tenant zákazníka má například povolené [výchozí hodnoty zabezpečení Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), což vyžaduje, aby všechny účty s právy správce se přihlásily k klientovi zákazníka s ověřováním MFA, včetně agentů pro správu a agentů helpdesku. Pro účely testování můžou partneři povolit [výchozí hodnoty zabezpečení Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) v tenantovi zákazníka a potom se pokusit o přístup k tenantovi zákazníka pomocí oprávnění delegovaná Správa pro partnery.

> [!NOTE]
> Ne všechny portály online služeb Microsoftu vyžadují, aby se partnerské účty přihlásily k klientovi zákazníka při přístupu k zákaznickým prostředkům pomocí delegovaných oprávnění správce. Místo toho vyžadují, aby se partnerské účty přihlásily do partnerského tenanta. Příkladem je centrum pro správu serveru Exchange. V průběhu času očekáváme, že tyto portály při použití oprávnění delegovaného správce budou vyžadovat, aby se partnerské účty přihlásily k klientovi zákazníka.

### <a name="using-service-apis"></a>Používání rozhraní API služby

Některá rozhraní API služeb Microsoft Online Services (například Azure Resource Manager, Azure AD Graph, Microsoft Graph atd.) podporují partneři podpory prostřednictvím delegovaných oprávnění správce, aby mohli programově spravovat prostředky zákazníků. Aby mohla Partnerská aplikace při ověřování pomocí těchto rozhraní API využít oprávnění delegovaného správce, musí v hlavičce autorizace žádosti API zahrnovat přístupový token, ve kterém je přístupový token získaný pomocí partnerského uživatelského účtu, který se má ověřit ve službě Azure AD, a zákazníkovou sadou Azure AD nastavenou jako kontext ověřování. Partnerská aplikace musí mít k tenantovi zákazníka přihlášený partnerský uživatelský účet.

Když Azure AD obdrží jako požadavek na ověření, Azure AD bude vyžadovat, aby se k ověření MFA dokončilo i partnerský uživatelský účet. Pokud uživatelský účet partnera ještě není registrovaný pro MFA, zobrazí se uživateli výzva k dokončení registrace MFA.

Tato funkce má vliv na všechny partnerské aplikace, které jsou integrované s těmito rozhraními API pomocí delegovaných oprávnění správce. Aby mohly partnerské aplikace i nadále pracovat s těmito rozhraními API bez přerušení:

- Partner se musí při získání přístupového tokenu vyhnout použití metody neinteraktivního ověřování uživatelů ve službě Azure AD. Při použití neinteraktivní metody ověřování uživatele, jako je například [tok hesla](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password), služba Azure AD nebude moci vyzvat uživatele k dokončení ověřování MFA. Partner se musí přepnout na použití interaktivní metody ověřování uživatelů, jako je například [OpenID Connect Flow](/azure/active-directory/develop/v1-protocols-openid-connect-code) .

- Při ověřování pomocí interaktivního uživatele by partner měl používat partnerský uživatelský účet, který je už povolený pro MFA. Případně po zobrazení výzvy službou Azure AD může partner dokončit registraci MFA a ověřování MFA během přihlašování.

- To se podobá scénáři, kdy tenant koncového zákazníka implementoval MFA pro své správce. Tenant zákazníka má například povolené [výchozí hodnoty zabezpečení Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), což vyžaduje, aby všechny uživatelské účty s právy správce se přihlásily k klientovi zákazníka pomocí ověřování MFA, včetně agentů pro správu a agentů helpdesku. Pro účely testování můžou partneři povolit [výchozí nastavení zabezpečení Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) v tenantovi zákazníka a potom se pokusit o programový přístup k tenantovi zákazníka přes delegovaná oprávnění pro správu.

### <a name="mfa-registration-experience"></a>Prostředí registrace MFA

Pokud se během ověřování MFA ještě nezaregistroval Partnerský účet pro MFA, Azure AD vyzve uživatele, aby nejdřív dokončil registraci MFA:

:::image type="content" source="images/MfaRegistration1.png" alt-text="Registrace MFA – krok 1":::

Po kliknutí na tlačítko **Další** se uživateli zobrazí výzva k výběru ze seznamu metod ověřování.

:::image type="content" source="images/MfaRegistration2.png" alt-text="Registrace MFA – krok 1":::

Po úspěšné registraci se uživateli pak vyžaduje dokončení ověřování MFA na základě ověření, které uživatel zvolil.

## <a name="request-for-technical-exception"></a>Žádost o technickou výjimku

Partneři můžou požádat o technickou výjimku pro potlačení ověřování MFA, pokud se setkávají s technickými problémy s online službami Microsoftu a neexistuje žádné praktické řešení ani řešení. Než to uděláte, přečtěte si následující části:

- [Seznam běžných problémů hlášených partnery](#list-of-common-issues-reported-by-partners)
- [Odeslání žádosti o technickou výjimku](#how-to-submit-a-request-for-technical-exception)
 
### <a name="list-of-common-issues-reported-by-partners"></a>Seznam běžných problémů hlášených partnery
Před použitím pro technickou výjimku si přečtěte seznam běžných problémů hlášených ostatními partnery a zjistěte, zda se jedná o platné důvody pro technickou výjimku.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>Problém 1: partner potřebuje víc času na implementaci MFA pro své partnerské agenty.
Partner se nespustil nebo stále ještě v procesu implementace vícefaktorového ověřování pro své partnerské agenty, kteří vyžadují přístup k portálům služeb Microsoft Online Services pomocí oprávnění delegovaná Správa pro správu zákaznických prostředků. Partner potřebuje víc času na dokončení implementace MFA. Je to problém platným důvodem pro technickou výjimku?

**Odpověď** : ne. Partner potřebuje k tomu, aby se svým uživatelům naimplementoval MFA, aby se předešlo přerušení.

> [!NOTE]
> I když partner pro své partnerské agenty neimplementoval MFA, Partnerská agenti budou mít stále přístup k portálům Microsoft Online Services pomocí delegovaných oprávnění pro správu, za předpokladu, že se k zobrazení výzvy během přihlašování do tenanta zákazníka můžou dokončit registrace MFA a ověřování MFA. Dokončení registrace MFA automaticky nepovolí uživatele pro MFA.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>Problém 2: partner neimplementoval MFA pro uživatelské účty, kteří nepoužívají delegovaná oprávnění správce.
Partner má některé uživatele v jejich partnerských klientech, kteří nepotřebují přístup k portálům Microsoft Online Services pro správu zákaznických prostředků pomocí delegovaných oprávnění pro správu. Partner v procesu implementuje MFA pro tyto uživatele a potřebuje víc času na dokončení. Je to problém platným důvodem pro technickou výjimku?

**Odpověď** : ne. Vzhledem k tomu, že tyto uživatelské účty nepoužívají pro správu zákaznických prostředků oprávnění k delegované správě, nebudou se muset přihlašovat k tenantovi zákazníka. Nebudou ovlivněny službou Azure AD vyžadovat ověřování MFA během přihlašování k tenantovi zákazníka.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>Problém 3: partner neimplementoval MFA pro účty uživatelských služeb
Partner má některé uživatelské účty ve svých partnerských klientech, které zařízení používají jako účty služeb. Jedná se o účty s nízkými oprávněními, které nevyžadují přístup k partnerským centrům ani portálům Microsoft Online Services pro správu zákaznických prostředků pomocí delegovaných oprávnění pro správu. Je to problém platným důvodem pro technickou výjimku?

**Odpověď** : ne. Vzhledem k tomu, že tyto uživatelské účty nepoužívají pro správu zákaznických prostředků oprávnění k delegované správě, nebudou se muset přihlašovat k tenantovi zákazníka. Nebudou ovlivněny službou Azure AD vyžadovat ověřování MFA během přihlašování k tenantovi zákazníka.

##### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>Problém 4: partner nemůže implementovat MFA pomocí aplikace MS Authenticator.
Partner má "uklizenou" zásadu, která neumožňuje zaměstnancům, aby do své pracovní oblasti nastavili svá osobní mobilní zařízení. Bez přístupu k osobním mobilním zařízením nemohou zaměstnanci nainstalovat aplikaci MS Authenticator, což je jediné ověřování MFA podporované výchozími nastaveními zabezpečení Azure AD. Je to problém platným důvodem pro technickou výjimku?

**Odpověď** : Ne, nejedná se o platný důvod pro technickou výjimku. Partner by měl zvážit následující alternativy, aby jejich zaměstnanci mohli při přístupu k partnerskému centru i nadále provádět ověřování MFA:
- Partner se taky může zaregistrovat Azure AD Premium nebo řešení VÍCEFAKTOROVÉHO ověřování třetích stran (kompatibilní s Azure AD), které může poskytovat další metody ověřování.

##### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>Problém 5: partner nemůže implementovat MFA z důvodu použití starších protokolů ověřování.
Partner má některé agenty, kteří stále používají starší protokoly ověřování, což není kompatibilní s MFA. Uživatelé například pořád používají Outlook 2010, který je založený na starších protokolech ověřování. Povolení MFA pro tyto agenty budou rušit používání starších protokolů ověřování.

**Odpověď** : Ne, nejedná se o platný důvod pro technickou výjimku. Partnerům se důrazně doporučuje přesunout se z používání starších protokolů ověřování z důvodu potenciálních důsledků zabezpečení, protože tyto protokoly nelze chránit pomocí ověřování MFA a jsou mnohem náchylnější k ohrožení bezpečnosti přihlašovacích údajů. Pokud už nepoužíváte starší verze ověřovacích protokolů, partneři by si měli zvážit, že se zaregistrují Azure AD Premium, což podporuje používání hesel aplikací. Hesla aplikací jsou jednorázová systémem generovaná hesla a jsou obvykle silnější než hesla generovaná uživatelem. Díky použití hesel aplikací můžou partneři implementovat MFA pro svoje uživatele a přitom vracet hesla aplikací jenom pro starší protokoly ověřování.

Přečtěte si informace o [základním ověřování a Exchange Online](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-auth-and-exchange-online-february-2020-update/ba-p/1191282) , abyste porozuměli nejnovějšímu plánu, který podporuje starší verze ověřování pro Outlook, a Projděte si [Blog týmu Exchange](https://techcommunity.microsoft.com/t5/exchange-team-blog/bg-p/Exchange) , kde získáte nadcházející novinky. 

> [!NOTE]
> I když partner pro své partnerské agenty neimplementoval MFA, Partnerská agenti budou mít stále přístup k portálům Microsoft Online Services pomocí delegovaných oprávnění pro správu, za předpokladu, že se k zobrazení výzvy během přihlašování do tenanta zákazníka můžou dokončit registrace MFA a ověřování MFA. Dokončení registrace MFA automaticky nepovolí uživatele pro MFA.

##### <a name="issue-6-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>Problém 6: partner implementoval vícefaktorové ověřování třetí strany, které nerozpoznala služba Azure AD.
Partner implementoval MFA pro svoje uživatele pomocí řešení MFA od jiného výrobce. Partner ale nemůže správně nakonfigurovat řešení MFA třetí strany pro předávání do služby Azure AD, které bylo během ověřování uživatelů dokončeno ověřování MFA. Je to platný důvod pro technickou výjimku?

**Odpověď** : Ano, tento problém může být považován za platný důvod pro technickou výjimku. Před odesláním žádosti o technickou výjimku ověřte u poskytovatele řešení MFA třetí strany, že řešení MFA nejde nakonfigurovat tak, aby Flow *authenticationmethodsreferences* deklarací identity (s hodnotou *multipleauthn* ) do služby Azure AD, aby označovalo, že ověření MFA bylo během ověřování uživatele dokončeno. Při odesílání žádosti o technickou výjimku musíte poskytnout podrobnosti o použitém řešení MFA třetí strany a označit způsob integrace (například prostřednictvím federace identit nebo použití vlastního ovládacího prvku Azure AD) a zadat následující informace v žádosti o technickou výjimku jako podpůrné dokumenty:

- Konfigurace vícefaktorového ověřování třetích stran.

- Výsledek [testování partnerských požadavků na zabezpečení](/powershell/partnercenter/test-partner-security-requirements) , které jsou spuštěny účtem s POVOLENým ověřováním MFA třetí strany.

- Nákupní objednávka řešení MFA třetí strany, které používáte, nebo který plánujete použít.

### <a name="how-to-submit-a-request-for-technical-exception"></a>Odeslání žádosti o technickou výjimku

Odeslání žádosti o technickou výjimku:

1. Přihlaste se do partnerského centra jako globální správce nebo jako agent pro správu.

2. Vytvořte novou žádost o partnerskou službu tak, že přejdete na **podporu**  >  **žádostí o podporu partnerů** a kliknete na **nový požadavek** .

3. Ve vyhledávacím poli vyhledejte **MFA – požadavek na výjimku** ; nebo vyberte **CSP** z kategorie, vyberte **účty, registrace, přístup** z tématu a potom v dílčím tématu vyberte **MFA-Request pro výjimku** a pak vyberte **Další krok** .

4. Zadejte podrobnosti požadované k odeslání žádosti o technickou výjimku a klikněte na **Odeslat** .

Společnost Microsoft může trvat až tři pracovní dny a poskytnou odpověď na požadavek na technickou výjimku.