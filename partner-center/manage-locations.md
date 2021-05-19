---
title: Správa umístění v partnerském účtu
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Naučte se, jak přidat nové umístění a jak se v programu motivačních programů, v obchodních předplatných, předplatných a dalších transakcích používá umístění MPN ID.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 13d6e7dc4722227035be2b24df48427f2008bb14
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151776"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a>Správa umístění účtu MPN a přidání (odstranění) umístění


**Příslušné role**: globální správce | Správce účtu

ID MPN umístění identifikuje každé konkrétní umístění vaší společnosti. K registraci v programu motivačních programů použijete umístění MPN ID, a to za transakčního poskytovatele řešení cloudu (CSP) a další obchodní transakce. Globální ID MPN se používá pro netransakční aktivity, například žádosti o podporu.

## <a name="the-following-scenario-is-typical"></a>Typický je následující scénář:

Společnost Contoso má svůj partnerský globální účet (PGA) ve Spojeném království. PGA je jejich registrovaná právní společnost a její globální ID MPN se používá ke správě všech netransakčních obchodních činností. Společnost Contoso má také partnerské účty partnera (PLA) rovnocenné dceřiným společnostem nebo divizím v jiném umístění v USA, Francii a USA. Ve struktuře účtu MPN se tyto PLAs reprezentují jako jedinečná ID MPN. PLAs se používají pro transakční firmy, jako je CSP nebo pobídky programů. Výběry jsou vázané na konkrétní umístění. 

>[!NOTE]
>Mezi klientem CSP a ID umístění MPN je 1-1 vztah.

:::image type="content" source="images/locations/locations1.png" alt-text="Struktura míst MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>Požadavky, aby bylo možné přidat nový účet pro firmu CSP

Pokud chcete přidat nový obchodní účet CSP, začněte tím, že ověříte, že jste splnili požadavky.

1. Musíte mít umístění MPN ID v zemi, kde chcete, aby se zprostředkovatel CSP vystavil. Pokud chcete vytvořit nové umístění MPN, přečtěte si níže téma "Přidání umístění MPN".
  
