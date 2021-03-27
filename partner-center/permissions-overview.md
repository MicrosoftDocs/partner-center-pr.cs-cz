---
title: Přiřazení rolí & oprávnění uživatelům
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Seznamte se s rolemi, které jsou nejvhodnější pro uživatele vaší společnosti, kteří spravují komerční transakce, reference, pobídky nebo členství v programu MPN v partnerském centru.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperf-fy21q1
ms.openlocfilehash: a6e6424dfb787bbe9510d47299f945309dd00528
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633909"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a>Přiřazení rolí uživatelů a oprávnění pro uživatele společnosti, kteří potřebují pracovat v partnerském centru

**Příslušné role**

- Globální správce
- Správce správy uživatelů
- Správce partnera MPN

Nastavili jste svůj partnerský profil včetně právního jména a adresy, podrobností o podpoře, daňových odchylek souborů, bankovních údajů a primárního kontaktu pro vaši společnost. Další krok: Nastavte své uživatele s heslem a rolemi, aby mohli začít pracovat v partnerském centru s vámi.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Nastavení zaměstnanců pro práci v partnerském centru

Pomocí rolí a oprávnění, které přidáváte vašim uživatelům, určíte typy přístupu, které mají vaši uživatelé v partnerském centru. Role se vztahují k programům, které jsou součástí vašeho podniku. Pokud je vaše firma například podnikovým poskytovatelem Cloud Solution Provider (CSP), nebudete mít k dispozici pouze standardní role správy tenanta Azure Active Directory, jako je například globální správce, ale budou potřebovat role specifické pro program CSP. Každý program má specifické role.

>[!Note]
> Role klientů Azure Active Directory zahrnují role globálního správce, Správce uživatelů a CSP. Role adresáře mimo Azure – Active Directory jsou role, které nespravují tenanta, a zahrnují správce MPN, správce obchodních profilů, Správce odkazů, správce pro pobídku a uživatele s motivací. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Správa komerčních transakcí v partnerském centru (role Azure AD a CSP)

|**Role**|**Co můžou dělat**|**Další informace**|
|----------------------------------|---|:---------------------------------|
|Globální správce|* Má přístup ke všem službám účet Microsoft/Services s úplnými oprávněními.|[Správa účtu v Partnerském centru](partner-center-account-setup.md)
|      |* Vytvoření lístků podpory pro partnerské Centrum
||* Zobrazit lístky podpory partnerů, které vytvoříte
||* Zobrazit smlouvy, ceníky a nabídky
||* Zobrazení, vytvoření a Správa partnerských uživatelů|
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
||* Zobrazit ceny a nabídky
||* Fakturace
||* Správa jménem zákazníka
||* Zaregistrovat prodejce s přidanou hodnotou
||* Vytvoření lístků podpory pro partnerské Centrum
||* Zobrazit lístky podpory partnerů, které vytvoříte|
|Agent prodeje | * Správa zákazníků|[Poskytněte zákazníkům podporu pro fakturaci a pomůžou odpovědět na dotazy související s fakturací.](provide-billing-support.md)
||* Přidat seznam zařízení do partnerského centra
||* Správa předplatných
||* Zobrazit lístky podpory
||* Vyžádání vztahu se zákazníkem
||* Zobrazit ceny a nabídky
||* Správa potenciálních zákazníků
||* Zobrazit zákaznickou smlouvu
||* Registrace prodejce s přidanou hodnotou
||* Vytvoření lístků podpory pro partnerské Centrum
||* Zobrazit lístky podpory partnerů, které vytvoříte|
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

Tyto role nejsou Azure Active Directory rolí. Tyto role spravují firmu společnosti, nikoli tenanta.

|**Role** | **Co můžete dělat**|**Další informace**|
|----------------------------|:----------------------------|-----|
|Správce partnera MPN|* Zobrazení, vytvoření a správa žádostí o partnerských služeb|[Nákup nebo prodloužení platnosti předplatného programu Microsoft Action Pack nebo kompetencí Silver a Gold Competency](mpn-get-action-pack.md)
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
||* Přiřaďte role pro uživatele v tenantovi k rolím adresáře mimo Azure – Active Directory. 
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
