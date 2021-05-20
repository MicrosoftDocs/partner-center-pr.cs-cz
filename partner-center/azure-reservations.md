---
title: Prodej zákazníků Microsoft Azure rezervací
description: Jako Cloud Solution Provider můžete pro zákazníky nakupovat, prodávat nebo spravovat rezervace Azure. Použijte Partnerské centrum, Azure Portal nebo rozhraní API Partnerské centrum.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: b97cafea9ad2f36718418c7c7cfca5f91ee8849c
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149464"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="cdc7d-104">Prodej Microsoft Azure rezervací zákazníkům pomocí Partnerské centrum, Azure Portal nebo rozhraní API</span><span class="sxs-lookup"><span data-stu-id="cdc7d-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="cdc7d-105">**Odpovídající role:** Agent pro správu | Globální správce | Agent helpdesku | Sales agent | Správce správy uživatelů</span><span class="sxs-lookup"><span data-stu-id="cdc7d-105">**Appropriate roles**: Admin agent | Global admin | Helpdesk agent | Sales agent | User management admin</span></span>

<span data-ttu-id="cdc7d-106">Jako partner v Cloud Solution Provider (CSP) můžete pro zákazníky nakupovat, prodávat a spravovat rezervace Azure.</span><span class="sxs-lookup"><span data-stu-id="cdc7d-106">As a partner in the Cloud Solution Provider program (CSP), you can buy, sell, or manage Azure reservations for customers.</span></span> <span data-ttu-id="cdc7d-107">Použijte Partnerské centrum, Azure Portal nebo rozhraní API Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="cdc7d-107">Use Partner Center, the Azure portal, or the Partner Center API.</span></span>

> [!NOTE]
> <span data-ttu-id="cdc7d-108">Tento článek se týká jenom partnerů v CSP.</span><span class="sxs-lookup"><span data-stu-id="cdc7d-108">This article applies only to partners in CSP.</span></span> <span data-ttu-id="cdc7d-109">Zákazníci, kteří používají jiné typy předplatných (například předplatná s platbami, jednotlivá předplatná, Smlouva se zákazníkem Microsoftu nebo předplatná smlouva Enterprise), by si místo toho měli přečíst tuto dokumentaci k [rezervacím Azure.](/azure/cost-management-billing/reservations)</span><span class="sxs-lookup"><span data-stu-id="cdc7d-109">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="cdc7d-110">Partneři v programu CSP mohou svým zákazníkům nabídnout Microsoft Azure rezervace.</span><span class="sxs-lookup"><span data-stu-id="cdc7d-110">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="cdc7d-111">Zákazníci získají značné úspory, když si vyhradit předem.</span><span class="sxs-lookup"><span data-stu-id="cdc7d-111">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="cdc7d-112">Rezervace Azure nabízejí zákazníkům jednoduchost a flexibilitu následujícími způsoby:</span><span class="sxs-lookup"><span data-stu-id="cdc7d-112">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="cdc7d-113">Podmínky rezervace na jeden nebo tři roky</span><span class="sxs-lookup"><span data-stu-id="cdc7d-113">One or three-year reservation terms</span></span>
- <span data-ttu-id="cdc7d-114">Snadné zahájení práce; nastavení dokončeno v sekundách</span><span class="sxs-lookup"><span data-stu-id="cdc7d-114">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="cdc7d-115">Zrušení nebo výměna rezervovaných instancí za upravenou refundaci kdykoli</span><span class="sxs-lookup"><span data-stu-id="cdc7d-115">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="cdc7d-116">Správa využití rezervovaných instancí na úrovni organizace nebo jednotlivých oddělení</span><span class="sxs-lookup"><span data-stu-id="cdc7d-116">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="cdc7d-117">Rezervace Azure mohou oslovovat zákazníky následujícími způsoby:</span><span class="sxs-lookup"><span data-stu-id="cdc7d-117">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="cdc7d-118">Rezervace mohou nabízet významné úspory nad cenami s platbami podle tarifů s platbami.</span><span class="sxs-lookup"><span data-stu-id="cdc7d-118">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="cdc7d-119">Lepší rozpočtování a prognózování s platbou předem na jeden nebo tři roky</span><span class="sxs-lookup"><span data-stu-id="cdc7d-119">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="cdc7d-120">Výpočetní kapacita seřazená podle priority v oblasti Azure, která je nejblíže k jejich kancelářím</span><span class="sxs-lookup"><span data-stu-id="cdc7d-120">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="cdc7d-121">Rezervace Azure poskytují základ pro komplexní řešení infrastruktury v kombinaci se softwarem, jako je Microsoft Windows Server a Azure SQL Database</span><span class="sxs-lookup"><span data-stu-id="cdc7d-121">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="cdc7d-122">Rezervace Azure můžete kupovat, prodávat a spravovat v Partnerské centrum i Azure Portal a pomocí rozhraní Partnerské centrum API.</span><span class="sxs-lookup"><span data-stu-id="cdc7d-122">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="cdc7d-123">Zákazníkům můžete také udělit oprávnění k nákupu vlastních rezervací Azure z předplatného Azure, které jste pro ně zakoupili.</span><span class="sxs-lookup"><span data-stu-id="cdc7d-123">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="cdc7d-124">Postup najdete na následujících odkazech.</span><span class="sxs-lookup"><span data-stu-id="cdc7d-124">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="cdc7d-125">Prostředky rezervací Azure</span><span class="sxs-lookup"><span data-stu-id="cdc7d-125">Azure reservations resources</span></span>

|<span data-ttu-id="cdc7d-126">**Informace o**</span><span class="sxs-lookup"><span data-stu-id="cdc7d-126">**For information about**</span></span>   |<span data-ttu-id="cdc7d-127">**Přečtěte si:**</span><span class="sxs-lookup"><span data-stu-id="cdc7d-127">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="cdc7d-128">Dokumentace k rezervacím Azure pro vaše zákazníky</span><span class="sxs-lookup"><span data-stu-id="cdc7d-128">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="cdc7d-129">Co jsou rezervace Azure?</span><span class="sxs-lookup"><span data-stu-id="cdc7d-129">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="cdc7d-130">Nákup rezervací Azure pro zákazníky v Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="cdc7d-130">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="cdc7d-131">Nákup rezervací Azure</span><span class="sxs-lookup"><span data-stu-id="cdc7d-131">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="cdc7d-132">Správa rezervací Azure v Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="cdc7d-132">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="cdc7d-133">Správa rezervací Azure v Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="cdc7d-133">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="cdc7d-134">Určení správné velikosti virtuálního počítače a ověření využití virtuálních počítače zákazníka</span><span class="sxs-lookup"><span data-stu-id="cdc7d-134">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="cdc7d-135">Nastavení velikosti virtuálního počítače pro maximální využití rezervací Azure</span><span class="sxs-lookup"><span data-stu-id="cdc7d-135">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="cdc7d-136">Nákup rezervací Azure pomocí rozhraní PARTNERSKÉ CENTRUM API</span><span class="sxs-lookup"><span data-stu-id="cdc7d-136">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="cdc7d-137">[Informace Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) najdete v dokumentaci Partnerské centrum pro vývojáře.</span><span class="sxs-lookup"><span data-stu-id="cdc7d-137">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="cdc7d-138">Poskytuje zákazníkům oprávnění k nákupu vlastních rezervací Azure z vašeho předplatného CSP.</span><span class="sxs-lookup"><span data-stu-id="cdc7d-138">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="cdc7d-139">Udělit zákazníkům oprávnění k nákupu vlastních rezervací Azure</span><span class="sxs-lookup"><span data-stu-id="cdc7d-139">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |