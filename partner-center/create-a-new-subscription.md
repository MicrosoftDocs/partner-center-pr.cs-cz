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
ms.openlocfilehash: 8c3cfc2a6576029a8fdfb902a7b3889b4ea6c628
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/22/2020
ms.locfileid: "92527583"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="5e71c-103">Vytváření, pozastavování nebo rušení zákaznických předplatných</span><span class="sxs-lookup"><span data-stu-id="5e71c-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="5e71c-104">**Platí pro**</span><span class="sxs-lookup"><span data-stu-id="5e71c-104">**Applies to**</span></span>

- <span data-ttu-id="5e71c-105">Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="5e71c-105">Partner Center</span></span>
- <span data-ttu-id="5e71c-106">Partnerské centrum pro Microsoft Cloud pro státní správu USA</span><span class="sxs-lookup"><span data-stu-id="5e71c-106">Partner Center for Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="5e71c-107">Partneři CSP</span><span class="sxs-lookup"><span data-stu-id="5e71c-107">CSP partners</span></span>

<span data-ttu-id="5e71c-108">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="5e71c-108">**Appropriate roles**</span></span>

- <span data-ttu-id="5e71c-109">Agent správce</span><span class="sxs-lookup"><span data-stu-id="5e71c-109">Admin agent</span></span>
- <span data-ttu-id="5e71c-110">Správce fakturace</span><span class="sxs-lookup"><span data-stu-id="5e71c-110">Billing admin</span></span>
- <span data-ttu-id="5e71c-111">Globální správce</span><span class="sxs-lookup"><span data-stu-id="5e71c-111">Global admin</span></span>
- <span data-ttu-id="5e71c-112">Agent helpdesku</span><span class="sxs-lookup"><span data-stu-id="5e71c-112">Helpdesk agent</span></span>
- <span data-ttu-id="5e71c-113">Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="5e71c-113">Sales agent</span></span>

