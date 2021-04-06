---
title: Konsolidace tenanta regionální autorizace CSP
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Tyto pokyny slouží ke konsolidaci klientů pro různé země nebo oblasti. Sem patří postup migrace zákaznických účtů a zákaznických předplatných.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 2171e2b10101e99bdd8d415a936ba98af65c2a1b
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502566"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>Pokyny ke konsolidaci tenantů s regionální autorizací CSP

**Platí pro**

- Partnerské centrum pro Microsoft Cloud for US Government

**Příslušné role**

- Globální správce
- Agent správce

\[Některé informace se vztahují na předem vydaný produkt, který se před prodejem z komerčního vydání může podstatně upravit. Microsoft neposkytuje žádné záruky, výslovné ani předpokládané, týkající se zde uváděných informací.\]

Můžete konsolidovat klienty pro vaši firmu. Tyto pokyny slouží ke konsolidaci klientů pro různé země nebo oblasti.

>[!NOTE]  
>Musíte být vědomi všech zřízené předplatných a počty licencí pro každého ze svých zákazníků v účtu, ze kterého provádíte převod. V rámci tohoto procesu migrace se v rámci nového účtu centrálního CSP v rámci procesu migrace znovu zřídí stejné přesně stejné odběry se stejnými počty licencí. Pomocí funkce seznam pro export můžete vytvořit seznam zákazníků pro přesun do centralizovaného tenanta.  Po dokončení konsolidace se nemůžete vrátit k předchozímu stavu tenanta. Může se také vyžadovat akce zákazníka.

## <a name="prepare-for-migration"></a>Příprava migrace

- Přihlaste se k **partnerskému centru**  pomocí **přechodu** účtu (ten, který převedete na nový účet), a Projděte si všechny zákazníky a všechny služby zřízené pro tyto zákazníky.

- Odhlaste se z tohoto účtu.

## <a name="migrate-customer-accounts"></a>Migrace zákaznických účtů

1. Přihlaste se k **partnerskému centru**  pomocí účtu **přechodu** (nového) (ten, na který přecházíte zákazníky).

2. Vyberte **Zákazníci**.

3. Vyberte **požádat o vztah prodejce**. Zobrazí se výchozí e-mailová zpráva, která se odešle vašim zákazníkům. Tato zpráva obsahuje adresu URL s ID organizace, které je pro nový účet partnerského centra jedinečné.

4. **Akce zákazníka:** Ujistěte se, že každý z aktivních zákazníků, které chcete migrovat, navštíví tuto adresu URL. Při otevření adresy URL se zobrazí výzva, abyste se přihlásili na portál Office 365. Zákazník se přihlásí pomocí stejného ID organizace, které používají pro přístup k portálům pro správu Azure a Office 365.

5. Po přihlášení se globální správce pro **účet zákazníka** vyzve k odeslání smlouvy, která poskytuje oprávnění delegovaného správce k novému účtu CSP. Pokud souhlasí, zákazník vybere zaškrtávací políčko a souhlasí s autorizací vztahu.

Zákazníci se zobrazí v seznamu zákazníků partnera po odeslání smlouvy, jednu po jednu.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Migrace předplatných na základě využití pro Office 365 a jiné než Azure

1. Jakmile zákazník smlouvu podepíše, můžete znovu vytvořit své odběry v rámci centralizovaného partnerského tenanta.

2. Z **partnerského centra** vyberte **zákazníci**.

3. Otevřete název společnosti pro zákazníka, kterého chcete migrovat.

4. Vyberte **přidat odběr**.

5. Přidejte správné předplatné a počty licencí z katalogu. Ověřte s informacemi, které jsou k dispozici v **přechodu z** partnerských účtů.

   :::image type="content" source="images/regionalcustomer2.png" alt-text="seznam zákazníků":::

6. Vyberte **Odeslat.**

   Služby jsou nyní poskytovány zákazníkovi z **přechodu na** Partnerský účet.

7. Zopakováním těchto kroků migrujte odběry pro všechny další zákazníky.

Než budete pokračovat k další části, ujistěte se, že všechna předplatná zákazníka existující v rámci **přechodu z** partnerských účtů jsou znovu zřízena v rámci **přechodu na** Partnerský účet.

> [!NOTE]
> Partneři musí pozastavit odběry při **přechodu z** účtu partnerského tenanta v partnerském centru, a to za stejný den, kdy se tato předplatná přecházejí a nastavují v rámci **přechodu na** účet partnerského tenanta v partnerském centru, aby se zajistilo dvojí vyúčtování. Žádosti o podporu budou odepřeny pro kredity z důvodu překrytí při fakturaci, ke kterému dojde z nesprávného zákazu **přechodu z** předplatných.

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Zakázání předplatných Office 365 v rámci přechodu z partnerského účtu

Zakázáním předplatného CSP v rámci **přechodu z** partnerských účtů zastavíte jakoukoli budoucí fakturaci. Nemusíte ručně zakázat předplatná Azure, protože předplatná Azure se během procesu migrace automaticky vypnou.

