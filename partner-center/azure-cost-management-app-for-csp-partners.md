---
title: Azure Cost Management Cloudyn pro zprostředkovatele CSP
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se, jak zaregistrovat webovou aplikaci v Cloudyn a používat pro ni tajný klíč v partnerském centru, abyste mohli používat aplikaci ke sledování zákaznických využití a nákladů.
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4ea156ef0932fe1af20f3e3c4b9be1a5f931cdde
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/17/2020
ms.locfileid: "92527025"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a><span data-ttu-id="7c40b-103">Sledování využití a nákladů zákazníků Azure pomocí aplikace Azure cost management pro partnery CSP</span><span class="sxs-lookup"><span data-stu-id="7c40b-103">Track customer Azure usage and costs with the Azure cost management app for CSP partners</span></span>  

<span data-ttu-id="7c40b-104">**Platí pro**</span><span class="sxs-lookup"><span data-stu-id="7c40b-104">**Applies to**</span></span>

- <span data-ttu-id="7c40b-105">Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="7c40b-105">Partner Center</span></span>
- <span data-ttu-id="7c40b-106">Partneři programu Cloud Solution Provider</span><span class="sxs-lookup"><span data-stu-id="7c40b-106">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="7c40b-107">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="7c40b-107">**Appropriate roles**</span></span>

- <span data-ttu-id="7c40b-108">Globální správce</span><span class="sxs-lookup"><span data-stu-id="7c40b-108">Global admin</span></span>
- <span data-ttu-id="7c40b-109">Agent správce</span><span class="sxs-lookup"><span data-stu-id="7c40b-109">Admin agent</span></span>

[<span data-ttu-id="7c40b-110">Získat další informace o Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="7c40b-110">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="7c40b-111">Než začnete</span><span class="sxs-lookup"><span data-stu-id="7c40b-111">Before you begin</span></span>
<span data-ttu-id="7c40b-112">Než budete moci použít Azure Cost Management, ujistěte se, že splňujete následující požadavky:</span><span class="sxs-lookup"><span data-stu-id="7c40b-112">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="7c40b-113">Jste partnerem v programu Cloud Solution Provider.</span><span class="sxs-lookup"><span data-stu-id="7c40b-113">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="7c40b-114">Máte možnost vytvořit webovou aplikaci rozhraní API partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="7c40b-114">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="7c40b-115">Přehled</span><span class="sxs-lookup"><span data-stu-id="7c40b-115">Overview</span></span>

<span data-ttu-id="7c40b-116">Cloudyn je webová aplikace, která umožňuje sledovat a spravovat, kolik zákazníků využívá Azure, a náklady na toto využití.</span><span class="sxs-lookup"><span data-stu-id="7c40b-116">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="7c40b-117">Použijete ji prostřednictvím rozhraní API partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="7c40b-117">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="7c40b-118">Registrace webové aplikace v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="7c40b-118">Register your web app in the Partner Center</span></span>
<span data-ttu-id="7c40b-119">Když zaregistrujete Azure Active Directory webovou aplikaci v partnerském centru, povolíte přístup k rozhraní API partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="7c40b-119">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="7c40b-120">Přihlaste [se k partnerskému centru](https://partnercenter.microsoft.com/pcv/dashboard/overview) pomocí [účtu globálního správce nebo agenta správce](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="7c40b-120">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="7c40b-121">V **partnerském centru** vyberte **Nastavení účtu** &gt; **[Správa aplikací](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** .</span><span class="sxs-lookup"><span data-stu-id="7c40b-121">From the **Partner Center** , select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** .</span></span>
3.  <span data-ttu-id="7c40b-122">V části **Webová aplikace** klikněte na **Přidat novou webovou aplikaci** .</span><span class="sxs-lookup"><span data-stu-id="7c40b-122">In the **Web App** section, click **Add new web app** .</span></span>
<br> <span data-ttu-id="7c40b-123">**Poznámka** : Pokud jste dříve vytvořili webovou aplikaci, můžete přeskočit krok 3.</span><span class="sxs-lookup"><span data-stu-id="7c40b-123">**Note** : If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="7c40b-124">Zkopírujte a uložte GUID **ID pro Commerce ID** a identifikátor GUID **ID aplikace** pro vaši webovou aplikaci.</span><span class="sxs-lookup"><span data-stu-id="7c40b-124">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="7c40b-125">K používání 30denní bezplatné zkušební verze aplikace Azure cost management budete potřebovat obě ID.</span><span class="sxs-lookup"><span data-stu-id="7c40b-125">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="7c40b-126">Přidání tajného klíče do aplikace</span><span class="sxs-lookup"><span data-stu-id="7c40b-126">Add a secret key to your app</span></span>
1. <span data-ttu-id="7c40b-127">V rozevíracím seznamu vedle tlačítka **Přidat klíč** vyberte dobu trvání 1 nebo 2 roky.</span><span class="sxs-lookup"><span data-stu-id="7c40b-127">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="7c40b-128">Klikněte na **Přidat klíč** .</span><span class="sxs-lookup"><span data-stu-id="7c40b-128">Click **Add key** .</span></span> 
3. <span data-ttu-id="7c40b-129">Zkopírujte a uložte hodnotu tajného klíče.</span><span class="sxs-lookup"><span data-stu-id="7c40b-129">Copy and save the secret key value.</span></span> <span data-ttu-id="7c40b-130">Budete ho potřebovat pro 30denní bezplatnou zkušební verzi.</span><span class="sxs-lookup"><span data-stu-id="7c40b-130">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="7c40b-131">Tajné klíče aplikace jako hesla mají delší datum vypršení platnosti.</span><span class="sxs-lookup"><span data-stu-id="7c40b-131">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="7c40b-132">Uložte prosím hodnotu klíče do zabezpečeného umístění pro budoucí použití.</span><span class="sxs-lookup"><span data-stu-id="7c40b-132">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7c40b-133">Další kroky</span><span class="sxs-lookup"><span data-stu-id="7c40b-133">Next steps</span></span>
<span data-ttu-id="7c40b-134">Spusťte [30denní bezplatnou zkušební verzi](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="7c40b-134">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="7c40b-135">Ke spuštění zkušební verze potřebujete následující podrobnosti:</span><span class="sxs-lookup"><span data-stu-id="7c40b-135">You need the following details to start the trial:</span></span>
- <span data-ttu-id="7c40b-136">Přihlašovací údaje pro přihlašovací údaje partnerského centra</span><span class="sxs-lookup"><span data-stu-id="7c40b-136">Partner Center sign in credentials</span></span>
- <span data-ttu-id="7c40b-137">Identifikátor GUID ID obchodu</span><span class="sxs-lookup"><span data-stu-id="7c40b-137">Commerce ID GUID</span></span>
- <span data-ttu-id="7c40b-138">Identifikátor GUID ID aplikace</span><span class="sxs-lookup"><span data-stu-id="7c40b-138">App ID GUID</span></span>
- <span data-ttu-id="7c40b-139">Hodnota tajného klíče aplikace</span><span class="sxs-lookup"><span data-stu-id="7c40b-139">Application secret key value</span></span>