<span data-ttu-id="5e71c-114">Až vytvoříte záznam o zákazníkovi v partnerském centru, můžete si ho prodávat do produktů v katalogu.</span><span class="sxs-lookup"><span data-stu-id="5e71c-114">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="5e71c-115">To zahrnuje produkty publikované společností Microsoft i produkty SaaS (software jako služba), které publikovali nezávislí výrobci softwaru (ISV) třetích stran na [komerčním tržišti](https://azuremarketplace.microsoft.com/marketplace).</span><span class="sxs-lookup"><span data-stu-id="5e71c-115">This includes products published by Microsoft as well as Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="5e71c-116">Některé nabídky jsou omezené na jedno předplatné na zákazníka.</span><span class="sxs-lookup"><span data-stu-id="5e71c-116">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="5e71c-117">Pokud chcete zobrazit seznam nabídek, které jsou omezené, navštivte stránku ceny a nabídky partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="5e71c-117">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="5e71c-118">Jako partner v programu CSP můžete zakoupit jenom SaaS odběry **založené na licencích** od vydavatelů ISV v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="5e71c-118">As a partner in the CSP program, you can only purchase **license-based** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="5e71c-119">To znamená, že si můžete koupit jakoukoli nabídku SaaS **založenou na licencích** , kterou vám vydavatel ISV zpřístupnila, včetně [exkluzivních nabídek](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) , ke kterým máte přístup.</span><span class="sxs-lookup"><span data-stu-id="5e71c-119">This means you can purchase any **license-based** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="5e71c-120">Pokud si chcete koupit nebo spravovat jiné komerční nabídky na webu Marketplace od nezávislého výrobce softwaru (jako jsou nabídky na základě **využití** , měřené nebo spotřebované na základě spotřeby zahrnující aplikace, kontejnery nebo virtuální počítače Azure), musíte přejít na [portál pro správu Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="5e71c-120">To purchase or manage other, commercial marketplace offers from ISVs (such as **usage-based** , metered, or consumption-based offers involving Azure applications, Containers or VMs), you must go to the [Azure management portal](https://portal.azure.com/).</span></span> <span data-ttu-id="5e71c-121">Další informace najdete v tématu [Nákup produktů z komerčního tržiště](csp-commercial-marketplace-purchase.md).</span><span class="sxs-lookup"><span data-stu-id="5e71c-121">For more information, see [Purchase commercial marketplace products](csp-commercial-marketplace-purchase.md).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="5e71c-122">Vytvoření nového předplatného</span><span class="sxs-lookup"><span data-stu-id="5e71c-122">Create a new subscription</span></span>

1. <span data-ttu-id="5e71c-123">Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="5e71c-123">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="5e71c-124">V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="5e71c-124">From the Partner Center menu, select **Customers** , then choose a customer from the list.</span></span>

3. <span data-ttu-id="5e71c-125">Vyberte **přidat odběr** .</span><span class="sxs-lookup"><span data-stu-id="5e71c-125">Select **Add subscription** .</span></span> <span data-ttu-id="5e71c-126">Na kartě **online služby** se zobrazí všechny dostupné nabídky SaaS Marketplace.</span><span class="sxs-lookup"><span data-stu-id="5e71c-126">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="5e71c-127">Chcete-li zobrazit pouze určité typy předplatných, proveďte výběr v dostupných filtrech:</span><span class="sxs-lookup"><span data-stu-id="5e71c-127">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="5e71c-128">**Vydavatel** : vyberte **Microsoft** , pokud chcete zobrazit jenom nabídky od Microsoftu nebo **partnera** , aby viděli produkty z komerčního tržiště publikované prostřednictvím nezávislého výrobce softwaru.</span><span class="sxs-lookup"><span data-stu-id="5e71c-128">**Publisher** : Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="5e71c-129">**Typ fakturace** : Vyberte typ fakturace předplatného, který chcete použít: **licence** nebo **použití** .</span><span class="sxs-lookup"><span data-stu-id="5e71c-129">**Billing type** : Select the type of subscription billing you want to use: **License** or **Usage** .</span></span> <span data-ttu-id="5e71c-130">Informace, které vám pomůžou při rozhodování mezi měsíční a roční frekvencí fakturace, najdete v tématu [fakturace na základě licencí](license-based-billing.md) .</span><span class="sxs-lookup"><span data-stu-id="5e71c-130">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="5e71c-131">**Kategorie** : vyberte **podnik** , **malý podnik** nebo **zkušební verzi** .</span><span class="sxs-lookup"><span data-stu-id="5e71c-131">**Category** : Choose **Enterprise** , **Small business** , or **Trial** .</span></span> <span data-ttu-id="5e71c-132">Informace o zkušebních předplatných najdete v tématu [Nabídka vašich zákazníků s zkušebními produkty Microsoftu](offer-your-customers-trials-of-microsoft-products.md).</span><span class="sxs-lookup"><span data-stu-id="5e71c-132">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="5e71c-133">Vyberte předplatné produktů, které chcete pro zákazníka koupit.</span><span class="sxs-lookup"><span data-stu-id="5e71c-133">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="5e71c-134">Produkty, které vidíte, závisí na typu segmentu zákazníka (vzdělávání, státní správa atd.) a na použitých filtrech.</span><span class="sxs-lookup"><span data-stu-id="5e71c-134">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="5e71c-135">Některé nabídky zobrazené na webu Marketplace nemusí být vždy dostupné konkrétnímu zákazníkovi nebo konkrétnímu partnerovi CSP.</span><span class="sxs-lookup"><span data-stu-id="5e71c-135">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="5e71c-136">To může být způsobeno tím, že:</span><span class="sxs-lookup"><span data-stu-id="5e71c-136">This can be because:</span></span>

   - <span data-ttu-id="5e71c-137">Zákazník už má k tomuto produktu předplatné a je povolený jenom jeden.</span><span class="sxs-lookup"><span data-stu-id="5e71c-137">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="5e71c-138">Předplatné zákazníka může být pozastavené (v takovém případě můžete předplatné znovu aktivovat, ale nekoupit nové).</span><span class="sxs-lookup"><span data-stu-id="5e71c-138">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="5e71c-139">V případě nabídek ISV SaaS může být nabídka k dispozici z několika důvodů k zakoupení: ISV nemusí podporovat fakturační zemi nebo oblast zákazníka; nezávislý výrobce softwaru se možná rozhodl, že nabídku zpřístupní prostřednictvím programu CSP. nebo nezávislý výrobce softwaru mohl vytvořit nabídku [výhradně](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) pro určité partnery CSP.</span><span class="sxs-lookup"><span data-stu-id="5e71c-139">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="5e71c-140">Nabídku ISV nelze také využít v partnerském centru (například v kontejnerech nebo v některých nabídkách založených na používání).</span><span class="sxs-lookup"><span data-stu-id="5e71c-140">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="5e71c-141">U každého předplatného, které chcete přidat, zadejte počet licencí (v případě potřeby) a vyberte **Přidat do košíku** .</span><span class="sxs-lookup"><span data-stu-id="5e71c-141">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart** .</span></span>

7. <span data-ttu-id="5e71c-142">Až skončíte s přidáváním předplatných, vyberte **zkontrolovat** a zkontrolovat vaši objednávku.</span><span class="sxs-lookup"><span data-stu-id="5e71c-142">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="5e71c-143">Po kontrole objednávek a jejich přípravě na nákup můžete vybrat **koupit** .</span><span class="sxs-lookup"><span data-stu-id="5e71c-143">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy** .</span></span>

9. <span data-ttu-id="5e71c-144">Po zakoupení předplatného pro zákazníka dojde k následujícímu:</span><span class="sxs-lookup"><span data-stu-id="5e71c-144">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="5e71c-145">Předplatné můžete zkontrolovat nebo upravit výběrem názvu předplatného ze stránky **předplatné** daného zákazníka.</span><span class="sxs-lookup"><span data-stu-id="5e71c-145">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="5e71c-146">Tady můžete vybrat licence pro doplňky, pokud jsou k dispozici, změnit množství licencí nebo pozastavit předplatné.</span><span class="sxs-lookup"><span data-stu-id="5e71c-146">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="5e71c-147">**Pro předplatná ISV SaaS (založená na licencích):**</span><span class="sxs-lookup"><span data-stu-id="5e71c-147">**For ISV SaaS (license-based) subscriptions:**</span></span>
    - <span data-ttu-id="5e71c-148">Zobrazí se odkaz na web vydavatele ISV.</span><span class="sxs-lookup"><span data-stu-id="5e71c-148">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="5e71c-149">Tento odkaz by vám měl pomáhat s dokončením nastavení nasazení nebo účtu u předplatného zákazníka.</span><span class="sxs-lookup"><span data-stu-id="5e71c-149">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="5e71c-150">Ani vy ani váš zákazník neobdrží e-mail s pokyny k dokončení nastavení/zřizování pro tento typ předplatného ISV.)</span><span class="sxs-lookup"><span data-stu-id="5e71c-150">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="5e71c-151">Pokud vaše předplatné předchází 30denní bezplatnou zkušební verzi, použije se k automatickému vyzkoušení bezplatné zkušební období.</span><span class="sxs-lookup"><span data-stu-id="5e71c-151">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="5e71c-152">Jako partner v programu CSP se nemůžete vzdát bezplatné zkušební doby pro nabídky, které zakoupíte pro zákazníky.</span><span class="sxs-lookup"><span data-stu-id="5e71c-152">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="5e71c-153">Po skončení bezplatné zkušební doby se předplatné spustí a předplatné se převede na placený stav.</span><span class="sxs-lookup"><span data-stu-id="5e71c-153">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="5e71c-154">Předplatné se pak automaticky obnoví podle stejného plánu.</span><span class="sxs-lookup"><span data-stu-id="5e71c-154">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="5e71c-155">Aktualizace předplatných o doplňky</span><span class="sxs-lookup"><span data-stu-id="5e71c-155">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="5e71c-156">Aby si zákazník mohl koupit doplněk, musí nejprve mít aktivní základní předplatné.</span><span class="sxs-lookup"><span data-stu-id="5e71c-156">To purchase an add-on the customer must first have an active base subscription.</span></span>  <span data-ttu-id="5e71c-157">Doplňky není možné kupovat prostřednictvím katalogu.</span><span class="sxs-lookup"><span data-stu-id="5e71c-157">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="5e71c-158">Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="5e71c-158">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="5e71c-159">V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="5e71c-159">From the Partner Center menu, select **Customers** , then choose a customer from the list.</span></span>