1. Pokud chcete vytvořit novou registraci CSP Indirect Reseller, přečtěte si o [práci s nepřímými poskytovateli.](indirect-reseller-tasks-in-partner-center.md#get-started) 

>[!NOTE] 
 >Nezapomeňte se přihlásit pomocí nových **přihlašovacích** údajů pro **nový účet** CSP. Nepoužívejte stávající přihlašovací údaje, protože Partnerské centrum poznáte, že už účet máte.

2. Přijměte Smlouva s partnerem Microsoftu a aktivujte účet.

1. Pokud se chcete zaregistrovat jako partner s přímým vyúčtováním, přečtěte si požadavky [na partnery s přímým vyúčtováním.](direct-partner-new-requirements.md)

## <a name="view-and-update-your-mpn-locations"></a>Zobrazení a aktualizace umístění MPN

1. Přihlaste se k řídicímu Partnerské centrum [pomocí](https://partner.microsoft.com/dashboard/home) přihlašovacích údajů účtu MPN. (Vaše přihlašovací údaje MPN se mohou lišit od vašich přihlašovacích údajů CSP)) 
 
1. V **ikoně** Nastavení vyberte **Nastavení účtu**, **Profil organizace**, **Právní.** 

1. Na kartě **Partner** ověřte, že není chybová zpráva s upozorněním s žádostí o opravu migrovaných umístění z PMC.  Pokud vaše umístění nebyla v PMC správně nastavená a ještě nebyla přemísněna na počítač PC, musíte tato umístění aktualizovat.

:::image type="content" source="images/locations/location-two.png" alt-text="Snímek obrazovky ukazuje, jak aktualizovat umístění.":::
 
4.  Na **obrazovce Review PMC locations (Zkontrolovat umístění PMC)** vyberte **Update (Aktualizovat).**
Aktualizujte následující pole:

- **Pole Název:** Ujistěte se, že je název umístění společnosti správný. Pokud se zobrazí duplicitní chyba, zkuste změnit například z Contoso na Contoso, Inc.

- **Pole právní osoby:** Ujistěte se, že jste zvolili právnickou osobu, se kterou je umístění vázané.

- **Řádek adresy 1 & 2:** Ujistěte se, že je adresa správná.

- **Pole & stát/kraj:** Ujistěte se, že je kombinace mezi městem a krajem správná. V některých zemích se použije rozevírací nabídka pro výběr státu/kraje a v jiných zemích bude nutné toto pole vložit ručně.

- **PSČ – pole** poštovního směrovacího čísla: Ujistěte se, že pole PSČ odpovídá vaší zadané zemi, oblasti, města nebo adrese.

- **Pole primárních kontaktních informací**: Ujistěte se, že pole jméno a příjmení jsou vyplněna a že e-mailová adresa je pracovní e-mailová adresa, nikoli osobní (například,, @outlook.com @live.com atd.).

- **Pole telefonní číslo**: Ujistěte se, že telefonní číslo neobsahuje speciální znaky, mezery ani kód země. Hodnota zadaná v poli telefonní číslo bude vždycky obsahovat maximálně 10 znaků.

5. Pokud není k dispozici žádná chybová zpráva, pak z  **Nastavení** vyberte  **Nastavení účtu**, **Profil organizace**, **identifikátory**.

6. Vyhledejte ID MPN s typem "umístění", které odpovídá zemi tohoto účtu CSP, a použijte ji k dokončení přidružení.

7. Pokud nemůžete najít umístění MPN ID, které odpovídá účtu CSP, který chcete použít, můžete přidat nové umístění, ve kterém se vytvoří nové ID MPN. Viz téma **Přidání umístění MPN** níže.

## <a name="add-an-mpn-location"></a>Přidat umístění MPN

1. Přihlaste se pomocí účtu MPN v partnerském centru. (Vaše přihlašovací údaje programu MPN se můžou lišit od vašich přihlašovacích údajů CSP.) Účet MPN by měl mít oprávnění globálního správce nebo správce účtů. 

1. V **ikoně nastavení** vyberte **Nastavení účtu** a pak vyberte **Profil organizace**.

2. Vyberte možnost **právní** a pak na kartě **partner** vyberte **obchodní umístění** a vyberte **Přidat umístění.**

3. Zadejte požadované podrobnosti, včetně názvu firmy, adresy a kontaktu pro umístění, které chcete přidat do své společnosti.
 
1. Vyberte **Přidat umístění**. Tím se vytvoří nové ID MPN pro nové umístění, které můžete použít pro transakce a pobídky CSP.

:::image type="content" source="images/legal-biz.png" alt-text="Přidat novou právní firmu":::

> [!NOTE]
> Jakmile je umístění přidané v partnerském centru, nemůžete ho odebrat. Pokud jste pro přihlášení použili správné ID **MPN, zobrazí se v levé** nabídce centra pro partnery v nabídce vlevo.

## <a name="add-the-registration-number-id"></a>Přidat ID registračního čísla

Pokud jste nepřímý poskytovatel, partner s přímým vyúčtováním nebo nepřímý prodejce a podnikáte s novými nebo stávajícími zákazníky v následujících zemích, musíte pro svou firmu zadat identifikační čísla registrace. Pokud země, ve které podnikáte, není uvedená níže, ID registrace je volitelné.

- Arménie 
- Ázerbájdžán 
- Bělorusko 
- Brazílie 
- Maďarsko 
- Indie 
- Irák 
- Kazachstán 
- Kyrgyzstán 
- Moldavsko 
- Myanmar 
- Polsko 
- Rusko 
- Saúdská Arábie 
- Jižní Afrika 
- Jižní Súdán  
- Tádžikistán 
- Thajsko
- Turecko 
- Ukrajina 
- Spojené arabské emiráty 
- Uzbekistán 
- Venezuela
- Vietnam 


Další informace najdete v článku [o čísle ID registrace.](reg-number-id.md)

## <a name="delete-a-location"></a>Odstranění umístění

Pokud chcete umístění z vašeho účtu odstranit, budete se muset obrátit na [podporu partnerů.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b) Ujistěte se, že rozumíte dopadu, který tato akce má. Odstraněná umístění není možné načíst a cokoli svázané s konkrétním ID MPN se už nerozpozná nebo nebude pro vaši společnost aktivní.

## <a name="change-country-of-partner-global-account"></a>Změna země globálního účtu partnera 

1. Přihlaste se pomocí účtu MPN v Partnerské centrum. (Vaše přihlašovací údaje MPN se mohou lišit od vašich přihlašovacích údajů CSP.) Účet MPN by měl mít oprávnění globálního správce nebo správce účtu. 

2. Na kartě **Partner (Partner)** přejděte na **Obchodní** umístění a zkontrolujte seznam umístění a ujistěte se, že je uvedená lokalita, ve které je uvedená vaše právní osoba. 
 
1. Pokud chcete přidat umístění, klikněte na Přidat umístění a v okně zadejte požadované podrobnosti, včetně obchodního jména, adresy **a** primárního kontaktu pro umístění, které chcete přidat do vaší společnosti. 
 
1. Vyberte **Změnit zemi** vedle rozevíracího seznamu **Země/oblast** a postupujte podle těchto kroků. 

:::image type="content" source="images/lbp.png" alt-text="Právní informace o datech obchodního profilu":::

5. Vyberte **Uložit**.

6. Globální země účtu MPN se změní na novou právní zemi.
  
## <a name="next-steps"></a>Další kroky

- Přečtěte si o [procesu ověřování.](verification-responses.md)
