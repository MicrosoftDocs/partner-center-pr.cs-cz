---
title: Hlášení problémů jménem zákazníka
ms.topic: how-to
ms.date: 02/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, kdy předáte microsoftu problém se službou zákazníkům a jak vyřešit lístek podpory pro různé typy služby Microsoft.
author: Kim-Davis
ms.author: kimnich
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6ba25d0bfc4796ca43d36bb34bf6d9e82889881c
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855705"
---
# <a name="report-a-service-problem-on-behalf-of-a-customer---including-when-and-how-to-do-so"></a>Nahlášení problému se službou jménem zákazníka – včetně toho, kdy a jak to udělat

**Platí pro**: Partnerské centrum | Partnerské centrum pro Microsoft Cloud for US Government

**Odpovídající role:** Globální správce

Pokud u zákazníka dochází k problému se službou, který nemůžete vyřešit a který splňuje kritéria popsaná v části Eskalace problémů [do Microsoftu,](escalate-problems-to-microsoft.md)může za ně váš nepřímý poskytovatel vytvořit lístek podpory. Tento proces je také užitečný pro eskalaci problémů s fakturací nebo sporů a pro problémy s podvody.

## <a name="submit-a-service-request-for-a-customer"></a>Odeslání žádosti o služby pro zákazníka

1. V nabídce Partnerské centrum v části CSP vyberte **Zákazníci.**

2. Na stránce Zákazníci vyberte nebo vyhledejte zákazníka, kterého chcete.
    
3. V nabídce zákazníka vyberte Žádosti **o služby.**

4. V rozevírací **nabídce Nový** požadavek vyberte **Azure** nebo **Office 365, Dynamics 365, Enterprise Mobility Suite.** Budete přesměrováni do centra pro správu portál Microsoft Azure Office 365.

