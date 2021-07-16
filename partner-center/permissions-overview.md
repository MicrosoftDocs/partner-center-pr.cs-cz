---
title: Přiřazení rolí & oprávnění uživatelům
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, které role jsou pro uživatele vaší společnosti, kteří spravují komerční transakce, referenční seznam, pobídky nebo členství v programu MPN, nejlepší Partnerské centrum.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperf-fy21q1
ms.openlocfilehash: a9cca322d7a37dce099c5bec44530b2006da7758
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2021
ms.locfileid: "114373667"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a>Přiřaďte uživatelům role a oprávnění pro firemní uživatele, kteří potřebují pracovat v Partnerské centrum

**Odpovídající role:** Globální správce | Správce správy uživatelů | Správce partnera MPN

Nastavili jste profil partnera, včetně oficiálního jména a adresy, podrobností o podpoře, osvobození od daně ze souborů, bankovních údajů a primárního kontaktu vaší společnosti. Další krok: Nastavení hesel a rolí pro uživatele, aby s Partnerské centrum mohli začít pracovat.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Nastavení zaměstnanců pro práci v Partnerské centrum

Určíte typy přístupu, které uživatelé musí Partnerské centrum rolemi a oprávněními, které jim poskytnete. Role souvisejí s programy, do které se vaše firma podílí. Pokud je například vaše firma podnikem Cloud Solution Provider (CSP), budete mít nejen standardní role správy tenanta Azure Active Directory (Azure AD), jako je globální správce, ale budete potřebovat role specifické pro program CSP. Každý program má role, které jsou pro něj specifické.

>[!Note]
> Role tenanta Azure AD zahrnují role globálního správce, správce uživatelů a CSP. Role mimo Azure-AD jsou role, které tenanta nespravuje, a zahrnují správce partnera MPN (Microsoft Partner Network), správce obchodního profilu, správce referenčních doporučení, správce pobídek a uživatele pobídek. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Správa komerčních transakcí v Partnerské centrum (role Azure AD a CSP)

|**Role**|**Co mohou dělat**|**Další informace**|
|----------------------------------|---|:---------------------------------|
|Globální správce|* Má přístup ke všem účet Microsoft nebo službám s úplnými oprávněními.|[Správa účtu v Partnerském centru](partner-center-account-setup.md)
|      |* Vytvoření lístků podpory pro Partnerské centrum
||* Zobrazit lístky podpory pro partnery, které vytvoříte
||* Zobrazení smluv, ceníků a nabídek
||* Zobrazení, vytváření a správa partnerských uživatelů|
||  Zobrazení, vytvoření a správa fakturace, faktur a souborů odsoustavy
|Správce správy uživatelů   | * Zobrazení, vytváření a správa uživatelů|[Správa výhod a nabídek Microsoft Partner Network vašeho členství v Partnerské centrum](manage-your-partner-network-benefits.md)
||* Zobrazit vše profily partnerů
||* Vytvoření lístků podpory pro Partnerské centrum
||* Zobrazit lístky podpory pro partnery, které vytvoříte
|Správce fakturace | – Zobrazení, vytvoření a správa faktur, faktur a souborů odsoustavy|[Čtení informací na faktuře](billing.md)
||* Zobrazit ceny
||* Vytvoření lístků podpory pro Partnerské centrum
||* Zobrazit lístky podpory pro partnery, které vytvoříte
|Výchozí uživatel|  Zobrazit Můj profil   |[Resetování hesla](reset-my-pasword.md)
|Agent pro správu | * Správa zákazníků|[Spojení se zákazníky](connect-with-your-customers.md)
||* Přidání seznamu zařízení do Partnerské centrum
||* Vytvoření a použití profilů na zařízeních
||* Správa předplatného
||* Stav služby a žádosti o služby pro zákazníky
||* Požádat o delegovaná oprávnění správce
||* Zobrazení cen a nabídek
||* Fakturace
||* Správa jménem zákazníka
||* Registrace prodejce s přidanou hodnotou
||* Vytvoření lístků podpory pro Partnerské centrum
||* Zobrazit lístky podpory pro partnery, které vytvoříte|
|Agent prodeje | * Správa zákazníků|[Poskytování podpory fakturace pro vaše zákazníky a pomoc s zodpovězení jejich dotazů k fakturaci](provide-billing-support.md)
||* Přidání seznamu zařízení do Partnerské centrum
||* Správa předplatného
||* Zobrazení lístků podpory
||* Žádost o vztah se zákazníkem
||* Zobrazení cen a nabídek
||* Správa potenciálních zákazníků
||* Zobrazení smlouvy se zákazníkem
||* Registrace prodejce s přidanou hodnotou
||* Vytvoření lístků podpory pro Partnerské centrum
||* Zobrazit lístky podpory pro partnery, které vytvoříte|
|Agent helpdesku| * Vyhledání a zobrazení zákazníka|[Eskalace problémů do Microsoftu a informace o problémech, které jsou pro eskalaci Microsoftu vhodné](escalate-problems-to-microsoft.md)
||* Upravit podrobnosti o zákazníkovi
||* Pomoc s řešením problémů zákazníků s fakturací nebo s předplatným
||* Žádost o podporu jménem zákazníků 
||* Správa předplatných a problémů s fakturací jménem zákazníků
||* Vytvoření lístků podpory pro Partnerské centrum
||* Zobrazit lístky podpory pro partnery, které vytvoříte| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a>Ovládací panely dodavatele (CPV). (role CSP a role mimo Azure AD)