3. <span data-ttu-id="5e71c-160">Vyberte předplatné, které chcete spravovat.</span><span class="sxs-lookup"><span data-stu-id="5e71c-160">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="5e71c-161">Pod oddílem **stav** je seznam dostupných doplňků pro předplatné.</span><span class="sxs-lookup"><span data-stu-id="5e71c-161">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="5e71c-162">Aktualizujte množství licencí pro každý požadovaný doplněk.</span><span class="sxs-lookup"><span data-stu-id="5e71c-162">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="5e71c-163">Pak změny **odešlete** .</span><span class="sxs-lookup"><span data-stu-id="5e71c-163">Then **Submit** your changes.</span></span>

<span data-ttu-id="5e71c-164">Možnost zakoupit doplňky prostřednictvím partnerského centra je dostupná jenom pro přímé faktury a nepřímé poskytovatele.</span><span class="sxs-lookup"><span data-stu-id="5e71c-164">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="5e71c-165">Na základě základních požadavků a regionální dostupnosti se zobrazují jenom opravňující doplňky.</span><span class="sxs-lookup"><span data-stu-id="5e71c-165">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="5e71c-166">Další informace o cenách a nabídkách najdete v tabulce nabídek pro prodejce cloudových řešení.</span><span class="sxs-lookup"><span data-stu-id="5e71c-166">Refer to the Cloud Reseller offer matrix for more information about pricing and offers.</span></span>  <span data-ttu-id="5e71c-167">Pozastavením základního předplatného se pozastaví také všechny přidružené doplňky.</span><span class="sxs-lookup"><span data-stu-id="5e71c-167">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="5e71c-168">Počáteční datum doplňků odpovídá základnímu předplatnému a poplatky se u první faktury účtují poměrně a následně se účtují na základě počátečního a koncového data účtování poplatků.</span><span class="sxs-lookup"><span data-stu-id="5e71c-168">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="5e71c-169">Další informace najdete v tématu [fakturace na základě licencí](license-based-billing.md).</span><span class="sxs-lookup"><span data-stu-id="5e71c-169">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="5e71c-170">Pozastavení nebo zrušení předplatného</span><span class="sxs-lookup"><span data-stu-id="5e71c-170">Suspend or cancel a subscription</span></span>

