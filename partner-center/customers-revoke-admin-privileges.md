---
title: Získání oprávnění správce zákazníka
ms.topic: how-to
ms.date: 12/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Získejte oprávnění, která potřebujete ke správě služby nebo předplatného zákazníka jejich jménem. Zjistěte, jak jsou oprávnění udělena, odvolána a spravována.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.openlocfilehash: 779e76d6bb3e8df679a5ca6fa8ce441e42529161
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147288"
---
# <a name="obtain-permissions-to-manage-a-customers-service-or-subscription"></a>Získání oprávnění ke správě služby nebo předplatného zákazníka

**Odpovídající role:** Agent pro správu | Agent prodeje

Pokud chcete spravovat služby nebo předplatné zákazníka jejich jménem, zákazník vám musí udělit oprávnění správce pro službu. Pokud chcete od zákazníka získat oprávnění správce, pošlete jim e-mail na žádost o vztah prodejce. Jakmile zákazník vaši žádost schválí, budete se moct přihlásit k portálu pro správu služby a spravovat ji jménem zákazníka. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Pozvání zákazníka k navázání vztahu prodejce s váma

1.  Vyberte **Customers (Zákazníci)** a pak **vyberte Request a reseller relationship (Požádat o vztah prodejce).**

2.  Na další stránce zkontrolujte koncept e-mailové zprávy. Koncept zprávy můžete otevřít ve výchozí e-mailové aplikaci nebo můžete zprávu zkopírovat do schránky a vložit do e-mailu. 

    >[!IMPORTANT]
    >Text e-mailu můžete upravit, ale nezapomeňte do něj zahrnout přizpůsobený odkaz, který propojí zákazníka přímo z vaším účtem. 
    
3.  Po **dokončení** tohoto kroku vyberte Hotovo.

4.  Odešlete e-mail zákazníkovi.

5.  Jakmile zákazník vaši pozvánku přijme, zobrazí  se na stránce Vašich zákazníků a vy budete moct službu pro zákazníka zřídit a spravovat odtud.

6.  Pokud chcete spravovat účet zákazníka, služby, uživatele a licence, rozbalte záznam zákazníka tak, že vyberete šipku dolů u jeho jména a pak vyberete portál pro správu služby, kterou chcete spravovat.

>[!IMPORTANT]  
>Zákazníci mohou změnit přiřazení nebo odebrání oprávnění správce na portálu pro správu služby. Musíte ale informovat zákazníka, že odebrání oprávnění správce znamená, že už nebudete moct za něj otevřít žádost o služby Microsoftu. Tyto typy žádostí o služby nebudete moct otevřít jménem zákazníka, dokud nesnídíte svou smlouvu se zákazníkem.

Vaši zákazníci na portálu pro správu Office 365 mohou zjistit, kteří z jejich partnerů mají ke svému tenantovi oprávnění správce. Použijte následující postup:

1. Zákazník se musí přihlásit k portálu pro správu Office 365 jako globální správce.

2. Vyberte **Nastavení Partnerské**  >  **vztahy.**

3. Na stránce **Vztahy s** partnery se zákazníkovi zobrazí seznam partnerů, se kterými pracují, a partnerů, kterým byla udělena delegovaná oprávnění pro správu jejich tenanta.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Zákazníci mohou spravovat delegovaná oprávnění správce partnera. 

Zákazník se může rozhodnout odebrat delegovaná oprávnění správce ze svého tenanta, ale zachovat s ním vztah pro účely prodloužení platnosti předplatného a licence. Zákazníci spravují práva a oprávnění ke svým účtům Office 365 na stránce **Vztahy** s partnery v Centru pro správu Office 365. Na této stránce mohou zákazníci:

- Podívejte se, se kterým partnerem mají vztah a kteří partneři mají delegovaná oprávnění správce.

- Odebrání delegovaných oprávnění pro správu partnera z tenanta

Odebrání delegovaných oprávnění správce od partnera:

1. Na **stránce Vztahy s** partnery vyberte partnera, který vás zajímá.
2. V podokně podrobností vyberte Odebrat **delegovaného správce.**
3. V potvrzovacím podokně vyberte **Odebrat.**

>[!IMPORTANT]  
>Přiřazení rolí Azure AD partnerovi jsou implicitní. Pokud se pokusíte zobrazit seznam členů rolí Azure AD pomocí portálu Azure AD, PowerShellu nebo Graphu, partner se vrátí. Pokud chcete zjistit, jestli jsou partneři přiřazení k rolím Azure AD, musíte na stránce Vztahy s partnery na portálu pro správu Office 365 zjistit, jestli má partner udělené delegované oprávnění pro správu.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Delegovaná oprávnění správce v Azure AD 

V tenantovi Azure AD partnera existují dvě skupiny zabezpečení, agenti pro správu a agenti helpdesku, které se používají pro delegovanou správu. Když zákazník partnerovi udělí delegovaná oprávnění pro správu:

- Skupina Agent pro správu je přiřazená k roli globálního správce v tenantovi Azure AD zákazníka.

- Skupina Agent helpdesku je přiřazená k roli Správce helpdesku v tenantovi Azure AD zákazníka.

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
