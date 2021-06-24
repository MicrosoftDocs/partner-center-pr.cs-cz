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
ms.openlocfilehash: 582fdc98617be7d82c0bc61a0bf46ceb662954d3
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565079"
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
||* Zobrazit profily legálního, podnikového a MPN
||* Zobrazení podrobností o uživateli a jejich údajů o dovednostech
||* Zobrazit kompetence
||* Zobrazení a Správa výhod
||* Zobrazit a koupit nabídky MPN
||* Zobrazit nabídku MPN nabízí historii objednávek a faktury
||* Zobrazit data ukazatele příspěvku partnera
||* Může fungovat v nástroji pro ověřování dokladů.|
||* Zobrazení analýzy zákaznických dat
||* Zobrazit další uživatelské role v rámci společnosti, ale nemůžou přiřadit role
||* Vytvoření lístků podpory pro partnerské Centrum
||* Zobrazit lístky podpory partnerů, které vytvoříte
|Správce účtu| Přidat umístění|[Správa umístění](manage-locations.md)
|| Správa profilů souvisejících s účty, ke kterým jste správce 
||* Přiřaďte role pro uživatele v tenantovi k rolím mimo Azure AD. 
||* Registrace umístění do programů
||* Vytvoření lístků podpory pro partnerské Centrum
||* Zobrazit lístky podpory partnerů, které vytvoříte

## <a name="manage-referrals"></a>Správa odkazů

|**Role** | **Co můžete dělat**|**Další informace**
|------------------------------|:-------------------------|---|
|Správce odkazů|Vytvoření a Správa všeho v části karta odkazy v partnerském centru|[Správa příležitostí ke spoluprodeji](manage-co-sell-opportunities.md)
||    Může zobrazit a upravit všechny příležitosti a potenciální zákazníky ve společném prodeji.
||    Může přiřadit členy týmu pro obchod.
||    Může zobrazovat a upravovat obchodní profily.
||    Může zobrazit a zaregistrovat obchody pro příležitosti, které jsou označené jako získané a které mají nárok na registraci koupí.
||    Může vytvářet a zobrazovat lístky podpory
|Uživatel s odkazy|Vytváření a správa příležitostí společného prodeje pouze v případě, že jsou součástí týmu |[Správa příležitostí ke spoluprodeji](manage-co-sell-opportunities.md)
||    Může vytvořit příležitosti pro společný prodej pro umístění, kde jsou přiřazena role.
||    Může zobrazit a zaregistrovat obchody pro příležitosti, které jsou označené jako získané a mají nárok na registraci koupě, pokud jsou členy týmu.
||    Může vytvářet a zobrazovat lístky podpory
|Správce obchodního profilu|Vytváření a Správa obchodních profilů | [Správa obchodních profilů](create-a-marketing-profile.md)
||    Může vytvářet a zobrazovat lístky podpory

Společně s novou referenční rolí uživatele zavádíme také rozsah umístění pro obchody. V tabulce níže najdete informace o přístupu na základě umístění.

|**Scope** | **Co můžete dělat** |
|------------------------------|:-------------------------|
|Celá společnost | Správci i uživatelé mají přístup k vytváření obchodů pro libovolné umístění ve své společnosti.|
|| Správce odkazů má přístup k zobrazení a úpravám všech obchodů. |
|| Uživatelé s odkazem mají přístup k zobrazení a úpravám všech obchodů pouze v případě, že jsou součástí týmu. |
|Jedno nebo více umístění | Správci i uživatelé mají přístup k vytváření obchodů pro přiřazené umístění ve společnosti.|
|| Správce odkazů má přístup, který umožňuje zobrazit a upravit všechny obchody patřící do přiřazených umístění.|
|| Příslušní uživatelé mají přístup k zobrazení a úpravám všech obchodů náležejících k přiřazeným umístěním, pokud jsou součástí týmu.|

## <a name="manage-incentives"></a>Správa pobídek

|**Role** | **Co můžete dělat**|**Další informace**
|------------------------------|:-------------------------|---|
|Motivace správce|* Iniciuje a spravuje pobídky. |[Tyto materiály vám pomůžou začít s motivací.](incentives-get-started-intro.md)
||* Může zobrazit a upravit všechny aspekty programu pobídek.
||* Může zobrazit a upravit informace o bance a daních
||* Zobrazit příjem rabatu a souběžných op
||* Podpora přístupu
||* Pobídky sporů|
|Motivace uživatelů|* Může zobrazit pobídky programů
||* Může zobrazit a iniciovat deklarace motivů.
||* Zobrazit příjem rabatu a souběžných op
||* Vytvoření lístků podpory pro partnerské Centrum
||* Zobrazit lístky podpory partnerů, které vytvoříte

## <a name="view-partner-center-insights-data"></a>Zobrazení dat služby partner Center Insights

|**Role** | **Co můžete dělat**|**Další informace**|
|------------------------------|:-------------------------|---|
|Prohlížeč sestav Executive|Přístup ke všem datovým sadám pro vytváření sestav, vytváření lístků podpory partnerů, zobrazení lístků podpory partnera, které vytvoříte|[Přehled sestav řídicích panelů dostupných ve službě partner Center – přehledy](pci-overview-report.md)
|Prohlížeč sestav|Přístup k sestavám dat s výjimkou výnosů a osobních údajů zákazníků a zaměstnanců, vytváření lístků podpory partnerů, zobrazení lístků podpory partnerů, které vytvoříte|

## <a name="next-steps"></a>Další kroky

- [Vytváření uživatelských účtů a přiřazování rolí a oprávnění](create-user-accounts-and-set-permissions.md)
- [Ověření informací o účtu při registraci do nového programu partnerského centra](verification-responses.md)
