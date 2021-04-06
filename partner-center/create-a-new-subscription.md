---
title: Vytváření zákaznických předplatných v partnerském centru
ms.topic: how-to
ms.date: 07/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si, jak prodávat předplatná vašim zákazníkům pro produkty publikované Microsoftem a také pro produkty SaaS publikované třetí stranou nezávislého výrobce softwaru.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 559d1fbd2efc1417ae89931279b9d3c9a1d67f7c
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502931"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="d3618-103">Vytváření, pozastavování nebo rušení zákaznických předplatných</span><span class="sxs-lookup"><span data-stu-id="d3618-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="d3618-104">**Platí pro**</span><span class="sxs-lookup"><span data-stu-id="d3618-104">**Applies to**</span></span>

- <span data-ttu-id="d3618-105">Partnerské centrum pro Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="d3618-105">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="d3618-106">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="d3618-106">**Appropriate roles**</span></span>

- <span data-ttu-id="d3618-107">Agent správce</span><span class="sxs-lookup"><span data-stu-id="d3618-107">Admin agent</span></span>
- <span data-ttu-id="d3618-108">Správce fakturace</span><span class="sxs-lookup"><span data-stu-id="d3618-108">Billing admin</span></span>
- <span data-ttu-id="d3618-109">Globální správce</span><span class="sxs-lookup"><span data-stu-id="d3618-109">Global admin</span></span>
- <span data-ttu-id="d3618-110">Agent helpdesku</span><span class="sxs-lookup"><span data-stu-id="d3618-110">Helpdesk agent</span></span>
- <span data-ttu-id="d3618-111">Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="d3618-111">Sales agent</span></span>

<span data-ttu-id="d3618-112">Až vytvoříte záznam o zákazníkovi v partnerském centru, můžete si ho prodávat do produktů v katalogu.</span><span class="sxs-lookup"><span data-stu-id="d3618-112">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="d3618-113">To zahrnuje produkty publikované produkty Microsoft a software jako služba (SaaS), které publikovali nezávislí výrobci softwaru (ISV) třetích stran na [komerčním tržišti](https://azuremarketplace.microsoft.com/marketplace).</span><span class="sxs-lookup"><span data-stu-id="d3618-113">This includes products published by Microsoft and Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="d3618-114">Některé nabídky jsou omezené na jedno předplatné na zákazníka.</span><span class="sxs-lookup"><span data-stu-id="d3618-114">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="d3618-115">Pokud chcete zobrazit seznam nabídek, které jsou omezené, navštivte stránku ceny a nabídky partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="d3618-115">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="d3618-116">Jako partner v programu CSP si můžete koupit předplatné SaaS **založené na licencích** nebo **účtované podle objemu** od vydavatelů ISV v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="d3618-116">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="d3618-117">To znamená, že si můžete koupit jakoukoli nabídku **založenou na licencích** nebo **měřený** SaaS. Vydavatel ISV vám k dispozici, včetně [exkluzivních nabídek](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) , ke kterým máte přístup.</span><span class="sxs-lookup"><span data-stu-id="d3618-117">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="d3618-118">Pokud si chcete koupit nebo spravovat jiné komerční nabídky na webu Marketplace od nezávislého výrobce softwaru (jako jsou nabídky na základě využití zahrnující aplikace a kontejnery Azure), musíte přejít na [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="d3618-118">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="d3618-119">Vytvoření nového předplatného</span><span class="sxs-lookup"><span data-stu-id="d3618-119">Create a new subscription</span></span>

1. <span data-ttu-id="d3618-120">Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="d3618-120">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d3618-121">V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="d3618-121">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d3618-122">Vyberte **přidat odběr**.</span><span class="sxs-lookup"><span data-stu-id="d3618-122">Select **Add subscription**.</span></span> <span data-ttu-id="d3618-123">Na kartě **online služby** se zobrazí všechny dostupné nabídky SaaS Marketplace.</span><span class="sxs-lookup"><span data-stu-id="d3618-123">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="d3618-124">Chcete-li zobrazit pouze určité typy předplatných, proveďte výběr v dostupných filtrech:</span><span class="sxs-lookup"><span data-stu-id="d3618-124">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="d3618-125">**Vydavatel**: vyberte **Microsoft** , pokud chcete zobrazit jenom nabídky od Microsoftu nebo **partnera** , aby viděli produkty z komerčního tržiště publikované prostřednictvím nezávislého výrobce softwaru.</span><span class="sxs-lookup"><span data-stu-id="d3618-125">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="d3618-126">**Typ fakturace**: Vyberte typ fakturace předplatného, který chcete použít: **licence** nebo **použití**.</span><span class="sxs-lookup"><span data-stu-id="d3618-126">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="d3618-127">Informace, které vám pomůžou při rozhodování mezi měsíční a roční frekvencí fakturace, najdete v tématu [fakturace na základě licencí](license-based-billing.md) .</span><span class="sxs-lookup"><span data-stu-id="d3618-127">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="d3618-128">**Kategorie**: vyberte **podnik**, **malý podnik** nebo **zkušební verzi**.</span><span class="sxs-lookup"><span data-stu-id="d3618-128">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="d3618-129">Informace o zkušebních předplatných najdete v tématu [Nabídka vašich zákazníků s zkušebními produkty Microsoftu](offer-your-customers-trials-of-microsoft-products.md).</span><span class="sxs-lookup"><span data-stu-id="d3618-129">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="d3618-130">Vyberte předplatné produktů, které chcete pro zákazníka koupit.</span><span class="sxs-lookup"><span data-stu-id="d3618-130">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="d3618-131">Produkty, které vidíte, závisí na typu segmentu zákazníka (vzdělávání, státní správa atd.) a na použitých filtrech.</span><span class="sxs-lookup"><span data-stu-id="d3618-131">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="d3618-132">Některé nabídky zobrazené na webu Marketplace nemusí být vždy dostupné konkrétnímu zákazníkovi nebo konkrétnímu partnerovi CSP.</span><span class="sxs-lookup"><span data-stu-id="d3618-132">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="d3618-133">To může být způsobeno tím, že:</span><span class="sxs-lookup"><span data-stu-id="d3618-133">This can be because:</span></span>

   - <span data-ttu-id="d3618-134">Zákazník už má k tomuto produktu předplatné a je povolený jenom jeden.</span><span class="sxs-lookup"><span data-stu-id="d3618-134">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="d3618-135">Předplatné zákazníka může být pozastavené (v takovém případě můžete předplatné znovu aktivovat, ale nekoupit nové).</span><span class="sxs-lookup"><span data-stu-id="d3618-135">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="d3618-136">V případě nabídek ISV SaaS může být nabídka k dispozici z několika důvodů k zakoupení: ISV nemusí podporovat fakturační zemi nebo oblast zákazníka; nezávislý výrobce softwaru se možná rozhodl, že nabídku zpřístupní prostřednictvím programu CSP. nebo nezávislý výrobce softwaru mohl vytvořit nabídku [výhradně](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) pro určité partnery CSP.</span><span class="sxs-lookup"><span data-stu-id="d3618-136">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="d3618-137">Nabídku ISV nelze také využít v partnerském centru (například v kontejnerech nebo v některých nabídkách založených na používání).</span><span class="sxs-lookup"><span data-stu-id="d3618-137">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="d3618-138">U každého předplatného, které chcete přidat, zadejte počet licencí (v případě potřeby) a vyberte **Přidat do košíku**.</span><span class="sxs-lookup"><span data-stu-id="d3618-138">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="d3618-139">Až skončíte s přidáváním předplatných, vyberte **zkontrolovat** a zkontrolovat vaši objednávku.</span><span class="sxs-lookup"><span data-stu-id="d3618-139">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="d3618-140">Po kontrole objednávek a jejich přípravě na nákup můžete vybrat **koupit**.</span><span class="sxs-lookup"><span data-stu-id="d3618-140">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="d3618-141">Po zakoupení předplatného pro zákazníka dojde k následujícímu:</span><span class="sxs-lookup"><span data-stu-id="d3618-141">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="d3618-142">Předplatné můžete zkontrolovat nebo upravit výběrem názvu předplatného ze stránky **předplatné** daného zákazníka.</span><span class="sxs-lookup"><span data-stu-id="d3618-142">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="d3618-143">Tady můžete vybrat licence pro doplňky, pokud jsou k dispozici, změnit množství licencí nebo pozastavit předplatné.</span><span class="sxs-lookup"><span data-stu-id="d3618-143">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="d3618-144">**V případě předplatných ISV SaaS (podle licencí a měřených):**</span><span class="sxs-lookup"><span data-stu-id="d3618-144">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="d3618-145">Zobrazí se odkaz na web vydavatele ISV.</span><span class="sxs-lookup"><span data-stu-id="d3618-145">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="d3618-146">Tento odkaz by vám měl pomáhat s dokončením nastavení nasazení nebo účtu u předplatného zákazníka.</span><span class="sxs-lookup"><span data-stu-id="d3618-146">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="d3618-147">Ani vy ani váš zákazník neobdrží e-mail s pokyny k dokončení nastavení/zřizování pro tento typ předplatného ISV.)</span><span class="sxs-lookup"><span data-stu-id="d3618-147">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="d3618-148">Pokud vaše předplatné předchází 30denní bezplatnou zkušební verzi, použije se k automatickému vyzkoušení bezplatné zkušební období.</span><span class="sxs-lookup"><span data-stu-id="d3618-148">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="d3618-149">Jako partner v programu CSP se nemůžete vzdát bezplatné zkušební doby pro nabídky, které zakoupíte pro zákazníky.</span><span class="sxs-lookup"><span data-stu-id="d3618-149">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="d3618-150">Po skončení bezplatné zkušební doby se předplatné spustí a předplatné se převede na placený stav.</span><span class="sxs-lookup"><span data-stu-id="d3618-150">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="d3618-151">Předplatné se pak automaticky obnoví podle stejného plánu.</span><span class="sxs-lookup"><span data-stu-id="d3618-151">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="d3618-152">Aktualizace předplatných o doplňky</span><span class="sxs-lookup"><span data-stu-id="d3618-152">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="d3618-153">K nákupu doplňku musí zákazník nejdřív mít aktivní základní předplatné.</span><span class="sxs-lookup"><span data-stu-id="d3618-153">To purchase an add-on, the customer must first have an active base subscription.</span></span>  <span data-ttu-id="d3618-154">Doplňky není možné kupovat prostřednictvím katalogu.</span><span class="sxs-lookup"><span data-stu-id="d3618-154">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="d3618-155">Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="d3618-155">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d3618-156">V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="d3618-156">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d3618-157">Vyberte předplatné, které chcete spravovat.</span><span class="sxs-lookup"><span data-stu-id="d3618-157">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="d3618-158">Pod oddílem **stav** je seznam dostupných doplňků pro předplatné.</span><span class="sxs-lookup"><span data-stu-id="d3618-158">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="d3618-159">Aktualizujte množství licencí pro každý požadovaný doplněk.</span><span class="sxs-lookup"><span data-stu-id="d3618-159">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="d3618-160">Pak změny **odešlete**.</span><span class="sxs-lookup"><span data-stu-id="d3618-160">Then **Submit** your changes.</span></span>

