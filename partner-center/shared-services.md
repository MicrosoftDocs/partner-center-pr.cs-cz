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
ms.openlocfilehash: 40ba485cecce394dc81632d01f8774859690c522
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551601"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a><span data-ttu-id="cb896-103">Přidejte služby Azure partner Shared Services, aby partneři mohli koupit předplatné Azure pro vlastní použití.</span><span class="sxs-lookup"><span data-stu-id="cb896-103">Add Azure Partner Shared Services so partners can buy Azure subscriptions for their own use</span></span>

<span data-ttu-id="cb896-104">**Příslušné role**: globální správce | Agent správce | Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="cb896-104">**Appropriate roles**: Global admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="cb896-105">Azure partner Shared Services (APSS) je nový typ nabídky pro partnery v programu Cloud Solution Provider (CSP), který umožňuje partnerům koupit si předplatné Azure pro vlastní použití.</span><span class="sxs-lookup"><span data-stu-id="cb896-105">Azure Partner Shared Services (APSS) is a new offer type for partners in the Cloud Solution Provider (CSP) program, enabling partners to purchase Azure subscriptions for their own use.</span></span><span data-ttu-id="cb896-106">Vytvoří příležitost pro partnery, aby používali jednotnou metodu pro nákup, sledování a správu Azure společně s možností konsolidovat své licence na Azure a prodávat smlouvy s Microsoftem.</span><span class="sxs-lookup"><span data-stu-id="cb896-106">  It creates the opportunity for partners to use a uniform method for purchasing, tracking, and managing Azure in addition to the ability to consolidate their Azure licensing and reselling agreements with Microsoft.</span></span> <span data-ttu-id="cb896-107">Díky APSS mají partneři teď stejnou flexibilitu při používání předplatných Azure ve zprostředkovateli CSP, protože jsou v aplikacích Microsoft smlouva Enterprise a web Direct, otevírají scénáře, jako je například vývoj sestavení a testovací prostředí, nasazení interních úloh a hostování sdílených služeb nebo víceklientské aplikace.</span><span class="sxs-lookup"><span data-stu-id="cb896-107">With APSS, partners now have the same flexibility to use Azure subscriptions in CSP as they do in the Microsoft Enterprise Agreement and Web Direct programs, opening up scenarios such as:  build development and test environments, deploy internal workloads, and host shared services or multi-tenant applications.</span></span>  

## <a name="create-the-shared-services-tenant"></a><span data-ttu-id="cb896-108">Vytvoření tenanta sdílených služeb</span><span class="sxs-lookup"><span data-stu-id="cb896-108">Create the shared services tenant</span></span>

1. <span data-ttu-id="cb896-109">Přejít na **Nastavení** nastavení  >  **účtu**  >  **sdílené služby**.</span><span class="sxs-lookup"><span data-stu-id="cb896-109">Go to **Settings** > **Account settings** > **Shared services**.</span></span>

   :::image type="content" source="images/sharedservices2.png" alt-text="Nastavení účtu > sdílené služby":::

2. <span data-ttu-id="cb896-111">Pokud ještě nemáte tenanta sdílených služeb, vyberte **vytvořit sdílené služby**.</span><span class="sxs-lookup"><span data-stu-id="cb896-111">If you don't already have a shared services tenant, select **Create shared services**.</span></span>

   :::image type="content" source="images/sharedservices3.png" alt-text="Vytvořte sdílené služby.":::

3. <span data-ttu-id="cb896-113">Tím se vytvoří tenant sdílených služeb a nakupují předplatné Azure CSP Shared Services, které se bude používat pro sdílené prostředky a interní úlohy.</span><span class="sxs-lookup"><span data-stu-id="cb896-113">This creates a shared services tenant and purchases the Azure CSP Shared Services subscription, to be used for shared resources and internal workload.</span></span>

   :::image type="content" source="images/sharedservices5.png" alt-text="Vytvořte tenanta a zakupte předplatné.":::

## <a name="about-the-azure--internalshared-services-offer"></a><span data-ttu-id="cb896-115">O nabídce Azure-Internal/Shared Services</span><span class="sxs-lookup"><span data-stu-id="cb896-115">About the Azure- Internal/Shared Services offer</span></span>

- <span data-ttu-id="cb896-116">Azure-Internal/Shared Services předplatné je nový typ nabídky Azure ve zprostředkovateli CSP, ke kterému se přistupoval prostřednictvím partnerského centra, které partneři získají k vlastnímu používání Azure.</span><span class="sxs-lookup"><span data-stu-id="cb896-116">The Azure - Internal/Shared Services subscription is a new Azure offer type in CSP accessed through Partner Center that partners get for their own use of Azure.</span></span>

