---
title: Vytvořit přidružení zákazníka
ms.topic: article
ms.date: 09/11/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Vytvořte přidružení zákazníka s modelem deklarace identity Partner of Record (CPOR). Pomáhá spravovat prodej, použití, pobídky pro Microsoft 365 & zákazníky Dynamics 365.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e34698b51a159445f4354e366f79f510533e6f30
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/19/2020
ms.locfileid: "92527737"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a><span data-ttu-id="b6b0d-104">Přidružení zákazníků prostřednictvím deklarovaného modelu CPOR (Partner of Record) pro Microsoft 365 a Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="b6b0d-104">Customer associations via the Claimed Partner of Record (CPOR) model for Microsoft 365 and Dynamics 365</span></span>

<span data-ttu-id="b6b0d-105">**Platí pro**</span><span class="sxs-lookup"><span data-stu-id="b6b0d-105">**Applies to**</span></span>

- <span data-ttu-id="b6b0d-106">Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="b6b0d-106">Partner Center</span></span>

<span data-ttu-id="b6b0d-107">**Příslušné role:**</span><span class="sxs-lookup"><span data-stu-id="b6b0d-107">**Appropriate roles:**</span></span>

- <span data-ttu-id="b6b0d-108">Motivace správce</span><span class="sxs-lookup"><span data-stu-id="b6b0d-108">Incentives admin</span></span>

<span data-ttu-id="b6b0d-109">Od 1. října 2019 společnost Microsoft začala používat model CPOR (claiming Partner of Record) pro správu přidružení, která máte s vašimi zákazníky s Microsoft 365 a Dynamics 365, s ohledem na online Poradce pro služby Online Services (OSU) – Microsoft 365 a OSU-Business motivace aplikací.</span><span class="sxs-lookup"><span data-stu-id="b6b0d-109">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regards to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentives.</span></span>

>[!Important]
> <span data-ttu-id="b6b0d-110">Deklarace identity Customer (CPOR) se vztahují jenom na zákazníky Online Services Advisor (OSA), používání služeb online (OSU) – Microsoft 365 a OSU-Business aplikací pro motivaci aplikací.</span><span class="sxs-lookup"><span data-stu-id="b6b0d-110">Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="b6b0d-111">Pokud odesíláte deklaraci identity pro jiný program, třeba pro Cloud Solution Provider, spravovaného prodejce, hostování nebo Surface, přečtěte si prosím proces deklarace identity, který je zde popsaný.</span><span class="sxs-lookup"><span data-stu-id="b6b0d-111">If you are submitting a co-op claim for another program such as Cloud Solution Provider, Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span> <br><br><span data-ttu-id="b6b0d-112">Po odeslání vaší deklarace ji Microsoft ověří.</span><span class="sxs-lookup"><span data-stu-id="b6b0d-112">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="b6b0d-113">V tomto okamžiku vám můžeme požádat o další informace.</span><span class="sxs-lookup"><span data-stu-id="b6b0d-113">We may ask you for more information at this point.</span></span> <span data-ttu-id="b6b0d-114">Také upozorníme zákazníka na vaši žádost o přidružení.</span><span class="sxs-lookup"><span data-stu-id="b6b0d-114">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="b6b0d-115">Zákazníci mají pět pracovních dnů na odhlášení. Pokud se nerozhodnete, vaše přidružení k tomuto konkrétnímu tenantovi a úlohám budou oficiální.</span><span class="sxs-lookup"><span data-stu-id="b6b0d-115">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="b6b0d-116">V tomto okamžiku budete mít přístup k datům o využití zákazníka.</span><span class="sxs-lookup"><span data-stu-id="b6b0d-116">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="b6b0d-117">K dokončení deklarace identity budete potřebovat následující informace:</span><span class="sxs-lookup"><span data-stu-id="b6b0d-117">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="b6b0d-118">**ID MPN** pro vaši entitu, která provádí deklaraci identity</span><span class="sxs-lookup"><span data-stu-id="b6b0d-118">The **MPN ID** for your entity that makes the claim</span></span>

- <span data-ttu-id="b6b0d-119">**Název domény** zákazníka [najdete](find-domain-name.md) tady.</span><span class="sxs-lookup"><span data-stu-id="b6b0d-119">Customer's **domain name** [Find this](find-domain-name.md)</span></span>

- <span data-ttu-id="b6b0d-120">[Toto zjištění](find-domain-name.md) **ID adresáře** nebo **ID tenanta** zákazníka</span><span class="sxs-lookup"><span data-stu-id="b6b0d-120">Customer's **Directory ID** or **Tenant ID** [Find this](find-domain-name.md)</span></span>

- <span data-ttu-id="b6b0d-121">**Oblast řešení** , například Business Applications nebo Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="b6b0d-121">The **Solution area** , such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="b6b0d-122">**Aktivita** , kterou jste provedli, a typ deklarace identity, kterou chcete provést, například přidružení před prodejem, využití nebo výnosy</span><span class="sxs-lookup"><span data-stu-id="b6b0d-122">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="b6b0d-123">**Kontaktní jméno** , název a e-mailové adresy vašeho zákazníka</span><span class="sxs-lookup"><span data-stu-id="b6b0d-123">Your customer's **Contact name** , title, and email address</span></span>

- <span data-ttu-id="b6b0d-124">Pro Dynamics 365 musíte taky **zadat jméno, název a** e-mailovou adresu zákazníka.</span><span class="sxs-lookup"><span data-stu-id="b6b0d-124">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="b6b0d-125">**Kontaktní jméno** a e-mailová adresa vaší společnosti</span><span class="sxs-lookup"><span data-stu-id="b6b0d-125">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="b6b0d-126">Vytvoříte **název** této deklarace identity.</span><span class="sxs-lookup"><span data-stu-id="b6b0d-126">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="b6b0d-127">**Produkt (y)** nebo úlohy, na které přidáváte nárok</span><span class="sxs-lookup"><span data-stu-id="b6b0d-127">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="b6b0d-128">**Důkaz provedení (PoE)** , jako je například prohlášení o práci podepsané zákazníkem.</span><span class="sxs-lookup"><span data-stu-id="b6b0d-128">**Proof of execution (PoE)** , such as a statement of work signed by the customer.</span></span> <span data-ttu-id="b6b0d-129">Můžete si také stáhnout šablonu PoE, která se má použít.</span><span class="sxs-lookup"><span data-stu-id="b6b0d-129">You can also download a PoE template to use.</span></span>

- <span data-ttu-id="b6b0d-130">Jenom pro partnery, kteří mají nárok na přiřazení výnosů: **název prodávajícího řešení** , jméno **zákazníka** a **název produktu/řešení ISV** .</span><span class="sxs-lookup"><span data-stu-id="b6b0d-130">For partners claiming revenue association only: **Dynamics solution seller name** , **Customer name** , and **Name of ISV product/solution** .</span></span> 

<span data-ttu-id="b6b0d-131">Měli byste taky pochopit následující body:</span><span class="sxs-lookup"><span data-stu-id="b6b0d-131">You should also understand the following points:</span></span>

- <span data-ttu-id="b6b0d-132">Pokud již máte Microsoft 365 zákazníky, bude nutné znovu přidružit ty, které chcete nadále získávat OSU pobídky pomocí tohoto procesu.</span><span class="sxs-lookup"><span data-stu-id="b6b0d-132">If you have existing Microsoft 365 customers, you'll need to re-associate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="b6b0d-133">Pokud máte existující přidružení k Dynamics 365 nebo zákazníkům Power BI, budou tato přidružení platit až do vypršení platnosti jejich předplatných.</span><span class="sxs-lookup"><span data-stu-id="b6b0d-133">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="b6b0d-134">Zákazník může mít více partnerů, ale každá úloha (pro OSU-Microsoft 365) nebo předplatné (pro OSA-Sell a OSU-Business aplikace) může být přidružená jenom k jednomu partnerovi.</span><span class="sxs-lookup"><span data-stu-id="b6b0d-134">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="b6b0d-135">Vytvořit přidružení zákazníka</span><span class="sxs-lookup"><span data-stu-id="b6b0d-135">Create a customer association</span></span>

1. <span data-ttu-id="b6b0d-136">Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="b6b0d-136">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="b6b0d-137">Vyberte kartu **pobídky** , vyberte **Přehled** a pak vyberte **přidružení zákazníků** .</span><span class="sxs-lookup"><span data-stu-id="b6b0d-137">Select the **Incentives** tab, select **Overview** , and then select **Customer associations** .</span></span>

3. <span data-ttu-id="b6b0d-138">V horní části stránky přidružení zákazníka vyberte **+ přidružení zákazníka** .</span><span class="sxs-lookup"><span data-stu-id="b6b0d-138">At the top of the Customer associations page, select **+ Customer association** .</span></span>

4. <span data-ttu-id="b6b0d-139">Vyberte **ID MPN** umístění partnera, které se má k zákazníkovi přidružit, a pak přidejte název domény zákazníka a ID adresáře.</span><span class="sxs-lookup"><span data-stu-id="b6b0d-139">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="b6b0d-140">Najít</span><span class="sxs-lookup"><span data-stu-id="b6b0d-140">Find this</span></span>](find-domain-name.md)

5. <span data-ttu-id="b6b0d-141">Vyberte **Pokračovat** .</span><span class="sxs-lookup"><span data-stu-id="b6b0d-141">Select **Continue** .</span></span>

6. <span data-ttu-id="b6b0d-142">Vyberte **oblast řešení** a **aktivitu** .</span><span class="sxs-lookup"><span data-stu-id="b6b0d-142">Select the **Solution area** and **Activity** .</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="b6b0d-143">Pokud vyberete Business Applications, vyberte buď možnost **použití nebo přidružení před prodejem** nebo **výnosy** , a pak vyberte **pokračovat** .</span><span class="sxs-lookup"><span data-stu-id="b6b0d-143">If you select Business Applications, select either **Usage and/or Pre-sales** , or **Revenue association** , and then select **Continue** .</span></span> 
   <br><br><span data-ttu-id="b6b0d-144">Pokud vyberete Přidružení výnosů, zobrazí se výzva k zadání mírně odlišných informací, než jsou uvedené níže.</span><span class="sxs-lookup"><span data-stu-id="b6b0d-144">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

7. <span data-ttu-id="b6b0d-145">Zadejte příslušné informace na stránce **přidružit zákazníka** a potom vyberte **vytvořit deklaraci identity** .</span><span class="sxs-lookup"><span data-stu-id="b6b0d-145">Enter the appropriate information on the **Associate customer** page, and then select **Create claim** .</span></span>

8. <span data-ttu-id="b6b0d-146">Vyberte produkty přidružené k tomuto přidružení zákazníka a pak vyberte **pokračovat** .</span><span class="sxs-lookup"><span data-stu-id="b6b0d-146">Select the product(s) associated with this customer association, and then select **Continue** .</span></span>

9. <span data-ttu-id="b6b0d-147">Vyplňte kontaktní údaje zákazníka a vaší společnosti.</span><span class="sxs-lookup"><span data-stu-id="b6b0d-147">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="b6b0d-148">Všechna pole jsou povinná.</span><span class="sxs-lookup"><span data-stu-id="b6b0d-148">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="b6b0d-149">Pokud máte produkt Dynamics 365 a produkt, který zvolíte, má více předplatných pro tohoto konkrétního zákazníka, budete také muset zadat ID předplatného.</span><span class="sxs-lookup"><span data-stu-id="b6b0d-149">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

10. <span data-ttu-id="b6b0d-150">Poskytněte důkaz o provedení (PoE).</span><span class="sxs-lookup"><span data-stu-id="b6b0d-150">Supply your proof of execution (PoE).</span></span> <span data-ttu-id="b6b0d-151">Můžete ho přetáhnout do pole, vyhledat ve vaší doprovodné dokumentaci nebo vybrat **Stáhnout šablonu** a použít šablonu.</span><span class="sxs-lookup"><span data-stu-id="b6b0d-151">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template** .</span></span> 

11. <span data-ttu-id="b6b0d-152">Pokud chcete, přidejte a uložte komentáře, a pak vyberte **Odeslat žádost** .</span><span class="sxs-lookup"><span data-stu-id="b6b0d-152">Add and save comments if you like, and then select **Submit claim** .</span></span> <span data-ttu-id="b6b0d-153">Zákazníkovi pošleme e-mail s žádostí o schválení vašeho přidružení zákazníka.</span><span class="sxs-lookup"><span data-stu-id="b6b0d-153">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="b6b0d-154">Po odeslání přidružení zákazníka ho nemůžete upravovat.</span><span class="sxs-lookup"><span data-stu-id="b6b0d-154">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="b6b0d-155">Stav vašeho přidružení zákazníka se zobrazí v poli **Stav** .</span><span class="sxs-lookup"><span data-stu-id="b6b0d-155">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="b6b0d-156">Výběrem **Historie** můžete zobrazit historii přidružení zákazníka.</span><span class="sxs-lookup"><span data-stu-id="b6b0d-156">Select **History** to view the history of a customer association.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b6b0d-157">Další kroky</span><span class="sxs-lookup"><span data-stu-id="b6b0d-157">Next steps</span></span>

- [<span data-ttu-id="b6b0d-158">Správa přidružení zákazníků</span><span class="sxs-lookup"><span data-stu-id="b6b0d-158">Manage customer associations</span></span>](incentives-manage-customer-associations.md)