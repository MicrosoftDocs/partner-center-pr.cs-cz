---
title: Vytváření zákaznických předplatných v partnerském centru
ms.topic: how-to
ms.date: 05/17/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si, jak prodávat předplatná vašim zákazníkům pro produkty publikované Microsoftem a také pro produkty SaaS publikované třetí stranou nezávislého výrobce softwaru.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 3269fa994d704c0a0dae067087bad8589a7ce031
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148190"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="441e1-103">Vytváření, pozastavování nebo rušení zákaznických předplatných</span><span class="sxs-lookup"><span data-stu-id="441e1-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="441e1-104">**Platí pro**: partnerské Centrum | Partnerské centrum pro Microsoft Cloud pro státní správu USA</span><span class="sxs-lookup"><span data-stu-id="441e1-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="441e1-105">**Příslušné role**: Agent správce | Správce fakturace | Globální správce | Agent helpdesku | Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="441e1-105">**Appropriate roles**: Admin agent | Billing admin | Global admin | Helpdesk agent | Sales agent</span></span>

<span data-ttu-id="441e1-106">Až vytvoříte záznam o zákazníkovi v partnerském centru, můžete si ho prodávat do produktů v katalogu.</span><span class="sxs-lookup"><span data-stu-id="441e1-106">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="441e1-107">To zahrnuje produkty publikované produkty Microsoft a software jako služba (SaaS), které publikovali nezávislí výrobci softwaru (ISV) třetích stran na [komerčním tržišti](https://azuremarketplace.microsoft.com/marketplace).</span><span class="sxs-lookup"><span data-stu-id="441e1-107">This includes products published by Microsoft and Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="441e1-108">Některé nabídky jsou omezené na jedno předplatné na zákazníka.</span><span class="sxs-lookup"><span data-stu-id="441e1-108">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="441e1-109">Pokud chcete zobrazit seznam nabídek, které jsou omezené, navštivte stránku ceny a nabídky partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="441e1-109">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="441e1-110">Jako partner v programu CSP si můžete koupit předplatné SaaS **založené na licencích** nebo **účtované podle objemu** od vydavatelů ISV v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="441e1-110">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="441e1-111">To znamená, že si můžete koupit jakoukoli nabídku **založenou na licencích** nebo **měřený** SaaS. Vydavatel ISV vám k dispozici, včetně [exkluzivních nabídek](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) , ke kterým máte přístup.</span><span class="sxs-lookup"><span data-stu-id="441e1-111">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="441e1-112">Pokud si chcete koupit nebo spravovat jiné komerční nabídky na webu Marketplace od nezávislého výrobce softwaru (jako jsou nabídky na základě využití zahrnující aplikace a kontejnery Azure), musíte přejít na [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="441e1-112">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="441e1-113">Vytvoření nového předplatného</span><span class="sxs-lookup"><span data-stu-id="441e1-113">Create a new subscription</span></span>

1. <span data-ttu-id="441e1-114">Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="441e1-114">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="441e1-115">V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="441e1-115">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="441e1-116">Vyberte **přidat odběr**.</span><span class="sxs-lookup"><span data-stu-id="441e1-116">Select **Add subscription**.</span></span> <span data-ttu-id="441e1-117">Na kartě **online služby** se zobrazí všechny dostupné nabídky SaaS Marketplace.</span><span class="sxs-lookup"><span data-stu-id="441e1-117">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="441e1-118">Chcete-li zobrazit pouze určité typy předplatných, proveďte výběr v dostupných filtrech:</span><span class="sxs-lookup"><span data-stu-id="441e1-118">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="441e1-119">**Vydavatel**: vyberte **Microsoft** , pokud chcete zobrazit jenom nabídky od Microsoftu nebo **partnera** , aby viděli produkty z komerčního tržiště publikované prostřednictvím nezávislého výrobce softwaru.</span><span class="sxs-lookup"><span data-stu-id="441e1-119">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="441e1-120">**Typ fakturace**: Vyberte typ fakturace předplatného, který chcete použít: **licence** nebo **použití**.</span><span class="sxs-lookup"><span data-stu-id="441e1-120">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="441e1-121">Informace, [které vám pomůžou](license-based-billing.md) s rozhodováním mezi měsíční a roční frekvencí fakturace, najdete v tématu Fakturace na základě licencí.</span><span class="sxs-lookup"><span data-stu-id="441e1-121">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="441e1-122">**Kategorie:** Zvolte **Enterprise**, **Small business** nebo **Trial**.</span><span class="sxs-lookup"><span data-stu-id="441e1-122">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="441e1-123">Informace o zkušebních předplatných najdete v tématu [Nabídka zkušebních verzí produktů Microsoftu zákazníkům.](offer-your-customers-trials-of-microsoft-products.md)</span><span class="sxs-lookup"><span data-stu-id="441e1-123">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="441e1-124">Vyberte předplatná produktů, která chcete pro zákazníka zakoupit.</span><span class="sxs-lookup"><span data-stu-id="441e1-124">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="441e1-125">Produkty, které se zobrazí, závisí na typu segmentu zákazníků (vzdělávání, státní správa atd.) a použitých filtrech.</span><span class="sxs-lookup"><span data-stu-id="441e1-125">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="441e1-126">Některé nabídky zobrazené na Marketplace nemusí být vždy dostupné konkrétnímu zákazníkovi nebo konkrétnímu partnerovi CSP.</span><span class="sxs-lookup"><span data-stu-id="441e1-126">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="441e1-127">Může to být proto, že:</span><span class="sxs-lookup"><span data-stu-id="441e1-127">This can be because:</span></span>

   - <span data-ttu-id="441e1-128">Zákazník už má předplatné tohoto produktu a má povolené jenom jedno.</span><span class="sxs-lookup"><span data-stu-id="441e1-128">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="441e1-129">Předplatné zákazníka může být pozastavené (v tomto případě můžete předplatné znovu aktivovat a nekupovat nové).)</span><span class="sxs-lookup"><span data-stu-id="441e1-129">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="441e1-130">U nabídek SaaS od isv může být několik důvodů, proč není možné nabídku koupit: Tento isv nemusí podporovat fakturační zemi nebo oblast zákazníka. Je možné, že se isV rozhodl nabídku nezvolovat prostřednictvím programu CSP. nebo může isv made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span><span class="sxs-lookup"><span data-stu-id="441e1-130">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="441e1-131">Nabídku isv také není možné provádět prostřednictvím Partnerské centrum (například kontejnery nebo některé nabídky založené na využití).</span><span class="sxs-lookup"><span data-stu-id="441e1-131">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="441e1-132">Pro každé předplatné, které chcete přidat, zadejte počet licencí (v případě potřeby) a vyberte **Přidat do košíku.**</span><span class="sxs-lookup"><span data-stu-id="441e1-132">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="441e1-133">Až přidávání předplatných dokončíte, vyberte **Zkontrolovat** a zkontrolovat objednávku.</span><span class="sxs-lookup"><span data-stu-id="441e1-133">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="441e1-134">Jakmile si prošete objednávky a jste připravení si tato předplatná koupit, vyberte **Koupit.**</span><span class="sxs-lookup"><span data-stu-id="441e1-134">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="441e1-135">Po zakoupení předplatného pro zákazníka dojde k těmto akcím:</span><span class="sxs-lookup"><span data-stu-id="441e1-135">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="441e1-136">Předplatné můžete zkontrolovat nebo upravit výběrem názvu předplatného na stránce **Předplatná** tohoto zákazníka.</span><span class="sxs-lookup"><span data-stu-id="441e1-136">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="441e1-137">Tady můžete vybrat případné další licence, změnit jejich počet nebo předplatné pozastavit.</span><span class="sxs-lookup"><span data-stu-id="441e1-137">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="441e1-138">**Pro předplatná ISV SaaS (založená na licencích a na základě měření):**</span><span class="sxs-lookup"><span data-stu-id="441e1-138">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="441e1-139">Zobrazí se odkaz na web vydavatele ISV.</span><span class="sxs-lookup"><span data-stu-id="441e1-139">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="441e1-140">Tento odkaz by vám měl pomáhat s dokončením nastavení nasazení nebo účtu u předplatného zákazníka.</span><span class="sxs-lookup"><span data-stu-id="441e1-140">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="441e1-141">Ani vy ani váš zákazník neobdrží e-mail s pokyny k dokončení nastavení/zřizování pro tento typ předplatného ISV.)</span><span class="sxs-lookup"><span data-stu-id="441e1-141">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="441e1-142">Pokud vaše předplatné předchází 30denní bezplatnou zkušební verzi, použije se k automatickému vyzkoušení bezplatné zkušební období.</span><span class="sxs-lookup"><span data-stu-id="441e1-142">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="441e1-143">Jako partner v programu CSP se nemůžete vzdát bezplatné zkušební doby pro nabídky, které zakoupíte pro zákazníky.</span><span class="sxs-lookup"><span data-stu-id="441e1-143">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="441e1-144">Po skončení bezplatné zkušební doby se předplatné spustí a předplatné se převede na placený stav.</span><span class="sxs-lookup"><span data-stu-id="441e1-144">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="441e1-145">Předplatné se pak automaticky obnoví podle stejného plánu.</span><span class="sxs-lookup"><span data-stu-id="441e1-145">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="441e1-146">Aktualizace předplatných o doplňky</span><span class="sxs-lookup"><span data-stu-id="441e1-146">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="441e1-147">K nákupu doplňku musí zákazník nejdřív mít aktivní základní předplatné.</span><span class="sxs-lookup"><span data-stu-id="441e1-147">To purchase an add-on, the customer must first have an active base subscription.</span></span>  <span data-ttu-id="441e1-148">Doplňky není možné kupovat prostřednictvím katalogu.</span><span class="sxs-lookup"><span data-stu-id="441e1-148">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="441e1-149">Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="441e1-149">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="441e1-150">V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="441e1-150">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="441e1-151">Vyberte předplatné, které chcete spravovat.</span><span class="sxs-lookup"><span data-stu-id="441e1-151">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="441e1-152">Pod oddílem **stav** je seznam dostupných doplňků pro předplatné.</span><span class="sxs-lookup"><span data-stu-id="441e1-152">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="441e1-153">Aktualizujte množství licencí pro každý požadovaný doplněk.</span><span class="sxs-lookup"><span data-stu-id="441e1-153">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="441e1-154">Pak změny **odešlete**.</span><span class="sxs-lookup"><span data-stu-id="441e1-154">Then **Submit** your changes.</span></span>

