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
ms.openlocfilehash: b1b02967209ba36088b0c7bb7487428ab08b8a37
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152575"
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


| Stránka chráněná MFA       | Agenti pro správu      |  Agenti prodeje     |   Agenti helpdesku     | Globální správce      |  Správce fakturace     | 
|---    |---    |---    |---    |---    |---    |
| Všechny stránky na kartě Zákazníci      |   x    |    x   |  x     |       |       |
| Všechny stránky na kartě Support > Customer Requests (Žádosti zákazníků)     | x      |       |    x   |       |       |
| Stránka fakturace     |   x    |       |       |    x   |   x    |

Pokud se pokusíte získat přístup k kterékoli z těchto stránek a ještě jste dříve neskončili ověřování MFA, budete k tomu muset použít . Další stránky na Partnerské centrum, jako je například stránka Přehled, Service Health kontrola stavu nevyžadují MFA.

## <a name="verification-examples"></a>Příklady ověřování

Pokud chcete ilustrovat, jak funguje ověřování Partnerské centrum řídicím panelu, zvažte následující příklady.

### <a name="example-1-partner-has-implemented-azure-ad-mfa"></a>Příklad 1: Partner implementovali Azure AD MFA

1. Jana pracuje pro CSP Contoso. Contoso implementovali MFA pro všechny své uživatele v partnerském tenantovi Společnosti Contoso pomocí Azure Active Directory (Azure AD) MFA.

2. Jana spustí novou relaci prohlížeče a přejde na Partnerské centrum přehledu řídicího panelu (která není chráněná MFA). Partnerské centrum přesměruje Janu do Azure AD, aby se přihlašuje.

3. Kvůli stávajícímu nastavení Azure AD MFA od společnosti Contoso je Jana nutná k dokončení ověřování MFA. Po úspěšném přihlášení a ověření MFA se Jana přesměruje zpět na Partnerské centrum řídicího panelu.

4. Jana se pokusí získat přístup k jedné ze stránek chráněných více ověřováním v Partnerské centrum. Vzhledem k tomu, že Jana už dříve dokončila ověřování MFA při přihlašování, může získat přístup na stránku chráněnou vícefainem, aniž by se vyžadovalo, aby znovu prošla ověřením MFA.

### <a name="example-2-partner-has-implemented-third-party-mfa-using-identity-federation"></a>Příklad 2: Partner implementovali vícefabové ověřování třetích stran pomocí federace identit

1. Ve společnosti CSP Wingtip funguje Takét. Společnost Wingtip implementovala vícefaktorové ověřování pro všechny své uživatele v partnerském tenantovi klienta Wingtip pomocí MFA, která je integrovaná se službou Azure AD prostřednictvím federace identit.

2. Trent spustí novou relaci prohlížeče a přejde na stránku s přehledem řídicího panelu partnerského centra (což není chráněna MFA). Partnerské centrum přesměruje Trent do služby Azure AD, aby se přihlásil.

3. Vzhledem k tomu, že společnost Wingtip má nastavení federace identit, Azure AD přesměruje Trent na federovaného zprostředkovatele identity, aby bylo možné dokončit přihlášení a ověřování MFA. Po úspěšném přihlášení a ověření MFA se Trent přesměruje zpátky na Azure AD a pak na stránku Přehled řídicího panelu partnerského centra.

4. Trent se snaží o přístup k jedné ze stránek chráněných MFA v partnerském centru. Vzhledem k tomu, že Trent již dokončila ověřování MFA během přihlašování, Trent má přístup ke stránce chráněné MFA, aniž by bylo nutné se znovu projít ověřováním MFA.

### <a name="example-3-partner-hasnt-implemented-mfa"></a>Příklad 3: partner neimplementoval MFA

1. Jan funguje pro zprostředkovatele CSP Fabrikam. Společnost Fabrikam neimplementovala MFA pro žádného uživatele v partnerském tenantovi Fabrikam.