- <span data-ttu-id="cb896-117">Předplatné Azure partner Shared Services má nárok a dá se použít k zakoupení služeb vzdálené instalace.</span><span class="sxs-lookup"><span data-stu-id="cb896-117">Azure Partner Shared Services subscriptions are eligible and can be used to purchase RIs.</span></span>

- <span data-ttu-id="cb896-118">Nabídku Azure-Internal/Shared Services lze použít pouze pro tenanta sdílených služeb.</span><span class="sxs-lookup"><span data-stu-id="cb896-118">The Azure - Internal/Shared Services offer can only be applied to the shared services tenant.</span></span>

- <span data-ttu-id="cb896-119">Primárním využitím předplatného Azure-Internal/Shared Services je, abyste mohli Azure používat pro vlastní účely vývoje.</span><span class="sxs-lookup"><span data-stu-id="cb896-119">The primary use for the Azure - Internal/Shared Services subscription is so that you can use Azure for your own development purposes.</span></span> <span data-ttu-id="cb896-120">Sdílený tenant, který použijete k zřízení této nabídky, se nedá použít pro jiné služby, jako jsou licence na Office 365 nebo Dynamics.</span><span class="sxs-lookup"><span data-stu-id="cb896-120">The shared tenant you use to provision this offer cannot be used for other services such as Office 365 or Dynamics licenses.</span></span>

- <span data-ttu-id="cb896-121">Předplatné můžete zrušit stejně jako jakékoli jiné předplatné.</span><span class="sxs-lookup"><span data-stu-id="cb896-121">You can cancel the subscription like any other subscription.</span></span> <span data-ttu-id="cb896-122">Přejít na **Nastavení**  >  **Zobrazit všechna nastavení**  >  **sdílené služby**.</span><span class="sxs-lookup"><span data-stu-id="cb896-122">Go to the **settings** > **View all settings** > **Shared services**.</span></span> <span data-ttu-id="cb896-123">Vyberte předplatné Azure-Internal/Shared Services a zrušte ho.</span><span class="sxs-lookup"><span data-stu-id="cb896-123">Select the Azure - Internal/Shared Services subscription and cancel it.</span></span>

## <a name="accessing-azure-partner-shared-services-consumption-details"></a><span data-ttu-id="cb896-124">Přístup k podrobnostem o spotřebě Azure partner Shared Services</span><span class="sxs-lookup"><span data-stu-id="cb896-124">Accessing Azure Partner Shared Services consumption details</span></span>

<span data-ttu-id="cb896-125">Na faktuře CSP a souboru pro odsouhlasení najdete spotřebu Azure.</span><span class="sxs-lookup"><span data-stu-id="cb896-125">You will find the Azure consumption on your CSP invoice and the reconciliation file.</span></span> <span data-ttu-id="cb896-126">Bude obsažena jako součást Microsoft Azure položky řádku na faktuře.</span><span class="sxs-lookup"><span data-stu-id="cb896-126">It will be included as part of Microsoft Azure line item in the invoice.</span></span> <span data-ttu-id="cb896-127">Podrobné informace o spotřebě budou k dispozici v souboru pro odsouhlasení s klientem vytvořeným pro tuto nabídku.</span><span class="sxs-lookup"><span data-stu-id="cb896-127">The detailed consumption information will be available in the reconciliation file logged against the tenant that was created for this offer.</span></span>

## <a name="azure-partner-shared-services-pricing"></a><span data-ttu-id="cb896-128">Ceny za službu Azure partner Shared Services</span><span class="sxs-lookup"><span data-stu-id="cb896-128">Azure Partner Shared Services pricing</span></span>

<span data-ttu-id="cb896-129">Pokud chcete zobrazit nový soubor s cenami pro APSS, přejděte na **prodej**  >  **ceny a nabídky** a vyberte ceník aktuální měsíc.</span><span class="sxs-lookup"><span data-stu-id="cb896-129">To see the new pricing file for APSS, go to **Sell** > **Pricing and offers** and select the current month's price list.</span></span> <span data-ttu-id="cb896-130">V nadcházejících týdnech se uvolní také rozhraní API pro specifickou míru karet.</span><span class="sxs-lookup"><span data-stu-id="cb896-130">In the coming weeks, a specific rate card api will also be released.</span></span>

## <a name="marketplace-offers-and-azure-partner-shared-services"></a><span data-ttu-id="cb896-131">Nabídky Marketplace a služby Azure partner Shared Services</span><span class="sxs-lookup"><span data-stu-id="cb896-131">Marketplace offers and Azure Partner Shared Services</span></span>

