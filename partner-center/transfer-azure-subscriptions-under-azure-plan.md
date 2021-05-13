---
title: Převod předplatného Azure v rámci plánu Azure na jiného partnera CSP
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak změnit Cloud Solution Provider programu přidruženého k předplatným Azure zákazníka v rámci plánu Azure.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: dcacc6da51fe40c7eb05997f5409ef5fadbcf693
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856045"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a>Převod předplatných plánu Azure zákazníka na jiného partnera

**Odpovídající role:** Správce účtu | Sales agent | Agent fakturace

Tento článek popisuje, jak může zákazník přepnout svá předplatná Azure v rámci plánu Azure z jednoho Cloud Solution Provider (CSP) na jiný.

Pokud chcete přepnout předplatná Azure zákazníka od jiného partnera, postupujte podle těchto kroků. Kroky k dokončení musí provést partner i zákazník.

>[!Note]  
>K nástrojům pro přechod mají přístup pouze partneři s přímým fakturačním vztahem s Microsoftem. Nepřímí prodejci musí spolupracovat se svými nepřímými poskytovateli, aby tento převodní nástroj využili.

Zákazník musí před využitím tohoto nástroje konverzovat s oběma partnery (aktuální i budoucí). Offline konverzace se musí vyhnout nejasnostem a četnosti změn. Partneři a zákazníci by navíc měli před zahájením přechodu porozumět těmto požadavkům a požadavkům:

**Klíčové aspekty:**

- Rezervace Azure se s předplatným nebudou přesouvat k budoucímu partnerovi.
- Ceny CSP pro služby Azure u aktuálního partnera se nebudou přechádovat  
- Odpovědnosti za podporu pro zákazníka se přesunou k budoucímu partnerovi.
- Fakturace a fakturace se v okamžiku převodu přesunou na budoucího partnera.
- Převod Role-Based Access Control (RBAC) není ovlivněný službou Azure.
- AOBO (Admin on Behalf Of) se ve výchozím nastavení neudělí budoucímu partnerovi.
- Produkty z marketplace třetích stran se přenesou, dokud produkty projdou kontrolu způsobilosti pro Marketplace.
    - Neexistují žádné zvláštní slevy ani regionální omezení.
    - Produkty nejsou založené na předplatném.
    - Budoucí partner by měl spolupracovat s vydavatelem a ujistit se, že je na seznamu povolení pro nasazení produktu.
    - Pokud nejsou splněny všechny tyto podmínky pro převod produktů z Marketplace, měly by být zrušeny, převedená předplatná Azure a pak znovu zakoupit produkty z Marketplace s novým partnerem.

**Požadavky:**

- Zákazník zapojuje aktuálního partnera CSP do svého záměru na přechod
- Budoucí partner CSP spolupracuje se zákazníkem, aby zajistil, že bude možné splnit potřeby zákazníků.
- Budoucí partner CSP vytvoří vztah se zákazníkem a před zahájením přechodu si zakoupí plán Azure.  
- Zákazník se musí Smlouva se zákazníkem Microsoftu s budoucím partnerem CSP.
- Budoucí partner CSP musí mít podepsanou Smlouva s partnerem Microsoftu pro použití tohoto nástroje.

## <a name="customer-tasks-to-be-completed"></a>Úkoly zákazníka, které se musí dokončit

Pokud chcete převést předplatné Azure v rámci plánu Azure, zákazník musí zahájit proces kontaktováním jeho aktuálního partnera. Společnost by měla shromáždit název a doménu společnosti aktuálního partnera, aby budoucí partner mohl formulář žádosti o převod vyplnit jejich jménem.

Zákazník musí také identifikovat předplatná, která chtějí převést od svého aktuálního partnera. Nemůžete měnit partnery pro předplatná Office 365, Enterprise Mobility Suite ani Microsoft Dynamics CRM.