Společnost CPV vyvíjí aplikace, které používají partneři CSP, aby jim umožnily integrovat své systémy s Partnerské centrum rozhraními API. 

|**Role**   |**Co můžete dělat**|**Další informace**|
|------------------------------|:----------------------------|----|
|Globální správce| Zobrazení a správa profilu Ovládací panely dodavatele hardwaru (CPV)|[Zaregistrujte se jako dodavatel Ovládací panely, který vám pomůže integrovat partnerské systémy CSP s Partnerské centrum API.](enroll-as-cpv.md)
||Zobrazení a správa všech uživatelů, kteří potřebují přístup k funkcím CPV|

### <a name="guest-user-must-be-added-to-the-azure-ad-tenant"></a>Uživatel hosta (musí být přidán do tenanta Azure AD)

|**Uživatel hosta**   | **Role**|
|---------------------------|:--------------------|
||Správce partnera MPN|
||Správce obchodního profilu|
||Správce referenčních odkazů|


## <a name="manage-mpn-membership-and-your-company"></a>Správa členství v programu MPN a vaší společnosti 

Tyto role nejsou role Azure AD. Tyto role spravují podnik společnosti, nikoli tenanta.

|**Role** | **Co můžete dělat**|**Další informace**|
|----------------------------|:----------------------------|-----|
|Správce partnera MPN|* Zobrazení, vytváření a správa žádostí o partnerské služby|[Nákup nebo prodloužení platnosti předplatného programu Microsoft Action Pack nebo kompetencí Silver a Gold Competency](mpn-get-action-pack.md)
||* Zobrazit právní profily, profily společnosti, firmy a MPN
||* Zobrazit podrobnosti o uživateli a jeho dovednosti
||* Zobrazení kompetencí
||* Zobrazení a správa výhod
||* Zobrazení a nákup nabídek MPN
||* Zobrazení historie objednávek a faktur nabídek MPN
||* Zobrazit data indikátoru příspěvku partnera
||* Může pracovat v nástroji pro ověřování poukazů|
||* Zobrazení analýzy dat zákazníků
||* Zobrazit další role uživatelů v rámci společnosti, ale nemůže přiřazovat role
||* Vytvoření lístků podpory pro Partnerské centrum
||* Zobrazit lístky podpory pro partnery, které vytvoříte
|Správce účtu| Přidání umístění|[Správa umístění](manage-locations.md)
|| Správa profilů souvisejících s účty, pro které jste správcem 
||* Přiřaďte role uživatelům v tenantovi k rolím mimo Azure AD. 
||* Registrace umístění do programů
||* Vytvoření lístků podpory pro Partnerské centrum
||* Zobrazit lístky podpory pro partnery, které vytvoříte

## <a name="manage-referrals"></a>Správa referenčních odkazů

