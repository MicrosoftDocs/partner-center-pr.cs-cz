---
title: Převeďte předplatné Azure v rámci plánu Azure na jiného partnera CSP.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se, jak změnit partnera programu Cloud Solution Provider přidružený k předplatným Azure v rámci plánu Azure.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: f0abfdfd2fbb242f7cdbe0ded04d387ea712cce5
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702718"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a>Přenos předplatných plánu Azure pro zákazníka na jiného partnera

**Příslušné role**

- Správce účtu
- Agent prodeje
- Fakturační Agent

Tento článek popisuje, jak může zákazník přepnout svoje předplatné Azure v rámci plánu Azure z jednoho Cloud Solution Provider (CSP) na jiný.

Pokud chcete přepnout předplatná Azure pro zákazníka z jiného partnera, postupujte podle těchto kroků. Oba partneři i zákazník mají postup k dokončení.

>[!Note]  
>Přístup k nástrojům pro přechod mají jenom partneři s přímým fakturačním vztahem a Microsoftem. Nepřímí prodejci musí spolupracovat s jejich nepřímými poskytovateli pro využití tohoto nástroje pro přechod.

Před využitím tohoto nástroje se zákazník musí nacházet v konverzaci s oběma partnery (aktuální i budoucí). Aby se zabránilo nejasnostem a záměnám, musí být nutné provést konverzaci v režimu offline. Kromě toho by měli partneři a zákazníci pochopit tyto požadavky a předpoklady před zahájením přechodu:

**Klíčové důležité pokyny:**

- Azure Reservations se s předplatným nepřesunou na budoucího partnera
- Ceny za CSP pro služby Azure v rámci aktuálního partnera nebudou převedeny  
- Odpovědnosti podpory pro zákazníka se přesunou na budoucího partnera.
- Fakturace a fakturace se přesunou k budoucímu partnerovi v době přenosu.
- Přenos z Azure Role-Based Access Control (RBAC) není ovlivněný.
- Správce jménem (ADMINISTRATE) se ve výchozím nastavení neudělí budoucímu partnerovi.
- Produkty z Marketplace třetích stran se přenesou, dokud produkty nespravují kontrolu nároků na Marketplace.
    - Neexistují žádné zvláštní slevy ani oblastní omezení.
    - Produkty nejsou založené na předplatném
    - Budoucí partner musí spolupracovat s vydavatelem, aby se ujistil, že se nachází v seznamu povolených pro nasazení produktu.
    - Pokud nejsou splněné všechny tyto podmínky, aby bylo možné přenést produkty z webu Marketplace, je třeba přenášet předplatné Azure a pak znovu koupit produkty z Marketplace novým partnerem.

**Požadavky:**

- Zákazník v rámci svého záměru zahájí převod na stávajícího partnera CSP
- Budoucí partner CSP spolupracuje se zákazníkem, aby se zajistilo splnění zákaznických potřeb.
- Budoucí partner CSP naváže vztah se zákazníkem a koupí plán Azure před zahájením přechodu.  
- Zákazník musí podepsat zákaznickou smlouvu Microsoftu s budoucím partnerem CSP.
- Budoucí partner CSP musí mít podepsané smlouvy Microsoftu pro použití tohoto nástroje.

## <a name="customer-tasks-to-be-completed"></a>Úkoly zákazníků, které se mají dokončit

Aby bylo možné přenést předplatné Azure v rámci plánu Azure, zákazník musí zahájit proces tím, že se spojí se svým aktuálním partnerem. Měly by shromažďovat název a doménu společnosti aktuálního partnera, aby jejich budoucí partneři mohli dokončit formulář žádosti o přenos svým jménem.

Zákazník musí také identifikovat předplatná, která chtějí přenést z aktuálního partnera. Nemůžete změnit partnery pro Office 365, Enterprise Mobility Suite nebo Microsoft Dynamics CRM Subscriptions.

>[!Note]  
>Je to budoucí zodpovědnost partnera za účelem vyplnění formuláře žádosti o přenos, který zahájí proces přenosu. Společnost Microsoft se nemůže zasáhnout jménem zákazníka ani aktuálního partnera. Zákazník by měl v úmyslu spolupracovat s budoucím a aktuálním partnerem, aby přechod přešel do hladké míry.

## <a name="future-partner-tasks-to-be-completed"></a>Budoucí úkoly partnerských serverů

Budoucí partner předplatného musí vyplnit formulář žádosti o přenos z partnerského centra, aby vyžádal přenos předplatného:

1.  V nabídce partnerského centra vyberte **zákazníci** a pak vyberte zákazníka, kterému chcete vyplnit formulář žádosti o přenos.
2.  V nabídce zákazník vyberte **předplatná**.
3.  Vyberte část **žádost o přenos** .
4.  V **části žádost o přenos** vyberte **Přidat novou žádost**.

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Oddíl transfery":::

5.  Vyplňte formulář **nové žádosti o přenos** .

