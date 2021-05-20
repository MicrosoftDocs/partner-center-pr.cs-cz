---
title: Migrace z PMC na Partnerské centrum
ms.topic: article
ms.date: 10/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak migrovat společnost z Partner Membership Center (PMC) do Partnerské centrum, včetně kroků, které je potřeba provést.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 511612042f7da5e43d045d2991fa7d5251612726
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150739"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>Příručka k migraci z PMC na Partnerské centrum

**Odpovídající role:** Globální správce

Partnerský web Microsoftu v partner.microsoft.com je jednotné digitální prostředí pro partnery. Na partnerském webu budete moct prozkoumat své příležitosti a zapojit se do prostředí s průvodcem, která vaší společnosti pomůžou vytvářet a prodávat vaše aplikace a služby s Microsoftem. Pomocí odkazu Řídicí panel, který je k dispozici na webu partnera, se členové Microsoft Partner Network mohou přihlásit k Partnerskému centru, kde spravujete svůj vztah s Microsoftem, zaregistrovat se v programech a zaregistrovat nabídky.

Partner Membership Center (PMC) vyřazována z provozu. Vaše společnost byla pozvána k převodu správy Microsoft Partner Network členství na Partnerské centrum. Tato příručka vás připraví na to, co můžete očekávat při přechodu z PMC na Partnerské centrum.

>[!NOTE]
>I když má vaše společnost více než jeden účet nebo umístění, přechod na Partnerské centrum začíná přesunutím jednoho (prvního) účtu do Partnerské centrum.

## <a name="get-started"></a>Začínáme

Přesun začíná v PMC. Globální správce dostane pozvánku k zahájení přesunu.

### <a name="prepare-in-pmc"></a>Příprava v PMC

- Ověření podrobností o společnosti
- Ověření kontaktu primárního programu
- Ověření obchodních umístění
- Aktualizace schválených uživatelů

### <a name="when-youre-ready"></a>Až budete připraveni

U **pozvánky** vyberte Začínáme. Budete na přihlašovací Partnerské centrum.

:::image type="content" source="images/migration/getstarted.jpg" alt-text="Začínáme":::

## <a name="start-with-your-work-email"></a>Začínáme s pracovním e-mailem

Pokud vaše společnost nemá pracovní e-maily a tenanta AAD, můžeme vám v rámci procesu přihlašování z partnerského centra pomůžeme ho nastavit. Když se pokusíte přihlásit pomocí e-mailového účtu, který není pracovním e-mailem, jako je například váš osobní účet, budete přesměrováni na poskytnutí informací o vaší společnosti, abyste mohli nastavit tenanta AAD a pracovní e-mail. Tyto podrobnosti společnosti se použijí k finalizaci účtu v partnerském centru, takže se ujistěte, že jsou přesné.

>[!NOTE]
>Pokud jste partner v Číně a zaregistrovali jste v programu Microsoft Partner Network i Cloud Solution Provider (CSP), budete mít pro každý účet samostatného tenanta. Váš účet pomocí programu Cloud Solution Provider se spravuje v národním cloudu a váš Microsoft Partner Network účet se spravuje v globálním cloudu. Tyto dva účty nelze propojit.

:::image type="content" source="images/migration/newtellusabout.png" alt-text="Řekněte nám o své společnosti":::

Jakmile ověříte nebo aktualizujete informace, vyberte **přijmout a pokračovat**.
Podmínky a ujednání na této stránce jsou **přesně stejné** jako smlouva, kterou vaše společnost už přihlásila v PMC.  
Tento krok iniciuje vytvoření vašeho tenanta Azure AD a poskytne vám pracovní účet.

Výběr možnosti **přijmout a pokračovat** provede také následující akce:

- Migruje váš účet spolu se všemi jeho umístěními do partnerského centra.

- Migruje jakékoli kompetence nebo mapy, které jste si mohli koupit v PMC.

- Migruje všechny marketingové prostředky, nabídky a programy (MAPs, stříbrné, Gold), které jste měli v PMC.

## <a name="invite-employees-to-join-you"></a>Pozvání zaměstnanců k připojení

Když se vytvoří nový tenant Azure AD, můžete svým zaměstnancům pozvat, aby se přihlásili k partnerskému centru.

