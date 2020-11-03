---
title: Získání oprávnění správce pro zákazníka
ms.topic: how-to
ms.date: 06/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Získejte oprávnění, která potřebujete ke správě služby nebo předplatného zákazníka jménem uživatele. Přečtěte si, jak se udělují, odvolají a spravují oprávnění.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.openlocfilehash: dcfc552016560ecc3167deebf96f7a75a72048bc
ms.sourcegitcommit: 8dc139749916c822c5c438f54a03d2f147697dd5
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/04/2020
ms.locfileid: "92527121"
---
# <a name="obtain-permissions-to-manage-a-customers-service-or-subscription"></a>Získejte oprávnění ke správě služby nebo předplatného zákazníka.

**Platí pro**

- Partnerské centrum

**Příslušné role**

- Agent správce
- Agent prodeje

Pokud chcete spravovat službu nebo předplatné zákazníka jménem uživatele, musí vám udělit oprávnění správce této služby. Pokud chcete získat oprávnění správce od zákazníka, pošlete mu e-mail s žádostí o vztah prodejce. Jakmile zákazník vaši žádost schválí, budete se moct přihlásit k portálu pro správu služby a spravovat službu jménem zákazníka. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Pozvání zákazníka k navázání vztahu prodejce s vámi

1.  Vyberte **zákazníci** a potom zvolte **požádat o vztah prodejce** .

2.  Na další stránce zkontrolujte koncept e-mailové zprávy. Koncept zprávy můžete otevřít ve výchozí e-mailové aplikaci nebo můžete zprávu zkopírovat do schránky a vložit do e-mailu. 

    >[!IMPORTANT]
    >Text e-mailu můžete upravit, ale nezapomeňte do něj zahrnout přizpůsobený odkaz, který propojí zákazníka přímo z vaším účtem. 
    
3.  Po dokončení tohoto kroku vyberte **Hotovo** .

4.  Odešlete e-mail zákazníkovi.

5.  Jakmile zákazník vaši pozvánku přijme, zobrazí se na stránce vaši **zákazníci** a vy budete moci zřídit a spravovat službu pro zákazníka.

6.  Pokud chcete spravovat účet, služby, uživatele a licence zákazníka, rozbalte záznam zákazníka tak, že vyberete šipku dolů vedle svého jména a pak vyberete portál pro správu služby, kterou chcete spravovat.

>[!IMPORTANT]  
>Zákazníci můžou na portálu pro správu služby změnit přiřazení nebo odebrání oprávnění správce. Nicméně pokud a dokud neprovedete znovu vyjednávání vaší smlouvy se zákazníkem, budete mít i nadále odpovědnost za poskytování zákaznické podpory a dodržování podmínek smlouvy pro prodejce v cloudu, a to i když zákazník znovu přiřadí nebo odebere oprávnění správce. V takové situaci, pokud zákazník vyžaduje pomoc, požádejte podporu Microsoftu o otevření žádosti o služby jménem zákazníka.

Vaši zákazníci si můžou zjistit, kteří z jejich partnerů mají oprávnění správce ke svému tenantovi z portálu pro správu Office 365. Použijte následující postup:

1. Zákazník se musí přihlásit k portálu pro správu Office 365 jako globální správce.

2. Vyberte **Nastavení**  >  **partnerské vztahy** .

3. Na stránce **partnerské vztahy** se zobrazí zákazník se seznamem partnerů, se kterými pracují, a s uživateli, kterým byla udělena oprávnění delegovaná Správa ke svému tenantovi.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Zákazníci můžou spravovat oprávnění delegovaného správce partnera. 

Zákazník se může rozhodnout odebrat vaše delegovaná oprávnění správce ze svého tenanta, ale zachovat vztah s vámi pro účely obnovení předplatného a licence. Zákazníci spravují práva a oprávnění ke svým účtům Office 365 na stránce **partnerské vztahy** v centru pro správu sady Office 365. Na této stránce můžou zákazníci:

- Podívejte se, kteří partneři mají relaci s a kteří partneři mají delegovaná oprávnění správce.

- Odebrání oprávnění delegované správy partnera z tenanta

Odebrání oprávnění delegované správy z partnera:

1. Na stránce **partnerské vztahy** vyberte partnera, který vás zajímá.
2. V podokně podrobností vyberte **Odebrat delegovaného správce** .
3. V podokně potvrzení vyberte **Odebrat** .

>[!IMPORTANT]  
>Přiřazení rolí Azure AD k partnerovi jsou implicitní. Pokud se pokusíte zobrazit seznam členů rolí Azure AD pomocí portálu Azure AD nebo PowerShellu nebo grafu, partner se nevrátí. Pokud chcete zjistit, jestli se partneři přiřazují k rolím Azure AD, musíte na stránce partnerské vztahy na portálu pro správu Office 365 zjistit, jestli je partnerovi udělené oprávnění k delegované správě.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Delegovaná oprávnění správce v Azure AD 

Existují dvě skupiny zabezpečení, agenti správců a agenti helpdesku v tenantovi Azure AD partnera, kteří se používají pro delegovanou správu. Když zákazník udělí partnerovi oprávnění k delegované správě:

- Skupina agentů pro správu je přiřazená k roli globálního správce v tenantovi Azure AD zákazníka.

- Skupina agentů helpdesku je přiřazená k roli správce helpdesku v tenantovi Azure AD zákazníka.

Na základě přiřazených rolí adresáře se můžou členové obou skupin přihlásit ke klientovi Azure AD a službám O365 pomocí svých partnerských přihlašovacích údajů a správce jménem zákazníka.

Pokud zákazník odebere delegovaná oprávnění správce, odeberou se přiřazení rolí Azure AD a nebudete už moct spravovat tenanta Azure AD zákazníka.

### <a name="azure-subscriptions-and-resource-management"></a>Předplatná Azure a Správa prostředků

Každé předplatné Azure má svou vlastní sadu rolí správy prostředků. Předtím, než může partner CSP spravovat předplatné Azure zákazníka, musí být tento partner přiřazený k jedné nebo více rolím v rámci předplatného Azure. Konkrétně se jedná o tyto:

- Když zákazník přijme pozvánku pro prodejce a udělí partnerovi oprávnění k delegované správě, partner automaticky nezíská přístup ke stávajícím předplatným Azure v rámci tenanta zákazníka.

- Když partner CSP zřídí pro zákazníka nové předplatné Azure, v rámci tohoto předplatného je automaticky přiřazená skupina agenti pro správu v rámci partnerského tenanta CSP. Na základě přiřazení role můžou členové skupiny přistupovat k prostředkům v rámci předplatného a spravovat je.

- Když zákazník odebere delegovaná oprávnění pro správu z partnera pomocí portálu Office 365, partner stále může spravovat předplatné Azure, pokud je partner pořád přiřazený k jedné nebo více rolím v rámci předplatného. Aby bylo možné zastavit partnera se správou předplatného Azure, zákazník musí přiřazení role odebrat.

## <a name="windows-autopilot"></a>Windows Autopilot

V partnerském centru můžou partneři CSP spravovat profily autopilotu pro zákazníky bez delegovaných oprávnění správce za těchto okolností: 

- Pokud zákazník odebere delegovaná oprávnění pro správu, ale zachová s vámi vztah prodejce, můžete pro ně nadále spravovat profily autopilotu.

- Můžete spravovat zákaznická zařízení, která jste vy nebo jiný partner přidali. 

- Nemůžete spravovat zařízení, která zákazník přidal prostřednictvím Microsoft Store pro firmy, Microsoft Store pro vzdělávání nebo Microsoft Intune Portal.

Další informace o autopilotu najdete v tématu [zjednodušení nastavení zařízení pomocí technologie Windows autopilot](autopilot.md).

>[!IMPORTANT]  
>Aktuální prostředí pro správu autopilotu v partnerském centru se může i nadále měnit. V době publikování tohoto článku jsou zváženy tyto změny:

- Partnerovi musí být udělené oprávnění k delegované správě, než může partner Přidat/aktualizovat/odebrat profily a použít nebo odebrat profil z libovolného zařízení v tenantovi zákazníka.

- Partnerovi musí být udělené oprávnění k delegované správě, než může partner odebrat zařízení, která přidali jiní partneři nebo zákazník v tenantovi zákazníka. V opačném případě může partner odebrat jenom zařízení, která dřív přidal stejný partner.