<span data-ttu-id="441e1-155">Možnost zakoupit doplňky prostřednictvím partnerského centra je dostupná jenom pro přímé faktury a nepřímé poskytovatele.</span><span class="sxs-lookup"><span data-stu-id="441e1-155">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="441e1-156">Na základě základních požadavků a regionální dostupnosti se zobrazují jenom opravňující doplňky.</span><span class="sxs-lookup"><span data-stu-id="441e1-156">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="441e1-157">Další informace o cenách a nabídkách najdete v tématu matice nabídky prodejce cloudu.</span><span class="sxs-lookup"><span data-stu-id="441e1-157">For more information about pricing and offers, refer to the Cloud Reseller offer matrix.</span></span> <span data-ttu-id="441e1-158">Pozastavením základního předplatného se pozastaví také všechny přidružené doplňky.</span><span class="sxs-lookup"><span data-stu-id="441e1-158">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="441e1-159">Počáteční datum doplňků odpovídá základnímu předplatnému a poplatky se u první faktury účtují poměrně a následně se účtují na základě počátečního a koncového data účtování poplatků.</span><span class="sxs-lookup"><span data-stu-id="441e1-159">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="441e1-160">Další informace najdete v tématu [fakturace na základě licencí](license-based-billing.md).</span><span class="sxs-lookup"><span data-stu-id="441e1-160">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="441e1-161">Pozastavení nebo zrušení předplatného</span><span class="sxs-lookup"><span data-stu-id="441e1-161">Suspend or cancel a subscription</span></span>

