---
title: Vytvoření přidružení zákazníka
ms.topic: article
ms.date: 10/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Vytvořte přidružení zákazníka s modelem deklarace identity Partner of Record (CPOR). Pomáhá spravovat prodej, použití, pobídky pro Microsoft 365 & zákazníky Dynamics 365.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7a7e3ed40dcc6b1248f008201bff667a9eb9a0f8
ms.sourcegitcommit: ec33c2352a9dd3e5a941f0f42ff1e8d256bb2399
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/24/2021
ms.locfileid: "105028311"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a><span data-ttu-id="20944-104">Přidružení zákazníků prostřednictvím deklarovaného modelu CPOR (Partner of Record) pro Microsoft 365 a Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="20944-104">Customer associations via the Claimed Partner of Record (CPOR) model for Microsoft 365 and Dynamics 365</span></span>


<span data-ttu-id="20944-105">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="20944-105">**Appropriate roles**</span></span>

- <span data-ttu-id="20944-106">Motivace správce</span><span class="sxs-lookup"><span data-stu-id="20944-106">Incentives admin</span></span>

<span data-ttu-id="20944-107">Od 1. října 2019 společnost Microsoft zahájila používání modelu CPOR (Claim Partner of Record) pro správu přidružení, která máte s vašimi zákazníky Microsoft 365 a Dynamics 365 s ohledem na online Poradce pro služby Online Services (OSU) – Microsoft 365 a OSU-Businessch motivů aplikací.</span><span class="sxs-lookup"><span data-stu-id="20944-107">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regard to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365, and OSU-Business Application incentives.</span></span>

>[!Important]
> <span data-ttu-id="20944-108">Deklarace identity Customer (CPOR) se vztahují jenom na zákazníky Online Services Advisor (OSA), používání služeb online (OSU) – Microsoft 365 a OSU-Business aplikací pro motivaci aplikací.</span><span class="sxs-lookup"><span data-stu-id="20944-108">Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="20944-109">Pokud odesíláte deklaraci identity pro jiný program, třeba pro Cloud Solution Provider, spravovaného prodejce, hostování nebo Surface, přečtěte si prosím proces deklarace identity, který je zde popsaný.</span><span class="sxs-lookup"><span data-stu-id="20944-109">If you are submitting a co-op claim for another program such as Cloud Solution Provider, Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span> <br><br><span data-ttu-id="20944-110">Po odeslání vaší deklarace ji Microsoft ověří.</span><span class="sxs-lookup"><span data-stu-id="20944-110">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="20944-111">V tomto okamžiku vám můžeme požádat o další informace.</span><span class="sxs-lookup"><span data-stu-id="20944-111">We may ask you for more information at this point.</span></span> <span data-ttu-id="20944-112">Také upozorníme zákazníka na vaši žádost o přidružení.</span><span class="sxs-lookup"><span data-stu-id="20944-112">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="20944-113">Zákazníci mají pět pracovních dnů na odhlášení. Pokud se nerozhodnete, vaše přidružení k tomuto konkrétnímu tenantovi a úlohám budou oficiální.</span><span class="sxs-lookup"><span data-stu-id="20944-113">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="20944-114">V tomto okamžiku budete mít přístup k datům o využití zákazníka.</span><span class="sxs-lookup"><span data-stu-id="20944-114">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="20944-115">K dokončení deklarace identity budete potřebovat následující informace:</span><span class="sxs-lookup"><span data-stu-id="20944-115">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="20944-116">**ID MPN** pro vaši entitu, která provádí deklaraci identity</span><span class="sxs-lookup"><span data-stu-id="20944-116">The **MPN ID** for your entity that makes the claim</span></span>

- <span data-ttu-id="20944-117">**Název domény** zákazníka [najdete](find-ids-and-domain-names.md) tady.</span><span class="sxs-lookup"><span data-stu-id="20944-117">Customer's **domain name** [Find this](find-ids-and-domain-names.md)</span></span>

- <span data-ttu-id="20944-118">[Toto zjištění](find-ids-and-domain-names.md) **ID adresáře** nebo **ID tenanta** zákazníka</span><span class="sxs-lookup"><span data-stu-id="20944-118">Customer's **Directory ID** or **Tenant ID** [Find this](find-ids-and-domain-names.md)</span></span>

