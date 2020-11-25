---
title: Vytváření zákaznických předplatných v partnerském centru
ms.topic: how-to
ms.date: 07/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se prodávat předplatné vašich zákazníků k produktům publikovaným společností Microsoft a produktům SaaS zveřejněným nezávislým výrobcům softwaru.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 85a40974557817825d58246c2c010c7cf8a6a5e1
ms.sourcegitcommit: f34f2f69e6df4f260479a205d94010cf47987ff2
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/25/2020
ms.locfileid: "96038876"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="f9cef-103">Vytváření, pozastavování nebo rušení zákaznických předplatných</span><span class="sxs-lookup"><span data-stu-id="f9cef-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="f9cef-104">**Platí pro**</span><span class="sxs-lookup"><span data-stu-id="f9cef-104">**Applies to**</span></span>

- <span data-ttu-id="f9cef-105">Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="f9cef-105">Partner Center</span></span>
- <span data-ttu-id="f9cef-106">Partnerské centrum pro Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="f9cef-106">Partner Center for Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="f9cef-107">Partneři CSP</span><span class="sxs-lookup"><span data-stu-id="f9cef-107">CSP partners</span></span>

<span data-ttu-id="f9cef-108">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="f9cef-108">**Appropriate roles**</span></span>

- <span data-ttu-id="f9cef-109">Agent správce</span><span class="sxs-lookup"><span data-stu-id="f9cef-109">Admin agent</span></span>
- <span data-ttu-id="f9cef-110">Správce fakturace</span><span class="sxs-lookup"><span data-stu-id="f9cef-110">Billing admin</span></span>
- <span data-ttu-id="f9cef-111">Globální správce</span><span class="sxs-lookup"><span data-stu-id="f9cef-111">Global admin</span></span>
- <span data-ttu-id="f9cef-112">Agent helpdesku</span><span class="sxs-lookup"><span data-stu-id="f9cef-112">Helpdesk agent</span></span>
- <span data-ttu-id="f9cef-113">Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="f9cef-113">Sales agent</span></span>

