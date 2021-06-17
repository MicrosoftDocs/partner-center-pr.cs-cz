---
title: Mandating Multi-Factor Authentication (MFA) pro vašeho partnerského tenanta
ms.topic: article
ms.date: 10/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se, jak mandating MFA pro vaše partnerské klienty pomůže zabezpečit váš přístup k zákaznickým prostředkům. Obsahuje vzorové scénáře.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9fe1d894ec933072a64f2abdfbb795b6ef046168
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276004"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>Mandating Multi-Factor Authentication (MFA) pro vašeho partnerského tenanta

**Příslušné role**: Agent správce | Prodejní agent | Agent helpdesku | Správce fakturace | Globální správce

Tento článek obsahuje podrobné příklady a pokyny pro mandating Multi-Factor Authentication (MFA) v partnerském centru. Účelem této funkce je pomáhat partnerům zabezpečit svůj přístup k zákaznickým prostředkům proti zneužití přihlašovacích údajů. Partneři se musí vymáhat MFA pro všechny uživatelské účty ve svém partnerském tenantovi, včetně uživatelů typu Host. Uživatelům bude uděleno pověření k dokončení ověřování MFA pro následující oblasti:

- [Řídicí panel partnerského centra](#partner-center-dashboard)
- [Rozhraní API partnerského centra](#partner-center-api)
- [Delegovaná Správa partnera](#partner-delegated-administration)

Vyšší a nepřetržité zabezpečení a ochrana osobních údajů jsou z našich nejdůležitějších priorit a budeme dál pomáhat partnerům chránit své zákazníky a klienty. Všem partnerům zapojeným v programu Cloud Solution Provider (CSP), v Ovládacích panelech (CPVs) a poradcích by měli implementovat [požadavky na zabezpečení partnerů](partner-security-requirements.md) , aby zůstaly v souladu.

Abychom svým firmám a zákazníkům usnadnili ochranu proti krádežím identity a neoprávněnému přístupu, aktivovali jsme další bezpečnostní zabezpečení pro partnerské klienty, kteří ověřují a ověřují MFA. 

## <a name="partner-center-dashboard"></a>Řídicí panel partnerského centra

Některé stránky na řídicím panelu partnerského centra budou chráněny MFA, včetně:

- Všechny stránky na kartě **zákazníci** , například všechny stránky, které jsou dostupné prostřednictvím následující adresy URL: https://partner.microsoft.com/commerce/*
- Všechny stránky na kartě **podpora > žádosti zákazníků** , například stránka přístupná v části https://partner.microsoft.com/dashboard/support/csp/customers/*
- Stránka fakturace

Následující tabulka uvádí, které typy uživatelů mají autorizaci pro přístup k těmto stránkám chráněným pro MFA (a jsou tedy touto funkcí ovlivněny).


| Stránka chráněná MFA       | Agenti správce      |  Prodejní agenti     |   Agenti helpdesku     | Globální správce      |  Správce fakturace     | 
|---    |---    |---    |---    |---    |---    |
| Všechny stránky na kartě Customers      |   x    |    x   |  x     |       |       |
| Všechny stránky v rámci podpory > kartě žádosti o zákazníky     | x      |       |    x   |       |       |
| Stránka fakturace     |   x    |       |       |    x   |   x    |

Pokud se pokusíte získat přístup k některým z těchto stránek a jste předtím nedokončili ověřování MFA, budete se muset udělat. Jiné stránky v partnerském centru, jako je například stránka přehled, Service Health stavová stránka pro kontrolu stavu nevyžadují MFA.

## <a name="verification-examples"></a>Příklady ověřování

K ilustraci, jak ověřování funguje na řídicím panelu partnerského centra, vezměte v úvahu následující příklady.

### <a name="example-1-partner-has-implemented-azure-ad-mfa"></a>Příklad 1: partner implementoval Azure AD MFA

1. Jana funguje pro poskytovatele CSP společnosti Contoso. Společnost Contoso implementovala MFA pro všechny své uživatele v rámci partnerského tenanta contoso s použitím služby Azure Active Directory (Azure AD) MFA.

2. Jana spustí novou relaci prohlížeče a přejde na stránku s přehledem řídicího panelu partnerského centra (která není chráněna MFA). Partnerské centrum přesměruje Jana na službu Azure AD, aby se přihlásil.

3. Vzhledem k existující instalaci Azure AD MFA pomocí společnosti Contoso je potřeba, aby se dokončilo ověřování MFA. Po úspěšném přihlášení a ověření MFA je Jana přesměrován na stránku Přehled řídicího panelu partnerského centra.

4. Jana se pokusí získat přístup k jedné ze stránek chráněných MFA v partnerském centru. Vzhledem k tomu, že Jana již dokončila ověřování MFA během přihlášení, má Jana přístup na stránku chráněnou MFA, aniž by bylo nutné provést ověření MFA znovu.

### <a name="example-2-partner-has-implemented-third-party-mfa-using-identity-federation"></a>Příklad 2: partner implementoval vícefaktorové ověřování třetí strany pomocí federace identit.

1. Trent funguje pro zprostředkovatele CSP Wingtip. Společnost Wingtip implementovala vícefaktorové ověřování pro všechny své uživatele v partnerském tenantovi klienta Wingtip pomocí MFA, která je integrovaná se službou Azure AD prostřednictvím federace identit.

2. Trent spustí novou relaci prohlížeče a přejde na stránku s přehledem řídicího panelu partnerského centra (což není chráněna MFA). Partnerské centrum přesměruje Trent do služby Azure AD, aby se přihlásil.

3. Vzhledem k tomu, že společnost Wingtip má nastavení federace identit, Azure AD přesměruje Trent na federovaného zprostředkovatele identity, aby bylo možné dokončit přihlášení a ověřování MFA. Po úspěšném přihlášení a ověření MFA se Trent přesměruje zpátky na Azure AD a pak na stránku Přehled řídicího panelu partnerského centra.

4. Trent se snaží o přístup k jedné ze stránek chráněných MFA v partnerském centru. Vzhledem k tomu, že Trent již dokončila ověřování MFA během přihlašování, Trent má přístup ke stránce chráněné MFA, aniž by bylo nutné se znovu projít ověřováním MFA.

### <a name="example-3-partner-hasnt-implemented-mfa"></a>Příklad 3: partner neimplementoval MFA

1. Jan funguje pro zprostředkovatele CSP Fabrikam. Společnost Fabrikam neimplementovala MFA pro žádného uživatele v partnerském tenantovi Fabrikam.

2. Jan spustí novou relaci prohlížeče a přejde na stránku s přehledem řídicího panelu partnerského centra (která není chráněna MFA). Partnerské centrum přesměruje Jan na službu Azure AD, aby se přihlásil.

3. Vzhledem k tomu, že společnost Fabrikam neimplementovala MFA, nepotřebuje Jan dokončit ověřování MFA. Po úspěšném přihlášení se Jan přesměruje zpátky na stránku Přehled řídicího panelu partnerského centra.

4. Jan se pokusí získat přístup k jedné ze stránek chráněných MFA v partnerském centru. Vzhledem k tomu, že Jan nedokončil ověřování MFA, Partnerské centrum přesměruje Jan na Azure AD, aby se dokončilo ověřování MFA. Vzhledem k tomu, že se jedná o první požadavek Jan, aby bylo možné provést MFA, je pro [vícefaktorové ověřování](#mfa-registration-experience)také požádána Jan. Po úspěšné registraci MFA a ověřování MFA teď má Jan přístup na stránku chráněnou MFA.

5. Druhý den před tím, než společnost Fabrikam implementuje MFA pro libovolného uživatele, spustí novou relaci prohlížeče a přejde na stránku Přehled řídicího panelu partnerského centra (což není chráněno MFA). Partnerské centrum přesměruje Jan na službu Azure AD, aby se přihlásil bez výzvy MFA. 

6. Jan se pokusí získat přístup k jedné ze stránek chráněných MFA v partnerském centru. Vzhledem k tomu, že Jan nedokončil ověřování MFA, Partnerské centrum přesměruje Jan na Azure AD, aby se dokončilo ověřování MFA. Vzhledem k tomu, že Jan zaregistroval MFA, tak v tomto okamžiku se zobrazí pouze výzva k dokončení ověřování MFA.

> [!NOTE]
>Akce: Správci společnosti mají pro implementaci vícefaktorového ověřování [tři možnosti](partner-security-requirements.md#implementing-multi-factor-authentication) .

## <a name="partner-center-api"></a>Rozhraní API partnerského centra

Rozhraní API partnerského centra podporuje ověřování jenom pro aplikace a ověřování uživatelů a aplikací. 

Když se použije ověřování aplikace + uživatel, bude partnerské Centrum vyžadovat ověření MFA. Konkrétně, když Partnerská aplikace chce odeslat požadavek rozhraní API partnerskému centru, musí do autorizační hlavičky žádosti zahrnovat přístupový token. 

> [!NOTE]
>Rozhraní [zabezpečení aplikačního modelu](/partner-center/develop/enable-secure-app-model) je škálovatelné rozhraní pro ověřování partnerů CSP a CPVs prostřednictvím architektury MFA Microsoft Azure při volání rozhraní API partnerského centra. Před povolením vícefaktorového ověřování ve vašem tenantovi musíte implementovat toto rozhraní. 

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

Když se použije ověřování App-Only, rozhraní API, která podporují ověřování App-Only, budou nepřetržitě fungovat, aniž by to vyžadovalo MFA.

## <a name="partner-delegated-administration"></a>Delegovaná Správa partnera

Partnerské účty, včetně agentů pro správu a agentů helpdesku, můžou používat svá oprávnění správce delegovaná pro správu zákaznických prostředků prostřednictvím portálů Microsoft Online Services, rozhraní příkazového řádku (CLI) a rozhraní API (pomocí ověřování aplikací a uživatelů).

### <a name="using-service-portals"></a>Používání portálů služeb

Při přístupu k portálům služby Microsoft Online Services pomocí delegovaných oprávnění správce (admin-on-of) za účelem správy zákaznických prostředků musí mnoho z těchto portálů vyžadovat interaktivní ověření partnerského účtu s klientem Azure AD, který je nastaven jako kontext ověřování – Partnerský účet je vyžadován pro přihlášení k tenantovi zákazníka.

Když Azure AD obdrží takové žádosti o ověření, bude vyžadovat, aby Partnerský účet dokončil ověřování MFA. Existují dvě možná uživatelská prostředí v závislosti na tom, jestli je partnerským účtem spravovaná nebo federované identita:

- Pokud je partnerským účtem **spravovaná** identita, služba Azure AD bude přímo vyzvat uživatele k dokončení ověřování MFA. Pokud partnerský účet není pro MFA s Azure AD zaregistrovaný, zobrazí se uživateli výzva, aby nejdřív [dokončil registraci MFA](#mfa-registration-experience) .

- Pokud je Partnerský účet **federované** identitou, bude prostředí závislé na tom, jak správce partnera nakonfiguroval federaci ve službě Azure AD. Při nastavování federace ve službě Azure AD může správce partnera naznačovat službě Azure AD, jestli zprostředkovatel federovaných identit podporuje vícefaktorové ověřování (MFA). Pokud ano, Azure AD přesměruje uživatele na federovaného zprostředkovatele identity, aby se dokončilo ověřování MFA. V opačném případě Azure AD vyzve uživatele přímo k dokončení ověřování MFA. Pokud se partnerský účet ještě nezaregistruje k MFA ve službě Azure AD, uživatel se nejprve zobrazí s dotazem, jestli musí [dokončit registraci MFA.](#mfa-registration-experience)

Celkové prostředí je podobné scénáři, ve kterém tenant koncového zákazníka implementovali MFA pro své správce. Například tenant zákazníka povolil výchozí nastavení zabezpečení [Azure AD,](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)což vyžaduje, aby se všechny účty s právy správce přihlašují k tenantovi zákazníka s ověřováním MFA, včetně agentů pro správu a agentů helpdesku. Pro účely testování mohou partneři povolit výchozí nastavení zabezpečení [Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) v tenantovi zákazníka a pak se pokusit použít oprávnění delegované správy partnera pro přístup k tenantovi zákazníka.

> [!NOTE]
> Ne všechny portály služeb Microsoft Online Vyžadují, aby se partnerské účty při přístupu k prostředkům zákazníků pomocí delegovaných oprávnění správce partnera přihlašují k tenantovi zákazníka. Místo toho vyžadují jenom, aby se partnerské účty přihlašují k partnerského tenantovi. Příkladem je Centrum pro správu Exchange. V průběhu času očekáváme, že tyto portály budou při použití delegovaných oprávnění správce partnerů vyžadovat, aby se partnerské účty přihlašují k tenantovi zákazníka.

### <a name="using-service-apis"></a>Použití rozhraní API služby

Některá rozhraní API služeb Microsoft Online Services (například Azure Resource Manager, Azure AD Graph, Microsoft Graph atd.) podporují partnery, kteří k programové správě prostředků zákazníků používají delegovaná oprávnění správce partnerů. Pokud partnerská delegovaná oprávnění správce s těmito rozhraními API chcete používat, partnerská aplikace musí v hlavičce autorizace požadavku rozhraní API obsahovat přístupový token, kde se přístupový token získá tak, že má uživatelský účet partnera pro ověřování pomocí Azure AD a zákazník azure AD nastaví jako kontext ověřování. Partnerská aplikace musí mít k tenantovi zákazníka přihlášení pomocí partnerského uživatelského účtu.

Když Azure AD obdrží takovou žádost o ověření, Azure AD bude vyžadovat, aby uživatelský účet partnera dokončil ověření MFA. Pokud se uživatelský účet partnera ještě nezaregistroval pro MFA, zobrazí se mu nejprve výzva k dokončení registrace MFA.

Tato funkce ovlivňuje všechny partnerské aplikace integrované s těmito rozhraními API pomocí oprávnění delegovaného správce partnera. Pokud chcete zajistit, aby partnerské aplikace i nadále fungovaly s těmito rozhraními API bez přerušení:

- Partner se musí vyhnout použití neinteraktivní metody ověřování uživatelů se službou Azure AD k získání přístupového tokenu. Pokud používáte neinteraktivní metodu ověřování [uživatelů,](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password)jako je tok hesel, Azure AD nebude moct vyzvat uživatele k dokončení ověřování MFA. Partner musí místo toho přepnout na interaktivní metodu ověřování [uživatelů, OpenID Connect tok.](/azure/active-directory/develop/v1-protocols-openid-connect-code)

- Během interaktivní metody ověřování uživatelů by partner měl používat partnerský uživatelský účet, který je už povolený pro MFA. Případně po zobrazení výzvy azure AD může partner dokončit registraci MFA a ověření MFA během přihlašování.

- Je to podobné scénáři, ve kterém tenant koncového zákazníka implementovali více ověřování pro své správce. Tenant zákazníka například povolil výchozí nastavení zabezpečení [Azure AD,](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)což vyžaduje, aby se všechny uživatelské účty s právy správce přihlašují k tenantovi zákazníka s ověřováním MFA, včetně agentů pro správu a agentů helpdesku. Pro účely testování mohou partneři povolit výchozí nastavení zabezpečení [Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) v tenantovi zákazníka a pak se pokusí použít oprávnění delegované správy partnera k programovému přístupu k tenantovi zákazníka.

### <a name="mfa-registration-experience"></a>Prostředí registrace MFA

Pokud se během ověřování MFA ještě nezaregistrl partnerský účet pro více ověřování, Azure AD vyzve uživatele nejprve k dokončení registrace MFA:

:::image type="content" source="images/MfaRegistration1.png" alt-text="Registrace MFA – krok 1.":::

Po kliknutí **na** Další se uživateli zobrazí dotaz, jestli si má vybrat ze seznamu metod ověřování.

:::image type="content" source="images/MfaRegistration2.png" alt-text="Registrace MFA – krok 2.":::

Po úspěšné registraci se po uživateli vyžaduje dokončení více ověřování na základě ověření zvoleného uživatelem.
 
## <a name="list-of-common-issues"></a>Seznam běžných problémů

Než začnete [zažádat o](#how-to-submit-a-request-for-technical-exception) technickou výjimku z požadavku na MFA, zkontrolujte seznam běžných problémů hlášených jinými partnery a zkontrolujte, jestli je vaše žádost platná.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>Problém 1: Partner potřebuje více času na implementaci MFA pro své partnerské agenty
Partner ještě nezahájí nebo stále provádí implementaci MFA pro partnerskou agenty, kteří ke správě prostředků zákazníků vyžadují přístup k portálům služeb Microsoft Online Services pomocí oprávnění delegované správy pro partnery. Partner potřebuje více času k dokončení implementace MFA. Je tento problém platným důvodem pro technickou výjimku?

**Odpověď:** Ne. Aby se zabránilo přerušení služeb, partner musí pro své uživatele vytvořit plány na implementaci MFA.

> [!NOTE]
> I když partner pro své partnery ne implementoval MFA, partnerská agenti mají stále přístup k portálům Microsoft Online Services pomocí oprávnění delegované správy pro partnery za předpokladu, že po zobrazení výzvy při přihlášení k zákaznickému tenantovi mohou dokončit registraci MFA a ověření MFA. Dokončením registrace MFA se uživateli automaticky nepomáhá MFA.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>Problém 2: Partner ne implementovali MFA pro uživatelské účty, které nevyu účtu využívají delegovaná oprávnění správce
Partner má některé uživatele ve svých partnerských tenantech, kteří nepožadují přístup k portálům služeb Microsoft Online Services, aby bylo možné spravovat prostředky zákazníků pomocí oprávnění delegované správy pro partnery. Partner je v procesu implementace MFA pro tyto uživatele a potřebuje více času k dokončení. Je tento problém platným důvodem pro technickou výjimku?

**Odpověď:** Ne. Vzhledem k tomu, že tyto uživatelské účty ke správě prostředků zákazníků používají oprávnění delegované správy partnera, nebudou se muset přihlašovat k tenantovi zákazníka. Nebudou ovlivněny službou Azure AD, která během přihlašování k tenantovi zákazníka vyžaduje více ověření více ověření.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>Problém 3: Partner ne implementovali MFA pro účty uživatelských služeb
Partner má ve svých partnerských tenantech několik uživatelských účtů, které zařízení používají jako účty služeb. Jedná se o účty s nízkými oprávněními, které nevyžadují přístup k Partnerské centrum ani portálům služeb Microsoft Online Services ke správě prostředků zákazníků pomocí oprávnění delegované správy pro partnery. Je tento problém platným důvodem pro technickou výjimku?

**Odpověď:** Ne. Vzhledem k tomu, že tyto uživatelské účty ke správě prostředků zákazníků používají oprávnění delegované správy partnera, nebudou se muset přihlašovat k tenantovi zákazníka. Nebudou ovlivněny službou Azure AD, která během přihlašování k tenantovi zákazníka vyžaduje více ověření více ověření.

##### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>Problém 4: Partner nemůže implementovat MFA pomocí aplikace MS Authenticator
Partner má zásady "čistého stolu", které zaměstnancům neumožnují přinášet svá osobní mobilní zařízení do jejich pracovní oblasti. Bez přístupu ke svým osobním mobilním zařízením zaměstnanci nemohou nainstalovat aplikaci MS Authenticator, což je jediné ověřování MFA podporované výchozím nastavením zabezpečení Azure AD. Je tento problém platným důvodem pro technickou výjimku?

**Odpověď:** Ne, toto není platný důvod pro technickou výjimku. Partner by měl zvážit následující alternativy, aby jejich zaměstnanci mohli při přístupu k více informacím stále Partnerské centrum:
- Partner se také může zaregistrovat k Azure AD Premium nebo řešení MFA třetích stran (kompatibilní s Azure AD), která mohou poskytovat další metody ověřování.

##### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>Problém 5: Partner nemůže implementovat MFA kvůli použití starších ověřovacích protokolů
Partner má několik partnerských agentů, kteří stále používají starší ověřovací protokoly, které nejsou kompatibilní s MFA. Uživatelé například stále používají Outlook 2010, který je založený na starších ověřovacích protokolech. Povolení MFA pro tyto partnerské agenty naruší používání starších ověřovacích protokolů.

**Odpověď:** Ne, toto není platný důvod pro technickou výjimku. Partnerům se důrazně doporučuje, aby se z důvodu možných bezpečnostních důsledků posunuli od používání starších ověřovacích protokolů, protože tyto protokoly není možné chránit pomocí ověřování MFA a jsou mnohem náchylnější k ohrožení přihlašovacích údajů. Pokud se od používání starších ověřovacích protokolů nepřidáte, měli by partneři zvážit registraci do služby Azure AD Premium, která podporuje používání hesel aplikací. Hesla aplikací jsou jednou vygenerovaná systémem a obvykle jsou silnější než hesla generovaná člověkem. Pomocí hesel aplikací mohou partneři implementovat MFA pro své uživatele a zároveň se vracet k hesly aplikací jenom pro starší verze ověřovacích protokolů.

Přečtěte si příspěvek o základním ověřování a [Exchange Online,](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-auth-and-exchange-online-february-2020-update/ba-p/1191282) abyste pochopili nejnovější plán podpory starší verze ověřování pro Outlook, a sledujte blog týmu [Exchange](https://techcommunity.microsoft.com/t5/exchange-team-blog/bg-p/Exchange) a získejte chystané novinky. 

> [!NOTE]
> I když partner pro své partnery ne implementoval MFA, partnerská agenti mají stále přístup k portálům Microsoft Online Services pomocí oprávnění delegované správy pro partnery za předpokladu, že po zobrazení výzvy při přihlášení k zákaznickému tenantovi mohou dokončit registraci MFA a ověření MFA. Dokončením registrace MFA se uživateli automaticky nepomáhá MFA.

##### <a name="issue-6-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>Problém 6: Partner implementovali více ověřování třetích stran, které služba Azure AD nerozpoznala
Partner implementovali MFA pro své uživatele pomocí řešení MFA jiného výrobce. Partner ale nemůže správně nakonfigurovat řešení MFA třetí strany tak, aby předá službu Azure AD, že ověřování MFA bylo dokončeno během ověřování uživatelů. Je to platný důvod technické výjimky?

**Odpověď:** Ano, tento problém se může považovat za platný důvod technické výjimky. Před odesláním žádosti o technickou výjimku u poskytovatele řešení MFA třetí strany ověřte, že řešení MFA není možné nakonfigurovat tak, aby předávalo deklaraci identity *authenticationmethodsreferences* (s hodnotou *multipleauthn)* do Služby Azure AD, aby bylo indikované, že ověřování MFA bylo dokončeno během ověřování uživatelů. Při odesílání žádosti o technickou výjimku musíte zadat podrobnosti o použitém řešení MFA třetí strany a uvést metodu integrace (například prostřednictvím federace identit nebo použití vlastního ovládacího prvku Azure AD) a v žádosti o technickou výjimku zadat následující informace jako podpůrné dokumenty:

- Konfigurace MFA třetích stran.

- Výsledek testu [požadavků na zabezpečení](/powershell/partnercenter/test-partner-security-requirements) partnerů spuštěných účtem s povoleným více ověřováním třetích stran

- Nákupní objednávka řešení MFA třetí strany, které používáte nebo které plánujete použít.

## <a name="how-to-submit-a-request-for-technical-exception"></a>Odeslání žádosti o technickou výjimku

Pokud se partneři setkávají s technickými problémy se službami Microsoft Online Services a neexistují žádné proveditelné řešení nebo alternativní řešení, mohou požádat o technickou výjimku, aby potlačil ověřování MFA. Před tím si prohlédněte [seznam běžných problémů v](#list-of-common-issues) předchozí části.

Odeslání žádosti o technickou výjimku:

1. Přihlaste se k Partnerské centrum jako globální správce nebo agent pro správu.

2. Vytvořte novou žádost o partnerskou službu tak, že přejdete na **žádosti o** podporu partnerů podpory a  >   **vyberete Nová žádost.**

3. Ve **vyhledávacím poli vyhledejte MFA – Žádost** o výjimku. nebo vyberte **CSP** z kategorie, pak vyberte **Účty, Onboarding, Přístup** z tématu, pak **vyberte MFA – Žádost** o výjimku z dílčího tématu a pak vyberte další **krok.**

4. Zadejte podrobnosti požadované k odeslání žádosti o služby pro technickou výjimku a vyberte **Odeslat.**

Poskytnutí odpovědi na žádost o technickou výjimku může Microsoftu trvat až tři pracovní dny.

## <a name="next-steps"></a>Další kroky

 - [Stav požadavků na zabezpečení partnerů](partner-security-compliance.md)