<span data-ttu-id="d3618-161">Možnost zakoupit doplňky prostřednictvím partnerského centra je dostupná jenom pro přímé faktury a nepřímé poskytovatele.</span><span class="sxs-lookup"><span data-stu-id="d3618-161">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="d3618-162">Na základě základních požadavků a regionální dostupnosti se zobrazují jenom opravňující doplňky.</span><span class="sxs-lookup"><span data-stu-id="d3618-162">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="d3618-163">Další informace o cenách a nabídkách najdete v tématu matice nabídky prodejce cloudu.</span><span class="sxs-lookup"><span data-stu-id="d3618-163">For more information about pricing and offers, refer to the Cloud Reseller offer matrix.</span></span> <span data-ttu-id="d3618-164">Pozastavením základního předplatného se pozastaví také všechny přidružené doplňky.</span><span class="sxs-lookup"><span data-stu-id="d3618-164">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="d3618-165">Počáteční datum doplňků odpovídá základnímu předplatnému a poplatky se u první faktury účtují poměrně a následně se účtují na základě počátečního a koncového data účtování poplatků.</span><span class="sxs-lookup"><span data-stu-id="d3618-165">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="d3618-166">Další informace najdete v tématu [fakturace na základě licencí](license-based-billing.md).</span><span class="sxs-lookup"><span data-stu-id="d3618-166">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="d3618-167">Pozastavení nebo zrušení předplatného</span><span class="sxs-lookup"><span data-stu-id="d3618-167">Suspend or cancel a subscription</span></span>

