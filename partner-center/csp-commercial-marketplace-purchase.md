---
title: Nákup nabídek pro komerční web Marketplace
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si, jak partneři programu CSP můžou použít tržiště partnerského centra k nákupu SaaS nabídek od nezávislých dodavatelů softwaru (ISV).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 841308d535d4071ee0a8eabf3e70325edea5777c
ms.sourcegitcommit: a78dd3c532860d01867d116bfb4e2c88b84bcd25
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/08/2021
ms.locfileid: "97979712"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a><span data-ttu-id="b0854-103">Nákup produktů z komerčního tržiště pro vaše zákazníky v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="b0854-103">Purchase commercial marketplace products for your customers in Partner Center</span></span>


<span data-ttu-id="b0854-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="b0854-104">**Appropriate roles**</span></span>

- <span data-ttu-id="b0854-105">Globální správce</span><span class="sxs-lookup"><span data-stu-id="b0854-105">Global admin</span></span>
- <span data-ttu-id="b0854-106">Agent správce</span><span class="sxs-lookup"><span data-stu-id="b0854-106">Admin agent</span></span>

<span data-ttu-id="b0854-107">Jako partner v programu Cloud Solution Provider (CSP) můžete pomocí komerčního tržiště koupit předplatné pro zákazníky na určité produkty SaaS (software jako služba), které nabízí nezávislí dodavatelé softwaru (ISV).</span><span class="sxs-lookup"><span data-stu-id="b0854-107">As a partner in the Cloud Solution Provider (CSP) program, you can use the commercial marketplace to purchase subscriptions for your customers to certain Software as a Service (SaaS) products offered by Independent Software Vendors (ISVs).</span></span>

<span data-ttu-id="b0854-108">Díky nabídce předplatným ISV SaaS vašim zákazníkům můžete lépe odlišit své podnikání.</span><span class="sxs-lookup"><span data-stu-id="b0854-108">By offering ISV SaaS subscriptions to your customers, you can help differentiate your business.</span></span> <span data-ttu-id="b0854-109">Zákazníkům můžete také poskytnout přístup k softwarovým balíčkům, které řeší jejich konkrétní obchodní potřeby.</span><span class="sxs-lookup"><span data-stu-id="b0854-109">You can also give customers access to software bundles that address their specific business needs.</span></span> <span data-ttu-id="b0854-110">Licence a odběry pro tyto produkty SaaS z webu Marketplace od vydavatelů ISV můžete spravovat stejným způsobem jako vy při správě licencí a předplatných pro produkty Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="b0854-110">You manage licenses and subscriptions for these marketplace SaaS products from ISV publishers just as you manage licenses and subscriptions for Microsoft products.</span></span>

<span data-ttu-id="b0854-111">Můžete si koupit buď odběry SaaS **založené na licencích** , nebo předplatné **založené na využití** .</span><span class="sxs-lookup"><span data-stu-id="b0854-111">You can purchase either **license-based** SaaS subscriptions or **usage-based** subscriptions.</span></span> <span data-ttu-id="b0854-112">Další informace o rozdílu mezi účtováním na základě licencí a na základě využití najdete v tématu [základy fakturace](billing-basics.md).</span><span class="sxs-lookup"><span data-stu-id="b0854-112">To learn more about the difference between license-based and usage-based billing, see [Billing basics](billing-basics.md).</span></span>

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a><span data-ttu-id="b0854-113">Nákup SaaS předplatných na základě licencí a vyměřených předplatných v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="b0854-113">Purchase license-based and metered SaaS subscriptions in Partner Center</span></span>

<span data-ttu-id="b0854-114">Zakoupíte si předplatné pro produkty založené na licenci nebo SaaS, které nabízí vydavatelé ISV, pomocí stejného procesu, který používáte k nákupu předplatných pro produkty Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="b0854-114">You purchase subscriptions for license-based or metered SaaS products offered by ISV publishers using the same process you use to purchase subscriptions for Microsoft products.</span></span>

<span data-ttu-id="b0854-115">Pokud si chcete koupit předplatné SaaS na základě licence nebo účtované podle objemu dat v partnerském centru, přečtěte si téma [Vytvoření, pozastavení nebo zrušení zákaznických předplatných](create-a-new-subscription.md#create-a-new-subscription).</span><span class="sxs-lookup"><span data-stu-id="b0854-115">To purchase a license-based or metered SaaS subscription in Partner Center, see [Create, suspend, or cancel customer subscriptions](create-a-new-subscription.md#create-a-new-subscription).</span></span>

<span data-ttu-id="b0854-116">[Rozhraní API partnerského centra](/partner-center/develop/) můžete použít také k vytváření předplatných komerčního tržiště pro vaše zákazníky.</span><span class="sxs-lookup"><span data-stu-id="b0854-116">You can also use [Partner Center APIs](/partner-center/develop/) to create commercial marketplace subscriptions for your customers.</span></span> <span data-ttu-id="b0854-117">(Další informace o používání rozhraní API partnerského centra najdete v tématu [Vytvoření odběru pro produkty z komerčního tržiště](/partner-center/develop/create-subscription-azure-marketplace-products).)</span><span class="sxs-lookup"><span data-stu-id="b0854-117">(For more info on using Partner Center APIs, see [Create a subscription for commercial marketplace products](/partner-center/develop/create-subscription-azure-marketplace-products).)</span></span>

>[!IMPORTANT]
> <span data-ttu-id="b0854-118">Jako partner v programu CSP si můžete koupit předplatné SaaS **založené na licencích** nebo **účtované podle objemu** od vydavatelů ISV v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="b0854-118">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="b0854-119">To znamená, že si můžete koupit jakoukoli nabídku **založenou na licencích** nebo **měřený** SaaS. Vydavatel ISV vám k dispozici, včetně [exkluzivních nabídek](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) , ke kterým máte přístup.</span><span class="sxs-lookup"><span data-stu-id="b0854-119">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="b0854-120">Pokud si chcete koupit nebo spravovat jiné komerční nabídky na webu Marketplace od nezávislého výrobce softwaru (jako jsou nabídky na základě využití zahrnující aplikace a kontejnery Azure), musíte přejít na [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="b0854-120">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a><span data-ttu-id="b0854-121">Nákup předplatných na základě využití v Azure Portal</span><span class="sxs-lookup"><span data-stu-id="b0854-121">Purchase usage-based subscriptions in the Azure portal</span></span>

<span data-ttu-id="b0854-122">Na rozdíl od předplatných SaaS založených na licencích od vydavatelů ISV, předplatná založená na využití nejprve vyžadují, aby zákazník měl předplatné Azure.</span><span class="sxs-lookup"><span data-stu-id="b0854-122">In contrast to license-based SaaS subscriptions from third-party ISV publishers, usage-based subscriptions first require a customer to have an Azure subscription.</span></span> <span data-ttu-id="b0854-123">Fakturace za komerční tržiště, prostředky na základě využití spadají do předplatného Azure zákazníka.</span><span class="sxs-lookup"><span data-stu-id="b0854-123">Billing for commercial marketplace, usage-based resources falls under the customer's Azure subscription.</span></span> <span data-ttu-id="b0854-124">Jakmile má zákazník předplatné Azure, může partner v programu CSP pomocí těchto kroků koupit předplatné komerčního tržiště pro tyto uživatele:</span><span class="sxs-lookup"><span data-stu-id="b0854-124">Once your customer has an Azure subscription, a partner in the CSP program can follow these steps to purchase a commercial marketplace subscription for them:</span></span>

1. <span data-ttu-id="b0854-125">Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard)partnerského centra a v nabídce na levé straně vyberte **zákazníci** .</span><span class="sxs-lookup"><span data-stu-id="b0854-125">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **Customers** from the left-hand menu.</span></span>

2. <span data-ttu-id="b0854-126">Vyberte konkrétního zákazníka a pak vyberte **předplatná**.</span><span class="sxs-lookup"><span data-stu-id="b0854-126">Select the specific customer, then select **Subscriptions**.</span></span>  

3. <span data-ttu-id="b0854-127">V části **předplatná založená na využití** vyberte **všechny prostředky**.</span><span class="sxs-lookup"><span data-stu-id="b0854-127">Under the **Usage-based subscriptions**, select **All resources**.</span></span> <span data-ttu-id="b0854-128">Tím přejdete na portál pro správu Azure.</span><span class="sxs-lookup"><span data-stu-id="b0854-128">This takes you to the Azure Management portal.</span></span>

4. <span data-ttu-id="b0854-129">Na portálu pro správu Azure vyberte v nabídce na levé straně **vytvořit prostředek** .</span><span class="sxs-lookup"><span data-stu-id="b0854-129">In the Azure Management portal, select **Create a resource** from the left-hand menu.</span></span>

5. <span data-ttu-id="b0854-130">V horní části seznamu Azure Marketplace vyberte **Zobrazit vše** .</span><span class="sxs-lookup"><span data-stu-id="b0854-130">Select **See all** at the top of the Azure Marketplace list.</span></span>

6. <span data-ttu-id="b0854-131">Pokud chcete seznam zúžit, použijte filtry v horní části seznamu Marketplace.</span><span class="sxs-lookup"><span data-stu-id="b0854-131">To narrow your list, use filters at the top of the Marketplace list.</span></span> <span data-ttu-id="b0854-132">V rozevíracím seznamu **vydavatele** můžete například vybrat **Microsoft** nebo **partner** a zobrazit jenom nabídky od Microsoftu nebo od vydavatele ISV.</span><span class="sxs-lookup"><span data-stu-id="b0854-132">For example, you can select **Microsoft** or **Partner** from the **Publisher** dropdown list to view only offers from Microsoft or those from an ISV publisher.</span></span>

7. <span data-ttu-id="b0854-133">Zvolte konkrétní nabídku a pak vyberte **vytvořit**.</span><span class="sxs-lookup"><span data-stu-id="b0854-133">Choose a specific offer, then select **Create**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b0854-134">Další kroky</span><span class="sxs-lookup"><span data-stu-id="b0854-134">Next steps</span></span>

- [<span data-ttu-id="b0854-135">Správa nabídek komerčních Marketplace</span><span class="sxs-lookup"><span data-stu-id="b0854-135">Manage commercial marketplace offers</span></span>](csp-commercial-marketplace-purchase.md)