<span data-ttu-id="5e71c-171">Partneři můžou předplatné pozastavit nebo zrušit, pokud ho požaduje zákazník nebo v případě nedoplatku nebo podvodu.</span><span class="sxs-lookup"><span data-stu-id="5e71c-171">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="5e71c-172">Pozastavení předplatného</span><span class="sxs-lookup"><span data-stu-id="5e71c-172">Suspend a subscription</span></span>

<span data-ttu-id="5e71c-173">Když změníte stav předplatného na **pozastaveno** , uživatelé se nebudou moct přihlašovat ani získat přístup ke službám.</span><span class="sxs-lookup"><span data-stu-id="5e71c-173">When you change the status of a subscription to **Suspended** , users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="5e71c-174">Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="5e71c-174">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="5e71c-175">V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="5e71c-175">From the Partner Center menu, select **Customers** , then choose a customer from the list.</span></span>

3. <span data-ttu-id="5e71c-176">Vyberte předplatné, které chcete spravovat.</span><span class="sxs-lookup"><span data-stu-id="5e71c-176">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="5e71c-177">V části **Stav** zvolte **Pozastaveno** .</span><span class="sxs-lookup"><span data-stu-id="5e71c-177">In the **Status** section, choose **Suspended** .</span></span> <span data-ttu-id="5e71c-178">Pak změny **odešlete** .</span><span class="sxs-lookup"><span data-stu-id="5e71c-178">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="5e71c-179">Všechna data budou odstraněna, pokud předplatné nebude znovu aktivováno během 90 dnů nebo 90 dnů plus počet dní mezi časem otevření účtu a prvním fakturačním obdobím (maximum 120 dní).</span><span class="sxs-lookup"><span data-stu-id="5e71c-179">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="5e71c-180">Když pozastavíte předplatné, datum zobrazené pod tlačítkem **pozastavit** indikuje, kdy by předplatné automaticky vyprší, pokud ho znovu neaktivujete.</span><span class="sxs-lookup"><span data-stu-id="5e71c-180">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

