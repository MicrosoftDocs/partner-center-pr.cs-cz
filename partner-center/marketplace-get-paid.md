---
title: Placení v Partnerské centrum
description: Seznamte se s příjmem plateb za příjmy jako partner Microsoftu, například prostřednictvím nabídek na komerčním marketplace, programů pobídek a Cloud Solution Provider programu. Zahrnuje zásady výplaty, stav výplaty a výpisy výplat.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
ms.date: 11/25/2020
author: eunjkim520
ms.author: eunjkim
ms.openlocfilehash: 3dc8b728ef20da77b9a6d2a925ebb0388ea53837
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146489"
---
# <a name="getting-paid-in-partner-center"></a>Placení v Partnerské centrum

**Odpovídající role:** Správce účtu | Globální správce

Tento článek obsahuje důležité informace o příjmu plateb za vaše nabídky, doplňky a příjmy z reklamy. Shrnuje zásady vyplácení, kroky potřebné před získáním platby a přehled výpisu platby.

## <a name="payout-policies-and-agreements"></a>Zásady a smlouvy o platbách

Placení vyžaduje, abyste dodržovali smlouvy a zásady výplaty.

- [Microsoft Azure Marketplace smlouvy s vydavatelem:](/legal/marketplace/msft-publisher-agreement)Před placení musíte tuto smlouvu s vydavatelem přijmout. Tato smlouva vysvětluje vztah mezi vámi a Microsoftem, protože se týká nabídek prodejců na komerčním marketplace, včetně poplatku za obchod, který Microsoft účtuje za každý provedený prodej.
- [Zásady plateb zobrazují](payout-policy-details.md) zásady plateb plateb, včetně platebního plánu a způsobů platby. Zásada také vysvětluje proces nezadání zákazníky.
- [Podrobnosti o daních](tax-details-marketplace.md) vysvětlují daňové aspekty výběru ceny a daňové odpovědnosti v rámci Smlouvy s [vydavatelem Microsoftu.](/legal/marketplace/msft-publisher-agreement)
- **Poplatky za** obchod se oficiálně definují ve smlouvě s vydavatelem. Store fee is applied to all offer sales collected by the commercial marketplace, including add-ons.
- **Platby** se provádí měsíčně (za předpokladu, že byla splněna prahová hodnota platby). Všechny splatné platby za daný měsíc obvykle zašleme do 15. dne daného měsíce. K dosažení platebního účtu obecně platí 3 až 10 dalších pracovních dnů. Podrobnosti najdete v tématu [Prahové hodnoty, metody a časové rámce plateb.](payment-thresholds-methods-timeframes.md)

## <a name="prerequisite-steps-before-getting-paid"></a>Před platbami požadovaných kroků

Před tím, než se vyhradíte poprvé, musíte nastavit svůj účet pro výběr a dokončit nezbytné bankovní a daňové formuláře. V bankách a daňovém formuláři budete poskytovat preferované způsoby platby a daňové formuláře pro srážkovou daň. Než budeme platit, je nutné, abyste si vyplatili daňové a daňové formuláře. Podrobnosti najdete v tématu [Nastavení účtu výběr a daňového formuláře](set-up-your-payout-account.md).

### <a name="payout-hold-status"></a>Stav blokování ve výběr

Ve výchozím nastavení pošleme platby měsíčně, jak je popsáno výše. Můžete však určit, jaké výběry programu podržíte, a společnost Microsoft neuvolní vaše platby na váš účet. Pokud se rozhodnete, že vaše výběry podržíte, budeme na stránce vydaných vydaných **výběrů** pokračovat v evidenci všech příjmů. Do vašeho účtu ale nepošleme žádné platby, dokud ho neodeberete.

Pokud chcete své platby zablokovat, vyberte ikonu ozubeného kolečka pro **Nastavení** v pravém horním rohu a pak klikněte na **Nastavení účtu**. V nabídce vlevo vyberte **Výběr a daň** a v části přiřazení k výběru **a daňovému profilu** Najděte program, pro který byste chtěli zadržené platby. Zaškrtněte políčko u **platby** pro tento program, pokud chcete uchovat platby. Stav blokování můžete kdykoli změnit, ale vaše rozhodnutí bude mít vliv na další měsíční výběr. Pokud například chcete pozastavit výběr z dubna, ujistěte se, že jste na konci března nastavili stav blokování vstupu na **zapnuto** .

Jakmile nastavíte stav blokování výběru **na zapnuto**, budou všechny výběry pro tento program pozastaveny, dokud nezrušíte zaškrtnutí **políčka.** Když to uděláte, budete zahrnuti během měsíčního cyklu výběrů (za předpokladu, že byla dodržena prahová hodnota platby). Pokud máte vaše výběry podržené, ale chcete mít vygenerovaný výběr v červnu, zrušte zaškrtnutí **políčka před** koncem května.

>[!Note]
> Váš výběr se vztahuje na každý program zvlášť (Microsoft Store, inzerce, Azure Marketplace atd.). Pokud chcete uchovat platby za všechny programy, udržte platbu za každý program jednotlivě.

## <a name="payout-statements"></a>Výpisy plateb

Výpis platby zobrazuje vaše příjmy z prodeje z vašich nabídek a doplňků v historii transakcí. Můžete také zobrazit podrobnosti o platbě a stáhnout sestavy ve formátu tsv nebo csv. Další [informace o přístupu k](payout-statement.md) výpisu plateb a podrobnostech o historii transakcí a sestavách plateb najdete v tématu Výpisy plateb. Kromě toho můžete k systematickému vytažení sestav [o platbách](https://apidocs.microsoft.com/services/partnerpayouts) použít rozhraní API pro výplaty partnerů.

## <a name="next-steps"></a>Další kroky

- [Rozhraní API pro výplaty partnerů](https://apidocs.microsoft.com/services/partnerpayouts)
- [Nejčastější dotazy k platbám](payout-faq.md)