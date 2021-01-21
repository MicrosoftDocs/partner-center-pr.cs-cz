---
title: Migrace z PMC do partnerského centra
ms.topic: article
ms.date: 10/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se migrovat společnost z partnerského centra členství (PMC) do partnerského centra, včetně kroků, které je potřeba provést.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 8b6646ff943ff219c41c975d60e66a46d1e0f595
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/19/2020
ms.locfileid: "92527759"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>Příručka k migraci z PMC na Partnerské centrum

**Příslušné role**

- Globální správce

Web partnera Microsoftu na adrese partner.microsoft.com je jednotnou digitálním prostředím pro partnery. Na webu partnera budete moci prozkoumat vaše příležitosti a zapojit se do práce s asistencí, které vaší společnosti pomáhají při sestavování a prodeji vašich aplikací a služeb společnosti Microsoft. Pomocí odkazu na řídicí panel, který je dostupný na webu partnera, se členové Microsoft Partner Network můžou přihlásit do partnerského centra, kde můžete spravovat svůj vztah s Microsoftem, zaregistrovat se do programů a zaregistrovat se k nabídkám.

Vyřazení partnerského centra členství (PMC) je vyřazené z provozu. Vaše společnost se pozvala k převedení správy členství Microsoft Partner Network do partnerského centra. Tato příručka vás připraví na to, co byste měli očekávat při přesunu z PMC do partnerského centra.

>[!NOTE]
>I v případě, že má vaše společnost více než jeden účet nebo umístění, přesune se na partnerské Centrum přesunutím jednoho (prvního) účtu do partnerského centra.

## <a name="get-started"></a>Začínáme

Přesun začíná v PMC. Váš globální správce obdrží pozvánku k zahájení přesunu.

### <a name="prepare-in-pmc"></a>Příprava v PMC

- Ověření podrobností společnosti
- Ověřit kontakt primárního programu
- Ověřit obchodní umístění
- Aktualizace schválených uživatelů

### <a name="when-youre-ready"></a>Až budete připraveni

Na **pozvánkě vyberte Začínáme** . Přejdete na přihlašovací stránku partnerského centra.

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

Pokud jste se přihlásili pomocí stávajícího tenanta AAD, vaši zaměstnanci se vám přesunuli. V takovém případě přiřaďte své role zaměstnanců, které určují, co můžou dělat v partnerském centru. 

>[!NOTE] 
>Role v partnerském centru se liší od rolí v PMC. Další informace najdete v tématu [Přesun z PMC do partnerského centra](move-pmc-pc-map.md).

## <a name="verify-your-domain-and-become-a-global-admin"></a>Ověření domény a stane se globálním správcem  

Pokud je váš tenant AAD nový, nebude mít nikdo přiřazenu roli globálního správce. Abyste se stali globálním správcem, musíte ověřit vlastnictví domény. Je možné, že budete potřebovat správce domény, který vám to může pomáhat.

I když můžete použít nabídky, které jste už zakoupili, nebudete moct koupit žádné nové nabídky, dokud nedokončíte krok přiřazení globálního správce.

:::image type="content" source="images/migration/takecontrol.png" alt-text="Převzít kontrolu":::

Když vyberete Začínáme, zobrazí se následující obrazovka:

:::image type="content" source="images/migration/verifytxt.png" alt-text="Ověřit vlastnictví domény":::

Váš doménový registrátor už pro vás bude vyplněný. Jenom vlastník domény může aktualizovat soubor DNS, takže tak, že zkopírujete a přidáte textový soubor do záznamu DNS, můžeme ověřit, že jste vlastníkem. Může to trvat několik minut, než se aktualizace dokončí. Budete se muset odhlásit z partnerského centra a pak se znovu přihlásit. Vaše role bude změněna na globální správce.

## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>Seznámení s řídicím panelem a Partnerským centrem

Projděte si řídicí panel. Tady je místo, kde můžete spravovat svoje členství, přidat obchodní profil pro referenční seznamy, zaregistrovat se v programu Cloud Solution Provider a kdykoli zobrazit oznámení a nabídky, které jsou pro vaši firmu relevantní. stačí vybrat **řídicí panel**. Můžete také spravovat pobídky, nakupovat na webu Marketplace, registrovat se ke službám pro uvedení na trh a další.  

:::image type="content" source="images/migration/fre.png" alt-text="Absolvovat prohlídku":::

## <a name="sign-the-microsoft-partner-agreement"></a>Podepsat smlouvu o partnerovi Microsoftu

Pokud jste nepřímý prodejce, pokud jste si nastavili účet partnerského centra, musíte si ho i nadále úředně zaregistrovat v programu Cloud Solution Provider. Pokud chcete zkontrolovat stav členství, vyhledejte svůj [partnerský profil](https://partner.microsoft.com/pcv/accountsettings/partnerprofile) a potvrďte typ účtu. Pak se jako [nepřímý prodejce](enrolling-in-the-csp-program.md)zaregistrujete do zprostředkovatele CSP.

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