<span data-ttu-id="f9cef-114">Až vytvoříte záznam o zákazníkovi v partnerském centru, můžete si ho prodávat do produktů v katalogu.</span><span class="sxs-lookup"><span data-stu-id="f9cef-114">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="f9cef-115">To zahrnuje produkty publikované společností Microsoft i produkty SaaS (software jako služba), které publikovali nezávislí výrobci softwaru (ISV) třetích stran na [komerčním tržišti](https://azuremarketplace.microsoft.com/marketplace).</span><span class="sxs-lookup"><span data-stu-id="f9cef-115">This includes products published by Microsoft as well as Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="f9cef-116">Některé nabídky jsou omezené na jedno předplatné na zákazníka.</span><span class="sxs-lookup"><span data-stu-id="f9cef-116">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="f9cef-117">Pokud chcete zobrazit seznam nabídek, které jsou omezené, navštivte stránku ceny a nabídky partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="f9cef-117">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="f9cef-118">Jako partner v programu CSP si můžete koupit předplatné SaaS **založené na licencích** nebo **účtované podle objemu** od vydavatelů ISV v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="f9cef-118">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="f9cef-119">To znamená, že si můžete koupit jakoukoli nabídku **založenou na licencích** nebo **měřený** SaaS. Vydavatel ISV vám k dispozici, včetně [exkluzivních nabídek](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) , ke kterým máte přístup.</span><span class="sxs-lookup"><span data-stu-id="f9cef-119">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="f9cef-120">Pokud si chcete koupit nebo spravovat jiné komerční nabídky na webu Marketplace od nezávislého výrobce softwaru (jako jsou nabídky na základě využití zahrnující aplikace a kontejnery Azure), musíte přejít na [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="f9cef-120">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="f9cef-121">Vytvoření nového předplatného</span><span class="sxs-lookup"><span data-stu-id="f9cef-121">Create a new subscription</span></span>

1. <span data-ttu-id="f9cef-122">Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="f9cef-122">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="f9cef-123">V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="f9cef-123">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="f9cef-124">Vyberte **přidat odběr**.</span><span class="sxs-lookup"><span data-stu-id="f9cef-124">Select **Add subscription**.</span></span> <span data-ttu-id="f9cef-125">Na kartě **online služby** se zobrazí všechny dostupné nabídky SaaS Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f9cef-125">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="f9cef-126">Chcete-li zobrazit pouze určité typy předplatných, proveďte výběr v dostupných filtrech:</span><span class="sxs-lookup"><span data-stu-id="f9cef-126">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="f9cef-127">**Vydavatel**: vyberte **Microsoft** , pokud chcete zobrazit jenom nabídky od Microsoftu nebo **partnera** , aby viděli produkty z komerčního tržiště publikované prostřednictvím nezávislého výrobce softwaru.</span><span class="sxs-lookup"><span data-stu-id="f9cef-127">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="f9cef-128">**Typ fakturace**: Vyberte typ fakturace předplatného, který chcete použít: **licence** nebo **použití**.</span><span class="sxs-lookup"><span data-stu-id="f9cef-128">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="f9cef-129">Informace, které vám pomůžou při rozhodování mezi měsíční a roční frekvencí fakturace, najdete v tématu [fakturace na základě licencí](license-based-billing.md) .</span><span class="sxs-lookup"><span data-stu-id="f9cef-129">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="f9cef-130">**Kategorie**: vyberte **podnik**, **malý podnik** nebo **zkušební verzi**.</span><span class="sxs-lookup"><span data-stu-id="f9cef-130">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="f9cef-131">Informace o zkušebních předplatných najdete v tématu [Nabídka vašich zákazníků s zkušebními produkty Microsoftu](offer-your-customers-trials-of-microsoft-products.md).</span><span class="sxs-lookup"><span data-stu-id="f9cef-131">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="f9cef-132">Vyberte předplatné produktů, které chcete pro zákazníka koupit.</span><span class="sxs-lookup"><span data-stu-id="f9cef-132">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="f9cef-133">Produkty, které vidíte, závisí na typu segmentu zákazníka (vzdělávání, státní správa atd.) a na použitých filtrech.</span><span class="sxs-lookup"><span data-stu-id="f9cef-133">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="f9cef-134">Některé nabídky zobrazené na webu Marketplace nemusí být vždy dostupné konkrétnímu zákazníkovi nebo konkrétnímu partnerovi CSP.</span><span class="sxs-lookup"><span data-stu-id="f9cef-134">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="f9cef-135">To může být způsobeno tím, že:</span><span class="sxs-lookup"><span data-stu-id="f9cef-135">This can be because:</span></span>

   - <span data-ttu-id="f9cef-136">Zákazník už má k tomuto produktu předplatné a je povolený jenom jeden.</span><span class="sxs-lookup"><span data-stu-id="f9cef-136">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="f9cef-137">Předplatné zákazníka může být pozastavené (v takovém případě můžete předplatné znovu aktivovat, ale nekoupit nové).</span><span class="sxs-lookup"><span data-stu-id="f9cef-137">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="f9cef-138">V případě nabídek ISV SaaS může být nabídka k dispozici z několika důvodů k zakoupení: ISV nemusí podporovat fakturační zemi nebo oblast zákazníka; nezávislý výrobce softwaru se možná rozhodl, že nabídku zpřístupní prostřednictvím programu CSP. nebo nezávislý výrobce softwaru mohl vytvořit nabídku [výhradně](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) pro určité partnery CSP.</span><span class="sxs-lookup"><span data-stu-id="f9cef-138">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="f9cef-139">Nabídku ISV nelze také využít v partnerském centru (například v kontejnerech nebo v některých nabídkách založených na používání).</span><span class="sxs-lookup"><span data-stu-id="f9cef-139">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="f9cef-140">U každého předplatného, které chcete přidat, zadejte počet licencí (v případě potřeby) a vyberte **Přidat do košíku**.</span><span class="sxs-lookup"><span data-stu-id="f9cef-140">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="f9cef-141">Až skončíte s přidáváním předplatných, vyberte **zkontrolovat** a zkontrolovat vaši objednávku.</span><span class="sxs-lookup"><span data-stu-id="f9cef-141">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="f9cef-142">Po kontrole objednávek a jejich přípravě na nákup můžete vybrat **koupit**.</span><span class="sxs-lookup"><span data-stu-id="f9cef-142">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="f9cef-143">Po zakoupení předplatného pro zákazníka dojde k následujícímu:</span><span class="sxs-lookup"><span data-stu-id="f9cef-143">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="f9cef-144">Předplatné můžete zkontrolovat nebo upravit výběrem názvu předplatného ze stránky **předplatné** daného zákazníka.</span><span class="sxs-lookup"><span data-stu-id="f9cef-144">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="f9cef-145">Tady můžete vybrat licence pro doplňky, pokud jsou k dispozici, změnit množství licencí nebo pozastavit předplatné.</span><span class="sxs-lookup"><span data-stu-id="f9cef-145">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="f9cef-146">**V případě předplatných ISV SaaS (podle licencí a měřených):**</span><span class="sxs-lookup"><span data-stu-id="f9cef-146">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="f9cef-147">Zobrazí se odkaz na web vydavatele ISV.</span><span class="sxs-lookup"><span data-stu-id="f9cef-147">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="f9cef-148">Tento odkaz by vám měl pomáhat s dokončením nastavení nasazení nebo účtu u předplatného zákazníka.</span><span class="sxs-lookup"><span data-stu-id="f9cef-148">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="f9cef-149">Ani vy ani váš zákazník neobdrží e-mail s pokyny k dokončení nastavení/zřizování pro tento typ předplatného ISV.)</span><span class="sxs-lookup"><span data-stu-id="f9cef-149">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="f9cef-150">Pokud vaše předplatné předchází 30denní bezplatnou zkušební verzi, použije se k automatickému vyzkoušení bezplatné zkušební období.</span><span class="sxs-lookup"><span data-stu-id="f9cef-150">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="f9cef-151">Jako partner v programu CSP se nemůžete vzdát bezplatné zkušební doby pro nabídky, které zakoupíte pro zákazníky.</span><span class="sxs-lookup"><span data-stu-id="f9cef-151">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="f9cef-152">Po skončení bezplatné zkušební doby se předplatné spustí a předplatné se převede na placený stav.</span><span class="sxs-lookup"><span data-stu-id="f9cef-152">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="f9cef-153">Předplatné se pak automaticky obnoví podle stejného plánu.</span><span class="sxs-lookup"><span data-stu-id="f9cef-153">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="f9cef-154">Aktualizace předplatných o doplňky</span><span class="sxs-lookup"><span data-stu-id="f9cef-154">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="f9cef-155">Aby si zákazník mohl koupit doplněk, musí nejprve mít aktivní základní předplatné.</span><span class="sxs-lookup"><span data-stu-id="f9cef-155">To purchase an add-on the customer must first have an active base subscription.</span></span>  <span data-ttu-id="f9cef-156">Doplňky není možné kupovat prostřednictvím katalogu.</span><span class="sxs-lookup"><span data-stu-id="f9cef-156">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="f9cef-157">Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="f9cef-157">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="f9cef-158">V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="f9cef-158">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="f9cef-159">Vyberte předplatné, které chcete spravovat.</span><span class="sxs-lookup"><span data-stu-id="f9cef-159">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="f9cef-160">Pod oddílem **stav** je seznam dostupných doplňků pro předplatné.</span><span class="sxs-lookup"><span data-stu-id="f9cef-160">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="f9cef-161">Aktualizujte množství licencí pro každý požadovaný doplněk.</span><span class="sxs-lookup"><span data-stu-id="f9cef-161">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="f9cef-162">Pak změny **odešlete**.</span><span class="sxs-lookup"><span data-stu-id="f9cef-162">Then **Submit** your changes.</span></span>

<span data-ttu-id="f9cef-163">Možnost zakoupit doplňky prostřednictvím partnerského centra je dostupná jenom pro přímé faktury a nepřímé poskytovatele.</span><span class="sxs-lookup"><span data-stu-id="f9cef-163">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="f9cef-164">Na základě základních požadavků a regionální dostupnosti se zobrazují jenom opravňující doplňky.</span><span class="sxs-lookup"><span data-stu-id="f9cef-164">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="f9cef-165">Další informace o cenách a nabídkách najdete v tabulce nabídek pro prodejce cloudových řešení.</span><span class="sxs-lookup"><span data-stu-id="f9cef-165">Refer to the Cloud Reseller offer matrix for more information about pricing and offers.</span></span>  <span data-ttu-id="f9cef-166">Pozastavením základního předplatného se pozastaví také všechny přidružené doplňky.</span><span class="sxs-lookup"><span data-stu-id="f9cef-166">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="f9cef-167">Počáteční datum doplňků odpovídá základnímu předplatnému a poplatky se u první faktury účtují poměrně a následně se účtují na základě počátečního a koncového data účtování poplatků.</span><span class="sxs-lookup"><span data-stu-id="f9cef-167">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="f9cef-168">Další informace najdete v tématu [fakturace na základě licencí](license-based-billing.md).</span><span class="sxs-lookup"><span data-stu-id="f9cef-168">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="f9cef-169">Pozastavení nebo zrušení předplatného</span><span class="sxs-lookup"><span data-stu-id="f9cef-169">Suspend or cancel a subscription</span></span>

