---
title: Sloučení partnerského účtu s jiným partnerským účtem
description: Zjistěte, jak sloučit partnerský účet s jiným partnerským účtem v Partnerské centrum – pro společnosti, které jsou aktivními partnery Microsoftu v Partnerské centrum.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: parthpandyaMSFT
ms.author: parthp
ms.custom: seodec18
ms.date: 06/12/2020
ms.openlocfilehash: 8c47204d54cf05113eae73cede4afedf106ac121
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146506"
---
# <a name="merge-your-partner-account-with-another-partner-account"></a>Sloučení partnerského účtu s jiným partnerským účtem

**Odpovídající role:** Správce účtu

Dvě nebo více společností, které jsou aktivními partnery Microsoftu a mají účty v Partnerské centrum si mohou zvolit sloučení svých účtů.

## <a name="what-happens-when-two-partners-elect-to-merge-their-partner-center-accounts"></a>Co se stane, když se dva partneři rozhodne sloučit své Partnerské centrum účty

- Partnerská organizace, která zahájí sloučení, bude globální účet partnera (PGA).

- Zzvaný PGA organizace se stane umístěním iniciující společnosti.

- Všechna umístění slučování účtu se stanou umístěními v rámci PGA.

- Po sloučení účtu se zobrazí podrobnosti o účtu, jako jsou umístění i uživatelé v rámci profilu PGA. Tento proces nelze vrátit zpět.

- Během této konsolidace se zachovají všechna ID MPN pro umístění.

- Role uživatelů se přenesly. Pokud by například uživatel byl správcem pobídek pro konkrétní lokalitu, měl by i po fúzi roli a mohl by vidět pobídky, které viděl před fúzí.

- Tenanti Azure AD a účty CSP se nesloučí a nemají žádný vliv.

- Publikované nabídky a data kanálu spoluproduování přidružená k oběma společnostem se zachovají.

### <a name="view-of-merged-accounts"></a>Zobrazení sloučených účtů

:::image type="content" source="images/merge-accounts/account-merge.png" alt-text="Fúze účtů":::

## <a name="what-to-expect-if-you-have-been-invited-to-merge-your-partner-center-account-with-another-partner-center-account"></a>Co očekávat, pokud jste byli pozváni ke sloučení účtu Partnerské centrum s jiným Partnerské centrum účtem

Pokud se rozhodnete přijmout pozvánku ke sloučení účtů: · Vaše ID MPN a umístění se sloučí s PGA partnerského účtu, který vás pozval.

- Vaši uživatelé se převedou do sloučeného účtu s jejich rolemi beze změny.

- Stávající výhody a kompetence budou pro obě společnosti zachovány po fúzi až do prodloužení. Při obnovení se budou účty považovat za jednu společnost a standardní pravidla obnovy.

## <a name="understand-the-impacts-to-programs-and-benefits-when-partners-elect-to-merge-accounts"></a>Pochopení dopadů na programy a výhody, když se partneři rozhodnou sloučit účty

- Všechny stávající kompetence (Gold/stříbrné), nákupy (například Microsoft Action Pack) a související výhody se během konsolidace uchovávají. Pokud mají obě společnosti stejnou kompetenci, ale jedna je zlatá a druhá stříbrná, bude udělována kompetence s nejvyšší úrovní znalostí a partneři budou mít pro tuto kompetenci jednu sadu výhod stříbra a jednu sadu zlatých výhod, dokud jejich další obnovení neproběhne. 

- Po spojení bude zachováno nejvyšší datum výročí pro sadu Microsoft Action Pack. Například pokud datum výročí pro společnost 1 je června 2020 pro obnovení sady Action Pack a datum výročí pro obnovení sady Action Pack pro společnost 2 je v 2020, bude společnost Microsoft 2020 používat datum. října, jako nové datum výročí pro sloučenou společnost.

- Během slučování účtů a až do dalšího obnovení se u každého účtu zachová jejich Akční balíček a výhody kompetence. Při obnovení se použijí standardní pravidla pro obnovení sady Action Pack a kompetence.

- Po obnovení jsou pro globální účet partnera partnerské společnosti implementovány výhody, které jsou součástí dosahování kompetence a sady Action Pack:

  - Microsoft Action Pack: Partnerská společnost bude moct zakoupit jeden globální účet pro každý partner.

  - Kompetence: Partnerská společnost dostane jeden balíček základních výhod, které jsou přidružené k jejich nejvyššímu dosahu, a výhody pro konkrétní kompetenci, na které má partner nárok na globální účet partnera.

