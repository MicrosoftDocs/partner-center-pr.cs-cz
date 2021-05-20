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
ms.openlocfilehash: 5294495403be729adecb5a7814ade4f9d454a0f6
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149821"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a>Přizpůsobení prostředí prvního spuštění nových zařízení s využitím profilů Windows Autopilot

**Příslušné role**: Agent správce | Globální správce | Prodejní agent | Správce správy uživatelů

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

- Přeskočit stránky nastavení registrace Cortany, OneDrive a OEM Všechna zařízení zaregistrovaná pomocí Autopilotu tyto stránky automaticky přeskočí během procesu spuštění zařízení.

- Přeskočte licenční smlouvu s koncovým uživatelem (EULA). Počínaje Windows 10 verze 1709 se organizace mohou rozhodnout přeskočit stránku se seznamem eula prezentovaných během procesu OOBE. Důležité Windows Autopilot o přeskočení stránky [eula](#windows-autopilot-eula-dismissal) během instalace Windows najdete níže v části o zamítnutí eula.

Pro správu profilů a zařízení platí následující oprávnění a omezení:

- Partneři CSP můžou dál spravovat profily Autopilot pro stávající zákazníky, se kterými mají vztah na úrovni prodejce, a to i v případě, že jim zákazníci odebrali delegované oprávnění správce.

- Pro zákazníky můžete spravovat existující zařízení, která jste přidali.

- Nemůžete spravovat zařízení, která zákazník nahrál na Microsoft pro firmy nebo portál Microsoft Intune.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Vytváření a správa profilů Autopilotu v Partnerské centrum

V Partnerské centrum můžete vytvořit profily Windows Autopilot nasazení a použít je na zařízení.

>[!NOTE]
>Profily mohou vytvářet a používat pouze agenti správy.

### <a name="create-a-new-autopilot-profile"></a>Vytvoření nového profilu Autopilotu

1. V **nabídce** Partnerské centrum vyberte Zákazníci a pak vyberte zákazníka, pro který vytváříte profil Autopilot.

2. Na stránce podrobností zákazníka vyberte **Zařízení.**

3. V **Windows Autopilot profilů** vyberte Přidat nový **profil.**

4. Zadejte název a popis profilu a pak nakonfigurujte nastavení OOBE. Vybírejte z těchto možností:  

   - Přeskočení nastavení ochrany osobních údajů v nastavení

   - Zakázání účtu místního správce v nastavení
  
   - Automatické přeskočení stránek v nastavení<br>
        (Zahrnuje *automaticky vybrat nastavení pro pracovní nebo* školní a přeskočit stránky nastavení *cortany, OneDrivu a registrace OEM*)
  
   - Přeskočení licenční smlouvy s koncovým uživatelem (EULA)<br> 
       >[!IMPORTANT] 
       >Důležité Windows Autopilot o přeskočení stránky [eula](#windows-autopilot-eula-dismissal) během instalace Windows najdete níže v části o zamítnutí eula.

5. Po **dokončení vyberte** Odeslat.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Použití profilu Autopilot na zařízeních zákazníků

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

Jakmile se zařízení zákazníka připojí k Internetu, stáhne nejnovější verzi profilu během procesu OOBE. Pokaždé, když zákazník obnoví zařízení do výchozího továrního nastavení, zařízení znovu stáhne nejnovější verzi profilu během procesu OOBE.

1. V **nabídce** Partnerské centrum vyberte Zákazníci a pak vyberte zákazníka, který chce, abyste změnili profil Autopilot.

2. Na stránce podrobností zákazníka vyberte **Zařízení.**

3. V **Windows Autopilot profilů** vyberte profil, který potřebujete aktualizovat. Proveďte požadované změny a pak vyberte **Odeslat.**

Pokud chcete tento profil odstranit, **vyberte Odstranit profil** v pravém horním rohu stránky.

### <a name="add-devices-to-a-customers-account"></a>Přidání zařízení do účtu zákazníka

>[!NOTE]
>Agenti prodeje a agenti pro správu mohou přidávat zařízení do účtu zákazníka.

Abyste mohli použít vlastní profily Autopilotu na zákaznická zařízení, musíte mít přístup k seznamu zařízení zákazníka.

Pokud plánujete použít kombinaci názvu, sériového čísla a modelu výrobce OEM, uvědomte si tato omezení:

- Tato řazená kolekce členů funguje pouze pro novější zařízení (například 4k hash) a nepodporuje se pro 128b hash (RS2 a předchozí zařízení).

- V registraci řazené kolekce členů se rozlišují velká a  malá písmena, takže data v souboru musí odpovídat názvům modelu a výrobce přesně tak, jak poskytuje poskytovatel OEM (poskytovatel hardwaru).

Podle následujících pokynů přidejte zařízení do účtu zákazníka v Partnerské centrum.

1. V **nabídce** Partnerské centrum vyberte Zákazníci a pak vyberte zákazníka, jehož zařízení chcete spravovat.

2. Na stránce podrobností zákazníka vyberte **Zařízení.**

3. V **části Použít profily u zařízení** vyberte Přidat **zařízení.**

4. Zadejte název seznamu zařízení a  pak vyberte Procházet a nahrajte seznam zákazníka (ve formátu souboru .csv) do Partnerské centrum.

    >[!NOTE]
    >Tento soubor .csv byste měli mít při nákupu zařízení. Pokud jste neobdrží soubor .csv, můžete si ho vytvořit sami podle postupu v tématu Přidání zařízení [do Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).  

5. Nahrajte soubor .csv a pak vyberte **Uložit.**

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