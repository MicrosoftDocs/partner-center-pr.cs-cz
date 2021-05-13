---
title: Zobrazení podrobností o pobídkách a programu
ms.topic: article
ms.date: 11/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Tyto stránky slouží k zobrazení a správě program Pobídky stavu.
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 798fde02b87e8f8105dad6d00c32b050fb90097e
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/12/2021
ms.locfileid: "109818741"
---
# <a name="view-your-incentives-program-details"></a>Zobrazení podrobností o programu pobídek

**Odpovídající role:** Správce pobídek | Uživatelské | Incentives Globální správce | Správce partnera MPN

Tento článek vysvětluje **stránku přehledu** Moje pobídky, která zobrazuje celkový stav vašich programů pobídek a také stav jednotlivých programů v jednotlivých umístěních. Poskytuje také různé stavy registrace.

>[!NOTE]
>Další informace o pobídkách a funkcích pobídek v Partnerské centrum tématu Investice a pobídky pro partnery [(vyžaduje](https://partner.microsoft.com/membership/partner-incentives) se přihlášení).

## <a name="access-the-incentives-overview-page"></a>Přístup na stránku přehledu pobídek

1. Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard).
1. Vyberte **Pobídky** a pak **v** nabídce vyberte Přehled.
1. V horní části stránky najdete souhrn příjmů a plateb a v tabulce níže najdete další podrobnosti. Doprovodnou tabulku můžete také řadit, seskupit a rozbalit:

   - Pokud chcete sloupec seřadit, vyberte název sloupce.
   - Pokud chcete seskupit podle programu, **vyberte nad tabulkou kartu** Podle programu.
   - Pokud chcete seskupit podle umístění, **vyberte nad tabulkou** kartu Podle umístění.
   - Pokud chcete zobrazit další podrobnosti o registracích v rámci konkrétní skupiny, vyberte symbol chevron na konci daného řádku. Tato chevron rozbalí vaše zobrazení.
1. Pokud se k registraci do programu vyžaduje další akce, tato informace se zobrazí ve sloupci **Stav**. V takovém případě můžete výběrem symbolu dvojité šipky zobrazit další kroky, které musíte provést.

## <a name="enrollment-status"></a>Stav registrace

Následující tabulka vysvětluje různé stavy registrace zobrazené ve **sloupci** Stav.

| **Stav**         | **Zobrazí se, když** |
|:------------------------------------|:------------------|
| Požadovaná akce  | Partner přijal pozvánku k registraci do programu pobídek, ale možná bude muset aktualizovat bankovní nebo daňové údaje. Další kroky **nebo odkazy** na aktualizaci bankovních nebo daňových údajů najdete ve sloupci Požadované akce v Partnerské centrum. |
| Přerušena  | Konkrétní pobídkový program již není nabízen v systému pobídek. |
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