<span data-ttu-id="d3618-168">Partneři můžou předplatné pozastavit nebo zrušit, pokud ho požaduje zákazník nebo v případě nedoplatku nebo podvodu.</span><span class="sxs-lookup"><span data-stu-id="d3618-168">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="d3618-169">Pozastavení předplatného</span><span class="sxs-lookup"><span data-stu-id="d3618-169">Suspend a subscription</span></span>

<span data-ttu-id="d3618-170">Když změníte stav předplatného na **pozastaveno**, uživatelé se nebudou moct přihlašovat ani získat přístup ke službám.</span><span class="sxs-lookup"><span data-stu-id="d3618-170">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="d3618-171">Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="d3618-171">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d3618-172">V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="d3618-172">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d3618-173">Vyberte předplatné, které chcete spravovat.</span><span class="sxs-lookup"><span data-stu-id="d3618-173">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="d3618-174">V části **Stav** zvolte **Pozastaveno**.</span><span class="sxs-lookup"><span data-stu-id="d3618-174">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="d3618-175">Pak změny **odešlete**.</span><span class="sxs-lookup"><span data-stu-id="d3618-175">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="d3618-176">Všechna data budou odstraněna, pokud předplatné nebude znovu aktivováno během 90 dnů nebo 90 dnů plus počet dní mezi časem otevření účtu a prvním fakturačním obdobím (maximum 120 dní).</span><span class="sxs-lookup"><span data-stu-id="d3618-176">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="d3618-177">Když pozastavíte předplatné, datum zobrazené pod tlačítkem **pozastavit** indikuje, kdy by předplatné automaticky vyprší, pokud ho znovu neaktivujete.</span><span class="sxs-lookup"><span data-stu-id="d3618-177">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

### <a name="cancel-a-subscription"></a><span data-ttu-id="d3618-178">Zrušení předplatného</span><span class="sxs-lookup"><span data-stu-id="d3618-178">Cancel a subscription</span></span>

<span data-ttu-id="d3618-179">Předplatné SaaS na základě licencí můžete zrušit od třetích stran vydavatelů ISV v rámci [obchodního tržiště](csp-commercial-marketplace-overview.md)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="d3618-179">You can cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="d3618-180">Pokud zrušíte v rámci období zrušení, obdržíte plnou refundaci.</span><span class="sxs-lookup"><span data-stu-id="d3618-180">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="d3618-181">U nezávislých výrobců softwaru nabízíme fakturaci za měsíc:</span><span class="sxs-lookup"><span data-stu-id="d3618-181">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="d3618-182">Pokud po umístění objednávky zrušíte méně než 24 hodin, obdržíte na další faktuře celý kredit.</span><span class="sxs-lookup"><span data-stu-id="d3618-182">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="d3618-183">Pokud zrušíte pozdější dobu než 24 hodin od okamžiku, kdy jste objednávku nastavili, zrušení se naplánuje při obnovení.</span><span class="sxs-lookup"><span data-stu-id="d3618-183">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="d3618-184">Pro nabídky účtované ročně:</span><span class="sxs-lookup"><span data-stu-id="d3618-184">For offers billed annually:</span></span>

