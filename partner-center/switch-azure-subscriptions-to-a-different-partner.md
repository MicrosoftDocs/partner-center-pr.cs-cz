---
title: Převod předplatného Azure na jiného partnera
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak změnit Cloud Solution Provider programu přidruženého k předplatným Azure zákazníka.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 02/09/2021
ms.openlocfilehash: 94f79762e7fabb377b8d7b559ff9ba2623b135fe
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856062"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>Přesun předplatných Azure zákazníka k jinému partnerovi

**Platí pro**: Partnerské centrum | Partnerské centrum pro Microsoft Cloud for US Government

**Odpovídající role:** Globální správce

Tento článek popisuje, jak může zákazník přepnout své Microsoft Azure služby z jednoho Cloud Solution Provider (CSP) na jiný.

Pokud chcete služby nebo předplatná Azure zákazníka přepnout na jiného partnera, postupujte podle těchto ručních kroků. Tento postup musí provést partner i zákazník.

>[!Note]  
>V současné době mohou předplatná převádět pouze nepřímí nebo nepřímí poskytovatelé.
>Nemůžete měnit partnery pro předplatná Cloud Solution Provider přidružených k plánu Azure, Office 365, enterprise mobility suite nebo předplatným Microsoft Dynamics CRM.

## <a name="switch-partners-for-azure-subscriptions"></a>Přepnutí partnerů pro předplatná Azure

1. Pokud chcete převést předplatné Azure na nového partnera, zákazník musí zahájit proces a v zápisu kontaktovat aktuálního partnera.

   >[!Note]
   > Za vytvoření lístku služby, který zahájí proces převodu, zodpovídá aktuální partner. Microsoft nemůže jednat jménem zákazníka ani nového partnera. Zákazník by měl naplánovat úzkou spolupráci s aktuálním partnerem, aby přechod plynule fungoval.

2. Partner předplatného musí provádět následující úlohy:

   Vytvořte lístek služby Azure z Partnerské centrum a požádejte o převod předplatného:

   1. V Partnerské centrum vyberte **Zákazníci,** v seznamu vyberte zákazníka a pak vyberte **Správa služeb**.

   2. V části **Lístky podpory** vyberte rozevírací seznam **Nový lístek** a zvolte **Microsoft Azure**.
   
   3. Na [Azure Portal](https://portal.azure.com)vyberte Nová **žádost o podporu.**
   
   4. V kroku 1 jako typ problému zvolte **Správa** předplatného, zadejte ID předplatného, které chcete převést, a **Cloud Solution Provider** jako plán podpory.
   
   5. V kroku 2 vyberte **C – minimální dopad** a jako typ problému zvolte **Další obecné otázky** .
   
   6. Stáhněte si [formulář pro přenos předplatného CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC).

3. Partner pro předplatné: Vyplňte [formulář pro přenos předplatného CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC), podepište ho a odešlete zákazníkovi. 

   K vyplnění formuláře budete potřebovat následující informace:

   - Kontaktní údaje aktuálního partnera a ID Microsoftu. V nabídce partnerské Centrum vyberte **Nastavení účtu** &gt; **Profil organizace** a použijte **ID společnosti Microsoft**, **název organizace** a uvedenou **adresu** .

   - ID Microsoftu zákazníka. V nabídce partnerské Centrum vyberte **zákazníci** a potom rozbalte seznam zákazníka, abyste viděli jeho **ID Microsoftu**.

   - ID předplatného, které se má přenést V rozbaleném seznamu zákazníků vyberte **Zobrazit předplatná** a potom rozbalte zvolené předplatné, abyste viděli **ID předplatného**.

   >[!Note]
   >Výsledkem převodu předplatného jsou dvě ID předplatného, které se zobrazí na stránce **Upravit odběr** přenesených předplatného: **1**-ID předplatného partnerského centra se používá pro účely fakturace. **2**– původní ID předplatného Azure se zachová a zobrazí se v partnerském centru i na portálu pro správu Azure. Toto ID se zobrazí v souboru rekognoskaci.  **Když protokolování podporuje lístky, je nutné použít obě ID.**

4. Zákazník a nový partner pro předplatné:

   Zkontrolujte formulář, vyplňte informace o novém partnerovi a přihlaste se. Potvrďte, že nový zákazník má smlouvu smlouvy. Odešle formulář zpátky aktuálnímu partnerovi záznamu.

   *Důležité*: Pokud nový partner CSP nemá vztah prodejce se zákazníkem, musí si ho před přenosem předplatného vytvořit. [Informace o tom, jak to udělat, najdete tady](request-a-relationship-with-a-customer.md).

   >[!Note]
   >Nový partner CSP a tenant zákazníka musí být ve stejné zemi. 

5. Aktuální partner:

   Ujistěte se, že formulář obsahuje kontaktní informace pro oba správce partnerů. Podpora Microsoftu o ověření přenosu budete kontaktovat oba správce. Ujistěte se, že máte všechny tři podpisy. Potom pomocí možnosti **Nahrání** souboru připojte vyplněný formulář ke stávající žádosti o služby. Technik podpory Microsoftu se k vám do osmi pracovních hodin vrátí a ověří příjem a dokončení.

6. Nový partner:

   Aktualizujte nastavení předplatného Azure a odeberte starého partnera z účtu. Pokud chcete zobrazit, která přiřazení rolí jsou zřízená, spusťte dvě rutiny PowerShellu.

   - Přidejte nového partnera jako prodejce do účtu:

     ```powershell
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     >[!NOTE]
     > ID tenanta zákazníka **se** Partnerské centrum jako ID **Microsoftu zákazníka.** Pokud chcete najít ID Microsoftu (ID tenanta) pro konkrétního zákazníka, přihlaste se k Partnerské centrum [řídicího panelu.](https://partner.microsoft.com/dashboard) Pak v **nabídce** vyberte Customers (Zákazníci). Vyhledejte zákazníka v seznamu. Výběrem šipky dolů rozbalte výpis zákazníka. Zobrazí se informace o názvu  domény zákazníka a ID **Microsoftu zákazníka.** V rutině PowerShellu použijte 16místné ID Microsoftu. 

   - Zobrazení rolí v účtu, včetně předchozích partnerů CSP:

     ```powershell
     Get-AzRoleAssignment
     ```

7. Odebrání zastaralých přístupových oprávnění:

   - V nabídce partnerské Centrum vyberte **zákazníci**.
   - Vyhledejte zákazníka na seznamu. Vyberte (dvakrát klikněte) jejich název společnosti. Tato akce otevře stránku **odběry** zákazníka.
   - V nabídce podrobnosti o zákazníkovi vyberte **Správa služeb**.
   - V části **Microsoft Azure** vyberte odkaz pro přechod na **portál pro správu Microsoft Azure**.

## <a name="next-steps"></a>Další kroky

- Stáhněte si [formulář pro přenos předplatného CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA).

- Přečtěte si další informace o [podpoře více partnerů](multipartner.md).

- [Podpora více partnerů](multipartner.md).
- [Podpora více kanálů](multichannel.md).
- [Přenos předplatných Azure](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)