---
title: Azure Cost Management by Cloudyn pro poskytovatele CSP
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se, jak zaregistrovat webovou aplikaci v Cloudyn a používat pro ni tajný klíč v partnerském centru, abyste mohli používat aplikaci ke sledování zákaznických využití a nákladů.
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: defa691a3bc70cbda45f01cb447d89364a49e3b8
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534980"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a><span data-ttu-id="acb26-103">Sledování využití a nákladů zákazníků Azure pomocí aplikace Azure cost management pro partnery CSP</span><span class="sxs-lookup"><span data-stu-id="acb26-103">Track customer Azure usage and costs with the Azure cost management app for CSP partners</span></span>  

<span data-ttu-id="acb26-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="acb26-104">**Appropriate roles**</span></span>

- <span data-ttu-id="acb26-105">Globální správce</span><span class="sxs-lookup"><span data-stu-id="acb26-105">Global admin</span></span>
- <span data-ttu-id="acb26-106">Agent správce</span><span class="sxs-lookup"><span data-stu-id="acb26-106">Admin agent</span></span>

[<span data-ttu-id="acb26-107">Získat další informace o Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="acb26-107">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="acb26-108">Než začnete</span><span class="sxs-lookup"><span data-stu-id="acb26-108">Before you begin</span></span>
<span data-ttu-id="acb26-109">Než budete moci použít Azure Cost Management, ujistěte se, že splňujete následující požadavky:</span><span class="sxs-lookup"><span data-stu-id="acb26-109">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="acb26-110">Jste partnerem v programu Cloud Solution Provider.</span><span class="sxs-lookup"><span data-stu-id="acb26-110">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="acb26-111">Máte možnost vytvořit webovou aplikaci rozhraní API partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="acb26-111">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="acb26-112">Přehled</span><span class="sxs-lookup"><span data-stu-id="acb26-112">Overview</span></span>

<span data-ttu-id="acb26-113">Cloudyn je webová aplikace, která umožňuje sledovat a spravovat, kolik zákazníků využívá Azure, a náklady na toto využití.</span><span class="sxs-lookup"><span data-stu-id="acb26-113">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="acb26-114">Použijete ji prostřednictvím rozhraní API partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="acb26-114">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="acb26-115">Registrace webové aplikace v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="acb26-115">Register your web app in the Partner Center</span></span>
<span data-ttu-id="acb26-116">Když zaregistrujete Azure Active Directory webovou aplikaci v partnerském centru, povolíte přístup k rozhraní API partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="acb26-116">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="acb26-117">Přihlaste se k [partnerskému centru](https://partnercenter.microsoft.com/pcv/dashboard/overview) pomocí [účtu globálního správce nebo agenta správce](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="acb26-117">Sign into [Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="acb26-118">Z **partnerského centra** vyberte **Nastavení účtu** &gt; **[Správa aplikací](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span><span class="sxs-lookup"><span data-stu-id="acb26-118">From **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="acb26-119">V části **Webová aplikace** klikněte na **Přidat novou webovou aplikaci**.</span><span class="sxs-lookup"><span data-stu-id="acb26-119">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="acb26-120">**Poznámka**: Pokud jste dříve vytvořili webovou aplikaci, můžete přeskočit krok 3.</span><span class="sxs-lookup"><span data-stu-id="acb26-120">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="acb26-121">Zkopírujte a uložte GUID **ID pro Commerce ID** a identifikátor GUID **ID aplikace** pro vaši webovou aplikaci.</span><span class="sxs-lookup"><span data-stu-id="acb26-121">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="acb26-122">K používání 30denní bezplatné zkušební verze aplikace Azure cost management budete potřebovat obě ID.</span><span class="sxs-lookup"><span data-stu-id="acb26-122">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="acb26-123">Přidání tajného klíče do aplikace</span><span class="sxs-lookup"><span data-stu-id="acb26-123">Add a secret key to your app</span></span>
1. <span data-ttu-id="acb26-124">V rozevíracím seznamu vedle tlačítka **Přidat klíč** vyberte dobu trvání 1 nebo 2 roky.</span><span class="sxs-lookup"><span data-stu-id="acb26-124">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="acb26-125">Klikněte na **Přidat klíč**.</span><span class="sxs-lookup"><span data-stu-id="acb26-125">Click **Add key**.</span></span> 
3. <span data-ttu-id="acb26-126">Zkopírujte a uložte hodnotu tajného klíče.</span><span class="sxs-lookup"><span data-stu-id="acb26-126">Copy and save the secret key value.</span></span> <span data-ttu-id="acb26-127">Budete ho potřebovat pro 30denní bezplatnou zkušební verzi.</span><span class="sxs-lookup"><span data-stu-id="acb26-127">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="acb26-128">Tajné klíče aplikace jako hesla mají delší datum vypršení platnosti.</span><span class="sxs-lookup"><span data-stu-id="acb26-128">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="acb26-129">Uložte prosím hodnotu klíče do zabezpečeného umístění pro budoucí použití.</span><span class="sxs-lookup"><span data-stu-id="acb26-129">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="acb26-130">Další kroky</span><span class="sxs-lookup"><span data-stu-id="acb26-130">Next steps</span></span>
<span data-ttu-id="acb26-131">Spusťte [30denní bezplatnou zkušební verzi](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="acb26-131">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="acb26-132">Ke spuštění zkušební verze potřebujete následující podrobnosti:</span><span class="sxs-lookup"><span data-stu-id="acb26-132">You need the following details to start the trial:</span></span>
- <span data-ttu-id="acb26-133">Přihlašovací údaje pro přihlašovací údaje partnerského centra</span><span class="sxs-lookup"><span data-stu-id="acb26-133">Partner Center sign in credentials</span></span>
- <span data-ttu-id="acb26-134">Identifikátor GUID ID obchodu</span><span class="sxs-lookup"><span data-stu-id="acb26-134">Commerce ID GUID</span></span>
- <span data-ttu-id="acb26-135">Identifikátor GUID ID aplikace</span><span class="sxs-lookup"><span data-stu-id="acb26-135">App ID GUID</span></span>
- <span data-ttu-id="acb26-136">Hodnota tajného klíče aplikace</span><span class="sxs-lookup"><span data-stu-id="acb26-136">Application secret key value</span></span>