<span data-ttu-id="cb896-132">Od 1. března 2019 APSS už nepodporuje nabídky Marketplace.</span><span class="sxs-lookup"><span data-stu-id="cb896-132">As of March 1, 2019, APSS no longer supports Marketplace offers.</span></span>

|<span data-ttu-id="cb896-133">**Podpora Marketplace**</span><span class="sxs-lookup"><span data-stu-id="cb896-133">**Marketplace support**</span></span>   |<span data-ttu-id="cb896-134">**APSS se podporuje do 1. března 2019**</span><span class="sxs-lookup"><span data-stu-id="cb896-134">**APSS supported before March 1, 2019**</span></span>|<span data-ttu-id="cb896-135">**Od 1. března 2019**</span><span class="sxs-lookup"><span data-stu-id="cb896-135">**After March 1, 2019**</span></span>|
|---------------------------|:----------------------------|:-------------------|
|<span data-ttu-id="cb896-136">Přineste si vlastní licenci (BYOL) a bezplatné služby</span><span class="sxs-lookup"><span data-stu-id="cb896-136">Bring your own license (BYOL) and free services</span></span>   | <span data-ttu-id="cb896-137">Yes</span><span class="sxs-lookup"><span data-stu-id="cb896-137">Yes</span></span>   | <span data-ttu-id="cb896-138">No</span><span class="sxs-lookup"><span data-stu-id="cb896-138">No</span></span>|
|<span data-ttu-id="cb896-139">Další nabídky na webu Marketplace třetích stran</span><span class="sxs-lookup"><span data-stu-id="cb896-139">Other third-party marketplace offers</span></span>   | <span data-ttu-id="cb896-140">No</span><span class="sxs-lookup"><span data-stu-id="cb896-140">No</span></span>   |<span data-ttu-id="cb896-141">No</span><span class="sxs-lookup"><span data-stu-id="cb896-141">No</span></span>|

<span data-ttu-id="cb896-142">Partneři, kteří mají BYOL nebo bezplatné služby nasazené pomocí APSS, nebudou ovlivněny. od 1. března 2019 ale nebude moct koupit nové BYOL nebo bezplatné služby.</span><span class="sxs-lookup"><span data-stu-id="cb896-142">Partners who have BYOL or free services deployed using APSS will not be impacted; however after March 1, 2019 they will not be able to purchase new BYOL or free services.</span></span>

<span data-ttu-id="cb896-143">Aby bylo možné využít kompletní katalog nabízených nabídek Marketplace (ne jenom BYOL a bezplatné služby), doporučujeme, aby partneři CSP nasadili sdílené služby s použitím předplatných Azure web Direct.</span><span class="sxs-lookup"><span data-stu-id="cb896-143">To take advantage of the full catalog of Marketplace offers available (not just BYOL and free services), we recommend CSP partners deploy shared services using web direct Azure subscriptions.</span></span>  <span data-ttu-id="cb896-144">Partneři CSP, kteří už dříve nasadili BYOL a bezplatné prostředky služeb z webu Marketplace a chtějí je dál používat a nasazovat další nabídky třetích stran, se doporučuje migrovat předplatné APSS na web přímo [migrací stávajících předplatných Azure](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).</span><span class="sxs-lookup"><span data-stu-id="cb896-144">CSP partners who have deployed third-party BYOL and free service resources from the Marketplace previously and wish to continue using them and deploy more third-party offerings are encouraged to migrate the APSS subscription to web direct [Migrating Existing Azure Subscriptions](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).</span></span>

<span data-ttu-id="cb896-145">Partneři, kteří plánují i nadále používat předplatné APSS po 1. březnu 2019 a chtějí nasadit nové [služby BYOL](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) třetích stran nebo bezplatné služby, můžou podle pokynů od nezávislých výrobců softwaru tyto informace nasadit do svých předplatných APSS.</span><span class="sxs-lookup"><span data-stu-id="cb896-145">Partners, who plan to continue using APSS subscription after the March 1, 2019 and wish to deploy new third-party [BYOL services](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) or free services, can follow the instructions from ISVs to deploy these to their APSS subscriptions.</span></span>

## <a name="next-steps"></a><span data-ttu-id="cb896-146">Další kroky</span><span class="sxs-lookup"><span data-stu-id="cb896-146">Next steps</span></span>

- [<span data-ttu-id="cb896-147">Prodej softwarových předplatných prostřednictvím CSP</span><span class="sxs-lookup"><span data-stu-id="cb896-147">Sell software subscriptions through CSP</span></span>](csp-software-subscriptions.md)