---
title: Zobrazit vaše informace o motivaci a programu
ms.topic: article
ms.date: 11/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Pomocí těchto stránek můžete zobrazit a spravovat programový stav programu pobídek.
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: a66e32a3c9320ac32b0749c67197c6a27574ce75
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712609"
---
# <a name="view-your-incentives-program-details"></a>Zobrazit podrobnosti o programu pobídek

**Příslušné role**

- Motivace správce
- Motivace uživatelů
- Globální správce
- Správce partnera MPN

Tento článek popisuje stránku s **přehledem mých motivů** , která zobrazuje celkový stav vašich motivů a také stav jednotlivých programů v jednotlivých umístěních. Poskytuje také různé stavy registrace.

>[!NOTE]
>Další informace o pobídek a motivačních funkcích v partnerském centru najdete v tématu [investice a pobídky partnerů](https://partner.microsoft.com/membership/partner-incentives) (vyžaduje se přihlášení).

## <a name="access-the-incentives-overview-page"></a>Přístup k stránce s přehledem motivů

1. Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard).
1. V nabídce vyberte **motivace** a pak klikněte na **Přehled** .
1. V horní části stránky najdete souhrn příjmů a plateb a v tabulce níže najdete další podrobnosti. V doprovodné tabulce můžete také řadit, seskupovat a rozbalovat:

   - Chcete-li řadit podle sloupce, vyberte název sloupce.
   - Chcete-li seskupit podle programu, vyberte kartu **po programu** nad tabulkou.
   - Pokud chcete seskupit podle umístění, vyberte kartu **podle umístění** nad tabulkou.
   - Chcete-li zobrazit více podrobností o registraci v rámci konkrétní skupiny, vyberte symbol dvojité šipky na konci daného řádku. Tato Dvojitá šipka rozbalí vaše zobrazení.
1. Pokud se k registraci do programu vyžaduje další akce, tato informace se zobrazí ve sloupci **Stav**. V takovém případě můžete výběrem symbolu dvojité šipky zobrazit další kroky, které musíte provést.

## <a name="enrollment-status"></a>Stav registrace

Následující tabulka popisuje různé stavy registrace zobrazené ve sloupci **stav** .

| **Stav**         | **Se zobrazí, když** |
|:------------------------------------|:------------------|
| Požadovaná akce  | Partner přijal pozvánku k registraci v programu pro podnět, ale možná bude muset aktualizovat bankovní nebo daňové informace. V případě všech dalších kroků nebo odkazů na aktualizaci bank nebo daňových informací v partnerském centru se podívejte na sloupec **požadované akce** . |
| Ukončená  | Konkrétní pobídkový program již není nabízen v systému pobídek. |
| Zaregistrované  | Všechny daňové a bankovní informace byly ověřeny. Partner nepožaduje žádnou další akci registrace. |
| Probíhá registrace  | Uživatel není motivem správce a registrace je v **požadované akci** nebo při ověřování stavů **registrace** .|
| Neaktivní/neoprávněné | V tuto chvíli není možné otevřít program k registraci, nebo partner nesplňuje aktuální způsobilost k registraci nebo opětovné registraci. <br><br> Pokud je stav **nezpůsobilý**, partner nesplňuje aktuální požadavky na způsobilost pro daný program. Když vyberete odkaz **Zobrazit požadavky na způsobilost** pod stavem registrace, zobrazí se požadavky na způsobilost a které z těchto požadavků jsou splněné. <br><br> Můžete se také podívat na **neaktivní** stav VORG (Virtual Organization) nebo partnerů pro registraci globálních účtů (PGA), které už nejsou aktivní v rámci programu motivačních aktivit.  |
| Zvaný  | Partnerovi se poslala nová pozvánka k registraci programu pro motivaci, ale partner ještě nezahájil proces registrace. Sloupec sousedících, **požadovaných akcí** zobrazuje další kroky a všechny související odkazy.  |
| Ověřování registrace  | Partner již dokončil nebo aktualizoval bankovní a daňové informace pro novou nebo existující registraci a čeká, až Microsoft tyto informace ověří. Během procesu ověřování se může zdát, že se **registrace** bude zobrazovat až 48 hodin.  |

## <a name="see-your-payment-information"></a>Zobrazit vaše platební údaje

V pravém horním rohu obrazovky vyberte ikonu výběr, abyste měli přístup k těmto různým souhrnům:

- Historie transakcí
- Platby
- Exportovat data

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Ukazuje ikonu Výběr v pravém horním rohu portálu partnerského centra.":::

Mezi tyto informace patří informace o celkových příjmech a platbách v rámci pobídek od vaší registrace do programů pobídek. Na této stránce najdete také informace o příjmech a platbách podle umístění nebo programu a případné informace o všech dalších akcích, které musíte provést, pokud se chcete zaregistrovat do programu v konkrétní oblasti. 

[Rozhraní API pro výběr partnerů](https://apidocs.microsoft.com/services/partnerpayouts) můžete použít také k připojení a získání transakcí výběrů a platebních údajů přímo. Další informace najdete v tématu [Výběr příkazů](payout-statement.md) .

## <a name="next-steps"></a>Další kroky

- [Výpisy plateb](payout-statement.md)
