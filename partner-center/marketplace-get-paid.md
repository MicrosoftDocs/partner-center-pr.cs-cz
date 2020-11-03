---
title: Vyplácení na komerčním marketplace
description: Přečtěte si o přijímání plateb za tržby na komerčním webu Marketplace – Azure Marketplace. Zahrnuje zásadu výběr, stav blokování a příkazy pro výběr.
ms.service: marketplace
ms.topic: conceptual
ms.date: 09/28/2020
author: eunjkim520
ms.author: eunjkim
ms.openlocfilehash: db347387df29dc36e256881546e632bd321dfde5
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/19/2020
ms.locfileid: "92527758"
---
# <a name="getting-paid-in-the-commercial-marketplace"></a>Vyplácení na komerčním marketplace

Tento článek obsahuje důležité informace o tom, jak přijímat platby za vaše nabídky, doplňky a příjmy z reklamy. Shrnuje seznam vypsaných zásad, kroky požadované před zaplacením a výpisem příkazu výběr.

## <a name="commercial-marketplace-payout-policies-and-agreements"></a>Zásady a smlouvy pro výběr komerčního tržiště

Při získání placeného vyžadování musíte dodržovat zásady smluv a výběr.

- [Smlouva Microsoft Azure Marketplace vydavatele](https://go.microsoft.com/fwlink/p/?LinkID=699560): před platbami musíte přijmout tuto smlouvu vydavatele. Tato smlouva vysvětluje vztah mezi vámi a Microsoftem, protože se vztahuje na prodávající nabídky na komerčním webu Marketplace, včetně poplatků za Store, které Microsoft účtuje za každý prodej.
- [Zásada výběrů](payout-policy-details.md) zobrazuje zásady plateb na výběr, včetně platebního plánu a způsobů platby. Zásada také vysvětluje proces pro zákazníky, kteří nepoužívají platby.
- [Daňové detaily](tax-details-marketplace.md) vysvětlují daňovou pozornost pro výběr ceny a zodpovědnost za daň v rámci [smlouvy Microsoft Publisher](https://go.microsoft.com/fwlink/p/?LinkID=699560).
- **Poplatky za Store** jsou v rámci smlouvy vydavatele oficiálně definovány. Poplatek za Store se použije na všechny prodejní nabídky shromážděné komerčním Marketplace, včetně doplňků.
- **Platby** se účtují měsíčně (za předpokladu, že prahová hodnota platby byla splněná). Obvykle posíláme jakékoli platby splatné v daném měsíci do 15. dne v měsíci. Platby obecně přijímají 3 až 10 dalších pracovních dnů k přístupu k vašemu účtu na výběr. Podrobnosti najdete v tématu [prahové hodnoty pro platby, metody a časové rámce](payment-thresholds-methods-timeframes.md).

## <a name="prerequisite-steps-before-getting-paid"></a>Před platbami požadovaných kroků

Před tím, než se vyhradíte poprvé, musíte nastavit svůj účet pro výběr a dokončit nezbytné bankovní a daňové formuláře. V bankách a daňovém formuláři budete poskytovat preferované způsoby platby a daňové formuláře pro srážkovou daň. Než budeme platit, je nutné, abyste si vyplatili daňové a daňové formuláře. Podrobnosti najdete v tématu [Nastavení účtu výběr a daňového formuláře](set-up-your-payout-account.md).

### <a name="payout-hold-status"></a>Stav blokování ve výběr

Ve výchozím nastavení pošleme platby měsíčně, jak je popsáno výše. Máte ale možnost umístit své výběry do pozastaveného programu a společnost Microsoft neuvolní vaše platby na váš účet. Pokud se rozhodnete, že vaše výběry podržíte, budeme na stránce vydaných vydaných **výběrů** pokračovat v evidenci všech příjmů. Do vašeho účtu ale nepošleme žádné platby, dokud ho neodeberete.

Pokud chcete své platby zablokovat, přečtěte si **Nastavení účtu** . V části **Výběr a daň** vyberte v části **přiřazení do výběrového a daňového profilu** program, pro který chcete, aby se platby držely. Zaškrtněte políčko u **platby** pro tento program, pokud chcete uchovat platby. Stav blokování můžete kdykoli změnit, ale vaše rozhodnutí bude mít vliv na další měsíční výběr. Pokud například chcete pozastavit výběr z dubna, ujistěte se, že jste na konci března nastavili stav blokování vstupu na **zapnuto** .

Jakmile nastavíte stav blokování výběru **na zapnuto** , budou všechny výběry pro tento program pozastaveny, dokud nezrušíte zaškrtnutí **políčka.** Když to uděláte, budete zahrnuti během měsíčního cyklu výběrů (za předpokladu, že byla dodržena prahová hodnota platby). Pokud máte vaše výběry podržené, ale chcete mít vygenerovaný výběr v červnu, zrušte zaškrtnutí **políčka před** koncem května.

>[!Note]
> Váš výběr se vztahuje na každý program zvlášť (Microsoft Store, inzerce, Azure Marketplace atd.). Pokud chcete uchovávat platby pro všechny své programy, požádejte o každý program každou platbu zvlášť.

## <a name="payout-statements"></a>Výpisy plateb

V příkazu výběr se zobrazí tržby z prodeje z nabídek a doplňků v historii transakcí. Můžete si také prohlédnout podrobnosti o platbě a stáhnout sestavy ve formátu TSV nebo CSV. Další informace o přístupu k příkazu výběr a podrobnostech o historii transakcí a platebních sestavách naleznete v tématu [Výběr příkazů](payout-statement.md) . Kromě toho můžete použít [rozhraní API pro výběr partnerů](https://apidocs.microsoft.com/services/partnerpayouts) k systematickému vyžádání sestav výběrů.

## <a name="next-steps"></a>Další kroky

- [Rozhraní API pro výběry partnerů](https://apidocs.microsoft.com/services/partnerpayouts)
- [Nejčastější dotazy k výběrům Marketplace](payout-faq.md)
