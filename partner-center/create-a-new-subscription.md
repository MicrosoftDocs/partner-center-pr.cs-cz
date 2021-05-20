---
title: Vytváření zákaznických předplatných v Partnerské centrum
ms.topic: how-to
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak zákazníkům prodávat předplatná pro produkty publikované Microsoftem i produkty SaaS publikované výrobcem softwaru třetích stran.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 9052954c81ef55a2bfa06778ace651c9d0f9b26f
ms.sourcegitcommit: e0444145d7720df948b9d02ae2469206db48dba5
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110201404"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="cba88-103">Vytváření, pozastavování nebo rušení zákaznických předplatných</span><span class="sxs-lookup"><span data-stu-id="cba88-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="cba88-104">**Platí pro**: Partnerské centrum | Partnerské centrum pro Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="cba88-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="cba88-105">**Odpovídající role:** Agent pro správu | Správce fakturace | Globální správce | Agent helpdesku | Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="cba88-105">**Appropriate roles**: Admin agent | Billing admin | Global admin | Helpdesk agent | Sales agent</span></span>

<span data-ttu-id="cba88-106">Po vytvoření záznamu zákazníka v katalogu Partnerské centrum můžete prodávat předplatná produktů v katalogu.</span><span class="sxs-lookup"><span data-stu-id="cba88-106">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="cba88-107">To zahrnuje produkty publikované společností Microsoft a produkty SaaS (software jako služba), které publikovali nezávislí dodavatelé softwaru (ISV) třetích stran na [komerčním marketplace.](https://azuremarketplace.microsoft.com/marketplace)</span><span class="sxs-lookup"><span data-stu-id="cba88-107">This includes products published by Microsoft and Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="cba88-108">Některé nabídky jsou omezené na jedno předplatné na zákazníka.</span><span class="sxs-lookup"><span data-stu-id="cba88-108">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="cba88-109">Pokud chcete zobrazit seznam nabídek, které jsou omezené, přejděte na Partnerské centrum Ceny a nabídky.</span><span class="sxs-lookup"><span data-stu-id="cba88-109">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="cba88-110">Jako partner v programu CSP můžete  zakoupit předplatná **SaaS** založená na licencích nebo na základě měření od vydavatelů ISV v rámci Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="cba88-110">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="cba88-111">To znamená, že si můžete zakoupit jakoukoli **nabídku** **SaaS** založenou na [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) licencích nebo na základě měření, kterou vám vydavatel ISV nabízí, včetně výhradních nabídek, ke kterým máte přístup.</span><span class="sxs-lookup"><span data-stu-id="cba88-111">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="cba88-112">Pokud chcete nakupovat nebo spravovat jiné nabídky na komerčním marketplace od isv (například nabídky založené na využití zahrnující aplikace Azure, kontejnery nebo virtuální počítače), musíte přejít na [web Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="cba88-112">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

>[!NOTE]
><span data-ttu-id="cba88-113">Všechna data a časy v Partnerské centrum jsou uvedeny v časovém standardu UTC (Universal Time Coordinated).</span><span class="sxs-lookup"><span data-stu-id="cba88-113">All dates and times in Partner Center are given in the Universal Time Coordinated (UTC) time standard.</span></span> <span data-ttu-id="cba88-114">To se může lišit až o 24 hodin od místního času.</span><span class="sxs-lookup"><span data-stu-id="cba88-114">This can differ by up to 24 hours from your local time.</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="cba88-115">Vytvoření nového předplatného</span><span class="sxs-lookup"><span data-stu-id="cba88-115">Create a new subscription</span></span>

1. <span data-ttu-id="cba88-116">Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="cba88-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="cba88-117">V Partnerské centrum vyberte **Zákazníci** a pak v seznamu zvolte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="cba88-117">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="cba88-118">Vyberte **Přidat předplatné.**</span><span class="sxs-lookup"><span data-stu-id="cba88-118">Select **Add subscription**.</span></span> <span data-ttu-id="cba88-119">Na **kartě Online služby** se zobrazí všechny dostupné nabídky SaaS na Marketplace.</span><span class="sxs-lookup"><span data-stu-id="cba88-119">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="cba88-120">Pokud chcete zobrazit pouze určité typy předplatných, proveďte výběr v dostupných filtrech:</span><span class="sxs-lookup"><span data-stu-id="cba88-120">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="cba88-121">**Vydavatel**: vyberte **Microsoft** , pokud chcete zobrazit jenom nabídky od Microsoftu nebo **partnera** , aby viděli produkty z komerčního tržiště publikované prostřednictvím nezávislého výrobce softwaru.</span><span class="sxs-lookup"><span data-stu-id="cba88-121">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="cba88-122">**Typ fakturace**: Vyberte typ fakturace předplatného, který chcete použít: **licence** nebo **použití**.</span><span class="sxs-lookup"><span data-stu-id="cba88-122">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="cba88-123">Informace, které vám pomůžou při rozhodování mezi měsíční a roční frekvencí fakturace, najdete v tématu [fakturace na základě licencí](license-based-billing.md) .</span><span class="sxs-lookup"><span data-stu-id="cba88-123">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="cba88-124">**Kategorie**: vyberte **podnik**, **malý podnik** nebo **zkušební verzi**.</span><span class="sxs-lookup"><span data-stu-id="cba88-124">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="cba88-125">Informace o zkušebních předplatných najdete v tématu [Nabídka vašich zákazníků s zkušebními produkty Microsoftu](offer-your-customers-trials-of-microsoft-products.md).</span><span class="sxs-lookup"><span data-stu-id="cba88-125">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="cba88-126">Vyberte předplatné produktů, které chcete pro zákazníka koupit.</span><span class="sxs-lookup"><span data-stu-id="cba88-126">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="cba88-127">Produkty, které vidíte, závisí na typu segmentu zákazníka (vzdělávání, státní správa atd.) a na použitých filtrech.</span><span class="sxs-lookup"><span data-stu-id="cba88-127">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="cba88-128">Některé nabídky zobrazené na webu Marketplace nemusí být vždy dostupné konkrétnímu zákazníkovi nebo konkrétnímu partnerovi CSP.</span><span class="sxs-lookup"><span data-stu-id="cba88-128">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="cba88-129">To může být způsobeno tím, že:</span><span class="sxs-lookup"><span data-stu-id="cba88-129">This can be because:</span></span>

   - <span data-ttu-id="cba88-130">Zákazník už má k tomuto produktu předplatné a je povolený jenom jeden.</span><span class="sxs-lookup"><span data-stu-id="cba88-130">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="cba88-131">Předplatné zákazníka může být pozastavené (v takovém případě můžete předplatné znovu aktivovat, ale nekoupit nové).</span><span class="sxs-lookup"><span data-stu-id="cba88-131">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="cba88-132">V případě nabídek ISV SaaS může být nabídka k dispozici z několika důvodů k zakoupení: ISV nemusí podporovat fakturační zemi nebo oblast zákazníka; nezávislý výrobce softwaru se možná rozhodl, že nabídku zpřístupní prostřednictvím programu CSP. nebo nezávislý výrobce softwaru mohl vytvořit nabídku [výhradně](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) pro určité partnery CSP.</span><span class="sxs-lookup"><span data-stu-id="cba88-132">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="cba88-133">Nabídku ISV nelze také využít v partnerském centru (například v kontejnerech nebo v některých nabídkách založených na používání).</span><span class="sxs-lookup"><span data-stu-id="cba88-133">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="cba88-134">U každého předplatného, které chcete přidat, zadejte počet licencí (v případě potřeby) a vyberte **Přidat do košíku**.</span><span class="sxs-lookup"><span data-stu-id="cba88-134">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="cba88-135">Až skončíte s přidáváním předplatných, vyberte **zkontrolovat** a zkontrolovat vaši objednávku.</span><span class="sxs-lookup"><span data-stu-id="cba88-135">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="cba88-136">Po kontrole objednávek a jejich přípravě na nákup můžete vybrat **koupit**.</span><span class="sxs-lookup"><span data-stu-id="cba88-136">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="cba88-137">Po zakoupení předplatného pro zákazníka dojde k následujícímu:</span><span class="sxs-lookup"><span data-stu-id="cba88-137">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="cba88-138">Předplatné můžete zkontrolovat nebo upravit výběrem názvu předplatného na stránce **Předplatná** tohoto zákazníka.</span><span class="sxs-lookup"><span data-stu-id="cba88-138">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="cba88-139">Tady můžete vybrat případné licence doplňků, změnit jejich počet nebo předplatné pozastavit.</span><span class="sxs-lookup"><span data-stu-id="cba88-139">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="cba88-140">**Pro předplatná ISV SaaS (založená na licencích a na základě měření):**</span><span class="sxs-lookup"><span data-stu-id="cba88-140">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="cba88-141">Zobrazí se odkaz na web vydavatele ISV.</span><span class="sxs-lookup"><span data-stu-id="cba88-141">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="cba88-142">Tento odkaz by vám měl pomoct dokončit nasazení nebo nastavení účtu předplatného zákazníka.</span><span class="sxs-lookup"><span data-stu-id="cba88-142">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="cba88-143">Ani vy ani váš zákazník neobdržíte e-mail s pokyny k dokončení nastavení nebo zřízení účtu pro tento typ předplatného ISV.)</span><span class="sxs-lookup"><span data-stu-id="cba88-143">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="cba88-144">Pokud se vaše předplatné dodává s 30denní bezplatnou zkušební verzí, automaticky se použije bezplatné zkušební období.</span><span class="sxs-lookup"><span data-stu-id="cba88-144">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="cba88-145">Jako partner v programu CSP se nemůžete u nabídek, které si koupíte pro zákazníky, uchýlíte bezplatné zkušební období.</span><span class="sxs-lookup"><span data-stu-id="cba88-145">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="cba88-146">Po uplynutí bezplatné zkušební doby začne období předplatného a předplatné se převede na placený stav.</span><span class="sxs-lookup"><span data-stu-id="cba88-146">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="cba88-147">Předplatné se pak automaticky prodlužuje podle stejného plánu.</span><span class="sxs-lookup"><span data-stu-id="cba88-147">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="cba88-148">Aktualizace předplatných o doplňky</span><span class="sxs-lookup"><span data-stu-id="cba88-148">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="cba88-149">Pokud si zákazník chcete koupit doplněk, musí nejprve mít aktivní základní předplatné.</span><span class="sxs-lookup"><span data-stu-id="cba88-149">To purchase an add-on, the customer must first have an active base subscription.</span></span>  <span data-ttu-id="cba88-150">Doplňky není možné kupovat prostřednictvím katalogu.</span><span class="sxs-lookup"><span data-stu-id="cba88-150">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="cba88-151">Přihlaste se k Partnerské centrum [řídicího panelu.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="cba88-151">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="cba88-152">V Partnerské centrum vyberte **Zákazníci** a pak v seznamu zvolte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="cba88-152">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="cba88-153">Zvolte předplatné, které chcete spravovat.</span><span class="sxs-lookup"><span data-stu-id="cba88-153">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="cba88-154">Pod **částí Stav** je seznam dostupných doplňků pro předplatné.</span><span class="sxs-lookup"><span data-stu-id="cba88-154">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="cba88-155">Aktualizujte počet licencí pro každý požadovaný doplněk.</span><span class="sxs-lookup"><span data-stu-id="cba88-155">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="cba88-156">Pak změny **odešlete**.</span><span class="sxs-lookup"><span data-stu-id="cba88-156">Then **Submit** your changes.</span></span>

<span data-ttu-id="cba88-157">Možnost nákupu doplňků prostřednictvím služby Partnerské centrum k dispozici pouze pro přímé vyúčtování a nepřímé poskytovatele.</span><span class="sxs-lookup"><span data-stu-id="cba88-157">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="cba88-158">V závislosti na základních požadavcích a regionální dostupnosti se zobrazí pouze oprávněné doplňky.</span><span class="sxs-lookup"><span data-stu-id="cba88-158">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="cba88-159">Další informace o cenách a nabídkách najdete v matici nabídek cloudových prodejců.</span><span class="sxs-lookup"><span data-stu-id="cba88-159">For more information about pricing and offers, refer to the Cloud Reseller offer matrix.</span></span> <span data-ttu-id="cba88-160">Pozastavením základního předplatného se pozastaví také všechny přidružené doplňky.</span><span class="sxs-lookup"><span data-stu-id="cba88-160">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="cba88-161">Počáteční datum doplňků odpovídá základnímu předplatnému a poplatky se u první faktury účtují poměrně a následně se účtují na základě počátečního a koncového data účtování poplatků.</span><span class="sxs-lookup"><span data-stu-id="cba88-161">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="cba88-162">Další informace najdete v tématu [Fakturace na základě licencí.](license-based-billing.md)</span><span class="sxs-lookup"><span data-stu-id="cba88-162">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="cba88-163">Pozastavení nebo zrušení předplatného</span><span class="sxs-lookup"><span data-stu-id="cba88-163">Suspend or cancel a subscription</span></span>

<span data-ttu-id="cba88-164">Partneři můžou předplatné pozastavit nebo zrušit, pokud ho požaduje zákazník nebo v případě nedoplatku nebo podvodu.</span><span class="sxs-lookup"><span data-stu-id="cba88-164">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="cba88-165">Pozastavení předplatného</span><span class="sxs-lookup"><span data-stu-id="cba88-165">Suspend a subscription</span></span>

<span data-ttu-id="cba88-166">Když změníte stav předplatného na **pozastaveno**, uživatelé se nebudou moct přihlašovat ani získat přístup ke službám.</span><span class="sxs-lookup"><span data-stu-id="cba88-166">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="cba88-167">Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="cba88-167">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="cba88-168">V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="cba88-168">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="cba88-169">Vyberte předplatné, které chcete spravovat.</span><span class="sxs-lookup"><span data-stu-id="cba88-169">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="cba88-170">V části **Stav** zvolte **Pozastaveno**.</span><span class="sxs-lookup"><span data-stu-id="cba88-170">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="cba88-171">Pak změny **odešlete**.</span><span class="sxs-lookup"><span data-stu-id="cba88-171">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="cba88-172">Všechna data budou odstraněna, pokud předplatné nebude znovu aktivováno během 90 dnů nebo 90 dnů plus počet dní mezi časem otevření účtu a prvním fakturačním obdobím (maximum 120 dní).</span><span class="sxs-lookup"><span data-stu-id="cba88-172">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="cba88-173">Když pozastavíte předplatné, datum zobrazené pod tlačítkem **pozastavit** indikuje, kdy by předplatné automaticky vyprší, pokud ho znovu neaktivujete.</span><span class="sxs-lookup"><span data-stu-id="cba88-173">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

>[!NOTE]
><span data-ttu-id="cba88-174">Předplatné CSP neobsahují dobu platnosti (způsobující předplatná na webu), během které služby stále fungují, ale předplatné negeneruje žádné fakturační poplatky.</span><span class="sxs-lookup"><span data-stu-id="cba88-174">CSP subscriptions don't have an expired period (the way web-direct subscriptions do) during which the services are still working but the subscription doesn't generate any billing charges.</span></span> <span data-ttu-id="cba88-175">Odběry CSP jsou aktivní nebo pozastavené (nebo zcela odstraněny).</span><span class="sxs-lookup"><span data-stu-id="cba88-175">CSP subscriptions are either active or suspended (or fully deleted).</span></span>

### <a name="cancel-a-subscription"></a><span data-ttu-id="cba88-176">Zrušení předplatného</span><span class="sxs-lookup"><span data-stu-id="cba88-176">Cancel a subscription</span></span>

<span data-ttu-id="cba88-177">Předplatné SaaS na základě licencí můžete zrušit od třetích stran vydavatelů ISV v rámci [obchodního tržiště](csp-commercial-marketplace-overview.md)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="cba88-177">You can cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="cba88-178">Pokud zrušíte v rámci období zrušení, obdržíte plnou refundaci.</span><span class="sxs-lookup"><span data-stu-id="cba88-178">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="cba88-179">U nezávislých výrobců softwaru nabízíme fakturaci za měsíc:</span><span class="sxs-lookup"><span data-stu-id="cba88-179">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="cba88-180">Pokud po umístění objednávky zrušíte méně než 24 hodin, obdržíte na další faktuře celý kredit.</span><span class="sxs-lookup"><span data-stu-id="cba88-180">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="cba88-181">Pokud zrušíte pozdější dobu než 24 hodin od okamžiku, kdy jste objednávku nastavili, zrušení se naplánuje při obnovení.</span><span class="sxs-lookup"><span data-stu-id="cba88-181">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="cba88-182">Pro nabídky účtované ročně:</span><span class="sxs-lookup"><span data-stu-id="cba88-182">For offers billed annually:</span></span>

- <span data-ttu-id="cba88-183">Pokud po umístění objednávky zrušíte méně než 14 dní, obdržíte na další faktuře celý kredit.</span><span class="sxs-lookup"><span data-stu-id="cba88-183">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="cba88-184">Pokud zrušíte akci později než 14 dní po umístění objednávky, zrušení se naplánuje při obnovení.</span><span class="sxs-lookup"><span data-stu-id="cba88-184">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="cba88-185">Po uplynutí těchto období se už nebude zobrazovat možnost zrušit předplatné.</span><span class="sxs-lookup"><span data-stu-id="cba88-185">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="cba88-186">Služby isv třetích stran založené na využití a na základě měření (které například používají virtuální počítače nebo kontejnery) nemají nárok na vrácení.</span><span class="sxs-lookup"><span data-stu-id="cba88-186">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="cba88-187">Služby založené na využití je možné zrušit jako metodu zrušení.</span><span class="sxs-lookup"><span data-stu-id="cba88-187">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="cba88-188">Vzhledem k tomu, že se poplatky účtují po použití, nemají tyto služby nárok na refundaci.</span><span class="sxs-lookup"><span data-stu-id="cba88-188">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="cba88-189">Pokud chcete zrušit předplatné SaaS založené na licencích od vydavatele ISV, postupujte následovně:</span><span class="sxs-lookup"><span data-stu-id="cba88-189">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="cba88-190">Přihlaste se k Partnerské centrum [řídicího panelu.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="cba88-190">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="cba88-191">V Partnerské centrum vyberte **Zákazníci** a pak v seznamu zvolte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="cba88-191">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="cba88-192">Vyhledejte předplatné, které chcete zrušit.</span><span class="sxs-lookup"><span data-stu-id="cba88-192">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="cba88-193">Ve **sloupci Stav** vyberte **Zrušit.**</span><span class="sxs-lookup"><span data-stu-id="cba88-193">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="cba88-194">Pak změny **odešlete**.</span><span class="sxs-lookup"><span data-stu-id="cba88-194">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="cba88-195">Pokud se zobrazí dialogové okno, vyplňte všechny relevantní podrobnosti a pak vyberte **Odeslat.**</span><span class="sxs-lookup"><span data-stu-id="cba88-195">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="cba88-196">Zrušení potvrdíte výběrem **možnosti Ano, zrušit**.</span><span class="sxs-lookup"><span data-stu-id="cba88-196">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="cba88-197">Můžete se také rozhodnout zrušit předplatné Azure Marketplace pomocí rozhraní API.</span><span class="sxs-lookup"><span data-stu-id="cba88-197">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="cba88-198">Pokud to chcete udělat, podívejte [se na Azure Marketplace předplatného.](/partner-center/develop/cancel-an-azure-marketplace-subscription)</span><span class="sxs-lookup"><span data-stu-id="cba88-198">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="cba88-199">Zvolte, jestli se má předplatné komerčního marketplace automaticky obnovit.</span><span class="sxs-lookup"><span data-stu-id="cba88-199">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="cba88-200">Ve výchozím nastavení jsou aktivní předplatná nastavená tak, aby se při vypršení jejich časového limitu automaticky prodlužovala jejich platnost.</span><span class="sxs-lookup"><span data-stu-id="cba88-200">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="cba88-201">U [předplatných produktů komerčního marketplace](csp-commercial-marketplace-overview.md)můžete volitelně zvolit, že se předplatné automaticky neobnoví.</span><span class="sxs-lookup"><span data-stu-id="cba88-201">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="cba88-202">Pokud chcete zabránit automatickému prodlužování platnosti aktivního předplatného komerčního marketplace:</span><span class="sxs-lookup"><span data-stu-id="cba88-202">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="cba88-203">Přihlaste se k Partnerské centrum [řídicího panelu.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="cba88-203">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="cba88-204">V Partnerské centrum vyberte **Zákazníci** a pak v seznamu zvolte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="cba88-204">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="cba88-205">Vyberte **Předplatná**.</span><span class="sxs-lookup"><span data-stu-id="cba88-205">Select **Subscriptions**.</span></span> <span data-ttu-id="cba88-206">Zobrazí se seznam všech předplatných založených na licencích, která jste pro zákazníka zakoupili.</span><span class="sxs-lookup"><span data-stu-id="cba88-206">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="cba88-207">Ve **sloupci Předplatné** vyberte předplatné, které chcete upravit.</span><span class="sxs-lookup"><span data-stu-id="cba88-207">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="cba88-208">Na stránce s podrobnostmi o předplatném vyhledejte **část Stav** a zrušte zaškrtnutí políčka **Automatické prodloužení platnosti.**</span><span class="sxs-lookup"><span data-stu-id="cba88-208">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="cba88-209">Vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="cba88-209">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="cba88-210">Další kroky</span><span class="sxs-lookup"><span data-stu-id="cba88-210">Next steps</span></span>

- [<span data-ttu-id="cba88-211">Nákup produktů komerčního marketplace pro vaše zákazníky</span><span class="sxs-lookup"><span data-stu-id="cba88-211">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="cba88-212">Správa produktů z komerčního tržiště pro vaše zákazníky</span><span class="sxs-lookup"><span data-stu-id="cba88-212">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="cba88-213">Přehled komerčního marketplace</span><span class="sxs-lookup"><span data-stu-id="cba88-213">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)