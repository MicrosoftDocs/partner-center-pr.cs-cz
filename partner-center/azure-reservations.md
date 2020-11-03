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
ms.openlocfilehash: 317d1f0295b79b79bf06f1091ae365bc7012b749
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/22/2020
ms.locfileid: "92527341"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="a5cd3-104">Prodej Microsoft Azure rezervacích zákazníkům pomocí partnerského centra, Azure Portal nebo rozhraní API</span><span class="sxs-lookup"><span data-stu-id="a5cd3-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="a5cd3-105">**Platí pro**</span><span class="sxs-lookup"><span data-stu-id="a5cd3-105">**Applies to**</span></span>

- <span data-ttu-id="a5cd3-106">Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="a5cd3-106">Partner Center</span></span>
- <span data-ttu-id="a5cd3-107">Microsoft Azure Portal</span><span class="sxs-lookup"><span data-stu-id="a5cd3-107">Microsoft Azure portal</span></span>
- <span data-ttu-id="a5cd3-108">Partneři v programu CSP</span><span class="sxs-lookup"><span data-stu-id="a5cd3-108">Partners in the CSP program</span></span>

<span data-ttu-id="a5cd3-109">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="a5cd3-109">**Appropriate roles**</span></span>

- <span data-ttu-id="a5cd3-110">Agent správce</span><span class="sxs-lookup"><span data-stu-id="a5cd3-110">Admin agent</span></span>
- <span data-ttu-id="a5cd3-111">Globální správce</span><span class="sxs-lookup"><span data-stu-id="a5cd3-111">Global admin</span></span>
- <span data-ttu-id="a5cd3-112">Agent helpdesku</span><span class="sxs-lookup"><span data-stu-id="a5cd3-112">Helpdesk agent</span></span>
- <span data-ttu-id="a5cd3-113">Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="a5cd3-113">Sales agent</span></span>
- <span data-ttu-id="a5cd3-114">Správce správy uživatelů</span><span class="sxs-lookup"><span data-stu-id="a5cd3-114">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="a5cd3-115">Tento článek se týká jenom partnerů v programu Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="a5cd3-115">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="a5cd3-116">[Tuto dokumentaci k rezervacím Azure](/azure/cost-management-billing/reservations)by si měli přečíst zákazníci, kteří používají jiné typy předplatných (například, platby na základě průběžných plateb, jednotlivce, smlouvy o zákaznících Microsoftu nebo předplatná smlouva Enterprise).</span><span class="sxs-lookup"><span data-stu-id="a5cd3-116">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="a5cd3-117">Partneři v programu CSP mohou nabízet své zákazníky Microsoft Azure rezervacích.</span><span class="sxs-lookup"><span data-stu-id="a5cd3-117">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="a5cd3-118">Zákazníci můžou při vyhradování předem získat významné úspory.</span><span class="sxs-lookup"><span data-stu-id="a5cd3-118">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="a5cd3-119">Rezervace Azure zákazníkům nabízí jednoduchost a flexibilitu následujícími způsoby:</span><span class="sxs-lookup"><span data-stu-id="a5cd3-119">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="a5cd3-120">Jeden nebo tři roky – rezervované výrazy</span><span class="sxs-lookup"><span data-stu-id="a5cd3-120">One or three-year reservation terms</span></span>
- <span data-ttu-id="a5cd3-121">Snadné je začít. instalace dokončena během několika sekund</span><span class="sxs-lookup"><span data-stu-id="a5cd3-121">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="a5cd3-122">Zrušit nebo vyměňovat rezervované instance kdykoli pro upravenou refundaci</span><span class="sxs-lookup"><span data-stu-id="a5cd3-122">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="a5cd3-123">Správa využívání rezervovaných instancí na úrovni organizace nebo jednotlivého oddělení</span><span class="sxs-lookup"><span data-stu-id="a5cd3-123">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="a5cd3-124">Rezervace Azure můžou zákazníkům vymezit odvolání následujícími způsoby:</span><span class="sxs-lookup"><span data-stu-id="a5cd3-124">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="a5cd3-125">Rezervace můžou nabízet významné úspory v rámci cen s průběžnými platbami (PAYG).</span><span class="sxs-lookup"><span data-stu-id="a5cd3-125">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="a5cd3-126">Lepší rozpočtování a prognózování s platbami předem na jeden nebo tři roky</span><span class="sxs-lookup"><span data-stu-id="a5cd3-126">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="a5cd3-127">Prioritní výpočetní kapacitu v oblasti Azure, která je nejblíže jejich kancelářím</span><span class="sxs-lookup"><span data-stu-id="a5cd3-127">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="a5cd3-128">Rezervace Azure poskytují základ pro kompletní řešení infrastruktury v kombinaci se softwarem, jako je Microsoft Windows Server a Azure SQL Database</span><span class="sxs-lookup"><span data-stu-id="a5cd3-128">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="a5cd3-129">Rezervace Azure můžete koupit, prodávat a spravovat v partnerském centru i v Azure Portal a pomocí rozhraní API partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="a5cd3-129">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="a5cd3-130">Zákazníkům můžete taky udělit oprávnění k nákupu svých rezervací Azure z předplatného Azure, které pro ně jste zakoupili.</span><span class="sxs-lookup"><span data-stu-id="a5cd3-130">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="a5cd3-131">Pomocí níže uvedených odkazů se dozvíte, jak.</span><span class="sxs-lookup"><span data-stu-id="a5cd3-131">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="a5cd3-132">Prostředky rezervací Azure</span><span class="sxs-lookup"><span data-stu-id="a5cd3-132">Azure reservations resources</span></span>