<span data-ttu-id="441e1-162">Partneři můžou předplatné pozastavit nebo zrušit, pokud ho požaduje zákazník nebo v případě nedoplatku nebo podvodu.</span><span class="sxs-lookup"><span data-stu-id="441e1-162">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="441e1-163">Pozastavení předplatného</span><span class="sxs-lookup"><span data-stu-id="441e1-163">Suspend a subscription</span></span>

<span data-ttu-id="441e1-164">Když změníte stav předplatného na **pozastaveno**, uživatelé se nebudou moct přihlašovat ani získat přístup ke službám.</span><span class="sxs-lookup"><span data-stu-id="441e1-164">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="441e1-165">Přihlaste se k řídicímu [Partnerské centrum.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="441e1-165">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="441e1-166">V Partnerské centrum vyberte **Zákazníci** a pak v seznamu zvolte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="441e1-166">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="441e1-167">Zvolte předplatné, které chcete spravovat.</span><span class="sxs-lookup"><span data-stu-id="441e1-167">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="441e1-168">V části **Stav** zvolte **Pozastaveno**.</span><span class="sxs-lookup"><span data-stu-id="441e1-168">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="441e1-169">Pak změny **odešlete**.</span><span class="sxs-lookup"><span data-stu-id="441e1-169">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="441e1-170">Všechna data se odstraní, pokud se předplatné znovu neaktivuje do 90 dnů nebo 90 dnů plus počet dní mezi časem otevření účtu a prvním fakturačním obdobím (maximálně 120 dnů).</span><span class="sxs-lookup"><span data-stu-id="441e1-170">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="441e1-171">Když předplatné pozastavíte, datum, které se zobrazí pod tlačítkem **Pozastaveno,** značí, kdy automaticky vyprší platnost předplatného, pokud ho znovu neaktivujete.</span><span class="sxs-lookup"><span data-stu-id="441e1-171">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

>[!NOTE]
><span data-ttu-id="441e1-172">Předplatná CSP nemají prošlé období (stejně jako předplatná s přímým přístupem na web), během kterého služby stále fungují, ale předplatné negeneruje žádné poplatky za fakturaci.</span><span class="sxs-lookup"><span data-stu-id="441e1-172">CSP subscriptions don't have an expired period (the way web-direct subscriptions do) during which the services are still working but the subscription doesn't generate any billing charges.</span></span> <span data-ttu-id="441e1-173">Předplatná CSP jsou aktivní nebo pozastavená (nebo úplně odstraněná).</span><span class="sxs-lookup"><span data-stu-id="441e1-173">CSP subscriptions are either active or suspended (or fully deleted).</span></span>

### <a name="cancel-a-subscription"></a><span data-ttu-id="441e1-174">Zrušení předplatného</span><span class="sxs-lookup"><span data-stu-id="441e1-174">Cancel a subscription</span></span>

<span data-ttu-id="441e1-175">Předplatná SaaS založená na licencích můžete zrušit od vydavatelů ISV třetích stran v rámci Partnerské centrum [komerčního marketplace.](csp-commercial-marketplace-overview.md)</span><span class="sxs-lookup"><span data-stu-id="441e1-175">You can cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="441e1-176">Pokud zrušíte v rámci období zrušení, obdržíte úplnou refundaci.</span><span class="sxs-lookup"><span data-stu-id="441e1-176">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="441e1-177">Nabídky isv fakturované měsíčně:</span><span class="sxs-lookup"><span data-stu-id="441e1-177">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="441e1-178">Pokud zrušíte méně než 24 hodin od vystavení objednávky, obdržíte úplný kredit na další faktuře.</span><span class="sxs-lookup"><span data-stu-id="441e1-178">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="441e1-179">Pokud ji zrušíte později než 24 hodin po vystavení objednávky, bude zrušení naplánováno na prodloužení.</span><span class="sxs-lookup"><span data-stu-id="441e1-179">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="441e1-180">Pro nabídky fakturované ročně:</span><span class="sxs-lookup"><span data-stu-id="441e1-180">For offers billed annually:</span></span>

- <span data-ttu-id="441e1-181">Pokud zrušíte méně než 14 dnů od vystavení objednávky, obdržíte úplný kredit na další faktuře.</span><span class="sxs-lookup"><span data-stu-id="441e1-181">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="441e1-182">Pokud objednávku zrušíte později než 14 dnů od vystavení objednávky, bude zrušení naplánováno na prodloužení.</span><span class="sxs-lookup"><span data-stu-id="441e1-182">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="441e1-183">Po uplynutí těchto období se už možnost zrušení předplatného nebude zobrazit.</span><span class="sxs-lookup"><span data-stu-id="441e1-183">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="441e1-184">Služby isv třetích stran založené na využití a na základě měření (které například používají virtuální počítače nebo kontejnery) nemají nárok na vrácení.</span><span class="sxs-lookup"><span data-stu-id="441e1-184">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="441e1-185">Služby založené na využití je možné zrušit jako metodu zrušení.</span><span class="sxs-lookup"><span data-stu-id="441e1-185">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="441e1-186">Vzhledem k tomu, že se poplatky účtují po použití, nemají tyto služby nárok na refundaci.</span><span class="sxs-lookup"><span data-stu-id="441e1-186">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="441e1-187">Pokud chcete zrušit předplatné SaaS založené na licencích od vydavatele ISV, postupujte následovně:</span><span class="sxs-lookup"><span data-stu-id="441e1-187">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="441e1-188">Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="441e1-188">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="441e1-189">V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="441e1-189">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="441e1-190">Vyhledejte předplatné, které chcete zrušit.</span><span class="sxs-lookup"><span data-stu-id="441e1-190">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="441e1-191">Ve sloupci **stav** vyberte **Zrušit**.</span><span class="sxs-lookup"><span data-stu-id="441e1-191">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="441e1-192">Pak změny **odešlete**.</span><span class="sxs-lookup"><span data-stu-id="441e1-192">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="441e1-193">Pokud se zobrazí dialogové okno, vyplňte příslušné podrobnosti a pak vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="441e1-193">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="441e1-194">Zrušení potvrďte tak, že vyberete **Ano, zrušit**.</span><span class="sxs-lookup"><span data-stu-id="441e1-194">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="441e1-195">Můžete také zvolit zrušení předplatného Azure Marketplace pomocí rozhraní API.</span><span class="sxs-lookup"><span data-stu-id="441e1-195">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="441e1-196">Pokud to chcete udělat, přečtěte si téma [zrušení předplatného Azure Marketplace](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span><span class="sxs-lookup"><span data-stu-id="441e1-196">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="441e1-197">Vyberte, jestli se má automaticky obnovit předplatné z komerčního tržiště.</span><span class="sxs-lookup"><span data-stu-id="441e1-197">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="441e1-198">Ve výchozím nastavení jsou aktivní předplatná nastavená tak, aby se při vypršení jejich časového limitu automaticky prodlužovala jejich platnost.</span><span class="sxs-lookup"><span data-stu-id="441e1-198">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="441e1-199">Pro [odběry komerčních produktů na webu Marketplace](csp-commercial-marketplace-overview.md)můžete volitelně zvolit automatické obnovení předplatného.</span><span class="sxs-lookup"><span data-stu-id="441e1-199">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="441e1-200">Pokud chcete zastavit aktivní předplatné komerčního tržiště z automatického obnovování:</span><span class="sxs-lookup"><span data-stu-id="441e1-200">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="441e1-201">Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="441e1-201">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="441e1-202">V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="441e1-202">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="441e1-203">Vyberte **Předplatná**.</span><span class="sxs-lookup"><span data-stu-id="441e1-203">Select **Subscriptions**.</span></span> <span data-ttu-id="441e1-204">Obsahuje seznam všech předplatných založených na licencích, které jste zakoupili pro zákazníka.</span><span class="sxs-lookup"><span data-stu-id="441e1-204">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="441e1-205">Ve sloupci **předplatné** vyberte předplatné, které chcete upravit.</span><span class="sxs-lookup"><span data-stu-id="441e1-205">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="441e1-206">Na stránce Podrobnosti předplatného vyhledejte část **stav** a zrušte kontrolu **automatického obnovení** .</span><span class="sxs-lookup"><span data-stu-id="441e1-206">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="441e1-207">Vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="441e1-207">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="441e1-208">Další kroky</span><span class="sxs-lookup"><span data-stu-id="441e1-208">Next steps</span></span>

- [<span data-ttu-id="441e1-209">Nákup produktů z komerčního tržiště pro vaše zákazníky</span><span class="sxs-lookup"><span data-stu-id="441e1-209">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="441e1-210">Správa produktů z komerčního tržiště pro vaše zákazníky</span><span class="sxs-lookup"><span data-stu-id="441e1-210">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="441e1-211">Přehled komerčního marketplace</span><span class="sxs-lookup"><span data-stu-id="441e1-211">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)