### <a name="cancel-a-subscription"></a><span data-ttu-id="5e71c-181">Zrušení předplatného</span><span class="sxs-lookup"><span data-stu-id="5e71c-181">Cancel a subscription</span></span>

<span data-ttu-id="5e71c-182">Máte možnost zrušit si předplatné SaaS založené na licencích od třetích stran vydavatelů ISV v rámci [obchodního tržiště](csp-commercial-marketplace-overview.md)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="5e71c-182">You have the option to cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="5e71c-183">Pokud zrušíte v rámci období zrušení, obdržíte plnou refundaci.</span><span class="sxs-lookup"><span data-stu-id="5e71c-183">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="5e71c-184">U nezávislých výrobců softwaru nabízíme fakturaci za měsíc:</span><span class="sxs-lookup"><span data-stu-id="5e71c-184">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="5e71c-185">Pokud po umístění objednávky zrušíte méně než 24 hodin, obdržíte na další faktuře celý kredit.</span><span class="sxs-lookup"><span data-stu-id="5e71c-185">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="5e71c-186">Pokud zrušíte pozdější dobu než 24 hodin od okamžiku, kdy jste objednávku nastavili, zrušení se naplánuje při obnovení.</span><span class="sxs-lookup"><span data-stu-id="5e71c-186">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="5e71c-187">Pro nabídky účtované ročně:</span><span class="sxs-lookup"><span data-stu-id="5e71c-187">For offers billed annually:</span></span>

- <span data-ttu-id="5e71c-188">Pokud po umístění objednávky zrušíte méně než 14 dní, obdržíte na další faktuře celý kredit.</span><span class="sxs-lookup"><span data-stu-id="5e71c-188">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="5e71c-189">Pokud zrušíte akci později než 14 dní po umístění objednávky, zrušení se naplánuje při obnovení.</span><span class="sxs-lookup"><span data-stu-id="5e71c-189">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="5e71c-190">Po uplynutí těchto období se už nebude zobrazovat možnost zrušit předplatné.</span><span class="sxs-lookup"><span data-stu-id="5e71c-190">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="5e71c-191">Služby nezávislé na používání a měřené od jiných výrobců ISV (například virtuální počítače nebo kontejnery) nejsou způsobilé k návratu.</span><span class="sxs-lookup"><span data-stu-id="5e71c-191">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="5e71c-192">Služby založené na využití se dají zrušit jako metoda zrušení.</span><span class="sxs-lookup"><span data-stu-id="5e71c-192">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="5e71c-193">Vzhledem k tomu, že se poplatky účtují po použití, tyto služby nemají nárok na refundaci.</span><span class="sxs-lookup"><span data-stu-id="5e71c-193">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="5e71c-194">Pokud chcete zrušit předplatné SaaS založené na licencích od vydavatele ISV, postupujte následovně:</span><span class="sxs-lookup"><span data-stu-id="5e71c-194">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="5e71c-195">Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="5e71c-195">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="5e71c-196">V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="5e71c-196">From the Partner Center menu, select **Customers** , then choose a customer from the list.</span></span>

