---
title: Správa umístění v partnerském účtu
ms.topic: how-to
ms.date: 02/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Naučte se, jak přidat nové umístění a jak se v programu motivačních programů, v obchodních předplatných, předplatných a dalších transakcích používá umístění MPN ID.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 41ffaeaf0fb46659142949872295523546bb91c1
ms.sourcegitcommit: 5768f10cd122a20fe3df3062ea34e7096d99f639
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/09/2021
ms.locfileid: "100005903"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a>Správa umístění účtu MPN a přidání (odstranění) umístění


**Příslušné role**

- Globální správce
- Správce účtu

ID MPN umístění identifikuje každé konkrétní umístění vaší společnosti. K registraci v programu motivačních programů použijete umístění MPN ID, a to za transakčního poskytovatele řešení cloudu (CSP) a další obchodní transakce. Globální ID MPN se používá pro netransakční aktivity, například žádosti o podporu.

## <a name="the-following-is-a-typical-scenario"></a>Následuje typický scénář:

Společnost Contoso má svůj partnerský globální účet (PGA) ve Spojeném království. Jedná se o své registrované právní firmy a globální ID MPN se používá ke správě všech netransakčních obchodních činností. Společnost Contoso má také partnerské účty partnera (PLA) rovnocenné dceřiným společnostem nebo divizím v jiném umístění v USA, Francii a USA. Ve struktuře účtu MPN se tyto PLAs reprezentují jako jedinečná ID MPN. PLAs se používají pro transakční firmy, jako je CSP nebo pobídky programů. Výběry jsou vázané na konkrétní umístění. 

>[!NOTE]
>Mezi klientem CSP a ID umístění MPN je 1-1 vztah.

:::image type="content" source="images/locations/locations1.png" alt-text="Struktura míst MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>Požadavky, aby bylo možné přidat nový účet pro firmu CSP

Pokud chcete přidat nový obchodní účet CSP, začněte tím, že ověříte, že jste splnili požadavky.

1. Musíte mít umístění MPN ID v zemi, kde chcete, aby se zprostředkovatel CSP vystavil. Pokud chcete vytvořit nové umístění MPN, přečtěte si níže téma "Přidání umístění MPN".
  
1. Chcete-li vytvořit nového poskytovatele nepřímých prodejců CSP, přečtěte si téma [práce s nepřímými poskytovateli](indirect-reseller-tasks-in-partner-center.md#get-started) 

>[!NOTE] 
 >Nezapomeňte se přihlásit pomocí **nových** přihlašovacích údajů **nového** účtu CSP. Nepoužívejte svoje stávající přihlašovací údaje, protože Partnerské centrum vám rozpozná, jak už účet máte.

2. Přijměte smlouvu s partnerem Microsoftu a aktivujte účet.

1. Pokud se chcete zaregistrovat jako přímý fakturační Server, [požadavky na čtení pro přímé partnery z fakturace](direct-partner-new-requirements.md)

## <a name="view-your-mpn-locations"></a>Zobrazení umístění MPN

1. Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard/home) partnerského centra s přihlašovacími údaji k účtu MPN. (Vaše přihlašovací údaje programu MPN se můžou lišit od vašich přihlašovacích údajů CSP.) 
 
1. V ikoně **Nastavení** vyberte **Nastavení účtu**, **Profil organizace**, **právní**. 

1. Na kartě **partner** ověřte, že není k dispozici zpráva banneru s výzvou k opravě umístění migrace z PMC. Pokud je, postupujte podle pokynů a opravte tato umístění. 

3. Pokud není k dispozici žádná chybová zpráva, pak z  **Nastavení** vyberte  **Nastavení účtu**, **Profil organizace**, **identifikátory**.

4. Vyhledejte ID MPN s typem "umístění", které odpovídá zemi tohoto účtu CSP, a použijte ji k vyhledávání níže a dokončení přidružení.

5. Pokud nemůžete najít umístění MPN ID, které odpovídá účtu CSP, který chcete použít, můžete přidat nové umístění, ve kterém se vytvoří nové ID MPN. Viz téma **Přidání umístění MPN** níže.

## <a name="add-an-mpn-location"></a>Přidat umístění MPN

1. Přihlaste se pomocí účtu MPN v partnerském centru. (Vaše přihlašovací údaje programu MPN se můžou lišit od vašich přihlašovacích údajů CSP). Účet MPN by měl mít oprávnění globálního správce nebo správce účtů. 

1. V **ikoně nastavení** vyberte **Nastavení účtu** a pak vyberte **Profil organizace**.

2. Vyberte možnost **právní** a pak na kartě **partner** vyberte **obchodní umístění** a klikněte na **Přidat umístění.**

3. Zadejte požadované podrobnosti, včetně názvu firmy, adresy a kontaktu pro umístění, které chcete přidat do své společnosti.
 
1. Klikněte na **Přidat umístění**. Tím se vytvoří nové ID MPN pro nové umístění, které můžete použít pro transakce a pobídky CSP.

:::image type="content" source="images/legal-biz.png" alt-text="Přidat novou právní firmu":::

> [!NOTE]
> Jakmile je umístění přidané v partnerském centru, nemůžete ho odebrat. Pokud jste pro přihlášení použili správné ID **MPN, zobrazí se v levé** nabídce centra pro partnery v nabídce vlevo.

## <a name="delete-a-location"></a>Odstranit umístění

Pokud chcete odstranit umístění z vašeho účtu, budete muset kontaktovat [podporu partnerů](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b). Ujistěte se, že rozumíte dopadu, který tato akce má. Odstraněná umístění nelze načíst a veškerá vázaná ID MPN již nebudou rozpoznána nebo bude pro vaši společnost aktivní.

## <a name="change-country-of-partner-global-account"></a>Změnit zemi globálního účtu partnera 

1. Přihlaste se pomocí účtu MPN v partnerském centru. (Vaše přihlašovací údaje programu MPN se můžou lišit od vašich přihlašovacích údajů CSP). Účet MPN by měl mít oprávnění globálního správce nebo správce účtů. 

2. Na kartě **partner** klikněte na **obchodní umístění** a zkontrolujte seznam umístění a ujistěte se, že je v seznamu uvedeno umístění, které chcete použít jako právní entitu. 
 
1. Chcete-li přidat umístění, klikněte na tlačítko **Přidat umístění** a za předpokladu zadejte požadované podrobnosti, včetně názvu firmy, adresy a primárního kontaktu pro umístění, které chcete přidat do své společnosti. 
 
1. Vyberte možnost **změnit zemi** vedle rozevíracího seznamu **země/oblast** a postupujte podle pokynů. 

:::image type="content" source="images/lbp.png" alt-text="Oficiální informace o obchodním profilu":::

5. Klikněte na **Uložit**.

6. Země globálního účtu MPN se změní na novou právní zemi.
  
## <a name="next-steps"></a>Další kroky

- Přečtěte si o [procesu ověřování](verification-responses.md).
