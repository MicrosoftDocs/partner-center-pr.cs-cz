---
title: Správa umístění v partnerském účtu
ms.topic: how-to
ms.date: 01/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Naučte se, jak přidat nové umístění a jak se v programu motivačních programů, v obchodních předplatných, předplatných a dalších transakcích používá umístění MPN ID.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 38ea8a451f51d80998643e2a023420ea3efaa6ba
ms.sourcegitcommit: e99882e9b6c9b1a0f7427fb133693b1d977be76b
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/26/2021
ms.locfileid: "98773431"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a>Správa umístění účtu MPN a přidání nového umístění


**Příslušné role**

- Globální správce
- Správce účtu

ID MPN umístění identifikuje každé konkrétní umístění vaší společnosti. K registraci v programu motivačních programů použijete umístění MPN ID, a to za transakčního poskytovatele řešení cloudu (CSP) a další obchodní transakce. Globální ID MPN se používá pro netransakční aktivity, například žádosti o podporu.

## <a name="the-following-is-a-typical-scenario"></a>Následuje typický scénář:

Společnost Contoso má svůj partnerský globální účet (PGA) ve Spojeném království. Jedná se o své registrované právní firmy a globální ID MPN se používá ke správě všech netransakčních obchodních činností. Společnost Contoso má také partnerské účty partnera (PLA) rovnocenné dceřiným společnostem nebo divizím v jiném umístění v USA, Francii a USA. Ve struktuře účtu MPN se tyto PLAs reprezentují jako jedinečná ID MPN. PLAs se používají pro transakční firmy, jako je CSP nebo pobídky programů. Výběry jsou vázané na konkrétní umístění. 

>[!NOTE]
>Mezi klientem CSP a ID umístění MPN je 1-1 vztah.

:::image type="content" source="images/locations/locations1.png" alt-text="Struktura míst MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-location-for-a-csp-business"></a>Požadavky, aby bylo možné přidat nové umístění účtu pro firmu CSP

Chcete-li přidat nové obchodní umístění CSP, je k dispozici několik požadavků:

1. V zemi, kde chcete provádět podnikání, musíte mít umístění MPN ID.

1. Budete potřebovat nového tenanta Azure AD v [oblasti podnikání](regional-authorization-overview.md) , která ještě není zaregistrovaná ve zprostředkovateli CSP. Tuto vytvořit, když se zaregistrujete v CSP.
 
3. Použijte nového tenanta AAD k registraci do programu CSP v oblasti.
Poskytování právních informací o společnosti, včetně právního jména společnosti, adresy, primárního kontaktního údaje. Tento účet se bude podrobit ověření, takže nezapomeňte přidat platné informace.

>[!NOTE] 
 >Nezapomeňte se přihlásit pomocí **nových** přihlašovacích údajů pro **nového** tenanta Azure AD. Nepoužívejte svoje stávající přihlašovací údaje, protože Partnerské centrum vám rozpozná, jak už účet máte.

4. Přijměte smlouvu s partnerem Microsoftu a aktivujte účet.

## <a name="add-an-mpn-location"></a>Přidat umístění MPN

1. Přihlaste se pomocí účtu MPN v partnerském centru. Účet MPN by měl mít oprávnění globálního správce nebo správce účtů. 

1. V **ikoně nastavení** vyberte **Nastavení organizace**.

2. Vyberte **právní** a potom vyberte **umístění.**

3. Vyberte **Přidat umístění** a vložte podrobnosti o umístění, které chcete přidat do své společnosti, i k primárnímu kontaktu pro dané umístění.

> [!NOTE]
> Po přidání umístění do partnerského centra ho nejde odebrat. Pokud jste pro přihlášení použili správné ID **MPN, zobrazí se v levé** nabídce centra pro partnery v nabídce vlevo.

## <a name="change-global-partner-account-location"></a>Změnit umístění globálního účtu partnera

1. V části **[obchodní umístění](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)** zkontrolujte seznam umístění a ujistěte se, že je v seznamu uvedeno umístění, které chcete jako právní entita. Pokud není, přidejte ho.

   :::image type="content" source="images/accountsettings/location1.png" alt-text="Snímek obrazovky se stránkou pro umístění účtů partnerského centra se seznamem všech aktuálních umístění":::

2. Vyberte **právní** a pak vyberte **aktualizovat platný obchodní profil** .
  
3. Vyberte oblast a právní entitu a **odešlete** ji.

  
## <a name="next-steps"></a>Další kroky

- Přečtěte si o [procesu ověřování](verification-responses.md).
