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
ms.date: 01/15/2021
ms.openlocfilehash: edc0ea8f0fda58f23cbce82bc7023a3277517cc3
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147135"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="6b0d2-103">Zaregistrovat jako dodavatele ovládacích panelů, který umožňuje integrovat partnerské systémy CSP s rozhraními API partnerského centra</span><span class="sxs-lookup"><span data-stu-id="6b0d2-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>


<span data-ttu-id="6b0d2-104">**Příslušné role**: globální správce</span><span class="sxs-lookup"><span data-stu-id="6b0d2-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="6b0d2-105">Dodavatel ovládacího panelu (CPV) je nezávislý dodavatel softwaru, který vyvíjí aplikace pro použití partnery poskytovatele cloudových řešení (CSP) a umožňuje jim integrovat své systémy s rozhraními API pro partnerské centra.</span><span class="sxs-lookup"><span data-stu-id="6b0d2-105">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="6b0d2-106">Dodavatel ovládacího panelu není partnerem CSP s přímým přístupem k rozhraním API řídicího panelu partnerského centra nebo partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="6b0d2-106">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="6b0d2-107">Ať už jste aktuální dodavatel ovládacího panelu (CPV) nebo nový CPV, který chce spolupracovat s partnery Microsoftu, Microsoft teď vyžaduje, abyste se zaregistrovali v partnerském centru, abyste mohli zaregistrovat své aplikace a podporovat partnery poskytovatele Cloud Solution Provider.</span><span class="sxs-lookup"><span data-stu-id="6b0d2-107">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="6b0d2-108">Partner CPV může vytvořit účet buď pomocí stávajícího partnerského tenanta CSP, nebo existujícího tenanta CPV nebo může vytvořit nového tenanta jako součást procesu připojování.</span><span class="sxs-lookup"><span data-stu-id="6b0d2-108">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="6b0d2-109">Pokud se partner CPV rozhodne použít stávajícího tenanta CSP, bude muset vytvořit samostatné aplikace s více klienty a zaregistrovat je v partnerském centru pro aktivity CPV.</span><span class="sxs-lookup"><span data-stu-id="6b0d2-109">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="6b0d2-110">Aplikace se nedá registrovat jako aplikace CSP i CPV.</span><span class="sxs-lookup"><span data-stu-id="6b0d2-110">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="6b0d2-111">Po registraci do partnerského centra a registraci vašich aplikací budete mít přístup k rozhraním API partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="6b0d2-111">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="6b0d2-112">Pokud potřebujete účet izolovaného prostoru (sandbox), obraťte se na společnost Microsoft prostřednictvím žádosti o podpora Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="6b0d2-112">Contact Microsoft through a Microsoft Support request if you need a sandbox account.</span></span> <span data-ttu-id="6b0d2-113">Pokud již máte účet izolovaného prostoru (sandbox), pokračujte v jeho používání.</span><span class="sxs-lookup"><span data-stu-id="6b0d2-113">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="6b0d2-114">Nebudete potřebovat nový izolovaný prostor (sandbox).</span><span class="sxs-lookup"><span data-stu-id="6b0d2-114">You won't need a new sandbox</span></span>

<span data-ttu-id="6b0d2-115">Kontrola [smlouvy dodavatele v Ovládacích panelech společnosti Microsoft](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="6b0d2-115">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="6b0d2-116">Práce v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="6b0d2-116">Working in Partner Center</span></span>

<span data-ttu-id="6b0d2-117">Po zaregistrování v prostředí partnerského centra CPV a přijetí smlouvy CPV můžete:</span><span class="sxs-lookup"><span data-stu-id="6b0d2-117">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="6b0d2-118">Spravujte aplikace s více klienty (přidejte aplikace pro Azure Portal, registraci a zrušení registrace aplikací v partnerském centru).</span><span class="sxs-lookup"><span data-stu-id="6b0d2-118">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="6b0d2-119">Aby bylo možné získat oprávnění pro Partnerské centrum rozhraní API, musí si procesory zaregistrovat své Partnerské centrum aplikace.</span><span class="sxs-lookup"><span data-stu-id="6b0d2-119">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="6b0d2-120">Přidáním aplikací do Azure Portal ne autorizuje aplikace CPV pro Partnerské centrum API.</span><span class="sxs-lookup"><span data-stu-id="6b0d2-120">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="6b0d2-121">Zobrazení a správa profilu CPV</span><span class="sxs-lookup"><span data-stu-id="6b0d2-121">View and manage your CPV profile</span></span> 

- <span data-ttu-id="6b0d2-122">Zobrazení a správa uživatelů, kteří potřebují přístup k funkcím CPV</span><span class="sxs-lookup"><span data-stu-id="6b0d2-122">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="6b0d2-123">Globální správce je jediná role, kterou může mít CPV.</span><span class="sxs-lookup"><span data-stu-id="6b0d2-123">Global admin is the only role a CPV can have.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6b0d2-124">Další kroky</span><span class="sxs-lookup"><span data-stu-id="6b0d2-124">Next steps</span></span>

<span data-ttu-id="6b0d2-125">-[Přidání dalších tenantů do Partnerské centrum účtu](multi-tenant-account.md)</span><span class="sxs-lookup"><span data-stu-id="6b0d2-125">-[Add additional tenants to your Partner Center account](multi-tenant-account.md)</span></span>