6.  Vyberte odeslat **žádost o odeslání žádosti o přenos**  >  .

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Formulář žádosti o dokončení přenosu":::

7.  Kontrola potvrzení žádosti o přenos

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Kontrola probíhajícího přenosu":::

    >[!Note]
    >Budoucí partner může žádost o přenos zrušit tak, že v pravém horním rohu vybere možnost **zrušit žádost** jenom v případě, že stav žádosti o přenos čeká na vyřízení. Jakmile je stav požadavku na přenos "probíhá" nebo "dokončeno", zrušení nebudou možné.

## <a name="current-partner-tasks-to-be-completed"></a>Aktuální úkoly partnerského serveru, které se mají dokončit

Agent pro správce aktuálního partnera dostane e-mail, že zákazník požaduje přenos svých předplatných:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Opakování":::

Pokud chcete dokončit přenos předplatného, přečtěte si a přijměte formulář žádosti o přenos z partnerského centra.

>[!Note]  
>Pokud aktuální partner neprovede žádnou akci během 30 dnů, vyprší platnost žádosti a budoucí partner bude mít k dispozici vytvoření nové žádosti o přenos.

1.  Vyberte **zkontrolovat žádost o přenos** z e-MAILu nebo
1.  V nabídce partnerské Centrum vyberte **zákazníci** a pak vyberte zákazníka, kterému byla odeslána žádost o přenos jménem.
2.  V nabídce zákazník vyberte **předplatná**.
3.  Vyberte část **žádost o přenos** .
4.  Rozbalte informace o přenosu výběrem zvoleného **ID žádosti o přenos** v části **přijaté požadavky** .

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Revize zdrojového kódu požadavek na přenos":::

5.  Zkontrolujte požadavek na přenos. Vyberte požadovaná předplatná Azure, která chcete přenést.

>[!Note]  
> Než budete pokračovat, nezapomeňte prosím, že už nebudete mít přístup k vybraným předplatným.
> Nebudeme vám fakturovat za další využití.
> Rezervace Azure se nepřenášejí s předplatnými.

6.  Pak vyberte **přijmout a přenést** a dokončete proces přenosu.

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Vyberte předplatná, která se mají přenést do vašich plánů Azure.":::

7.  Zobrazení potvrzení přijetí přenosu.

   V tomto okamžiku bude budoucí partner, zákazník a aktuální partner upozorněni na přijatý požadavek na přenos prostřednictvím e-mailu.

   Po je tento přechod přijatý až do 15 minut, než se systém aktualizuje, takže stav přenosu může zůstat nedokončený. Pokud bude trvat déle, systém se postará o tři dny. Pokud stav přenosu stále ještě čeká na vyřízení, partner by měl odeslat žádost o služby.

   Po dokončení přenosu se předplatná obsažená v žádosti zobrazí v plánu Azure budoucího partnera a už se nebude zobrazovat v seznamu.

>[!Note]  
>U nepřímých zprostředkovatelů: Informujte prosím svého nepřímý prodejce o přijetí žádosti o přenos.

### <a name="managing-your-transferred-customer-subscriptions"></a>Správa přenesených zákaznických předplatných

- Převod nebude mít vliv na přístup ke stávajícím uživatelům, skupinám nebo instančním objektům přiděleným pomocí řízení přístupu na základě role v Azure (RBAC). Řízení přístupu na základě role Azure [(Azure RBAC)](/azure/role-based-access-control/overview) pomáhá zákazníkům spravovat, kdo má přístup k prostředkům Azure, co s těmito prostředky může dělat a k jakým oblastem mají přístup. Jako nový partner jste nedostali přístup k prostředkům vašeho zákazníka po převodu předplatného. Předchozí partner vašeho zákazníka si zachová přístup RBAC. Spolupracujte se svým zákazníkem a zjistěte, kdo má ve svých předplatných nějaké informace a jakým způsobem je možné provést požadované změny.

- V důsledku toho je důležité, aby váš zákazník odebral přístup k Azure RBAC pro svého předchozího partnera a přidal přístup pro nového partnera. Další informace o zákazníkovi, který poskytuje nový přístup, najdete v tématu [co je řízení přístupu na základě role Azure (Azure RBAC)?](/azure/role-based-access-control/overview) Další informace o tom, jak zákazník odebírá přístup k organizaci RBAC z předchozího partnera, najdete v tématu [Odebrání přiřazení role](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).

- K vašemu předplatnému navíc nezískáte automaticky oprávnění [správce (administrate)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) . ADMINISTRATE je nutné, aby partneři spravovali svoje předplatná Azure na svých zákaznících jménem. Další informace o oprávněních Azure najdete v tématu [získání oprávnění ke správě služby nebo předplatného zákazníka.](./customers-revoke-admin-privileges.md)

## <a name="next-steps"></a>Další kroky:

- [(Azure RBAC)](/azure/role-based-access-control/overview)
- [Získejte oprávnění ke správě služby nebo předplatného zákazníka.](./customers-revoke-admin-privileges.md)
