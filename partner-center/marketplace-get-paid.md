---
title: Získání placeného centra partnera
description: přečtěte si, jak přijímat platby za tržby jako partnera microsoftu, jako je například prostřednictvím komerčních nabídek marketplace, motivačních programů a Cloud Solution Provider programu. Zahrnuje zásady pro výběr, stav blokování a výběr příkazů.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
ms.date: 07/12/2021
author: eunjkim520
ms.author: eunjkim
ms.openlocfilehash: 99cc0172f9cb1e09bdc77bbd9187ad2452c19c61
ms.sourcegitcommit: 207c86406e56346d01d85ce50ea494c0c293519a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/14/2021
ms.locfileid: "113798132"
---
# <a name="getting-paid-in-partner-center"></a>Získání placeného centra partnera

**Příslušné role**: správce účtu | Globální správce

Tento článek obsahuje důležité informace o tom, jak přijímat platby za vaše nabídky, doplňky a příjmy z reklamy. Shrnuje seznam vypsaných zásad, kroky požadované před zaplacením a výpisem příkazu výběr.

## <a name="payout-policies-and-agreements"></a>Výběr zásad a smluv

Při získání placeného vyžadování musíte dodržovat zásady smluv a výběr.

- [smlouva Microsoft Azure Marketplace Publisher](/legal/marketplace/msft-publisher-agreement): před tím, než se vyhradíte, musíte přijmout tuto smlouvu vydavatele. Tato smlouva vysvětluje vztah mezi vámi a Microsoftem, protože se vztahuje na prodávající nabídky na komerčním webu Marketplace, včetně poplatků za Store, které Microsoft účtuje za každý prodej.
- [Zásada výběrů](payout-policy-details.md) zobrazuje zásady plateb na výběr, včetně platebního plánu a způsobů platby. Zásada také vysvětluje proces pro zákazníky, kteří nepoužívají platby.
- [daňové detaily](tax-details-marketplace.md) vysvětlují daňovou pozornost pro výběr ceny a zodpovědnost za daň v rámci [smlouvy Microsoft Publisher](/legal/marketplace/msft-publisher-agreement).
- **Poplatky za Store** jsou oficiálně poskytovány na [komerčních poplatcích na webu Marketplace](/azure/marketplace/marketplace-commercial-transaction-capabilities-and-considerations).
- **Platby** se účtují měsíčně (za předpokladu, že prahová hodnota platby byla splněná). Obvykle posíláme jakékoli platby splatné v daném měsíci do 15. dne v měsíci. Platby obecně přijímají 3 až 10 dalších pracovních dnů k přístupu k vašemu účtu na výběr. Podrobnosti najdete v tématu [prahové hodnoty pro platby, metody a časové rámce](payment-thresholds-methods-timeframes.md).

## <a name="prerequisite-steps-before-getting-paid"></a>Před platbami požadovaných kroků

Před tím, než se vyhradíte poprvé, musíte nastavit svůj účet pro výběr a dokončit nezbytné bankovní a daňové formuláře. V bankách a daňovém formuláři budete poskytovat preferované způsoby platby a daňové formuláře pro srážkovou daň. Než budeme platit, je nutné, abyste si vyplatili daňové a daňové formuláře. Podrobnosti najdete v tématu [Nastavení účtu výběr a daňového formuláře](set-up-your-payout-account.md).

### <a name="payout-hold-status"></a>Stav blokování ve výběr

Ve výchozím nastavení pošleme platby měsíčně, jak je popsáno výše. Můžete však určit, jaké výběry programu podržíte, a společnost Microsoft neuvolní vaše platby na váš účet. Pokud se rozhodnete, že vaše výběry podržíte, budeme na stránce vydaných vydaných **výběrů** pokračovat v evidenci všech příjmů. Do vašeho účtu ale nepošleme žádné platby, dokud ho neodeberete.

pokud chcete své platby zablokovat, **Nastavení** vyberte v pravém horním rohu ikonu ozubeného kolace a pak **nastavení účtu**. V nabídce vlevo vyberte **Výběr a daň** a v části přiřazení k výběru **a daňovému profilu** Najděte program, pro který byste chtěli zadržené platby. Zaškrtněte políčko u **platby** pro tento program, pokud chcete uchovat platby. Stav blokování můžete kdykoli změnit, ale vaše rozhodnutí bude mít vliv na další měsíční výběr. Pokud například chcete pozastavit výběr z dubna, ujistěte se, že jste na konci března nastavili stav blokování vstupu na **zapnuto** .

Jakmile nastavíte stav blokování výběru **na zapnuto**, budou všechny výběry pro tento program pozastaveny, dokud nezrušíte zaškrtnutí **políčka.** Když to uděláte, budete zahrnuti během měsíčního cyklu výběrů (za předpokladu, že byla dodržena prahová hodnota platby). Pokud máte vaše výběry podržené, ale chcete mít vygenerovaný výběr v červnu, zrušte zaškrtnutí **políčka před** koncem května.

>[!Note]
> váš výběr se vztahuje na každý program zvlášť (Microsoft Store, inzerce, Azure Marketplace atd.). Pokud chcete uchovávat platby pro všechny své programy, požádejte o každý program každou platbu zvlášť.

## <a name="payout-statements"></a>Výpisy plateb

V příkazu výběr se zobrazí tržby z prodeje z nabídek a doplňků v historii transakcí. Můžete si také prohlédnout podrobnosti o platbě a stáhnout sestavy ve formátu TSV nebo CSV. Další informace o přístupu k příkazu výběr a podrobnostech o historii transakcí a platebních sestavách naleznete v tématu [Výběr příkazů](payout-statement.md) . Kromě toho můžete použít [rozhraní API pro výběr partnerů](https://apidocs.microsoft.com/services/partnerpayouts) k systematickému vyžádání sestav výběrů.

## <a name="next-steps"></a>Další kroky

- [Rozhraní API pro výběry partnerů](https://apidocs.microsoft.com/services/partnerpayouts)
- [Nejčastější dotazy k platbám](payout-faq.yml)