|<span data-ttu-id="a5cd3-133">**Pro informace o**</span><span class="sxs-lookup"><span data-stu-id="a5cd3-133">**For information about**</span></span>   |<span data-ttu-id="a5cd3-134">**Přečtěte si:**</span><span class="sxs-lookup"><span data-stu-id="a5cd3-134">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="a5cd3-135">Dokumentace k rezervacím Azure pro vaše zákazníky</span><span class="sxs-lookup"><span data-stu-id="a5cd3-135">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="a5cd3-136">Co jsou rezervace Azure?</span><span class="sxs-lookup"><span data-stu-id="a5cd3-136">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="a5cd3-137">Nákup rezervací Azure pro vaše zákazníky v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="a5cd3-137">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="a5cd3-138">Nákup rezervací Azure</span><span class="sxs-lookup"><span data-stu-id="a5cd3-138">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="a5cd3-139">Správa rezervací Azure v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="a5cd3-139">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="a5cd3-140">Správa rezervací Azure v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="a5cd3-140">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="a5cd3-141">Určení správné velikosti virtuálního počítače a ověření využití virtuálního počítače zákazníkům</span><span class="sxs-lookup"><span data-stu-id="a5cd3-141">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="a5cd3-142">Změna velikosti virtuálního počítače pro maximální využití rezervace Azure</span><span class="sxs-lookup"><span data-stu-id="a5cd3-142">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="a5cd3-143">Nákup rezervací Azure pomocí rozhraní API partnerského centra</span><span class="sxs-lookup"><span data-stu-id="a5cd3-143">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="a5cd3-144">[Koupit Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) v dokumentaci pro vývojáře partnerského centra</span><span class="sxs-lookup"><span data-stu-id="a5cd3-144">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="a5cd3-145">Udělení oprávnění zákazníkům k nákupu svých vlastních rezervací Azure z předplatného CSP.</span><span class="sxs-lookup"><span data-stu-id="a5cd3-145">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="a5cd3-146">Poskytněte zákazníkům oprávnění k nákupu svých rezervací Azure.</span><span class="sxs-lookup"><span data-stu-id="a5cd3-146">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |