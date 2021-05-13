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
ms.openlocfilehash: b1ac34bbb92d600805465ca5f6d1b28af54cd5e1
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855127"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a>Přiřaďte uživatelům role a oprávnění pro firemní uživatele, kteří potřebují pracovat v Partnerské centrum

**Odpovídající role:** Globální správce | Správce správy uživatelů | Správce partnera MPN

Nastavili jste profil partnera, včetně oficiálního jména a adresy, podrobností o podpoře, osvobození od daně ze souborů, bankovních údajů a primárního kontaktu vaší společnosti. Další krok: Nastavení hesel a rolí pro uživatele, aby s Partnerské centrum mohli začít pracovat.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Nastavení zaměstnanců pro práci v Partnerské centrum

Určíte typy přístupu, které vaši uživatelé musí Partnerské centrum rolemi a oprávněními, které jim poskytnete. Role souvisejí s programy, do které se vaše firma podílí. Pokud je například vaše firma podnikem Cloud Solution Provider (CSP), budete mít nejen standardní role správy tenantů Azure Active Directory, jako je globální správce, ale budete potřebovat role specifické pro program CSP. Každý program má role, které jsou pro něj specifické.

>[!Note]
> Azure Active Directory tenanta zahrnují role globálního správce, správce uživatelů a CSP. Role mimo Azure-Active-Directory jsou role, které tenanta nespravuje, a zahrnují správce MPN, správce obchodního profilu, správce referenčních seznamu, správce pobídek a uživatele pobídek. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Správa komerčních transakcí v Partnerské centrum (role Azure AD a CSP)

|**Role**|**Co mohou dělat**|**Další informace**|
|----------------------------------|---|:---------------------------------|
|Globální správce|* Má přístup ke všem účet Microsoft nebo službám s úplnými oprávněními.|[Správa účtu v Partnerském centru](partner-center-account-setup.md)
|      |* Vytvoření lístků podpory pro Partnerské centrum
||* Zobrazit lístky podpory pro partnery, které vytvoříte
||* Zobrazení smluv, ceníků a nabídek
||* Zobrazení, vytváření a správa partnerských uživatelů|
||  Zobrazení, vytvoření a správa fakturace, faktur a souborů rekognoskaci
|Správce správy uživatelů   | * Zobrazení, vytvoření a Správa uživatelů|[Správa výhod a nabídek členství v Microsoft Partner Network v partnerském centru](manage-your-partner-network-benefits.md)
||* Zobrazit všechny profily partnerů
||* Vytvoření lístků podpory pro partnerské Centrum
||* Zobrazit lístky podpory partnerů, které vytvoříte
|Správce fakturace | – Zobrazení, vytvoření a správa fakturace, faktur a souborů rekognoskaci|[Čtení informací na faktuře](billing.md)
||* Zobrazit ceny
||* Vytvoření lístků podpory pro partnerské Centrum
||* Zobrazit lístky podpory partnerů, které vytvoříte
|Výchozí uživatel|  Zobrazit můj profil   |[Resetování hesla](reset-my-pasword.md)
|Agent správce | * Správa zákazníků|[Spojení se zákazníky](connect-with-your-customers.md)
||* Přidat seznam zařízení do partnerského centra
||* Vytvoření a použití profilů pro zařízení
||* Správa předplatných
||* Požadavky na stav služby a služby pro zákazníky
||* Požádejte o oprávnění delegovaného správce.
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
|Agent helpdesku| * Vyhledat a zobrazit zákazníka|[Eskalace problémů společnosti Microsoft a zjištění, které problémy mají větší předpoklady pro eskalaci Microsoftu](escalate-problems-to-microsoft.md)
||* Upravit podrobnosti o zákazníkovi
||* Pomůžou vyřešit problémy zákazníků pomocí fakturace nebo správy předplatných.
||* Požádat o podporu jménem zákazníků 
||* Správa předplatných a fakturačních problémů jménem zákazníků
||* Vytvoření lístků podpory pro partnerské Centrum
||* Zobrazit lístky podpory partnerů, které vytvoříte| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a>Dodavatel ovládacího panelu (CPV). (Role CSP a role mimo Azure AD)

CPVs vyvíjet aplikace pro použití partnery CSP (Cloud Solution Provider), aby jim umožnily integraci svých systémů s rozhraními API partnerského centra. 

|**Role**   |**Co můžete dělat**|**Další informace**|
|------------------------------|:----------------------------|----|
|Globální správce| Umožňuje zobrazit a spravovat váš profil CPV.|[Zaregistrovat jako dodavatele ovládacích panelů, který umožňuje integrovat partnerské systémy CSP s rozhraními API partnerského centra](enroll-as-cpv.md)
||Umožňuje zobrazit a spravovat všechny uživatele, kteří potřebují přístup k možnostem CPV.|

### <a name="guest-user-must-be-added-to-the-azure-active-directory-tenant"></a>Uživatel typu Host (musí být přidán do tenanta Azure Active Directory)

|**Uživatel typu Host**   | **Role**|
|---------------------------|:--------------------|
||Správce partnera MPN|
||Správce obchodního profilu|
||Správce odkazů|


## <a name="manage-mpn-membership-and-your-company"></a>Spravovat členství v programu MPN a vaši společnost 

Tyto role nejsou Azure Active Directory role. Tyto role spravují podnik společnosti, nikoli tenanta.

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
||* Přiřaďte role uživatelům v tenantovi k rolím mimo Azure-Active-Directory. 
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

Společně s novou referenční rolí uživatele zavádíme také rozsah umístění pro obchody. Následující tabulka vysvětluje přístup k obchodům na základě umístění.

|**Scope** | **Co můžete dělat** |
|------------------------------|:-------------------------|
|Celá společnost | Správci i uživatelé mají přístup k vytváření dohod pro libovolnou lokalitu ve své společnosti.|
|| Správce referenčních seznamu má přístup k zobrazení a úpravám všech dohod. |
|| Uživatelé referenčních seznamu mají přístup k zobrazení a úpravě všech dohod jenom v případě, že jsou součástí týmu. |
|Jedno nebo více umístění | Správci i uživatelé mají přístup k vytváření dohod pro přiřazenou lokalitu ve své společnosti.|
|| Správce referenčních seznamu má přístup k zobrazení a úpravě všech dohod, které patří do přiřazených umístění.|
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
