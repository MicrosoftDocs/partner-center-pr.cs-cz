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
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a><span data-ttu-id="fbc92-103">Přenos nároků na předplatné mezi fakturačními účty</span><span class="sxs-lookup"><span data-stu-id="fbc92-103">Transfer eligibility for a subscription between billing accounts</span></span>

<span data-ttu-id="fbc92-104">Předplatné můžete [přenést](/azure/cost-management-billing/understand/subscription-transfer) z jednoho fakturačního účtu na jiný v části fakturace Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="fbc92-104">You can [transfer a subscription](/azure/cost-management-billing/understand/subscription-transfer) from one billing account to another in the billing section of the Azure portal.</span></span> <span data-ttu-id="fbc92-105">Před přenosem je předplatné prohledáváno pro produkty třetích stran.</span><span class="sxs-lookup"><span data-stu-id="fbc92-105">Prior to a transfer, the subscription is scanned for third-party products.</span></span> <span data-ttu-id="fbc92-106">Přenos je povolený jenom v případě, že se pro přenos vymažou *všechny* produkty (viz následující [kritéria](#criteria-for-transfer-approval-or-denial) ).</span><span class="sxs-lookup"><span data-stu-id="fbc92-106">The transfer is permitted only if *all* products are cleared for transfer (see the [criteria](#criteria-for-transfer-approval-or-denial) below).</span></span> <span data-ttu-id="fbc92-107">Systém vygeneruje relevantní chybové zprávy pro aplikace, které se nepodařilo vymazat, abyste mohli určit další kroky.</span><span class="sxs-lookup"><span data-stu-id="fbc92-107">The system will generate relevant error messages for the apps that failed to clear to help you determine next steps.</span></span>

> [!NOTE]
> <span data-ttu-id="fbc92-108">Tento článek neplatí pro nabídky SaaS, protože prostředky SaaS jsou připojené ke klientovi, ne k předplatnému.</span><span class="sxs-lookup"><span data-stu-id="fbc92-108">This article does not apply to SaaS offers because SaaS resources are attached to a tenant, not a subscription.</span></span> <span data-ttu-id="fbc92-109">Prostředky SaaS se přenášejí z jednoho fakturačního účtu na jiný, ale to se provádí na základě prostředků a podpory Azure jako žádosti o podporu.</span><span class="sxs-lookup"><span data-stu-id="fbc92-109">SaaS resources are transferable from one billing account to another, but this is done per resource and by Azure support as a support request.</span></span>

## <a name="criteria-for-transfer-approval-or-denial"></a><span data-ttu-id="fbc92-110">Kritéria pro schválení nebo zamítnutí přenosu</span><span class="sxs-lookup"><span data-stu-id="fbc92-110">Criteria for transfer approval or denial</span></span>

<span data-ttu-id="fbc92-111">Předplatné nejde přenést, pokud některý z jeho aplikací třetí strany splňuje některá z následujících kritérií:</span><span class="sxs-lookup"><span data-stu-id="fbc92-111">You cannot transfer a subscription if any of its third-party apps meet any of the following criteria:</span></span>

- <span data-ttu-id="fbc92-112">Cílový účet je komerční a aplikace se odsouhlasí, aby se dala prodávat přes partnery.</span><span class="sxs-lookup"><span data-stu-id="fbc92-112">The target account is commercial and the app is opt-out to be sold via partners.</span></span>
- <span data-ttu-id="fbc92-113">Aplikace se pro vybrané partnery odsouhlasí a cílový účet není v seznamu povolených.</span><span class="sxs-lookup"><span data-stu-id="fbc92-113">The app is opt-in for selected partners and the target account is not in the allow list.</span></span>
- <span data-ttu-id="fbc92-114">Nabídka byla v minulosti nabídka Preview pro vybraná předplatná nebo byla soukromá nabídka a předplatné už není v seznamu povolených.</span><span class="sxs-lookup"><span data-stu-id="fbc92-114">The offer was a preview offer in the past for selected subscriptions or was a private offer and the subscription is no longer in the allow list.</span></span>
- <span data-ttu-id="fbc92-115">Nový fakturační účet se nachází v jiné oblasti, než je nabídka prodávaná a nabídka se v této oblasti neprodává.</span><span class="sxs-lookup"><span data-stu-id="fbc92-115">The new billing account is in a region different from where the offer is sold AND the offer is not to be sold in that region.</span></span>

<span data-ttu-id="fbc92-116">Blokovaný přenos zůstane v platnosti, dokud neodeberete prostředek z předplatného, a potom ho můžete zkusit přenést znovu.</span><span class="sxs-lookup"><span data-stu-id="fbc92-116">A blocked transfer remains in effect until you remove the resource from the subscription, after which you can try the transfer again.</span></span>

## <a name="next-steps"></a><span data-ttu-id="fbc92-117">Další kroky</span><span class="sxs-lookup"><span data-stu-id="fbc92-117">Next steps</span></span>

[<span data-ttu-id="fbc92-118">Získat podporu pro Microsoft AppSource a Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="fbc92-118">Get support for Microsoft AppSource and Azure Marketplace</span></span>](get-support.md)

