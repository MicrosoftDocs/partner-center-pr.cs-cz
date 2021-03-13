---
title: Nárok na přenos – pokyny pro přenos předplatného mezi fakturačními účty, Azure Marketplace
description: Pokyny pro komerční kontroly před převodem předplatného mezi fakturačními účty v Azure Portal.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 4b235bd462915fc205813ae86e92f98b4fd49fe4
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412552"
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