- <span data-ttu-id="20944-119">**Oblast řešení**, například Business Applications nebo Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="20944-119">The **Solution area**, such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="20944-120">**Aktivita** , kterou jste provedli, a typ deklarace identity, kterou chcete provést, například přidružení před prodejem, využití nebo výnosy</span><span class="sxs-lookup"><span data-stu-id="20944-120">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="20944-121">**Kontaktní jméno**, název a e-mailové adresy vašeho zákazníka</span><span class="sxs-lookup"><span data-stu-id="20944-121">Your customer's **Contact name**, title, and email address</span></span>

- <span data-ttu-id="20944-122">Pro Dynamics 365 musíte taky **zadat jméno, název a** e-mailovou adresu zákazníka.</span><span class="sxs-lookup"><span data-stu-id="20944-122">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="20944-123">**Kontaktní jméno** a e-mailová adresa vaší společnosti</span><span class="sxs-lookup"><span data-stu-id="20944-123">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="20944-124">Vytvoříte **název** této deklarace identity.</span><span class="sxs-lookup"><span data-stu-id="20944-124">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="20944-125">**Produkt (y)** nebo úlohy, na které přidáváte nárok</span><span class="sxs-lookup"><span data-stu-id="20944-125">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="20944-126">**Důkaz provedení (PoE)**, jako je například prohlášení o práci podepsané zákazníkem.</span><span class="sxs-lookup"><span data-stu-id="20944-126">**Proof of execution (PoE)**, such as a statement of work signed by the customer.</span></span> <span data-ttu-id="20944-127">Můžete si také stáhnout šablonu PoE, která se má použít.</span><span class="sxs-lookup"><span data-stu-id="20944-127">You can also download a PoE template to use.</span></span>

- <span data-ttu-id="20944-128">Jenom pro partnery, kteří mají nárok na přiřazení výnosů: **název prodávajícího řešení**, jméno **zákazníka** a **název produktu/řešení ISV**.</span><span class="sxs-lookup"><span data-stu-id="20944-128">For partners claiming revenue association only: **Dynamics solution seller name**, **Customer name**, and **Name of ISV product/solution**.</span></span> 

<span data-ttu-id="20944-129">Měli byste taky pochopit následující body:</span><span class="sxs-lookup"><span data-stu-id="20944-129">You should also understand the following points:</span></span>

- <span data-ttu-id="20944-130">Pokud již máte Microsoft 365 zákazníky, bude nutné znovu přidružit ty, které chcete nadále získávat OSU pobídky pomocí tohoto procesu.</span><span class="sxs-lookup"><span data-stu-id="20944-130">If you have existing Microsoft 365 customers, you'll need to re-associate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="20944-131">Pokud máte existující přidružení k Dynamics 365 nebo zákazníkům Power BI, budou tato přidružení platit až do vypršení platnosti jejich předplatných.</span><span class="sxs-lookup"><span data-stu-id="20944-131">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="20944-132">Zákazník může mít více partnerů, ale každá úloha (pro OSU-Microsoft 365) nebo předplatné (pro OSA-Sell a OSU-Business aplikace) může být přidružená jenom k jednomu partnerovi.</span><span class="sxs-lookup"><span data-stu-id="20944-132">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="20944-133">Vytvoření přidružení zákazníka</span><span class="sxs-lookup"><span data-stu-id="20944-133">Create a customer association</span></span>

1. <span data-ttu-id="20944-134">Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="20944-134">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="20944-135">Vyberte kartu **pobídky** , vyberte **Přehled** a pak vyberte **přidružení zákazníků**.</span><span class="sxs-lookup"><span data-stu-id="20944-135">Select the **Incentives** tab, select **Overview**, and then select **Customer associations**.</span></span>

3. <span data-ttu-id="20944-136">V horní části stránky přidružení zákazníka vyberte **+ přidružení zákazníka**.</span><span class="sxs-lookup"><span data-stu-id="20944-136">At the top of the Customer associations page, select **+ Customer association**.</span></span>

4. <span data-ttu-id="20944-137">Vyberte **ID MPN** umístění partnera, které se má k zákazníkovi přidružit, a pak přidejte název domény zákazníka a ID adresáře.</span><span class="sxs-lookup"><span data-stu-id="20944-137">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="20944-138">Najít</span><span class="sxs-lookup"><span data-stu-id="20944-138">Find this</span></span>](find-ids-and-domain-names.md)

5. <span data-ttu-id="20944-139">Vyberte **Pokračovat**.</span><span class="sxs-lookup"><span data-stu-id="20944-139">Select **Continue**.</span></span>

6. <span data-ttu-id="20944-140">Vyberte **oblast řešení** a **aktivitu**.</span><span class="sxs-lookup"><span data-stu-id="20944-140">Select the **Solution area** and **Activity**.</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="20944-141">Pokud vyberete Business Applications, vyberte buď možnost **použití nebo přidružení před prodejem** nebo **výnosy**, a pak vyberte **pokračovat**.</span><span class="sxs-lookup"><span data-stu-id="20944-141">If you select Business Applications, select either **Usage and/or Pre-sales**, or **Revenue association**, and then select **Continue**.</span></span> 
   <br><br><span data-ttu-id="20944-142">Pokud vyberete Přidružení výnosů, zobrazí se výzva k zadání mírně odlišných informací, než jsou uvedené níže.</span><span class="sxs-lookup"><span data-stu-id="20944-142">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

7. <span data-ttu-id="20944-143">Zadejte příslušné informace na stránce **přidružit zákazníka** a potom vyberte **vytvořit deklaraci identity**.</span><span class="sxs-lookup"><span data-stu-id="20944-143">Enter the appropriate information on the **Associate customer** page, and then select **Create claim**.</span></span>

8. <span data-ttu-id="20944-144">Vyberte produkty přidružené k tomuto přidružení zákazníka a pak vyberte **pokračovat**.</span><span class="sxs-lookup"><span data-stu-id="20944-144">Select the product(s) associated with this customer association, and then select **Continue**.</span></span>

9. <span data-ttu-id="20944-145">Vyplňte kontaktní údaje zákazníka a vaší společnosti.</span><span class="sxs-lookup"><span data-stu-id="20944-145">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="20944-146">Všechna pole jsou povinná.</span><span class="sxs-lookup"><span data-stu-id="20944-146">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="20944-147">Pokud máte produkt Dynamics 365 a produkt, který zvolíte, má více předplatných pro tohoto konkrétního zákazníka, budete také muset zadat ID předplatného.</span><span class="sxs-lookup"><span data-stu-id="20944-147">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

10. <span data-ttu-id="20944-148">Poskytněte důkaz o provedení (PoE).</span><span class="sxs-lookup"><span data-stu-id="20944-148">Supply your proof of execution (PoE).</span></span> <span data-ttu-id="20944-149">Můžete ho přetáhnout do pole, vyhledat ve vaší doprovodné dokumentaci nebo vybrat **Stáhnout šablonu** a použít šablonu.</span><span class="sxs-lookup"><span data-stu-id="20944-149">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template**.</span></span> 

11. <span data-ttu-id="20944-150">Pokud chcete, přidejte a uložte komentáře, a pak vyberte **Odeslat žádost**.</span><span class="sxs-lookup"><span data-stu-id="20944-150">Add and save comments if you like, and then select **Submit claim**.</span></span> <span data-ttu-id="20944-151">Zákazníkovi pošleme e-mail s žádostí o schválení vašeho přidružení zákazníka.</span><span class="sxs-lookup"><span data-stu-id="20944-151">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="20944-152">Po odeslání přidružení zákazníka ho nemůžete upravovat.</span><span class="sxs-lookup"><span data-stu-id="20944-152">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="20944-153">Stav vašeho přidružení zákazníka se zobrazí v poli **Stav**.</span><span class="sxs-lookup"><span data-stu-id="20944-153">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="20944-154">Výběrem **Historie** můžete zobrazit historii přidružení zákazníka.</span><span class="sxs-lookup"><span data-stu-id="20944-154">Select **History** to view the history of a customer association.</span></span>

## <a name="next-steps"></a><span data-ttu-id="20944-155">Další kroky</span><span class="sxs-lookup"><span data-stu-id="20944-155">Next steps</span></span>

- [<span data-ttu-id="20944-156">Správa přidružení zákazníků</span><span class="sxs-lookup"><span data-stu-id="20944-156">Manage customer associations</span></span>](incentives-manage-customer-associations.md)