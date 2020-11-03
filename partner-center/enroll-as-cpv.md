---
title: Zaregistrovat jako dodavatele ovládacího panelu
description: Naučte se, jak se zaregistrovat jako dodavatel na řídicím panelu v partnerském centru, abyste mohli lépe integrovat partnerské systémy CSP s rozhraními API partnerského centra.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/20/2020
ms.openlocfilehash: 1bfcb4de27233283b6188903b3e1f6bbdf67698c
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/14/2020
ms.locfileid: "92527709"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="ba1a5-103">Zaregistrovat jako dodavatele ovládacích panelů, který umožňuje integrovat partnerské systémy CSP s rozhraními API partnerského centra</span><span class="sxs-lookup"><span data-stu-id="ba1a5-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>

<span data-ttu-id="ba1a5-104">**Platí pro**</span><span class="sxs-lookup"><span data-stu-id="ba1a5-104">**Applies to**</span></span>

- <span data-ttu-id="ba1a5-105">Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="ba1a5-105">Partner Center</span></span>

<span data-ttu-id="ba1a5-106">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="ba1a5-106">**Appropriate roles**</span></span>

- <span data-ttu-id="ba1a5-107">Globální správce</span><span class="sxs-lookup"><span data-stu-id="ba1a5-107">Global admin</span></span>

<span data-ttu-id="ba1a5-108">Dodavatel ovládacího panelu (CPV) je nezávislý dodavatel softwaru, který vyvíjí aplikace pro použití partnery poskytovatele cloudových řešení (CSP) a umožňuje jim integrovat své systémy s rozhraními API pro partnerské centra.</span><span class="sxs-lookup"><span data-stu-id="ba1a5-108">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="ba1a5-109">Dodavatel ovládacího panelu není partnerem CSP s přímým přístupem k rozhraním API řídicího panelu partnerského centra nebo partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="ba1a5-109">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="ba1a5-110">Ať už jste aktuální dodavatel ovládacího panelu (CPV) nebo nový CPV, který chce spolupracovat s partnery Microsoftu, Microsoft teď vyžaduje, abyste se zaregistrovali v partnerském centru, abyste mohli zaregistrovat své aplikace a podporovat partnery poskytovatele Cloud Solution Provider.</span><span class="sxs-lookup"><span data-stu-id="ba1a5-110">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="ba1a5-111">Partner CPV může vytvořit účet buď pomocí stávajícího partnerského tenanta CSP, nebo existujícího tenanta CPV nebo může vytvořit nového tenanta jako součást procesu připojování.</span><span class="sxs-lookup"><span data-stu-id="ba1a5-111">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="ba1a5-112">Pokud se partner CPV rozhodne použít stávajícího tenanta CSP, bude muset vytvořit samostatné aplikace s více klienty a zaregistrovat je v partnerském centru pro aktivity CPV.</span><span class="sxs-lookup"><span data-stu-id="ba1a5-112">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="ba1a5-113">Aplikace se nedá registrovat jako aplikace CSP i CPV.</span><span class="sxs-lookup"><span data-stu-id="ba1a5-113">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="ba1a5-114">Po registraci do partnerského centra a registraci vašich aplikací budete mít přístup k rozhraním API partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="ba1a5-114">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="ba1a5-115">Microsoft vás bude kontaktovat prostřednictvím oznámení partnerského centra s informacemi o izolovaném prostoru.</span><span class="sxs-lookup"><span data-stu-id="ba1a5-115">Microsoft will contact you via a Partner Center notification with your sandbox information.</span></span> <span data-ttu-id="ba1a5-116">Pokud již máte účet izolovaného prostoru (sandbox), pokračujte v jeho používání.</span><span class="sxs-lookup"><span data-stu-id="ba1a5-116">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="ba1a5-117">Nebudete potřebovat nový izolovaný prostor (sandbox).</span><span class="sxs-lookup"><span data-stu-id="ba1a5-117">You won't need a new sandbox.</span></span>

<span data-ttu-id="ba1a5-118">Kontrola [smlouvy dodavatele v Ovládacích panelech společnosti Microsoft](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="ba1a5-118">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="ba1a5-119">Práce v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="ba1a5-119">Working in Partner Center</span></span>
<span data-ttu-id="ba1a5-120">Po zaregistrování v prostředí partnerského centra CPV a přijetí smlouvy CPV můžete:</span><span class="sxs-lookup"><span data-stu-id="ba1a5-120">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="ba1a5-121">Spravujte aplikace s více klienty (přidejte aplikace pro Azure Portal, registraci a zrušení registrace aplikací v partnerském centru).</span><span class="sxs-lookup"><span data-stu-id="ba1a5-121">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="ba1a5-122">CPVs musí zaregistrovat své aplikace v partnerském centru, aby bylo možné získat autorizaci pro rozhraní API partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="ba1a5-122">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="ba1a5-123">Přidání aplikací do samotného Azure Portal neautorizuje aplikace CPV pro rozhraní API partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="ba1a5-123">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="ba1a5-124">Umožňuje zobrazit a spravovat váš profil CPV.</span><span class="sxs-lookup"><span data-stu-id="ba1a5-124">View and manage your CPV profile</span></span> 

- <span data-ttu-id="ba1a5-125">Umožňuje zobrazit a spravovat uživatele, kteří potřebují přístup k možnostem CPV.</span><span class="sxs-lookup"><span data-stu-id="ba1a5-125">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="ba1a5-126">Globální správce je jediná role, kterou může mít CPV.</span><span class="sxs-lookup"><span data-stu-id="ba1a5-126">Global admin is the only role a CPV can have.</span></span>