>[!NOTE]
>Partneři operací podpory, kteří provádí transakce s Dynamics 365 v CSP, musí udržovat smlouvu o podpoře s plánem rozšířené podpory pro partnery (ASfP) nebo vyšším. Tato smlouva o podpoře se vyžaduje k odesílání incidentů Dynamics 365 jménem zákazníka CSP. [Přečtěte si](https://partner.microsoft.com/support/partnersupport) další informace o možnostech smlouvy o podpoře.

### <a name="microsoft-azure"></a>Microsoft Azure

> [!IMPORTANT]
> Pokud potřebujete vytvořit žádost o služby pro zákazníka v Azure, uvědomte si následující:
>
>- Abyste jako nepřímý prodejce mohli vytvářet žádosti o služby pro zákazníka v Azure, musí vám nepřímý poskytovatel udělit přístup k účtu Azure zákazníka. To se liší od správy jménem zákazníků pro Office 365.
>
>- I když správce helpdesku v partnerském centru nemůže vytvářet žádosti o služby na portálu Azure Service, co můžou udělat, je vytvořit skupinu podpory na portálu Azure Service a dát této skupině oprávnění protokolovat požadavky na podporu.

1. Vyberte **Nová žádost o podporu**.

2. Do žádosti o podporu zadejte příslušné informace a pak vyberte **vytvořit**:

   - V části **základy** žádosti o podporu nezapomeňte vybrat **Cloud Solution Provider** v poli **plán podpory** .

   - V části **kontaktní** informace v žádosti o podporu zadejte svoje informace, ne informace o vašem zákazníkovi.

3. Později zkontrolujte žádosti o služby zákazníka v rámci portál Microsoft Azure tím, že vyberete **Spravovat žádosti o podporu**.

Možná budete muset vytvořit žádost o podporu pro zákazníka, pokud nemáte oprávnění správce pro daného zákazníka. K tomu může dojít v jednom ze dvou scénářů:

- Při prvním navázání relace jste nepožádali o oprávnění správce.
- Můžete spravovat jenom předplatná Azure zákazníka, takže nemáte oprávnění správce.
 
V obou těchto případech můžete k vytvoření žádosti o podporu použít následující postup. 

1. Zkopírujte název domény zákazníka ze stránky svého účtu v partnerském centru.

2. Přejít na https://portal.azure.com/ [customerdomainname]. 

3. Vyberte předplatné Azure, které vyžaduje podporu.

4. Vyberte **Nová žádost o podporu** a pak podle pokynů vytvořte žádost. 

 
### <a name="office-365-microsoft-dynamics-crm-online-enterprise-mobility-suite"></a>Office 365, Microsoft Dynamics CRM Online, Enterprise Mobility Suite

1. V části **vytvořit žádost o službu** vyberte příslušnou kategorii podpory. Možná budete muset vybrat **více...** a zobrazit další články.

2. Dokončete formulář žádosti o službu a vyberte **Odeslat**.

   > [!TIP]
   > Ujistěte se, že jste zahrnuli vaše kontaktní údaje, ne váš zákazník.

3. Později zkontrolujte žádosti o služby zákazníka tak, že přejděte do centra pro správu Office 365 a vyberte **Zobrazit všechny lístky podpory**.

### <a name="support-for-commercial-marketplace-products"></a>Podpora produktů komerčního marketplace

Microsoft neposkytuje podporu produktů na komerčním marketplace. Pokud chcete získat podporu, budete muset kontaktovat nezávislého výrobce softwaru (ISV), který produkt publikoval.

Kontaktní informace tohoto isv:

1.  Na stránce **Marketplace** vyberte produkt, se který potřebujete pomoct.

2.  Na stránce produktu najdete kontaktní údaje podpory. Může to být jedna nebo více z následujících možností:

    - Odkaz na vstupní bod podpory na webu isv
    - E-mail podpory
    - Telefonní číslo kontaktu podpory

## <a name="faq"></a>Časté otázky

Podívejte se na následující nejčastější dotazy týkající se žádostí o služby, které můžete odeslat jménem zákazníka. 

### <a name="what-is-included-as-part-of-the-support-entitlement"></a>Co je součástí nároku na podporu?

Žádosti o služby by se měly za Partnerské centrum. Jsou k dispozici pro Azure, systém Microsoft Office 365, Microsoft Dynamics CRM Online a Enterprise Mobility Suite. Jako partner zapojený do Cloud Solution Provider můžete očekávat prioritní dobu odezvy na vaše hlavní problémy.

Podpora vlastního partnerského tenanta není součástí výhody podpory CSP. Office 365, Microsoft Dynamics CRM Online a Enterprise Mobility Suite ale neúčtují partnerům nebo zákazníkům samostatný poplatek za předplatné podpory. Azure účtuje poplatek, ale pokud máte nárok na Signature Cloud Support nebo jiné výhody Microsoft Partner Network (MPN), můžete tyto výhody využít k platbě tohoto poplatku.

Tato výhoda se vztahuje na všechny partnery účastnící se Cloud Solution Provider programu, ať už placené nebo ve zkušebním období. Podpora fakturace a správy předplatných je také součástí bezplatné součásti tohoto balíčku.

### <a name="how-quickly-will-i-get-an-initial-response"></a>Jak rychle získám počáteční odpověď?

Naše doby první odezvy závisí na závažnosti odeslaného incidentu. Závažnost problému je dána označením dopadu na firmu při odeslání žádosti o služby.

Doby první odezvy pro **incidenty s technickým poškozením**:

- Kritický dopad (závažnost A): dvě hodiny (významné ztráty nebo snížení úrovně služeb. Provozní služby.)
- Střední dopad (závažnost B): čtyři hodiny (mírné ztráty nebo snížení úrovně služeb. Provozní služby byly částečně ovlivněny.)
- Minimální dopad (závažnost C): osm hodin (minimální ztráta nebo snížení úrovně služeb. Služby, které jsou stále dostupné nebo které neprodukční služby ovlivnily.)

Doba první odezvy je jenom pro podporu pro anglicky hovořící. Podpora místních jazyků se poskytuje během pracovní doby.
U incidentů spadajících do hranice nároků na podporu, ale nepovažují se za incidenty opravy, může být doba první odezvy až jeden pracovní den.

### <a name="can-i-submit-a-service-request-by-phone"></a>Můžu žádost o služby odeslat telefonicky?

Ne, telefonická podpora není k dispozici pro tento program.

### <a name="what-happens-if-i-sign-into-the-azure-portal-and-bypass-partner-center"></a>Co se stane, když se přihlásím partnerskému centru Azure Portal a obejít?

Pokud se přihlašujete k portál Microsoft Azure přímo, prohlížíte si střed ve vlastním kontextu, nikoli v kontextu zákazníka. To je důvod, proč byste měli při vytváření žádosti o služby pro vlastní odběry přihlašovat jenom přímo do portál Microsoft Azure.

Vaše nároky na podporu vašeho programu CSP neposkytují podporu vašeho vlastního předplatného partnera. Z tohoto důvodu musíte při vytváření žádosti o služby, která se týká vašeho vlastního předplatného partnera, zadat svůj platný nárok na plán podpory. Mezi příklady patří ID smlouvy MPN, Premier nebo podpora Azure plán. Další informace najdete v [nejčastějších dotazech Podpora Azure dotazy.](https://go.microsoft.com/fwlink/?LinkId=717532)

### <a name="what-happens-if-i-sign-into-the-office-365-admin-center-portal-and-bypass-partner-center"></a>Co se stane, když se přihlásím k portálu Centra pro správu Office 365 a vynechu Partnerské centrum?

Pokud se přihlásíte přímo do Centra pro správu Office 365, díváte se na centrum ve vlastním kontextu, nikoli v kontextu zákazníka. Proto byste se měli k centru pro správu Office 365 přihlašovat jenom přímo při vytváření žádosti o služby pro vlastní předplatná.

### <a name="how-do-i-get-additional-dynamics-365-support"></a>Návody další podporu Dynamics 365?

Pokud máte problémy související s předplatným plánu Dynamics 365, licencování, fakturací, financem & Operations, licencemi produktů Dynamics 365 nebo potřebujete další technickou podporu:
 
Kontaktujte [podporu Dynamics.](/dynamics365/customer-engagement/admin/contact-technical-support)

## <a name="next-steps"></a>Další kroky

- [Zajištění podpory pro zákazníky](customer-support.md)
- [Kontrola stavu služeb](check-service-health.md)