3. <span data-ttu-id="5e71c-197">Vyhledejte předplatné, které chcete zrušit.</span><span class="sxs-lookup"><span data-stu-id="5e71c-197">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="5e71c-198">Ve sloupci **stav** vyberte **Zrušit** .</span><span class="sxs-lookup"><span data-stu-id="5e71c-198">In the **Status** column, select **Cancel** .</span></span> <span data-ttu-id="5e71c-199">Pak změny **odešlete** .</span><span class="sxs-lookup"><span data-stu-id="5e71c-199">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="5e71c-200">Pokud se zobrazí dialogové okno, vyplňte příslušné podrobnosti a pak vyberte **Odeslat** .</span><span class="sxs-lookup"><span data-stu-id="5e71c-200">If a dialog box appears, fill out any relevant details then select **Submit** .</span></span>

6. <span data-ttu-id="5e71c-201">Zrušení potvrďte tak, že vyberete **Ano, zrušit** .</span><span class="sxs-lookup"><span data-stu-id="5e71c-201">To confirm the cancellation, select **Yes, cancel** .</span></span>

> [!NOTE]
> <span data-ttu-id="5e71c-202">Můžete také zvolit zrušení předplatného Azure Marketplace pomocí rozhraní API.</span><span class="sxs-lookup"><span data-stu-id="5e71c-202">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="5e71c-203">Pokud to chcete udělat, přečtěte si téma [zrušení předplatného Azure Marketplace](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span><span class="sxs-lookup"><span data-stu-id="5e71c-203">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="5e71c-204">Vyberte, jestli se má automaticky obnovit předplatné z komerčního tržiště.</span><span class="sxs-lookup"><span data-stu-id="5e71c-204">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="5e71c-205">Ve výchozím nastavení jsou aktivní předplatná nastavená tak, aby se při vypršení jejich časového limitu automaticky prodlužovala jejich platnost.</span><span class="sxs-lookup"><span data-stu-id="5e71c-205">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="5e71c-206">Pro [odběry komerčních produktů na webu Marketplace](csp-commercial-marketplace-overview.md)můžete volitelně zvolit automatické obnovení předplatného.</span><span class="sxs-lookup"><span data-stu-id="5e71c-206">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="5e71c-207">Pokud chcete zastavit aktivní předplatné komerčního tržiště z automatického obnovování:</span><span class="sxs-lookup"><span data-stu-id="5e71c-207">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="5e71c-208">Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="5e71c-208">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="5e71c-209">V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="5e71c-209">From the Partner Center menu, select **Customers** , then choose a customer from the list.</span></span>

3. <span data-ttu-id="5e71c-210">Vyberte **Předplatná** .</span><span class="sxs-lookup"><span data-stu-id="5e71c-210">Select **Subscriptions** .</span></span> <span data-ttu-id="5e71c-211">Obsahuje seznam všech předplatných založených na licencích, které jste zakoupili pro zákazníka.</span><span class="sxs-lookup"><span data-stu-id="5e71c-211">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="5e71c-212">Ve sloupci **předplatné** vyberte předplatné, které chcete upravit.</span><span class="sxs-lookup"><span data-stu-id="5e71c-212">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="5e71c-213">Na stránce Podrobnosti předplatného vyhledejte část **stav** a zrušte kontrolu **automatického obnovení** .</span><span class="sxs-lookup"><span data-stu-id="5e71c-213">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="5e71c-214">Vyberte **Odeslat** .</span><span class="sxs-lookup"><span data-stu-id="5e71c-214">Select **Submit** .</span></span>

## <a name="next-steps"></a><span data-ttu-id="5e71c-215">Další kroky</span><span class="sxs-lookup"><span data-stu-id="5e71c-215">Next steps</span></span>

- [<span data-ttu-id="5e71c-216">Nákup produktů z komerčního tržiště pro vaše zákazníky</span><span class="sxs-lookup"><span data-stu-id="5e71c-216">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="5e71c-217">Správa produktů z komerčního tržiště pro vaše zákazníky</span><span class="sxs-lookup"><span data-stu-id="5e71c-217">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="5e71c-218">Přehled komerčního tržiště</span><span class="sxs-lookup"><span data-stu-id="5e71c-218">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)