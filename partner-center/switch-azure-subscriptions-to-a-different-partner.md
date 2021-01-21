---
title: Přenos předplatného Azure na jiného partnera
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se změnit partnera programu Cloud Solution Provider přidružený k předplatným Azure zákazníka.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 07/29/2020
ms.openlocfilehash: 992dd7f9901efd0176395fb626e4048d5229e82b
ms.sourcegitcommit: e10d2a19dea7e317d227d7fbdcf1bbc3dc4f6257
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/13/2020
ms.locfileid: "92527659"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>Přesun předplatných Azure zákazníka k jinému partnerovi

**Platí pro**

- Partnerské centrum pro Microsoft Cloud pro státní správu USA
- Partnerské centrum pro globální Cloud Microsoft
- Partneři v programu Cloud Solution Provider (CSP)

Tento článek popisuje, jak může zákazník přepnout své Microsoft Azure služby od jednoho poskytovatele Cloud Solution Provider (CSP) na jiný.

Pokud chcete přepnout služby Azure nebo předplatné Azure na jiného partnera, postupujte podle těchto kroků ručně. Partner i zákazník musí provést kroky.

>[!Note]  
>V současné době můžou předplatná přenášet jenom přímá nebo nepřímá zprostředkovatelé.
>Nemůžete změnit partnery pro předplatné Cloud Solution Provider přidružená k plánu Azure, Office 365, Enterprise Mobility Suite nebo předplatným Microsoft Dynamics CRM.

## <a name="switch-partners-for-azure-subscriptions"></a>Přepnout partnery na předplatná Azure

1. Aby bylo možné přenést předplatné Azure na nového partnera, zákazník musí tento proces zahájit a kontaktovat svého současného partnera s psaním záznamu.

   >[!Note]
   > Jedná se o zodpovědnost aktuálního partnera, který vytvoří lístek služby, který zahájí proces přenosu. Společnost Microsoft se nemůže zasáhnout jménem zákazníka ani nového partnera. Zákazník by měl naplánovat úzce spolupracovat s aktuálním partnerem, aby přechod přešel plynule.

2. Partner pro předplatné musí provádět následující úlohy:

   Vytvoření lístku služby Azure z partnerského centra pro vyžádání přenosu předplatného:

   1. V nabídce partnerské Centrum vyberte **zákazníky**, ze seznamu vyberte zákazníka a potom vyberte **Správa služeb**. 

   2. V části **lístky podpory** vyberte rozevírací seznam **nový lístek** a zvolte možnost **Microsoft Azure**.
   
   3. V [Azure Portal](https://portal.azure.com)vyberte **nový požadavek na podporu**.
   
   4. V kroku 1 Zvolte jako typ problému možnost **Správa předplatného** , zadejte ID předplatného, které chcete přenést, a jako plán podpory zvolte **Cloud Solution Provider** .
   
   5. V kroku 2 vyberte **C – minimální dopad** a jako typ problému zvolte **Další obecné otázky** .
   
   6. Stáhněte si [formulář pro přenos předplatného CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA).

3. Partner pro předplatné: Vyplňte [formulář pro přenos předplatného CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA), podepište ho a odešlete zákazníkovi. 

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

   Ujistěte se, že formulář obsahuje kontaktní informace pro správce partnerů. Podpora Microsoftu bude kontaktovat oba správce, aby ověřili přenos. Ujistěte se, že máte všechny tři podpisy. Pak pomocí možnosti **nahrání souboru** připojte dokončený formulář k vaší stávající žádosti o služby. Pracovník podpory Microsoftu se vám pošle zpátky během osmi pracovních hodin, aby se ověřilo přijetí a dokončení.

6. Nový partner:

   Aktualizujte nastavení předplatného Azure, aby se odebral starý partner z účtu. Pokud chcete zjistit, která přiřazení rolí se zřídí, spusťte dva prostředí PowerShell rutin.

   - Přidejte nového partnera jako prodejce na účet:

     ```powershell
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     >[!NOTE]
     > **ID tenanta** zákazníka se zobrazí v partnerském centru jako **ID Microsoftu** zákazníka. Pokud chcete najít ID (ID tenanta) Microsoftu pro konkrétního zákazníka, přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard)partnerského centra. Pak z nabídky vyberte **zákazníci** . Vyhledejte zákazníka na seznamu. Výběrem šipky dolů rozbalte seznam zákazníka. Zobrazí se informace o *názvu domény* zákazníka a **ID Microsoftu** zákazníka. Použijte 16bitový **identifikátor Microsoft ID** v prostředí PowerShell rutiny.

   - Zobrazit role na účtu, včetně předchozích partnerů CSP:

     ```powershell
     Get-AzRoleAssignment
     ```

7. Odebrat zastaralá oprávnění k přístupu

   - V nabídce partnerské Centrum vyberte **zákazníci**.
   - Vyhledejte zákazníka na seznamu. Vyberte (dvakrát klikněte) jejich název společnosti. Tím se otevře stránka **předplatné** zákazníka.
   - V nabídce podrobnosti o zákazníkovi vyberte **Správa služeb**.
   - V části **Microsoft Azure** klikněte na odkaz pro přechod na **portál pro správu Microsoft Azure**.

## <a name="next-steps"></a>Další kroky

- Stáhněte si [formulář pro přenos předplatného CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA).

- Přečtěte si další informace o [podpoře více partnerů](multipartner.md).

- [Podpora více partnerů](multipartner.md).
- [Podpora více kanálů](multichannel.md).
- [Přenos předplatných Azure](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)