<span data-ttu-id="f9cef-170">Partneři můžou předplatné pozastavit nebo zrušit, pokud ho požaduje zákazník nebo v případě nedoplatku nebo podvodu.</span><span class="sxs-lookup"><span data-stu-id="f9cef-170">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="f9cef-171">Pozastavení předplatného</span><span class="sxs-lookup"><span data-stu-id="f9cef-171">Suspend a subscription</span></span>

<span data-ttu-id="f9cef-172">Když změníte stav předplatného na **pozastaveno**, uživatelé se nebudou moct přihlašovat ani získat přístup ke službám.</span><span class="sxs-lookup"><span data-stu-id="f9cef-172">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="f9cef-173">Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="f9cef-173">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="f9cef-174">V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="f9cef-174">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="f9cef-175">Vyberte předplatné, které chcete spravovat.</span><span class="sxs-lookup"><span data-stu-id="f9cef-175">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="f9cef-176">V části **Stav** zvolte **Pozastaveno**.</span><span class="sxs-lookup"><span data-stu-id="f9cef-176">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="f9cef-177">Pak změny **odešlete**.</span><span class="sxs-lookup"><span data-stu-id="f9cef-177">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="f9cef-178">Všechna data budou odstraněna, pokud předplatné nebude znovu aktivováno během 90 dnů nebo 90 dnů plus počet dní mezi časem otevření účtu a prvním fakturačním obdobím (maximum 120 dní).</span><span class="sxs-lookup"><span data-stu-id="f9cef-178">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="f9cef-179">Když pozastavíte předplatné, datum zobrazené pod tlačítkem **pozastavit** indikuje, kdy by předplatné automaticky vyprší, pokud ho znovu neaktivujete.</span><span class="sxs-lookup"><span data-stu-id="f9cef-179">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

### <a name="cancel-a-subscription"></a><span data-ttu-id="f9cef-180">Zrušení předplatného</span><span class="sxs-lookup"><span data-stu-id="f9cef-180">Cancel a subscription</span></span>

<span data-ttu-id="f9cef-181">Máte možnost zrušit si předplatné SaaS založené na licencích od třetích stran vydavatelů ISV v rámci [obchodního tržiště](csp-commercial-marketplace-overview.md)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="f9cef-181">You have the option to cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="f9cef-182">Pokud zrušíte v rámci období zrušení, obdržíte plnou refundaci.</span><span class="sxs-lookup"><span data-stu-id="f9cef-182">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="f9cef-183">U nezávislých výrobců softwaru nabízíme fakturaci za měsíc:</span><span class="sxs-lookup"><span data-stu-id="f9cef-183">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="f9cef-184">Pokud po umístění objednávky zrušíte méně než 24 hodin, obdržíte na další faktuře celý kredit.</span><span class="sxs-lookup"><span data-stu-id="f9cef-184">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="f9cef-185">Pokud zrušíte pozdější dobu než 24 hodin od okamžiku, kdy jste objednávku nastavili, zrušení se naplánuje při obnovení.</span><span class="sxs-lookup"><span data-stu-id="f9cef-185">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="f9cef-186">Pro nabídky účtované ročně:</span><span class="sxs-lookup"><span data-stu-id="f9cef-186">For offers billed annually:</span></span>

- <span data-ttu-id="f9cef-187">Pokud po umístění objednávky zrušíte méně než 14 dní, obdržíte na další faktuře celý kredit.</span><span class="sxs-lookup"><span data-stu-id="f9cef-187">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="f9cef-188">Pokud zrušíte akci později než 14 dní po umístění objednávky, zrušení se naplánuje při obnovení.</span><span class="sxs-lookup"><span data-stu-id="f9cef-188">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="f9cef-189">Po uplynutí těchto období se už nebude zobrazovat možnost zrušit předplatné.</span><span class="sxs-lookup"><span data-stu-id="f9cef-189">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="f9cef-190">Služby nezávislé na používání a měřené od jiných výrobců ISV (například virtuální počítače nebo kontejnery) nejsou způsobilé k návratu.</span><span class="sxs-lookup"><span data-stu-id="f9cef-190">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="f9cef-191">Služby založené na využití se dají zrušit jako metoda zrušení.</span><span class="sxs-lookup"><span data-stu-id="f9cef-191">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="f9cef-192">Vzhledem k tomu, že se poplatky účtují po použití, tyto služby nemají nárok na refundaci.</span><span class="sxs-lookup"><span data-stu-id="f9cef-192">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="f9cef-193">Pokud chcete zrušit předplatné SaaS založené na licencích od vydavatele ISV, postupujte následovně:</span><span class="sxs-lookup"><span data-stu-id="f9cef-193">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="f9cef-194">Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="f9cef-194">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="f9cef-195">V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="f9cef-195">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="f9cef-196">Vyhledejte předplatné, které chcete zrušit.</span><span class="sxs-lookup"><span data-stu-id="f9cef-196">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="f9cef-197">Ve sloupci **stav** vyberte **Zrušit**.</span><span class="sxs-lookup"><span data-stu-id="f9cef-197">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="f9cef-198">Pak změny **odešlete**.</span><span class="sxs-lookup"><span data-stu-id="f9cef-198">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="f9cef-199">Pokud se zobrazí dialogové okno, vyplňte příslušné podrobnosti a pak vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="f9cef-199">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="f9cef-200">Zrušení potvrďte tak, že vyberete **Ano, zrušit**.</span><span class="sxs-lookup"><span data-stu-id="f9cef-200">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="f9cef-201">Můžete také zvolit zrušení předplatného Azure Marketplace pomocí rozhraní API.</span><span class="sxs-lookup"><span data-stu-id="f9cef-201">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="f9cef-202">Pokud to chcete udělat, přečtěte si téma [zrušení předplatného Azure Marketplace](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span><span class="sxs-lookup"><span data-stu-id="f9cef-202">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="f9cef-203">Vyberte, jestli se má automaticky obnovit předplatné z komerčního tržiště.</span><span class="sxs-lookup"><span data-stu-id="f9cef-203">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="f9cef-204">Ve výchozím nastavení jsou aktivní předplatná nastavená tak, aby se při vypršení jejich časového limitu automaticky prodlužovala jejich platnost.</span><span class="sxs-lookup"><span data-stu-id="f9cef-204">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="f9cef-205">Pro [odběry komerčních produktů na webu Marketplace](csp-commercial-marketplace-overview.md)můžete volitelně zvolit automatické obnovení předplatného.</span><span class="sxs-lookup"><span data-stu-id="f9cef-205">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="f9cef-206">Pokud chcete zastavit aktivní předplatné komerčního tržiště z automatického obnovování:</span><span class="sxs-lookup"><span data-stu-id="f9cef-206">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="f9cef-207">Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="f9cef-207">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="f9cef-208">V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="f9cef-208">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="f9cef-209">Vyberte **Předplatná**.</span><span class="sxs-lookup"><span data-stu-id="f9cef-209">Select **Subscriptions**.</span></span> <span data-ttu-id="f9cef-210">Obsahuje seznam všech předplatných založených na licencích, které jste zakoupili pro zákazníka.</span><span class="sxs-lookup"><span data-stu-id="f9cef-210">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="f9cef-211">Ve sloupci **předplatné** vyberte předplatné, které chcete upravit.</span><span class="sxs-lookup"><span data-stu-id="f9cef-211">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="f9cef-212">Na stránce Podrobnosti předplatného vyhledejte část **stav** a zrušte kontrolu **automatického obnovení** .</span><span class="sxs-lookup"><span data-stu-id="f9cef-212">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="f9cef-213">Vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="f9cef-213">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f9cef-214">Další kroky</span><span class="sxs-lookup"><span data-stu-id="f9cef-214">Next steps</span></span>

- [<span data-ttu-id="f9cef-215">Nákup produktů z komerčního tržiště pro vaše zákazníky</span><span class="sxs-lookup"><span data-stu-id="f9cef-215">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="f9cef-216">Správa produktů z komerčního tržiště pro vaše zákazníky</span><span class="sxs-lookup"><span data-stu-id="f9cef-216">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="f9cef-217">Přehled komerčního marketplace</span><span class="sxs-lookup"><span data-stu-id="f9cef-217">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)