- <span data-ttu-id="d3618-185">Pokud po umístění objednávky zrušíte méně než 14 dní, obdržíte na další faktuře celý kredit.</span><span class="sxs-lookup"><span data-stu-id="d3618-185">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="d3618-186">Pokud zrušíte akci později než 14 dní po umístění objednávky, zrušení se naplánuje při obnovení.</span><span class="sxs-lookup"><span data-stu-id="d3618-186">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="d3618-187">Po uplynutí těchto období se už nebude zobrazovat možnost zrušit předplatné.</span><span class="sxs-lookup"><span data-stu-id="d3618-187">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="d3618-188">Služby nezávislé na používání a měřené od jiných výrobců ISV (například virtuální počítače nebo kontejnery) nejsou způsobilé k návratu.</span><span class="sxs-lookup"><span data-stu-id="d3618-188">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="d3618-189">Služby založené na využití se dají zrušit jako metoda zrušení.</span><span class="sxs-lookup"><span data-stu-id="d3618-189">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="d3618-190">Vzhledem k tomu, že se poplatky účtují po použití, tyto služby nemají nárok na refundaci.</span><span class="sxs-lookup"><span data-stu-id="d3618-190">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="d3618-191">Pokud chcete zrušit předplatné SaaS založené na licencích od vydavatele ISV, postupujte následovně:</span><span class="sxs-lookup"><span data-stu-id="d3618-191">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="d3618-192">Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="d3618-192">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d3618-193">V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="d3618-193">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d3618-194">Vyhledejte předplatné, které chcete zrušit.</span><span class="sxs-lookup"><span data-stu-id="d3618-194">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="d3618-195">Ve sloupci **stav** vyberte **Zrušit**.</span><span class="sxs-lookup"><span data-stu-id="d3618-195">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="d3618-196">Pak změny **odešlete**.</span><span class="sxs-lookup"><span data-stu-id="d3618-196">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="d3618-197">Pokud se zobrazí dialogové okno, vyplňte příslušné podrobnosti a pak vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="d3618-197">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="d3618-198">Zrušení potvrďte tak, že vyberete **Ano, zrušit**.</span><span class="sxs-lookup"><span data-stu-id="d3618-198">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="d3618-199">Můžete také zvolit zrušení předplatného Azure Marketplace pomocí rozhraní API.</span><span class="sxs-lookup"><span data-stu-id="d3618-199">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="d3618-200">Pokud to chcete udělat, přečtěte si téma [zrušení předplatného Azure Marketplace](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span><span class="sxs-lookup"><span data-stu-id="d3618-200">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="d3618-201">Vyberte, jestli se má automaticky obnovit předplatné z komerčního tržiště.</span><span class="sxs-lookup"><span data-stu-id="d3618-201">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="d3618-202">Ve výchozím nastavení jsou aktivní předplatná nastavená tak, aby se při vypršení jejich časového limitu automaticky prodlužovala jejich platnost.</span><span class="sxs-lookup"><span data-stu-id="d3618-202">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="d3618-203">Pro [odběry komerčních produktů na webu Marketplace](csp-commercial-marketplace-overview.md)můžete volitelně zvolit automatické obnovení předplatného.</span><span class="sxs-lookup"><span data-stu-id="d3618-203">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="d3618-204">Pokud chcete zastavit aktivní předplatné komerčního tržiště z automatického obnovování:</span><span class="sxs-lookup"><span data-stu-id="d3618-204">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="d3618-205">Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="d3618-205">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d3618-206">V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="d3618-206">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d3618-207">Vyberte **Předplatná**.</span><span class="sxs-lookup"><span data-stu-id="d3618-207">Select **Subscriptions**.</span></span> <span data-ttu-id="d3618-208">Obsahuje seznam všech předplatných založených na licencích, které jste zakoupili pro zákazníka.</span><span class="sxs-lookup"><span data-stu-id="d3618-208">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="d3618-209">Ve sloupci **předplatné** vyberte předplatné, které chcete upravit.</span><span class="sxs-lookup"><span data-stu-id="d3618-209">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="d3618-210">Na stránce Podrobnosti předplatného vyhledejte část **stav** a zrušte kontrolu **automatického obnovení** .</span><span class="sxs-lookup"><span data-stu-id="d3618-210">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="d3618-211">Vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="d3618-211">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d3618-212">Další kroky</span><span class="sxs-lookup"><span data-stu-id="d3618-212">Next steps</span></span>

- [<span data-ttu-id="d3618-213">Nákup produktů z komerčního tržiště pro vaše zákazníky</span><span class="sxs-lookup"><span data-stu-id="d3618-213">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="d3618-214">Správa produktů z komerčního tržiště pro vaše zákazníky</span><span class="sxs-lookup"><span data-stu-id="d3618-214">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="d3618-215">Přehled komerčního marketplace</span><span class="sxs-lookup"><span data-stu-id="d3618-215">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)