- Na všechny výhody se vztahují [Průvodce využitím Microsoft Partner Network výhody](https://aka.ms/partner-benefits-use-guide). Příklad: aktivovaný token O365 E3 je funkční po dobu 12 měsíců od aktivace. Po aktivaci tokenu pro licence na tenanta se tyto licence nemusí přesunout do jiného tenanta.

- Asociace ID MCP pro obě společnosti budou zachovaná a přidružená k PGA MPN ID.

- Možnosti uvedení na trh a technické výhody se nabízejí jako zvýhodnění Core. Po sloučení se doporučuje zkontrolovat bankovní a daňové údaje, aby se zajistila přesnost.

- Pokud je vaše společnost v programu pro odborníky na Azure, zachová se do obnovení výhody.

- Pokud vaše společnost získala pokročilé specializace, uchovávají se v obou účtech.

- Všechny doklady Software Assurance se uchovávají v obou účtech. 

- Neexistuje žádný vliv na přidružení partnera DPOR nebo PAL. Všechny přidružené příjmové příspěvky začnou přesměrovat do nového globálního účtu partnera.

## <a name="invite-a-company-to-merge-their-partner-center-account-with-your-partner-center-account"></a>Pozvání společnosti pro sloučení účtu partnerského centra s účtem partnerského centra

>[!Note]
>K provedení fúze účtu musíte být **správcem účtu** vaší společnosti.

1. Na řídicím panelu partnerského centra vyberte **Nastavení** . 

2. Vyberte **Sloučení účtů**.

3. Přidejte ID MPN nacházející se v **partnerském profilu** účtu, který chcete s vámi vyzvat ke sloučení. Musíte použít jeho globální ID MPN partnera. Nemůžete použít umístění MPN ID.

4. Když vyberete **Sloučit**, pošle se Partnerská společnost Pozvánka. Po přijetí žádosti můžete sloučení účtů zahájit v partnerském centru. Pokud společnost vaši žádost o sloučení účtů odmítne, může vysvětlit, proč žádost zamítla. Seznam všech sloučení vašich účtů najdete v části **Historie sloučení**.
 
### <a name="example-of-two-companies-merging-accounts"></a>Příklad dvou společností, které slučují účty

1. Contoso, Ltd. má 

    a. globální [ID MPN 1111111](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) a JEDNO ID MPN podřízeného [umístění 2222222.](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)
  
    b. tenant Azure AD = @contoso.com
 
    c. gold competency that expires October 1, 2020
2. Společnost Fabrikam, Inc. má
 
    a.  globální ID MPN 333333 a ID MPN dvou podřízených umístění 4444444 a 5555555

    b.  tenant Azure AD = @fabrikam.com

    c.  dvě zlaté kompetence, které vyprší 1. prosince 2020
3.  Společnost Contoso koupí společnost Fabrikam a přejde [sem,](https://partner.microsoft.com/dashboard/account/merger) aby zahájila žádost o sloučení.
4.  Společnost Fabrikam se Partnerské centrum přihlásí a přejde na stejnou stránku, na které se #3 contoso, aby schválila žádost společnosti Contoso.
5.  Společnost Contoso na stejné stránce proše informace o sloučení a poskytne potvrzení, že může pokračovat v fúzi účtů.
6.  Po fúzi se firemní účet zobrazí takto:

    a.  Společnost Contoso s globálním ID MPN 1111111 a 4 ID MPN podřízeného umístění 2222222, 3333333, 4444444 a 5555555
    
    b.  Bude mít dva tenanty Azure AD ( + ), kteří mají přístup ke @contoso.com @fabrikam.com stejnému Partnerské centrum účtu.
    
    c.  Bude mít balíčky se dvěma výhodami kompetencí– jednu, která vyprší 1. října 2020 a druhá vyprší 1. prosince 2020. 1. prosince 2020 budou moct prodloužit platnost jako balíček výhod s jednou kompetencí. Po prodloužení si společnost Contoso zachová všechny tři kompetence, i když si může zachovat pouze jeden balíček výhod.
    
7.  Správci společnosti Contoso budou nadále spravovat Partnerské centrum role @contoso.com uživatelů společnosti Contoso. Správci společnosti Fabrikam budou nadále spravovat Partnerské centrum role @fabrikam.com uživatelů společnosti Fabrikam. Správci společnosti Contoso mohou spravovat uživatele společnosti Fabrikam pouze v případě, že jsou pozvaní jako host do tenanta společnosti Fabrikam.
8.  Společnost Contoso se může rozhodnout tenanta ignorovat a znovu pro zaměstnance Fabrikam zadat nové přihlašovací údaje s novými rolemi a @fabrikam.com @contoso.com oprávněními.

## <a name="next-steps"></a>Další kroky

- [Přiřazování uživatelských rolí a oprávnění](permissions-overview.md)

- [Ověření informací o profilu partnera](update-your-partner-profile.md)

- [Přidání Azure Partner Shared Services, aby si partneři mohli koupit předplatná Azure pro vlastní použití](shared-services.md)
