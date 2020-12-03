---
title: Prodej zákazníků Microsoft Azure rezervacích
description: Jako poskytovatel cloudového řešení můžete provádět nákup, prodej nebo správu rezervací Azure pro zákazníky. Použijte Partnerské centrum, Azure Portal nebo rozhraní API partnerského centra.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 9dc92685503fd4b9b05e40337f72e810c1693779
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534892"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="659e5-104">Prodej Microsoft Azure rezervacích zákazníkům pomocí partnerského centra, Azure Portal nebo rozhraní API</span><span class="sxs-lookup"><span data-stu-id="659e5-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="659e5-105">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="659e5-105">**Appropriate roles**</span></span>

- <span data-ttu-id="659e5-106">Agent správce</span><span class="sxs-lookup"><span data-stu-id="659e5-106">Admin agent</span></span>
- <span data-ttu-id="659e5-107">Globální správce</span><span class="sxs-lookup"><span data-stu-id="659e5-107">Global admin</span></span>
- <span data-ttu-id="659e5-108">Agent helpdesku</span><span class="sxs-lookup"><span data-stu-id="659e5-108">Helpdesk agent</span></span>
- <span data-ttu-id="659e5-109">Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="659e5-109">Sales agent</span></span>
- <span data-ttu-id="659e5-110">Správce správy uživatelů</span><span class="sxs-lookup"><span data-stu-id="659e5-110">User management admin</span></span>

<span data-ttu-id="659e5-111">Jako partner v programu Cloud Solution Provider (CSP) můžete zakoupit, prodávat nebo spravovat rezervace Azure pro zákazníky.</span><span class="sxs-lookup"><span data-stu-id="659e5-111">As a partner in the Cloud Solution Provider program (CSP), you can buy, sell, or manage Azure reservations for customers.</span></span> <span data-ttu-id="659e5-112">Použijte Partnerské centrum, Azure Portal nebo rozhraní API partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="659e5-112">Use Partner Center, the Azure portal, or the Partner Center API.</span></span>

> [!NOTE]
> <span data-ttu-id="659e5-113">Tento článek se týká jenom partnerů v CSP.</span><span class="sxs-lookup"><span data-stu-id="659e5-113">This article applies only to partners in CSP.</span></span> <span data-ttu-id="659e5-114">[Tuto dokumentaci k rezervacím Azure](/azure/cost-management-billing/reservations)by si měli přečíst zákazníci, kteří používají jiné typy předplatných (například, platby na základě průběžných plateb, jednotlivce, smlouvy o zákaznících Microsoftu nebo předplatná smlouva Enterprise).</span><span class="sxs-lookup"><span data-stu-id="659e5-114">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="659e5-115">Partneři v programu CSP mohou nabízet své zákazníky Microsoft Azure rezervacích.</span><span class="sxs-lookup"><span data-stu-id="659e5-115">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="659e5-116">Zákazníci můžou při vyhradování předem získat významné úspory.</span><span class="sxs-lookup"><span data-stu-id="659e5-116">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="659e5-117">Rezervace Azure zákazníkům nabízí jednoduchost a flexibilitu následujícími způsoby:</span><span class="sxs-lookup"><span data-stu-id="659e5-117">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="659e5-118">Jeden nebo tři roky – rezervované výrazy</span><span class="sxs-lookup"><span data-stu-id="659e5-118">One or three-year reservation terms</span></span>
- <span data-ttu-id="659e5-119">Snadné je začít. instalace dokončena během několika sekund</span><span class="sxs-lookup"><span data-stu-id="659e5-119">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="659e5-120">Zrušit nebo vyměňovat rezervované instance kdykoli pro upravenou refundaci</span><span class="sxs-lookup"><span data-stu-id="659e5-120">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="659e5-121">Správa využívání rezervovaných instancí na úrovni organizace nebo jednotlivého oddělení</span><span class="sxs-lookup"><span data-stu-id="659e5-121">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="659e5-122">Rezervace Azure můžou zákazníkům vymezit odvolání následujícími způsoby:</span><span class="sxs-lookup"><span data-stu-id="659e5-122">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="659e5-123">Rezervace můžou nabízet významné úspory v rámci cen s průběžnými platbami (PAYG).</span><span class="sxs-lookup"><span data-stu-id="659e5-123">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="659e5-124">Lepší rozpočtování a prognózování s platbami předem na jeden nebo tři roky</span><span class="sxs-lookup"><span data-stu-id="659e5-124">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="659e5-125">Prioritní výpočetní kapacitu v oblasti Azure, která je nejblíže jejich kancelářím</span><span class="sxs-lookup"><span data-stu-id="659e5-125">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="659e5-126">Rezervace Azure poskytují základ pro kompletní řešení infrastruktury v kombinaci se softwarem, jako je Microsoft Windows Server a Azure SQL Database</span><span class="sxs-lookup"><span data-stu-id="659e5-126">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="659e5-127">Rezervace Azure můžete koupit, prodávat a spravovat v partnerském centru i v Azure Portal a pomocí rozhraní API partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="659e5-127">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="659e5-128">Zákazníkům můžete taky udělit oprávnění k nákupu svých rezervací Azure z předplatného Azure, které pro ně jste zakoupili.</span><span class="sxs-lookup"><span data-stu-id="659e5-128">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="659e5-129">Pomocí níže uvedených odkazů se dozvíte, jak.</span><span class="sxs-lookup"><span data-stu-id="659e5-129">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="659e5-130">Prostředky rezervací Azure</span><span class="sxs-lookup"><span data-stu-id="659e5-130">Azure reservations resources</span></span>

|<span data-ttu-id="659e5-131">**Pro informace o**</span><span class="sxs-lookup"><span data-stu-id="659e5-131">**For information about**</span></span>   |<span data-ttu-id="659e5-132">**Přečtěte si:**</span><span class="sxs-lookup"><span data-stu-id="659e5-132">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="659e5-133">Dokumentace k rezervacím Azure pro vaše zákazníky</span><span class="sxs-lookup"><span data-stu-id="659e5-133">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="659e5-134">Co jsou rezervace Azure?</span><span class="sxs-lookup"><span data-stu-id="659e5-134">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="659e5-135">Nákup rezervací Azure pro vaše zákazníky v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="659e5-135">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="659e5-136">Nákup rezervací Azure</span><span class="sxs-lookup"><span data-stu-id="659e5-136">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="659e5-137">Správa rezervací Azure v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="659e5-137">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="659e5-138">Správa rezervací Azure v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="659e5-138">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="659e5-139">Určení správné velikosti virtuálního počítače a ověření využití virtuálního počítače zákazníkům</span><span class="sxs-lookup"><span data-stu-id="659e5-139">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="659e5-140">Změna velikosti virtuálního počítače pro maximální využití rezervace Azure</span><span class="sxs-lookup"><span data-stu-id="659e5-140">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="659e5-141">Nákup rezervací Azure pomocí rozhraní API partnerského centra</span><span class="sxs-lookup"><span data-stu-id="659e5-141">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="659e5-142">[Koupit Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) v dokumentaci pro vývojáře partnerského centra</span><span class="sxs-lookup"><span data-stu-id="659e5-142">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="659e5-143">Udělení oprávnění zákazníkům k nákupu svých vlastních rezervací Azure z předplatného CSP.</span><span class="sxs-lookup"><span data-stu-id="659e5-143">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="659e5-144">Poskytněte zákazníkům oprávnění k nákupu svých rezervací Azure.</span><span class="sxs-lookup"><span data-stu-id="659e5-144">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |