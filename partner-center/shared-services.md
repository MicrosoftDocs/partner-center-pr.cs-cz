---
title: Přidat služby Azure partner Shared Services
description: Využijte Azure partner Shared Services k nákupu předplatných Azure pro vaše vlastní použití a k zajištění jednotné metody pro nákup, sledování a správu Azure.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: 929907c7c6f238fb84a13622227534797f0ac949
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855331"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a><span data-ttu-id="9a169-103">Přidejte služby Azure partner Shared Services, aby partneři mohli koupit předplatné Azure pro vlastní použití.</span><span class="sxs-lookup"><span data-stu-id="9a169-103">Add Azure Partner Shared Services so partners can buy Azure subscriptions for their own use</span></span>

<span data-ttu-id="9a169-104">**Příslušné role**: globální správce | Agent správce | Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="9a169-104">**Appropriate roles**: Global admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="9a169-105">Azure partner Shared Services je nový typ nabídky pro partnery v programu CSP, který umožňuje partnerům zakoupit si předplatné Azure pro vlastní použití.</span><span class="sxs-lookup"><span data-stu-id="9a169-105">Azure Partner Shared Services is a new offer type for partners in the CSP program enabling partners to purchase Azure subscriptions for their own use.</span></span><span data-ttu-id="9a169-106">Vytvoří příležitost pro partnery, aby používali jednotnou metodu pro nákup, sledování a správu Azure společně s možností konsolidovat své licence na Azure a prodávat smlouvy s Microsoftem.</span><span class="sxs-lookup"><span data-stu-id="9a169-106">  It creates the opportunity for partners to use a uniform method for purchasing, tracking, and managing Azure in addition to the ability to consolidate their Azure licensing and reselling agreements with Microsoft.</span></span> <span data-ttu-id="9a169-107">U partnerských sdílených služeb Azure teď mají partneři stejnou flexibilitu při používání předplatných Azure ve zprostředkovateli CSP, protože jsou v aplikacích Microsoft smlouva Enterprise a web Direct, otevírá scénáře jako: vývoj a testovací prostředí, nasazují interní úlohy a hostuje sdílené služby nebo víceklientské aplikace.</span><span class="sxs-lookup"><span data-stu-id="9a169-107">With Azure Partner Shared Services, partners now have the same flexibility to use Azure subscriptions in CSP as they do in the Microsoft Enterprise Agreement and Web Direct programs, opening up scenarios such as:  build development and test environments, deploy internal workloads, and host shared services or multi-tenant applications.</span></span>  

## <a name="create-the-shared-services-tenant"></a><span data-ttu-id="9a169-108">Vytvoření tenanta sdílených služeb</span><span class="sxs-lookup"><span data-stu-id="9a169-108">Create the shared services tenant</span></span>

1. <span data-ttu-id="9a169-109">Přejít na **Nastavení** nastavení  >  **účtu**  >  **sdílené služby**.</span><span class="sxs-lookup"><span data-stu-id="9a169-109">Go to **Settings** > **Account settings** > **Shared services**.</span></span>

   :::image type="content" source="images/sharedservices2.png" alt-text="Nastavení účtu > sdílené služby":::

2. <span data-ttu-id="9a169-111">Pokud ještě nemáte tenanta sdílených služeb, klikněte na **vytvořit sdílené služby**.</span><span class="sxs-lookup"><span data-stu-id="9a169-111">If you don't already have a shared services tenant, click **Create shared services**.</span></span>

   :::image type="content" source="images/sharedservices3.png" alt-text="Vytváření sdílených služeb":::

3. <span data-ttu-id="9a169-113">Tím se vytvoří tenant sdílených služeb a nakupují předplatné Azure CSP Shared Services, které se bude používat pro sdílené prostředky a interní úlohy.</span><span class="sxs-lookup"><span data-stu-id="9a169-113">This creates a shared services tenant and purchases the Azure CSP Shared Services subscription, to be used for shared resources and internal workload.</span></span>

   :::image type="content" source="images/sharedservices5.png" alt-text="Vytvoření tenanta a zakoupení předplatného":::

## <a name="about-the-azure--internalshared-services-offer"></a><span data-ttu-id="9a169-115">O nabídce Azure-Internal/Shared Services</span><span class="sxs-lookup"><span data-stu-id="9a169-115">About the Azure- Internal/Shared Services offer</span></span>

- <span data-ttu-id="9a169-116">Azure-Internal/Shared Services předplatné je nový typ nabídky Azure ve zprostředkovateli CSP, ke kterému se přistupoval prostřednictvím partnerského centra, které partneři získají k vlastnímu používání Azure.</span><span class="sxs-lookup"><span data-stu-id="9a169-116">The Azure - Internal/Shared Services subscription is a new Azure offer type in CSP accessed through Partner Center that partners get for their own use of Azure.</span></span>

- <span data-ttu-id="9a169-117">Předplatné Azure partner Shared Services má nárok a dá se použít k zakoupení služeb vzdálené instalace.</span><span class="sxs-lookup"><span data-stu-id="9a169-117">Azure Partner Shared Services subscriptions are eligible and can be used to purchase RIs.</span></span>

- <span data-ttu-id="9a169-118">Nabídku Azure-Internal/Shared Services lze použít pouze pro tenanta sdílených služeb.</span><span class="sxs-lookup"><span data-stu-id="9a169-118">The Azure - Internal/Shared Services offer can only be applied to the shared services tenant.</span></span>

- <span data-ttu-id="9a169-119">Primárním použitím předplatného Azure - Internal/Shared Services je, abyste mohli Azure používat pro vlastní účely vývoje.</span><span class="sxs-lookup"><span data-stu-id="9a169-119">The primary use for the Azure - Internal/Shared Services subscription is so that you can use Azure for your own development purposes.</span></span> <span data-ttu-id="9a169-120">Sdílený tenant, který použijete ke zřízení této nabídky, se nemůže používat pro jiné služby, jako jsou licence Office 365 nebo Dynamics.</span><span class="sxs-lookup"><span data-stu-id="9a169-120">The shared tenant you use to provision this offer cannot be used for other services such as Office 365 or Dynamics licenses.</span></span>

- <span data-ttu-id="9a169-121">Předplatné můžete zrušit stejně jako jakékoli jiné předplatné.</span><span class="sxs-lookup"><span data-stu-id="9a169-121">You can cancel the subscription like any other subscription.</span></span> <span data-ttu-id="9a169-122">Přejděte do **nastavení,**  >  **Zobrazit vše sdílené**  >  **služby**.</span><span class="sxs-lookup"><span data-stu-id="9a169-122">Go to the **settings** > **View all settings** > **Shared services**.</span></span> <span data-ttu-id="9a169-123">Vyberte předplatné Azure - Internal/Shared Services a zrušte ho.</span><span class="sxs-lookup"><span data-stu-id="9a169-123">Select the Azure - Internal/Shared Services subscription and cancel it.</span></span>

## <a name="accessing-azure-partner-shared-services-consumption-details"></a><span data-ttu-id="9a169-124">Přístup Azure Partner Shared Services s podrobnostmi o spotřebě</span><span class="sxs-lookup"><span data-stu-id="9a169-124">Accessing Azure Partner Shared Services consumption details</span></span>

<span data-ttu-id="9a169-125">Spotřebu Azure najdete na faktuře CSP a v souboru s vyrovnáním.</span><span class="sxs-lookup"><span data-stu-id="9a169-125">You will find the Azure consumption on your CSP invoice and the reconciliation file.</span></span> <span data-ttu-id="9a169-126">Bude zahrnut jako součást Microsoft Azure položky na faktuře.</span><span class="sxs-lookup"><span data-stu-id="9a169-126">It will be included as part of Microsoft Azure line item in the invoice.</span></span> <span data-ttu-id="9a169-127">Podrobné informace o spotřebě budou k dispozici v souboru odsouhlasení zaznamenaného v tenantovi vytvořeném pro tuto nabídku.</span><span class="sxs-lookup"><span data-stu-id="9a169-127">The detailed consumption information will be available in the reconciliation file logged against the tenant that was created for this offer.</span></span>

## <a name="azure-partner-shared-services-pricing"></a><span data-ttu-id="9a169-128">Azure Partner Shared Services ceny</span><span class="sxs-lookup"><span data-stu-id="9a169-128">Azure Partner Shared Services pricing</span></span>

<span data-ttu-id="9a169-129">Pokud chcete zobrazit nový soubor s cenami pro Azure Partner Shared Services, přejděte na **Sell**  >  **Pricing and offers (Prodejní** ceny a nabídky) a vyberte ceník pro aktuální měsíc.</span><span class="sxs-lookup"><span data-stu-id="9a169-129">To see the new pricing file for Azure Partner Shared Services, go to **Sell** > **Pricing and offers** and select the current month's price list.</span></span> <span data-ttu-id="9a169-130">V nadcházejících týdnech bude také vydáno rozhraní API pro konkrétní kartu sazeb.</span><span class="sxs-lookup"><span data-stu-id="9a169-130">In the coming weeks, a specific rate card api will also be released.</span></span>

## <a name="marketplace-offers-and-azure-partner-shared-services"></a><span data-ttu-id="9a169-131">Nabídky a Azure Partner Shared Services Marketplace</span><span class="sxs-lookup"><span data-stu-id="9a169-131">Marketplace offers and Azure Partner Shared Services</span></span>

<span data-ttu-id="9a169-132">Od 1. března 2019 Azure Partner Shared Services (APSS) už nepodporuje nabídky Marketplace.</span><span class="sxs-lookup"><span data-stu-id="9a169-132">As of March 1, 2019, Azure Partner Shared Services (APSS) no longer supports Marketplace offers.</span></span>

|<span data-ttu-id="9a169-133">**Podpora Marketplace**</span><span class="sxs-lookup"><span data-stu-id="9a169-133">**Marketplace support**</span></span>   |<span data-ttu-id="9a169-134">**Podpora APSS před 1. březnem 2019**</span><span class="sxs-lookup"><span data-stu-id="9a169-134">**APSS supported before March 1, 2019**</span></span>|<span data-ttu-id="9a169-135">**Po 1. březnu 2019**</span><span class="sxs-lookup"><span data-stu-id="9a169-135">**After March 1, 2019**</span></span>|
|---------------------------|:----------------------------|:-------------------|
|<span data-ttu-id="9a169-136">Použití vlastní licence (BYOL) a bezplatných služeb</span><span class="sxs-lookup"><span data-stu-id="9a169-136">Bring your own license (BYOL) and free services</span></span>   | <span data-ttu-id="9a169-137">Yes</span><span class="sxs-lookup"><span data-stu-id="9a169-137">Yes</span></span>   | <span data-ttu-id="9a169-138">No</span><span class="sxs-lookup"><span data-stu-id="9a169-138">No</span></span>|
|<span data-ttu-id="9a169-139">Další nabídky třetích stran na marketplace</span><span class="sxs-lookup"><span data-stu-id="9a169-139">Other third-party marketplace offers</span></span>   | <span data-ttu-id="9a169-140">No</span><span class="sxs-lookup"><span data-stu-id="9a169-140">No</span></span>   |<span data-ttu-id="9a169-141">No</span><span class="sxs-lookup"><span data-stu-id="9a169-141">No</span></span>|

<span data-ttu-id="9a169-142">Na partnery, kteří mají nasazené služby BYOL nebo bezplatné služby nasazené pomocí APSS, to nebude mít vliv. po 1. březnu 2019 ale nebudou moct nakupovat nové služby BYOL ani bezplatné služby.</span><span class="sxs-lookup"><span data-stu-id="9a169-142">Partners who have BYOL or free services deployed using APSS will not be impacted; however after March 1, 2019 they will not be able to purchase new BYOL or free services.</span></span>

<span data-ttu-id="9a169-143">Aby bylo možné využít kompletní katalog nabízených nabídek Marketplace (ne jenom BYOL a bezplatné služby), doporučujeme, aby partneři CSP nasadili sdílené služby s použitím předplatných Azure web Direct.</span><span class="sxs-lookup"><span data-stu-id="9a169-143">To take advantage of the full catalog of Marketplace offers available (not just BYOL and free services), we recommend CSP partners deploy shared services using web direct Azure subscriptions.</span></span>  <span data-ttu-id="9a169-144">Partneři CSP, kteří už dříve nasadili BYOL a bezplatné prostředky služeb z webu Marketplace a chtějí je dál používat a nasazovat další nabídky třetích stran, se doporučuje migrovat předplatné APSS na web přímo [migrací stávajících předplatných Azure](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).</span><span class="sxs-lookup"><span data-stu-id="9a169-144">CSP partners who have deployed third-party BYOL and free service resources from the Marketplace previously and wish to continue using them and deploy more third-party offerings are encouraged to migrate the APSS subscription to web direct [Migrating Existing Azure Subscriptions](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).</span></span>

<span data-ttu-id="9a169-145">Partneři, kteří plánují i nadále používat předplatné APSS po 1. březnu 2019 a chtějí nasadit nové [služby BYOL](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) třetích stran nebo bezplatné služby, můžou podle pokynů od nezávislých výrobců softwaru tyto informace nasadit do svých předplatných APSS.</span><span class="sxs-lookup"><span data-stu-id="9a169-145">Partners, who plan to continue using APSS subscription after the March 1, 2019 and wish to deploy new third-party [BYOL services](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) or free services, can follow the instructions from ISVs to deploy these to their APSS subscriptions.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9a169-146">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9a169-146">Next steps</span></span>

- [<span data-ttu-id="9a169-147">Prodej softwarových předplatných prostřednictvím CSP</span><span class="sxs-lookup"><span data-stu-id="9a169-147">Sell software subscriptions through CSP</span></span>](csp-software-subscriptions.md)