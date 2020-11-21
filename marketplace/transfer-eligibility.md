---
title: Nárok na přenos – pokyny pro přenos předplatného mezi fakturačními účty, Azure Marketplace
description: Pokyny pro komerční kontroly před převodem předplatného mezi fakturačními účty v Azure Portal.
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: a6a3c8954643ea982ae5107ae417a900ed51e77d
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007468"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a>Přenos nároků na předplatné mezi fakturačními účty

Předplatné můžete [přenést](/azure/cost-management-billing/understand/subscription-transfer) z jednoho fakturačního účtu na jiný v části fakturace Azure Portal. Před přenosem je předplatné prohledáváno pro produkty třetích stran. Přenos je povolený jenom v případě, že se pro přenos vymažou *všechny* produkty (viz následující [kritéria](#criteria-for-transfer-approval-or-denial) ). Systém vygeneruje relevantní chybové zprávy pro aplikace, které se nepodařilo vymazat, abyste mohli určit další kroky.

> [!NOTE]
> Tento článek neplatí pro nabídky SaaS, protože prostředky SaaS jsou připojené ke klientovi, ne k předplatnému. Prostředky SaaS se přenášejí z jednoho fakturačního účtu na jiný, ale to se provádí na základě prostředků a podpory Azure jako žádosti o podporu.

## <a name="criteria-for-transfer-approval-or-denial"></a>Kritéria pro schválení nebo zamítnutí přenosu

Předplatné nejde přenést, pokud některý z jeho aplikací třetí strany splňuje některá z následujících kritérií:

- Cílový účet je komerční a aplikace se odsouhlasí, aby se dala prodávat přes partnery.
- Aplikace se pro vybrané partnery odsouhlasí a cílový účet není v seznamu povolených.
- Nabídka byla v minulosti nabídka Preview pro vybraná předplatná nebo byla soukromá nabídka a předplatné už není v seznamu povolených.
- Nový fakturační účet se nachází v jiné oblasti, než je nabídka prodávaná a nabídka se v této oblasti neprodává.

Blokovaný přenos zůstane v platnosti, dokud neodeberete prostředek z předplatného, a potom ho můžete zkusit přenést znovu.

## <a name="next-steps"></a>Další kroky

[Získat podporu pro Microsoft AppSource a Azure Marketplace](get-support.md)