:::image type="content" source="images/migration/invite.png" alt-text="Pozvat zaměstnance":::

Pokud jste se přihlásili pomocí stávajícího tenanta AAD, vaši zaměstnanci se vám přesunuli. V takovém případě přiřaďte své role zaměstnanců, abyste mohli spravovat, co můžou dělat v partnerském centru. 

>[!NOTE] 
>Role v partnerském centru se liší od rolí v PMC. Další informace najdete v tématu [Přesun z PMC do partnerského centra](move-pmc-pc-map.md).

## <a name="verify-your-domain-and-become-a-global-admin"></a>Ověření domény a stane se globálním správcem  

Pokud je váš tenant AAD nový, nebude mít nikdo přiřazenu roli globálního správce. Abyste se stali globálním správcem, musíte ověřit vlastnictví domény. Je možné, že budete potřebovat správce domény, který vám to může pomáhat.

I když můžete použít nabídky, které jste už zakoupili, nebudete moct koupit žádné nové nabídky, dokud nedokončíte krok přiřazení globálního správce.

:::image type="content" source="images/migration/takecontrol.png" alt-text="Převzít kontrolu":::

Když vyberete Začínáme, zobrazí se následující obrazovka:

:::image type="content" source="images/migration/verifytxt.png" alt-text="Ověření vlastnictví domény":::

Váš doménový registrátor už pro vás bude vyplněný. Jenom vlastník domény může aktualizovat soubor DNS, takže tak, že zkopírujete a přidáte textový soubor do záznamu DNS, můžeme ověřit, že jste vlastníkem. Může to trvat několik minut, než se aktualizace dokončí. Budete se muset odhlásit z partnerského centra a pak se znovu přihlásit. Vaše role bude změněna na globální správce.

## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>Seznámení s řídicím panelem a Partnerským centrem

Projděte si řídicí panel. Tady je místo, kde můžete spravovat svoje členství, přidat obchodní profil pro referenční seznamy, zaregistrovat se v programu Cloud Solution Provider a kdykoli zobrazit oznámení a nabídky, které jsou pro vaši firmu relevantní. stačí vybrat **řídicí panel**. Můžete také spravovat pobídky, nakupovat na webu Marketplace, registrovat se ke službám pro uvedení na trh a další.  

:::image type="content" source="images/migration/fre.png" alt-text="Absolvovat prohlídku":::

## <a name="sign-the-microsoft-partner-agreement"></a>Podepsat smlouvu o partnerovi Microsoftu

Pokud jste nepřímý prodejce, pokud jste si nastavili účet partnerského centra, musíte si ho i nadále úředně zaregistrovat v programu Cloud Solution Provider. Pokud chcete zkontrolovat stav členství, klikněte na svůj [Oficiální profil](https://partner.microsoft.com/pcv/accountsettings/partnerprofile) a potvrďte typ účtu. Pak se jako [nepřímý prodejce](enrolling-in-the-csp-program.md)zaregistrujete do zprostředkovatele CSP.

 Jakmile se zaregistrujete jako nepřímý prodejce, přijměte [žádost o vztah CSP k vašemu nepřímému poskytovateli](indirect-reseller-tasks-in-partner-center.md).

Pak na [řídicím panelu](https://partner.microsoft.com/pvc/dashboard) partnerského centra s přihlašovacími údaji globálního správce Přijměte smlouvu s partnerem Microsoftu. Potvrďte, že jste si zaregistrovali smlouvu s partnerem Microsoftu v části informace o programu v profilu partnera. Na stránce Přehled CSP se zobrazí také oznámení potvrzující hlavičku. 

## <a name="next-steps"></a>Další kroky

- [Najít globálního správce](become-global-admin.md)

- [Smlouva s partnerem Microsoftu](microsoft-partner-agreement.md)

- [Vytváření uživatelských účtů](create-user-accounts-and-set-permissions.md)

- [Přiřazování uživatelských rolí a oprávnění](permissions-overview.md)

- [Správa programů členství](renew-mpn-offers.md)

- [Vytvoření obchodního profilu vaší společnosti](create-a-marketing-profile.md)

- [Spojte se se zákazníky prostřednictvím odkazů](manage-leads.md)

- [Průvodce migrací více společností z PMC do partnerského centra](move-multiple-companies.md)
