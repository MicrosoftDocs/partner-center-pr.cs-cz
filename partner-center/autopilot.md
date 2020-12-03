---
title: Přizpůsobení připraveného prostředí zařízení
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Předtím, než dodáte nové zařízení zákazníka, můžete použít profily Windows autopilotu k přizpůsobení nebo předběžnému nastavení prostředí pro počáteční nastavení zařízení.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 12057d50e4456dd2450ff497e00c89a9afa5dc4d
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534981"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a>Přizpůsobení prostředí prvního spuštění nových zařízení s využitím profilů Windows Autopilot

**Příslušné role**

- Agent správce
- Globální správce
- Agent prodeje
- Správce správy uživatelů

Pokud spravujete zákaznická zařízení, možná budete muset pro uživatele zákazníka přizpůsobit integrované prostředí (OOBE). Před dodáním zařízení zákazníkům a uplatněním nových profilů na zařízení, která si zákazníci už koupili, můžete předem nakonfigurovat nová zařízení pomocí profilů Windows autopilotu. 

Všimněte si, že výrobci OEM začali včetně dodacího štítku na vnějším panelu zařízení autopilotu, který zobrazuje **ID kódu Product Key zařízení (PKID)**.  Tento jednorozměrný čárový kód poskytuje podřízeným partnerům způsob, jak registrovat zařízení pro autopilota, aniž by museli zařízení Unbox a získat ID zařízení alternativním způsobem.

Tento článek vysvětluje, jak vytvořit a použít profily autopilotu na zařízeních v partnerském centru.

Pokud ještě nejste obeznámeni s autopilotem, přečtěte si informace v těchto článcích:

- [Přehled Windows Autopilotu](/windows/deployment/windows-10-auto-pilot)
- [Referenční příručka k nasazení autopilotu](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Přehled

Pomocí funkce Windows Autopilot v partnerském centru můžete vytvořit vlastní profily, které se použijí na zákaznická zařízení. Následující nastavení profilu byla k dispozici v době publikování tohoto článku:

- Přeskočit nastavení ochrany osobních údajů. Toto volitelné nastavení profilu autopilotu umožňuje organizacím, aby během procesu OOBE nežádali o nastavení ochrany osobních údajů.

- V zařízení zakažte vytváření účtu místního správce. Organizace se můžou rozhodnout, jestli uživatel, který má nastavení zařízení, musí mít po dokončení procesu přístup správce.

- Automaticky nastaví zařízení pro práci nebo školu. Všechna zařízení zaregistrovaná pomocí automatického pilotního projektu se automaticky považují za pracovní nebo školní zařízení, takže se během procesu OOBE nebude zobrazovat výzva.

- Přeskočit stránky nastavení registrace Cortany, OneDrive a OEM Všechna zařízení zaregistrovaná pomocí automatického pilotního nasazení automaticky přeskočí tyto stránky během procesu spouštěného při prvním spuštění počítače.

- Přeskočte si licenční smlouvu s koncovým uživatelem (EULA). Od verze 1709 ve Windows 10 se můžou organizace rozhodnout přeskočit stránku EULA, která se zobrazí během procesu OOBE. Důležité informace, které je třeba vzít v úvahu při přeskočení stránky EULA při instalaci systému Windows, najdete v článku o [neúspěšném odeslání služby Windows autopilot](#windows-autopilot-eula-dismissal) .

Pro správu profilů a zařízení platí následující oprávnění a omezení:

- Partneři CSP můžou dál spravovat profily Autopilot pro stávající zákazníky, se kterými mají vztah na úrovni prodejce, a to i v případě, že jim zákazníci odebrali delegované oprávnění správce.

- Pro zákazníky můžete spravovat existující zařízení, která jste přidali.

- Nemůžete spravovat zařízení, která zákazník nahrál na Microsoft pro firmy nebo portál Microsoft Intune.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Vytváření a Správa profilů pro Autopilot v partnerském centru

V partnerském centru můžete vytvořit profily nasazení Windows autopilot a použít je na zařízení.

>[!NOTE]
>Profily můžou vytvářet a používat jenom agenti pro správu.

### <a name="create-a-new-autopilot-profile"></a>Vytvoření nového profilu autopilotu

1. V nabídce partnerského centra vyberte **zákazníci** a pak vyberte zákazníka, pro který vytváříte profil pro autopilot.

2. Na stránce s podrobnostmi zákazníka vyberte **zařízení**.

3. V části **profily Windows autopilotu** vyberte **Přidat nový profil**.

4. Zadejte název a popis profilu a pak nakonfigurujte nastavení OOBE. Vybírejte z těchto možností:  

   - Přeskočit nastavení ochrany osobních údajů v instalačním programu

   - Zakázat účet místního správce v nastavení
  
   - Automaticky přeskočit stránky v instalačním programu<br>
        (Zahrnuje *automaticky výběr nastavení pracovní nebo školní* a *Přeskočit stránky pro nastavení registrace Cortany, OneDrive a OEM*)
  
   - Přeskočit licenční smlouvu s koncovým uživatelem (EULA)<br> 
       >[!IMPORTANT] 
       >Důležité informace, které je třeba vzít v úvahu při přeskočení stránky EULA při instalaci systému Windows, najdete v článku o [neúspěšném odeslání služby Windows autopilot](#windows-autopilot-eula-dismissal) .

5. Po dokončení vyberte **Odeslat** .

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Použití profilu autopilotu u zákaznických zařízení

>[!NOTE]
>Níže uvedené pokyny předpokládají, že jste už přidali zařízení zákazníka do partnerského centra a že máte přístup k seznamu zařízení. Pokud jste ještě nepřidali zařízení zákazníka, postupujte podle pokynů v části [Přidání zařízení na účet zákazníka](#add-devices-to-a-customers-account) a pak postupujte podle následujících pokynů.

Po vytvoření profilu autopilotu pro zákazníka ho můžete použít na zařízení zákazníka.

1. V nabídce partnerského centra vyberte **zákazníci** a potom vyberte zákazníka, pro který jste vytvořili profil pro autopilotu.

2. Na stránce s podrobnostmi zákazníka vyberte **zařízení**.

3. V části **použít profily na zařízení** vyberte skupiny zařízení nebo zařízení, do kterých chcete přidat profily, a pak vyberte **použít profil**. Profil, který jste právě použili, se zobrazí ve sloupci **profil** .

4. Postupujte podle následujících kroků a ověřte, zda se profil na zařízení úspěšně použije.

    a.  Připojte zařízení k síti a zapněte ho.

    b.  Ověřte, zda se zobrazí příslušné obrazovky OOBE.

    c.  Když se proces OOBE zastaví, resetujte zařízení do výchozího továrního nastavení, abyste ho připravili pro nového uživatele.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Odebrání profilu autopilotu ze zařízení zákazníka

1. V nabídce partnerského centra vyberte **zákazníci** a potom vyberte zákazníka, pro který jste vytvořili profil pro autopilotu.

2. Na stránce s podrobnostmi zákazníka vyberte **zařízení**.

3. V části **použít profily na zařízení** vyberte zařízení, ze kterých chcete profil odebrat, a pak vyberte **Odebrat profil**.

   >[!NOTE]
   >Když odeberete profil ze zařízení, profil ze seznamu se neodstraní. Pokud chcete odstranit profil, postupujte podle pokynů v části [aktualizace nebo odstranění profilu autopilotu](#update-or-delete-an-autopilot-profile).

### <a name="update-or-delete-an-autopilot-profile"></a>Aktualizace nebo odstranění profilu autopilotu

Pokud chce zákazník změnit integrované prostředí po odeslání zařízení do těchto zařízení, můžete změnit profil v partnerském centru.

Jakmile se zařízení zákazníka připojí k Internetu, stáhne nejnovější verzi profilu během procesu OOBE. I když zákazník obnoví zařízení do výchozího továrního nastavení, zařízení si znovu stáhne nejnovější verzi profilu během procesu OOBE.

1. V nabídce partnerského centra vyberte **zákazníci** a pak vyberte zákazníka, který požaduje, abyste změnili profil autopilotu.

2. Na stránce s podrobnostmi zákazníka vyberte **zařízení**.

3. V části **profily Windows autopilotu** vyberte profil, který potřebujete aktualizovat. Proveďte požadované změny a pak vyberte **Odeslat**.

Chcete-li odstranit tento profil, vyberte možnost **Odstranit profil** v pravém horním rohu stránky.

### <a name="add-devices-to-a-customers-account"></a>Přidání zařízení do účtu zákazníka

>[!NOTE]
>Prodejní agenti a agenti pro správu můžou přidat zařízení k účtu zákazníka.

Než budete moct použít vlastní profily autopilotu na zákaznická zařízení, musíte mít přístup k seznamu zařízení zákazníka.

Pokud máte v plánu používat název výrobce OEM, sériové číslo a kombinaci modelů, pamatujte na tato omezení:

- Tato řazená kolekce členů funguje jenom pro novější zařízení (například hodnoty hash 4k) a není podporovaná pro hodnoty hash 128B (RS2 a předchozí zařízení).

- Registrace řazené kolekce členů rozlišuje velká a malá písmena, takže data v souboru se musí shodovat s názvy modelů a výrobců **_přesně_* _, jak poskytuje poskytovatel OEM (poskytovatel hardwaru).

Podle pokynů níže přidejte zařízení k účtu zákazníka v partnerském centru.

1. V nabídce partnerského centra vyberte _ *zákazníci** a pak vyberte zákazníka, jehož zařízení chcete spravovat.

2. Na stránce s podrobnostmi zákazníka vyberte **zařízení**.

3. V části **použít profily na zařízení** vyberte **Přidat zařízení**.

4. Zadejte název seznamu zařízení a pak vyberte **Procházet** a nahrajte seznam zákazníků (ve formátu souboru. csv) do partnerského centra.

    >[!NOTE]
    >Tento soubor. csv byste měli při nákupu zařízení přijmout. Pokud jste neobdrželi soubor. csv, můžete si ho vytvořit sami podle kroků v části [Přidání zařízení do Windows autopilotu](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).  

5. Nahrajte soubor. csv a pak vyberte **Uložit**.

Pokud se vám při pokusu o nahrání souboru .csv zobrazí chybová zpráva, zkontrolujte formát souboru. Můžete použít pouze hodnotu hash hardwaru nebo název výrobce OEM, sériové číslo a model (v uvedeném pořadí sloupců), případně ID produktu Windows. K vytvoření seznamu zařízení můžete použít také ukázkový soubor. csv poskytnutý z odkazu vedle **Přidat zařízení** .

Váš soubor. csv by měl vypadat přibližně takto:

> **Sériové číslo zařízení, ID produktu Windows, hodnota hash hardwaru, název výrobce, model zařízení**

> **{Sériové},,, Microsoft Corporation, Surface notebooku**

>[!NOTE]
> V části název výrobce a model zařízení se rozlišují malá a velká písmena.

Pokud nevíte, jaká hodnota má být zadána pro název výrobce a model zařízení, můžete tuto akci spustit na zařízení a shromáždit správné hodnoty:

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a>Neúspěšné přijetí smlouvy EULA pro Windows autopilot

### <a name="important-information"></a>DŮLEŽITÉ INFORMACE

Windows autopilot umožňuje nakonfigurovat vlastní instalace Windows na zařízeních, která spravujete pro vaše zákazníky. Pokud k tomu má zákazník oprávnění, můžete potlačit nebo skrýt některé z nich, které se běžně uživatelům prezentují při nastavování Windows, včetně obrazovky EULA (licenční smlouva s koncovým uživatelem).

Pomocí této funkce, souhlasíte s tím, že potlačíte nebo skryjete všechny obrazovky, které jsou navržené tak, aby poskytovaly uživatelům upozornění, nebo přijetí podmínek znamená, že jste získali dostatečný souhlas a oprávnění od zákazníka ke skrytí podmínek a že jménem zákazníka (ať už je to organizace nebo jednotlivý uživatel), vyjádření souhlasu se všemi oznámeními a přijímají si podmínky, které platí pro vaše zákazníky. To zahrnuje souhlas s podmínkami a ujednáními licence nebo oznámení, která by se uživateli zobrazovala, pokud jste ho potlačili nebo skryli pomocí tohoto nástroje. Pokud zákazník nezískal licenci pro software od společnosti Microsoft nebo jejích licencovaných distributorů, nemusí na těchto zařízeních používat software Windows.