1. Přihlaste se k **partnerskému centru** pomocí **přechodu z** účtu CSP a přejděte do seznamu zákazníků.

2. Otevřete zákazníka s předplatnými, které chcete zakázat, a pak vyberte první nabídku, kterou chcete zakázat.

3. Nastavte předplatné na **pozastaveno** a pak vyberte **Odeslat**.

   >[!Note]
   >Pozastavení předplatného zajistí, že nedojde k dvojímu vyúčtování.

   V seznamu předplatných se zobrazí **pozastavené** předplatné.

4. Tento postup opakujte pro všechna předplatná v rámci zákazníka. Ověřte, že je **pozastavená** všechna zobrazení.

5. Vyberte dalšího zákazníka v seznamu a opakujte postup zakázání všech předplatných.

## <a name="migrating-azure-usage-based-subscriptions"></a>Migrace předplatných na základě využití Azure

Na rozdíl od předplatných CSP pro Office 365 se nemusíte migrovat ručně pomocí Azure, předplatných CSP na základě využití. Služba Microsoft Azure Support migruje předplatná Azure a všechny nasazené služby nebo prostředky z **přechodu z** účtů prodejců CSP na **převod na** účet prodejce CSP. Během tohoto přechodu nebudete mít k dispozici žádné přerušení služby pro zákazníka.

1. Ujistěte se, že účty zákazníků, které budou mít migrované předplatné Azure, přijaly smlouvu, která bude přidružená k novému **přechodu na** účet CSP.

2. Budete upozorněni na to, kteří zákaznické účty budou připravené k migraci, a poskytnout jim názvy společností.

3. Microsoft migruje předplatné založené na využití Azure a upozorní vás, až se migrace dokončí.

4. Musíte potvrdit, že předplatné Azure v rámci **přechodu z** účtu zprostředkovatele CSP je teď označené jako **pozastavené** v partnerském centru v části Předplatná zákazníka.

5. Potvrďte, že předplatné Azure v rámci **přechodu na** účet poskytovatele CSP teď zobrazuje stav **aktivní** v partnerském centru v části Předplatná zákazníka.

   >[!Note]
   > Zakázáním předplatných v rámci zákazníka se nezmění vzhled zákazníka v seznamu zákazníků. V tuto chvíli není k dispozici možnost odebrat zákazníky ze seznamu. Partneři by se měli vyhnout přidání předplatného zpátky těmto zákazníkům ze svých **přechodů z** účtu v budoucnu.

6. Opakujte tyto kroky u všech předplatných ve všech vašich zákaznících, abyste zastavili budoucí poplatky za **Převod z** účtů. Partner dostane jednu konečnou fakturu s kreditem na počet nevyužitých dní mezi dnem zrušení a posledním dnem fakturačního období. Po uplynutí tohoto finálního fakturačního období nebudou vygenerovány žádné budoucí faktury.

### <a name="additional-information"></a>Další informace

- Zakázání předplatného z **převodu z** účtu CSP nemá vliv na službu koncového zákazníka, pokud byla služba zřízená z **přechodu na** účet CSP před zakázáním předplatného.

- Předplatná nelze použít u zákazníka a při pozastavení nebo zrušení negeneruje poplatky.

- V současné době neexistuje způsob, jak úplně odebrat zákazníka ze seznamu **zákazníků** .
- 
    >[!Note]
    > Partneři musí pozastavit odběry při **přechodu z** účtu partnerského tenanta v partnerském centru. stejný den jsou tato předplatná přepnuta do a nastavena v rámci **přechodu na** účet, aby se zajistilo dvojí vyúčtování. Společnost Microsoft nebude podporovat žádosti o kredity z důvodu překrytí při fakturaci, ke kterému dojde z nesprávného nastavení **přechodu z** předplatných na pozastaveno.

### <a name="simplify-migration-using-export"></a>Zjednodušení migrace pomocí exportu

Pomocí **funkce exportu** můžete zachytit odběry, které je třeba použít v nové konsolidované struktuře:

1. Pokud chcete zobrazit seznam zákazníků, vyberte **zákazníky** v partnerském centru. 

2. Otevřete požadované jméno zákazníka.

3. Na stránce **předplatná** vyberte **exportovat odběry** a exportujte tak podrobnosti předplatných do excelového souboru.

4. Pomocí tohoto seznamu můžete znovu vytvořit odběry ve vašem novém konsolidovaném tenantovi.

### <a name="api-registration"></a>Registrace rozhraní API

Další informace o registraci rozhraní API najdete v tématu [nastavení přístupu k rozhraní API v partnerském centru](/partner-center/develop/set-up-api-access-in-partner-center).

## <a name="next-steps"></a>Další kroky

- [Poskytovatel řešení cloudu a místní trhy a měny, kde můžete prodávat nabídky CSP](regional-authorization-overview.md)
