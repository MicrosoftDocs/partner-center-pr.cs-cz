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
ms.openlocfilehash: d2168dcd60b8675a21960918dab49b778025fa51
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147577"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>Pokyny ke konsolidaci tenantů s regionální autorizací CSP

**Platí pro**: partnerské Centrum | Partnerské centrum pro Microsoft Cloud pro státní správu USA

**Příslušné role**: globální správce | Agent správce

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

4. **Akce zákazníka:** Ujistěte se, že každý aktivní zákazník, kterého chcete migrovat, navštíví tuto adresu URL. Při otevírání adresy URL se zákazníkovi zobrazí výzva k přihlášení k portálu Office 365. Zákazník se přihlásí pomocí stejného ID organizace, které používá pro přístup k portálům pro správu Azure a Office 365.

5. Po přihlášení se globálnímu  správci zákaznického účtu zobrazí výzva k odeslání smlouvy, která novému účtu CSP uděluje delegovaná oprávnění správce. Pokud zákazník souhlasí, zaškrtne políčko a souhlasí s autorizací relace.

Zákazníci se po jednom odeslaní smlouvy zobrazí v seznamu zákazníků partnera.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Migrace předplatných Office 365 a předplatných jiných než Azure založených na využití

1. Jakmile zákazník smlouvu podepíše, můžete znovu vytvořit jeho předplatná v rámci centralizovaného partnerského tenanta.

2. V **Partnerské centrum** vyberte **Zákazníci.**

3. Otevřete název společnosti zákazníka, kterého chcete migrovat.

4. Vyberte **Přidat předplatné.**

5. Přidejte správná předplatná a počty licencí z katalogu. Ověřte pomocí informací uvedených v části **Přechod z partnerských** účtů.

   :::image type="content" source="images/regionalcustomer2.png" alt-text="seznam zákazníků":::

6. Vyberte **Odeslat.**

   Služby se teď zákazníkům poskytují z účtu **přechodu na** partnerský účet.

7. Opakováním těchto kroků migrujte předplatná pro všechny další zákazníky.

Než budete pokračovat k další části, ujistěte  se, že všechna zákaznická předplatná v části Přechod z partnerských účtů se znovu zř zda jsou v rámci účtu Přechod **na** partnera znovu zřízena.

> [!NOTE]
> Partneři musí pozastavit  předplatná na účtu přechodu z partnerského tenanta v Partnerské centrum Partnerské centrum stejný  den, kdy se tato předplatná přenesou Partnerské centrum nastaví v rámci účtu přechodu na partnerského tenanta v Partnerské centrum, aby se zajistilo, že nedojde k dvojí fakturaci. Žádosti o podporu budou odepřeny pro kredity z důvodu překrytí při fakturaci, ke kterému dojde z nesprávného zákazu **přechodu z** předplatných.

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

4. Musíte potvrdit, že předplatné Azure v účtu prodejce Přechod  z **CSP** je teď označené jako pozastavené v Partnerské centrum v části Předplatná zákazníka.

5. Ověřte, že předplatné Azure v **rámci** účtu prodejce Přechod  na CSP teď zobrazuje stav aktivní v Partnerské centrum v části Předplatná zákazníků.

   >[!Note]
   > Zakázáním předplatných v rámci zákazníka se nezmění vzhled zákazníka v seznamu Zákazníci. V současné době není možné odebrat zákazníky ze seznamu. Partneři by se měli těmto zákazníkům v budoucnu vyhnout přidávání předplatných z **účtu,** který přechází z tohoto účtu.

6. Opakujte tento postup pro všechna předplatná v rámci všech vašich zákazníků, abyste zastavili budoucí poplatky na účtech **přechodu** z účtu nebo účtů. Partner obdrží jednu konečnou fakturu s kreditem na počet nevyužitých dnů mezi dnem zrušení a posledním dnem fakturačního období. Po tomto konečném fakturačním období se nebudou generovat žádné budoucí faktury.

### <a name="additional-information"></a>Další informace

- Zakázání předplatného z účtu Přechod z **CSP** nemá vliv na službu koncového zákazníka, pokud byla služba zřízena z účtu Přechod na **CSP** před zakázáním předplatného.

- Předplatná nemůže zákazník používat a po pozastavení nebo zrušení negenerují poplatky.

- V současné době neexistuje způsob, jak zákazníka ze seznamu Zákazníků úplně **odebrat.**
- 
    >[!Note]
    > Partneři musí pozastavit  předplatná na účtu tenanta přechodu z partnerského účtu Partnerské centrum ve stejný  den, kdy se tato předplatná přenesou na účet Přechod na Partnerské centrum nastaví je, aby se zajistilo, že nedojde k dvojí fakturaci. Microsoft nebude podporovat žádosti o kredity kvůli překrývání fakturace způsobené tím, že správně nenastaví přechod z **předplatných** na pozastavené.

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