2. Jan spustí novou relaci prohlížeče a přejde na stránku s přehledem řídicího panelu partnerského centra (která není chráněna MFA). Partnerské centrum přesměruje Jan na službu Azure AD, aby se přihlásil.

3. Vzhledem k tomu, že společnost Fabrikam neimplementovala MFA, nepotřebuje Jan dokončit ověřování MFA. Po úspěšném přihlášení se Jan přesměruje zpátky na stránku Přehled řídicího panelu partnerského centra.

4. Jan se pokusí získat přístup k jedné ze stránek chráněných MFA v partnerském centru. Vzhledem k tomu, že Jan nedokončil ověřování MFA, Partnerské centrum přesměruje Jan na Azure AD, aby se dokončilo ověřování MFA. Vzhledem k tomu, že se jedná o první požadavek Jan, aby bylo možné provést MFA, je pro [vícefaktorové ověřování](#mfa-registration-experience)také požádána Jan. Po úspěšné registraci MFA a ověřování MFA teď má Jan přístup na stránku chráněnou MFA.

5. Druhý den před tím, než společnost Fabrikam implementuje MFA pro libovolného uživatele, spustí novou relaci prohlížeče a přejde na stránku Přehled řídicího panelu partnerského centra (což není chráněno MFA). Partnerské centrum přesměruje Johna do Azure AD, aby se přihlašuje bez výzvy KFA. 

6. Jan se pokusí získat přístup k jedné ze stránek chráněných více ověřováním v Partnerské centrum. Vzhledem k tomu, že Jan nedokončil ověřování MFA, Partnerské centrum přesměruje Johna do Azure AD, aby se dokončilo ověřování MFA. Vzhledem k tomu, že Jan zaregistroval MFA, je tentokrát požádán pouze o dokončení ověřování MFA.

> [!NOTE]
>Akce: Správci společnosti [mají tři možnosti](partner-security-requirements.md#implementing-multi-factor-authentication) implementace MFA.

## <a name="partner-center-api"></a>Rozhraní API partnerského centra

Rozhraní Partnerské centrum API podporuje ověřování pouze na základě aplikace i ověřování aplikací a uživatelů. 

Při použití ověřování aplikací a uživatelů bude Partnerské centrum ověřování MFA. Konkrétněji řečeno, pokud partnerská aplikace chce odeslat požadavek rozhraní API do Partnerské centrum, musí v autorizační hlavičce požadavku obsahovat přístupový token. 

> [!NOTE]
>Architektura [Model zapezpečených aplikací je](/partner-center/develop/enable-secure-app-model) škálovatelná architektura pro ověřování partnerů CSP a procesorů prostřednictvím architektury MFA Microsoft Azure při volání rozhraní PARTNERSKÉ CENTRUM API. Toto rozhraní musíte implementovat před povolením MFA ve vašem tenantovi. 

Když Partnerské centrum rozhraní API s přístupový tokenem získaným pomocí ověřování aplikací a uživatelů, rozhraní Partnerské centrum API zkontroluje přítomnost hodnoty *MFA* v deklaraci identity *amr (Authentication Method Reference).* Dekodér JWT můžete použít k ověření, jestli přístupový token obsahuje očekávanou hodnotu odkazu na metodu ověřování (AMR):

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

Pokud je hodnota přítomná, Partnerské centrum, že se dokončilo ověřování MFA, a zpracuje požadavek rozhraní API. Pokud hodnota neexistuje, rozhraní API Partnerské centrum požadavek zamítne s následující odpovědí:

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

Při App-Only ověřování budou rozhraní API, která podporují ověřování App-Only, nepřetržitě fungovat bez vyžadování MFA.

## <a name="partner-delegated-administration"></a>Delegovaná správa partnerů

Partnerské účty, včetně agentů pro správu a agentů helpdesku, můžou používat svá oprávnění správce delegovaná pro správu zákaznických prostředků prostřednictvím portálů Microsoft Online Services, rozhraní příkazového řádku (CLI) a rozhraní API (pomocí ověřování aplikací a uživatelů).

### <a name="using-service-portals"></a>Používání portálů služeb

Při přístupu k portálům služby Microsoft Online Services pomocí delegovaných oprávnění správce (admin-on-of) za účelem správy zákaznických prostředků musí mnoho z těchto portálů vyžadovat interaktivní ověření partnerského účtu s klientem Azure AD, který je nastaven jako kontext ověřování – Partnerský účet je vyžadován pro přihlášení k tenantovi zákazníka.

Když Azure AD obdrží takové žádosti o ověření, bude vyžadovat, aby Partnerský účet dokončil ověřování MFA. Existují dvě možná uživatelská prostředí v závislosti na tom, jestli je partnerským účtem spravovaná nebo federované identita:

- Pokud je partnerským účtem **spravovaná** identita, služba Azure AD bude přímo vyzvat uživatele k dokončení ověřování MFA. Pokud partnerský účet není pro MFA s Azure AD zaregistrovaný, zobrazí se uživateli výzva, aby nejdřív [dokončil registraci MFA](#mfa-registration-experience) .

- Pokud je Partnerský účet **federované** identitou, bude prostředí závislé na tom, jak správce partnera nakonfiguroval federaci ve službě Azure AD. Při nastavování federace ve službě Azure AD může správce partnera naznačovat službě Azure AD, jestli zprostředkovatel federovaných identit podporuje vícefaktorové ověřování (MFA). Pokud ano, Azure AD přesměruje uživatele na federovaného zprostředkovatele identity, aby se dokončilo ověřování MFA. V opačném případě Azure AD vyzve uživatele přímo k dokončení ověřování MFA. Pokud partnerský účet není pro MFA s Azure AD zaregistrovaný, zobrazí se uživateli výzva, aby nejdřív [dokončil registraci MFA](#mfa-registration-experience) .

Celkové prostředí se podobá scénáři, kdy tenant koncového zákazníka implementoval MFA pro své správce. Například tenant zákazníka povolil výchozí nastavení zabezpečení [Azure AD,](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)což vyžaduje, aby se všechny účty s právy správce přihlašují k tenantovi zákazníka s ověřováním MFA, včetně agentů pro správu a agentů helpdesku. Pro účely testování mohou partneři povolit výchozí nastavení zabezpečení [Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) v tenantovi zákazníka a pak se pokusit použít oprávnění delegované správy partnera pro přístup k tenantovi zákazníka.

> [!NOTE]
> Ne všechny portály služeb Microsoft Online Vyžadují, aby se partnerské účty při přístupu k prostředkům zákazníků pomocí delegovaných oprávnění správce partnera přihlašují k tenantovi zákazníka. Místo toho vyžadují jenom, aby se partnerské účty přihlašují k partnerského tenantovi. Příkladem je Centrum pro správu Exchange. V průběhu času očekáváme, že tyto portály budou při použití delegovaných oprávnění správce partnerů vyžadovat, aby se partnerské účty přihlašují k tenantovi zákazníka.

### <a name="using-service-apis"></a>Použití rozhraní API služby

Některá rozhraní API služeb Microsoft Online Services (například Azure Resource Manager, Azure AD Graph, Microsoft Graph atd.) podporují partnery s využitím delegovaných oprávnění správce pro partnery k programové správě prostředků zákazníků. Pokud partnerská delegovaná oprávnění správce s těmito rozhraními API chcete používat, partnerská aplikace musí v hlavičce autorizace požadavku rozhraní API obsahovat přístupový token, kde se přístupový token získá tak, že má uživatelský účet partnera k ověření ve službě Azure AD a jako kontext ověřování nastaví zákazník Azure AD. Partnerská aplikace musí mít k tenantovi zákazníka přihlášení pomocí partnerského uživatelského účtu.

Když Azure AD obdrží takovou žádost o ověření, Azure AD bude vyžadovat, aby uživatelský účet partnera dokončil ověření MFA. Pokud se uživatelský účet partnera ještě nezaregistroval pro MFA, bude tento uživatelský účet vyzván k dokončení registrace MFA jako první.

Tato funkce ovlivňuje všechny partnerské aplikace integrované s těmito rozhraními API pomocí oprávnění delegovaného správce partnera. Pokud chcete zajistit, aby partnerské aplikace i nadále fungovaly s těmito rozhraními API bez přerušení:

- Partner se musí při získání přístupového tokenu vyhnout použití metody neinteraktivního ověřování uživatelů ve službě Azure AD. Při použití neinteraktivní metody ověřování uživatele, jako je například [tok hesla](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password), služba Azure AD nebude moci vyzvat uživatele k dokončení ověřování MFA. Partner se musí přepnout na použití interaktivní metody ověřování uživatelů, jako je například [OpenID Connect Flow](/azure/active-directory/develop/v1-protocols-openid-connect-code) .

- Při ověřování pomocí interaktivního uživatele by partner měl používat partnerský uživatelský účet, který je už povolený pro MFA. Případně po zobrazení výzvy službou Azure AD může partner dokončit registraci MFA a ověřování MFA během přihlašování.

- To se podobá scénáři, kdy tenant koncového zákazníka implementoval MFA pro své správce. Tenant zákazníka má například povolené [výchozí hodnoty zabezpečení Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), což vyžaduje, aby všechny uživatelské účty s právy správce se přihlásily k klientovi zákazníka pomocí ověřování MFA, včetně agentů pro správu a agentů helpdesku. Pro účely testování můžou partneři povolit [výchozí nastavení zabezpečení Azure AD](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) v tenantovi zákazníka a potom se pokusit o programový přístup k tenantovi zákazníka přes delegovaná oprávnění pro správu.

### <a name="mfa-registration-experience"></a>Prostředí registrace MFA

Pokud se během ověřování MFA ještě nezaregistroval Partnerský účet pro MFA, Azure AD vyzve uživatele, aby nejdřív dokončil registraci MFA:

:::image type="content" source="images/MfaRegistration1.png" alt-text="Registrace MFA – krok 1":::

Po kliknutí na tlačítko **Další** se uživateli zobrazí výzva k výběru ze seznamu metod ověřování.

:::image type="content" source="images/MfaRegistration2.png" alt-text="Registrace MFA – krok 2":::

Po úspěšné registraci se uživateli pak vyžaduje dokončení ověřování MFA na základě ověření, které uživatel zvolil.
 
## <a name="list-of-common-issues"></a>Seznam běžných problémů

Před použitím pro [technickou výjimku](#how-to-submit-a-request-for-technical-exception) z požadavku MFA si přečtěte seznam běžných problémů hlášených ostatními partnery, abyste zjistili, jestli je vaše žádost platná.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>Problém 1: partner potřebuje víc času na implementaci MFA pro své partnerské agenty.
Partner ještě nezačal nebo stále provádí implementaci MFA pro partnerskou agenty, kteří ke správě prostředků zákazníků vyžadují přístup k portálům služeb Microsoft Online Services pomocí oprávnění delegované správy pro partnery. Partner potřebuje více času k dokončení implementace MFA. Je tento problém platným důvodem pro technickou výjimku?

**Odpověď:** Ne. Aby se předešlo přerušení služeb, partner musí plánovat implementaci MFA pro své uživatele.

> [!NOTE]
> I když partner pro své partnery ne implementoval MFA, partnerská agenti mají stále přístup k portálům Microsoft Online Services pomocí oprávnění delegované správy pro partnery za předpokladu, že po zobrazení výzvy při přihlášení k zákaznickému tenantovi mohou dokončit registraci MFA a ověření MFA. Dokončení registrace MFA automaticky nepomáhá uživateli pro MFA.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>Problém 2: Partner ne implementovali MFA pro uživatelské účty, které nevyu používají delegovaná oprávnění správce
Partner má některé uživatele ve svých partnerských tenantech, kteří nepožadují přístup k portálům služeb Microsoft Online Services, aby bylo možné spravovat prostředky zákazníků pomocí oprávnění delegované správy pro partnery. Partner je v procesu implementace MFA pro tyto uživatele a potřebuje více času k dokončení. Je tento problém platným důvodem pro technickou výjimku?

**Odpověď:** Ne. Vzhledem k tomu, že tyto uživatelské účty ke správě prostředků zákazníků používají oprávnění delegované správy partnera, nebudou se muset přihlašovat k tenantovi zákazníka. Nebudou ovlivněny službou Azure AD, která během přihlašování k tenantovi zákazníka vyžaduje více ověřování.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>Problém 3: Partner ne implementovali MFA pro účty uživatelských služeb
Partner má ve svých partnerských tenantech několik uživatelských účtů, které zařízení používají jako účty služeb. Jedná se o účty s nízkými oprávněními, které nevyžadují přístup k Partnerské centrum ani portálům služeb Microsoft Online Services ke správě prostředků zákazníků pomocí oprávnění delegované správy pro partnery. Je tento problém platným důvodem pro technickou výjimku?

**Odpověď:** Ne. Vzhledem k tomu, že tyto uživatelské účty nepoužívají pro správu zákaznických prostředků oprávnění k delegované správě, nebudou se muset přihlašovat k tenantovi zákazníka. Nebudou ovlivněny službou Azure AD vyžadovat ověřování MFA během přihlašování k tenantovi zákazníka.

##### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>Problém 4: partner nemůže implementovat MFA pomocí aplikace MS Authenticator.
Partner má "uklizenou" zásadu, která neumožňuje zaměstnancům, aby do své pracovní oblasti nastavili svá osobní mobilní zařízení. Bez přístupu k osobním mobilním zařízením nemohou zaměstnanci nainstalovat aplikaci MS Authenticator, což je jediné ověřování MFA podporované výchozími nastaveními zabezpečení Azure AD. Je to problém platným důvodem pro technickou výjimku?

**Odpověď**: Ne, nejedná se o platný důvod pro technickou výjimku. Partner by měl zvážit následující alternativy, aby jejich zaměstnanci mohli při přístupu k partnerskému centru i nadále provádět ověřování MFA:
- Partner se taky může zaregistrovat Azure AD Premium nebo řešení VÍCEFAKTOROVÉHO ověřování třetích stran (kompatibilní s Azure AD), které může poskytovat další metody ověřování.

##### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>Problém 5: partner nemůže implementovat MFA z důvodu použití starších protokolů ověřování.
Partner má některé agenty, kteří stále používají starší protokoly ověřování, což není kompatibilní s MFA. Uživatelé například pořád používají Outlook 2010, který je založený na starších protokolech ověřování. Povolení MFA pro tyto agenty budou rušit používání starších protokolů ověřování.

**Odpověď**: Ne, nejedná se o platný důvod pro technickou výjimku. Partnerům se důrazně doporučuje přesunout se z používání starších protokolů ověřování z důvodu potenciálních důsledků zabezpečení, protože tyto protokoly nelze chránit pomocí ověřování MFA a jsou mnohem náchylnější k ohrožení bezpečnosti přihlašovacích údajů. Pokud už nepoužíváte starší verze ověřovacích protokolů, partneři by si měli zvážit, že se zaregistrují Azure AD Premium, což podporuje používání hesel aplikací. Hesla aplikací jsou jednou vygenerovaná systémem a obvykle jsou silnější než hesla generovaná člověkem. Pomocí hesel aplikací mohou partneři implementovat MFA pro své uživatele a zároveň se vracet k hesly aplikací jenom pro starší verze ověřovacích protokolů.

Přečtěte si příspěvek o základním ověřování a [Exchange Online,](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-auth-and-exchange-online-february-2020-update/ba-p/1191282) abyste pochopili nejnovější plán podpory starší verze ověřování pro Outlook, a sledujte blog týmu [Exchange](https://techcommunity.microsoft.com/t5/exchange-team-blog/bg-p/Exchange) a získejte chystané novinky. 

> [!NOTE]
> I když partner pro své partnery ne implementoval MFA, partnerská agenti mají stále přístup k portálům Microsoft Online Services pomocí oprávnění delegované správy pro partnery za předpokladu, že po zobrazení výzvy při přihlášení k zákaznickému tenantovi mohou dokončit registraci MFA a ověření MFA. Dokončení registrace MFA automaticky nepomáhá uživateli pro MFA.

##### <a name="issue-6-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>Problém 6: Partner implementovali více ověřování třetích stran, které služba Azure AD nerozpoznala
Partner implementovali MFA pro své uživatele pomocí řešení MFA jiného výrobce. Partner ale nemůže správně nakonfigurovat řešení MFA třetí strany tak, aby předá službu Azure AD, že ověřování MFA bylo dokončeno během ověřování uživatelů. Je to platný důvod technické výjimky?

**Odpověď:** Ano, tento problém se může považovat za platný důvod technické výjimky. Před odesláním žádosti o technickou výjimku u poskytovatele řešení MFA třetí strany ověřte, že řešení MFA není možné nakonfigurovat tak, aby přetékalo deklaraci identity *authenticationmethodsreferences* (s hodnotou *multipleauthn)* do Služby Azure AD, aby bylo indikované, že ověřování MFA bylo dokončeno během ověřování uživatelů. Při odesílání žádosti o technickou výjimku musíte zadat podrobnosti o použitém řešení MFA třetí strany a uvést metodu integrace (například prostřednictvím federace identit nebo použití vlastního ovládacího prvku Azure AD) a v žádosti o technickou výjimku zadat následující informace jako podpůrné dokumenty:

- Konfigurace vícefaktorového ověřování třetích stran.

- Výsledek [testování partnerských požadavků na zabezpečení](/powershell/partnercenter/test-partner-security-requirements) , které jsou spuštěny účtem s POVOLENým ověřováním MFA třetí strany.

- Nákupní objednávka řešení MFA třetí strany, které používáte, nebo který plánujete použít.

## <a name="how-to-submit-a-request-for-technical-exception"></a>Odeslání žádosti o technickou výjimku

Partneři můžou požádat o technickou výjimku pro potlačení ověřování MFA, pokud se setkávají s technickými problémy s online službami Microsoftu a neexistuje žádné praktické řešení ani řešení. Než to uděláte, Projděte si [seznam běžných problémů](#list-of-common-issues) v předchozí části.

Odeslání žádosti o technickou výjimku:

1. Přihlaste se do partnerského centra jako globální správce nebo jako agent pro správu.

2. Vytvořte novou žádost o partnerskou službu tak, že přejdete na **podporu**  >  **žádostí o podporu partnerů** a vyberete **nový požadavek**.

3. Ve vyhledávacím poli vyhledejte **MFA – požadavek na výjimku** ; nebo vyberte **CSP** z kategorie, vyberte **účty, registrace, přístup** z tématu, pak v dílčím tématu vyberte **MFA-Request pro výjimku** a pak vyberte **Další krok**.

4. Zadejte podrobnosti požadované k odeslání žádosti o technickou výjimku a vyberte **Odeslat**.

Společnost Microsoft může trvat až tři pracovní dny a poskytnou odpověď na požadavek na technickou výjimku.

## <a name="next-steps"></a>Další kroky

 - [Stav požadavků na zabezpečení partnerů](partner-security-compliance.md)