>[!Note]  
>Za dokončení formuláře žádosti o převod, který zahájí proces převodu, zodpovídá budoucí partner. Microsoft nemůže jednat jménem zákazníka ani aktuálního partnera. Zákazník by měl naplánovat úzkou spolupráci se svým budoucím a aktuálním partnerem, aby přechod plynule fungoval.

## <a name="future-partner-tasks-to-be-completed"></a>Budoucí úkoly partnerů, které se budou provádět

Budoucí partner předplatného musí vyplnit formulář žádosti o převod od Partnerské centrum požádat o převod předplatného:

1.  V Partnerské centrum vyberte Zákazníci a pak vyberte zákazníka, za nějž chcete formulář žádosti o převod vyplnit.
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

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Žádost o převod zdrojových recenzí":::

5.  Zkontrolujte žádost o převod. Vyberte požadovaná předplatná Azure, která chcete převést.

>[!Note]  
> Než budete pokračovat, mějte na vědomí, že už nebudete mít přístup k vybraným předplatným.
> Další využití se vám nebude fakturovat.
> Rezervace Azure se nepřenesou s předplatným.

6.  Pak **výběrem přijmout a přenést** proces převodu dokončete.

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Výběr předplatných, která se budou převést v rámci vašich plánů Azure":::

7.  Zobrazení potvrzení přijetí převodu

   V tomto okamžiku bude budoucí partner, zákazník a aktuální partner upozorněni na přijatou žádost o převod e-mailem.

   Po přijetí přechodu může stav přenosu během aktualizace systému zůstat až 15 minut ve stavu Čeká na vyřízení. Pokud to trvá déle, systém to bude zkoušet tři dny. Pokud stav převodu stále zůstává ve stavu Čeká na vyřízení, partner by měl odeslat žádost o služby.

   Po dokončení převodu se předplatná zahrnutá v žádosti zobrazí v plánu Azure budoucího partnera a už nebudou uvedená u vás.

>[!Note]  
>Nepřímí poskytovatelé: Informujte svého nepřímého prodejce, že žádost o převod byla přijata.

### <a name="managing-your-transferred-customer-subscriptions"></a>Správa převedených zákaznických předplatných

- Převod nebude mít vliv na přístup ke stávajícím uživatelům, skupinám nebo instančním objektům přiděleným pomocí řízení přístupu na základě role v Azure (RBAC). Řízení přístupu na základě role v Azure [(Azure RBAC)](/azure/role-based-access-control/overview) pomáhá zákazníkům spravovat, kdo má přístup k prostředkům Azure, co může s těmito prostředky dělat a k jakým oblastem má přístup. Jako nový partner nemáte po převodu předplatného žádný přístup RBAC k prostředkům zákazníka. Předchozí partner vašeho zákazníka si zachová přístup RBAC. Spolupracujte se zákazníkem, abyste pochopili, kdo má přehled o svých předplatných a jak provádět požadované změny.

- V důsledku toho je důležité, aby váš zákazník odebral přístup k Azure RBAC pro svého předchozího partnera a přidal přístup pro nového partnera. Další informace o zákazníkovi, který poskytuje nový přístup, najdete v tématu [co je řízení přístupu na základě role Azure (Azure RBAC)?](/azure/role-based-access-control/overview) Další informace o tom, jak zákazník odebírá přístup k organizaci RBAC z předchozího partnera, najdete v tématu [Odebrání přiřazení role](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).

- K vašemu předplatnému navíc nezískáte automaticky oprávnění [správce (administrate)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) . ADMINISTRATE je nutné, aby partneři spravovali svoje předplatná Azure na svých zákaznících jménem. Další informace o oprávněních Azure najdete v tématu [získání oprávnění ke správě služby nebo předplatného zákazníka.](./customers-revoke-admin-privileges.md)

## <a name="next-steps"></a>Další kroky:

- [(Azure RBAC)](/azure/role-based-access-control/overview)
- [Získejte oprávnění ke správě služby nebo předplatného zákazníka.](./customers-revoke-admin-privileges.md)