|**Role** | **Co můžete dělat**|**Další informace**
|------------------------------|:-------------------------|---|
|Správce referenčních odkazů|Vytvoření a správa všeho na kartě Referenční Partnerské centrum|[Správa příležitostí ke spoluprodeji](manage-co-sell-opportunities.md)
||    Může zobrazit a upravit všechny potenciální zákazníky a příležitosti ke spoluprodání.
||    Může přiřazovat členy týmu k dohody.
||    Může zobrazit a upravit obchodní profily.
||    Může zobrazit a zaregistrovat dohody pro příležitosti, které jsou označené jako won a mají nárok na registraci dohody.
||    Může vytvářet a prohlížet lístky podpory.
|Uživatel referenčních odkazů|Vytvářejte a spravujte příležitosti ke spoluprodání jenom v případě, že jsou součástí týmu. |[Správa příležitostí ke spoluprodeji](manage-co-sell-opportunities.md)
||    Může vytvářet příležitosti ke spoluprodání pro lokality, ve kterých mají přiřazenou roli.
||    Může zobrazit a zaregistrovat dohody pro příležitosti označené jako won a způsobilé k registraci dohody, pokud jsou členy týmu.
||    Může vytvářet a prohlížet lístky podpory.
|Správce obchodního profilu|Vytvoření a správa obchodních profilů | [Správa obchodních profilů](create-a-marketing-profile.md)
||    Může vytvářet a prohlížet lístky podpory.

Spolu s novou rolí uživatele referenčních seznamů také zavádíme rozsah umístění pro obchody. Následující tabulka vysvětluje přístup k obchodům na základě umístění.

|**Scope** | **Co můžete dělat** |
|------------------------------|:-------------------------|
|Celá společnost | Správci i uživatelé mají přístup k vytváření dohod pro libovolnou lokalitu ve své společnosti.|
|| Správce referenčních seznamu má přístup k zobrazení a úpravám všech dohod. |
|| Uživatelé referenčních seznamu mají přístup k zobrazení a úpravám všech dohod jenom v případě, že jsou součástí týmu. |
|Jedno nebo více umístění | Správci i uživatelé mají přístup k vytváření dohod pro přiřazenou lokalitu ve své společnosti.|
|| Správce referenčních seznamu má přístup k zobrazení a úpravám všech dohod, které patří do přiřazených umístění.|
|| Uživatelé referenčních seznamu mají přístup k zobrazení a úpravě všech dohod, které patří do přiřazených umístění, pokud jsou součástí týmu.|

## <a name="manage-incentives"></a>Správa pobídek

|**Role** | **Co můžete dělat**|**Další informace**
|------------------------------|:-------------------------|---|
|Správce pobídek|* Iniciuje a spravuje pobídky |[Tyto zdroje informací vám pomůžou začít s pobídky.](incentives-get-started-intro.md)
||* Může zobrazit a upravit všechny aspekty programů pobídek.
||* Může zobrazit a upravit bankovní a daňové údaje.
||* View rebate and co-op earnings
||* Podpora přístupu
||* Platby za pobídky sporů|
|Uživatel pobídek|* Může zobrazit programy pobídek
||* Může zobrazit a iniciovat žádosti o pobídky.
||* View rebate and co-op earnings
||* Vytvoření lístků podpory pro Partnerské centrum
||* Zobrazit lístky podpory pro partnery, které vytvoříte

## <a name="view-partner-center-insights-data"></a>Zobrazení Partnerské centrum Přehledy dat

|**Role** | **Co můžete dělat**|**Další informace**|
|------------------------------|:-------------------------|---|
|Prohlížeč výkonných sestav|Přístup ke všem datovým sadám pro vytváření sestav, vytváření lístků podpory pro partnery, zobrazení lístků podpory pro partnery, které vytvoříte|[Přehled sestav řídicího panelu dostupných v Partnerské centrum Přehledy](insights-overview-report.md)
|Prohlížeč sestav|Přístup k sestavě dat s výjimkou výnosů a osobních údajů zákazníků a zaměstnanců, vytváření lístků podpory pro partnery, zobrazení lístků podpory pro partnery, které vytvoříte|

## <a name="next-steps"></a>Další kroky

- [Vytváření uživatelských účtů a přiřazování rolí a oprávnění](create-user-accounts-and-set-permissions.md)
- [Ověření informací o účtu při registraci do nového Partnerské centrum programu](verification-responses.md)
