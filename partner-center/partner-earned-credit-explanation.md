---
title: Získaný kredit partnerů pro spravované služby
ms.topic: article
ms.date: 11/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Seznamte se s tím, jak se počítá a hradí Microsoft partnerd Credit (PEC) pro spravované služby a jak zajistit, abyste měli nárok na to.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 97af446c4021e9785833374131eee2f08431b5fe
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/01/2020
ms.locfileid: "96474304"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a><span data-ttu-id="2ebcc-103">Principy výpočtu a vyplácení kreditu získaného partnerem</span><span class="sxs-lookup"><span data-stu-id="2ebcc-103">How the partner earned credit is calculated and paid</span></span>

<span data-ttu-id="2ebcc-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="2ebcc-104">**Appropriate roles**</span></span>

- <span data-ttu-id="2ebcc-105">Globální správce</span><span class="sxs-lookup"><span data-stu-id="2ebcc-105">Global admin</span></span>
- <span data-ttu-id="2ebcc-106">Správce uživatelů</span><span class="sxs-lookup"><span data-stu-id="2ebcc-106">User admin</span></span>
- <span data-ttu-id="2ebcc-107">Agent správce</span><span class="sxs-lookup"><span data-stu-id="2ebcc-107">Admin agent</span></span>
- <span data-ttu-id="2ebcc-108">Správce fakturace</span><span class="sxs-lookup"><span data-stu-id="2ebcc-108">Billing admin</span></span>
- <span data-ttu-id="2ebcc-109">Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="2ebcc-109">Sales agent</span></span>

<span data-ttu-id="2ebcc-110">Získaný kredit partnerů pro spravované služby (PEC) rozpoznává a vyměňuje partnery, kteří mají nepřetržitou provozní kontrolu a správu částí, nebo celé prostředí Azure svých zákazníků.</span><span class="sxs-lookup"><span data-stu-id="2ebcc-110">Partner earned credit for managed services (PEC) recognizes and rewards partners that own the 24x7 IT operational control and management of parts of, or the entire, Azure environment of their customers.</span></span> <span data-ttu-id="2ebcc-111">Ve výchozím nastavení je ve zprostředkovateli CSP udělena potřebná přístupová práva k předplatnému zákazníka, což jim umožňuje provádět 24 × 7 provozní správu a kontrolu nad prostředky v rámci předplatného.</span><span class="sxs-lookup"><span data-stu-id="2ebcc-111">By default, in CSP, partners are granted the necessary access rights to the customer's subscription allowing them to perform 24 X 7 operational management and control of the resources on the subscription.</span></span> <span data-ttu-id="2ebcc-112">Další způsoby, jak zákazník může zřídit přístup pro transakčního partnera, je popsaný v následující části.</span><span class="sxs-lookup"><span data-stu-id="2ebcc-112">Additional ways in which customer can provision access for transacting partner is described in the following section.</span></span> <span data-ttu-id="2ebcc-113">Měsíční fakturovaná částka nezahrnuje kredit získaný partnerem.</span><span class="sxs-lookup"><span data-stu-id="2ebcc-113">The monthly invoice amount is net of partner earned credit.</span></span> <span data-ttu-id="2ebcc-114">Partneři můžou zobrazit podrobnosti o řadiči PEC na jejich měsíčním souboru rekognoskaci.</span><span class="sxs-lookup"><span data-stu-id="2ebcc-114">Partners can see the PEC details on their monthly recon file.</span></span> <span data-ttu-id="2ebcc-115">Další způsoby, jak může zákazník zřídit přístup pro transakčního partnera, najdete [v článku Správa předplatných a prostředků v plánu Azure](azure-plan-manage.md).</span><span class="sxs-lookup"><span data-stu-id="2ebcc-115">For additional ways in which a customer can provision access for the transacting partner, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="2ebcc-116">Také číst [obnovit oprávnění správce pro předplatná Azure CSP](revoke-reinstate-csp.md)</span><span class="sxs-lookup"><span data-stu-id="2ebcc-116">Also read [Reinstate admin privileges for Azure CSP subscriptions](revoke-reinstate-csp.md)</span></span>

## <a name="important-eligibility-and-calculation-information"></a><span data-ttu-id="2ebcc-117">Důležité informace o způsobilosti a výpočtech</span><span class="sxs-lookup"><span data-stu-id="2ebcc-117">Important eligibility and calculation information</span></span>

- <span data-ttu-id="2ebcc-118">Partner by měl mít aktivní smlouvu MPN a platnou roli RBAC, aby získal získaný kredit pro prostředky Azure, které spravují.</span><span class="sxs-lookup"><span data-stu-id="2ebcc-118">Partner should have an active MPN agreement and valid RBAC role to receive earned credit for the Azure assets they manage.</span></span> 

- <span data-ttu-id="2ebcc-119">V případě nepřímých zprostředkovatelů a jejich nepřímých prodejců budou mít nepřímý poskytovatel nárok na PEC, pokud buď nepřímý poskytovatel, nebo nepřímý prodejce nebo obojí mají nepřetržitou provozní kontrolu a správu prostředků Azure zákazníka v CSP.</span><span class="sxs-lookup"><span data-stu-id="2ebcc-119">In the case of indirect providers and their indirect resellers, the indirect provider will be eligible for PEC if either the indirect provider, or the indirect reseller or both have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span>

- <span data-ttu-id="2ebcc-120">K účtované (Fakturovatelné) spotřebě na Azure majetku v CSP spravovaném partnerem se přidruží služba PEC.</span><span class="sxs-lookup"><span data-stu-id="2ebcc-120">PEC is associated to billed (chargeable) consumption of customer's Azure estate in CSP managed by the partner.</span></span> <span data-ttu-id="2ebcc-121">K dispozici je PEC jenom partnerům v CSP, které účtuje Microsoft (nepřímý poskytovatel a partner poskytující přímý přístup k fakturaci).</span><span class="sxs-lookup"><span data-stu-id="2ebcc-121">PEC is made available only to partners in CSP billed by Microsoft (indirect provider and direct bill partner).</span></span> 

- <span data-ttu-id="2ebcc-122">Opravňující služby: získaný partnerský kredit se vztahuje na služby uvedené ve **cenách Azure plánu** , které mohou partneři exportovat na stránce s [cenami plánu Azure](https://partner.microsoft.com/commerce/sales) .</span><span class="sxs-lookup"><span data-stu-id="2ebcc-122">Eligible services: Partner earned credit is applicable to services listed in the **Azure plan consumption pricing** which partners can export from the [Azure plan pricing](https://partner.microsoft.com/commerce/sales) page.</span></span> 

- <span data-ttu-id="2ebcc-123">Nezpůsobilé služby: získaný kredit pro partnery je *_* nepoužit pro_\* následující:</span><span class="sxs-lookup"><span data-stu-id="2ebcc-123">Ineligible services: Partner earned credit is \**_not_* _ applicable to the following:</span></span>
    - <span data-ttu-id="2ebcc-124">Rezervace plánu Azure</span><span class="sxs-lookup"><span data-stu-id="2ebcc-124">Azure Plan reservations</span></span>
    - <span data-ttu-id="2ebcc-125">Produkty třetích stran identifikované jako *třetí strana*\* ve **sloupci značky** ceny spotřeby plánu Azure</span><span class="sxs-lookup"><span data-stu-id="2ebcc-125">Third-party products identified as _ *Third Party*\* in the **Tags column** of the Azure plan consumption price</span></span>    
    - <span data-ttu-id="2ebcc-126">Produkty v ceníku webu Marketplace</span><span class="sxs-lookup"><span data-stu-id="2ebcc-126">Products in the Marketplace price list</span></span>
   - [<span data-ttu-id="2ebcc-127">Virtual Machines na místě Azure</span><span class="sxs-lookup"><span data-stu-id="2ebcc-127">Azure Spot Virtual Machines</span></span>](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- <span data-ttu-id="2ebcc-128">PEC se počítá denně a je možné ji zobrazit v souboru denního využití a v souboru rekognoskaci pro měsíční fakturu.</span><span class="sxs-lookup"><span data-stu-id="2ebcc-128">PEC is calculated daily and can be viewed in the daily usage file and monthly invoice recon file.</span></span> <span data-ttu-id="2ebcc-129">Partner (nepřímý poskytovatel nebo nepřímý prodejce) musí mít přístup k celému dni (nepřetržitě), aby mohl získat PEC.</span><span class="sxs-lookup"><span data-stu-id="2ebcc-129">A partner (indirect provider or indirect reseller) must have access for the entire day (24x7) to ensure they earn PEC.</span></span> <span data-ttu-id="2ebcc-130">Na spravovaných prostředcích Azure se každý den počítá PEC.</span><span class="sxs-lookup"><span data-stu-id="2ebcc-130">PEC is calculated on daily basis on the managed Azure assets.</span></span> <span data-ttu-id="2ebcc-131">Maximální počet řadičů PEC pro dané fakturační období (měsíc) je 15%.</span><span class="sxs-lookup"><span data-stu-id="2ebcc-131">The maximum PEC for a given billing period (Month) is 15%.</span></span> <span data-ttu-id="2ebcc-132">Partneři uchovávají trvalý privilegovaný přístup v průběhu měsíce (rozsah přístupu) a u všech oprávněných prostředků (rozsah přístupu) získají úplné PEC o 15%.</span><span class="sxs-lookup"><span data-stu-id="2ebcc-132">Partners retaining persistent privileged access through the month(span of access) and for all the eligible resources (scope of access) will earn full PEC of 15%.</span></span> <span data-ttu-id="2ebcc-133">Snížení rozsahu a rozpětí rozpětí bude mít za měsíc nižší sazbu PEC.</span><span class="sxs-lookup"><span data-stu-id="2ebcc-133">Scope and span reduction will result in lower PEC rate for the month.</span></span> <span data-ttu-id="2ebcc-134">Denní hodnocený soubor využití se denně zobrazuje na prostředku Azure, ať už se používá PEC nebo ne.</span><span class="sxs-lookup"><span data-stu-id="2ebcc-134">Daily rated usage file shows on daily basis on an Azure asset whether PEC is applied or not.</span></span> <span data-ttu-id="2ebcc-135">Partneři taky můžou zaregistrovat výstrahy a zjistit, jestli existují změny trvalého privilegovaného přístupu.</span><span class="sxs-lookup"><span data-stu-id="2ebcc-135">Partners can also enroll in alerts to detect if there are changes to persistent privileged access.</span></span>

- <span data-ttu-id="2ebcc-136">Řadič PEC se získal na úrovni prostředků Azure.</span><span class="sxs-lookup"><span data-stu-id="2ebcc-136">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="2ebcc-137">Pokud má partner platný přístup v rámci předplatného nebo na úrovni skupiny prostředků, bude každý prostředek, který má role až k vyšší entitě, získávat řadiče PEC.</span><span class="sxs-lookup"><span data-stu-id="2ebcc-137">If the partner has valid access at the subscription, or resource group level, each resource that roles up to the higher entity will earn PEC.</span></span>  

- <span data-ttu-id="2ebcc-138">Podrobnosti o řadičích PEC budou také k dispozici ve [službě Azure cost management](/azure/cost-management-billing/costs/get-started-partners) .</span><span class="sxs-lookup"><span data-stu-id="2ebcc-138">PEC details will also be available on [Azure Cost management](/azure/cost-management-billing/costs/get-started-partners)</span></span>

## <a name="azure-cost-management"></a><span data-ttu-id="2ebcc-139">Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="2ebcc-139">Azure Cost Management</span></span>

<span data-ttu-id="2ebcc-140">Azure Cost Management (ACM) s využitím analýzy nákladů umožňuje jako partnera zobrazit náklady, které dostaly výhody PEC.</span><span class="sxs-lookup"><span data-stu-id="2ebcc-140">Azure Cost Management (ACM) using Cost Analysis enables you as a partner to view the costs that have received the benefit of PEC.</span></span>  

1. <span data-ttu-id="2ebcc-141">V [Azure Portal](https://portal.azure.com)se přihlaste ke svému partnerskému tenantovi a vyberte **cost management + fakturace**.</span><span class="sxs-lookup"><span data-stu-id="2ebcc-141">In the [Azure portal](https://portal.azure.com), sign into your partner tenant and select **Cost Management + Billing**.</span></span>

2. <span data-ttu-id="2ebcc-142">Vybrat **správu nákladů**</span><span class="sxs-lookup"><span data-stu-id="2ebcc-142">Select **Cost management**</span></span>

3. <span data-ttu-id="2ebcc-143">Vybrat **analýzu nákladů**</span><span class="sxs-lookup"><span data-stu-id="2ebcc-143">Select **Cost Analysis**</span></span>

   <span data-ttu-id="2ebcc-144">V zobrazení analýza nákladů se zobrazí náklady na fakturační účet pro všechny služby zakoupené a spotřebované v cenách, které platíte společnosti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2ebcc-144">The Cost Analysis view will display the costs for your billing account, for all the services purchased and consumed at the prices that you pay Microsoft.</span></span>

4. <span data-ttu-id="2ebcc-145">V rozevíracím seznamu v rozevíracím grafu vyberte **PartnerEarnedCreditApplied** , aby se zobrazily náklady s použitím pec.</span><span class="sxs-lookup"><span data-stu-id="2ebcc-145">Select **PartnerEarnedCreditApplied** in the drop down on a pivot chart to see costs that have PEC applied.</span></span> <span data-ttu-id="2ebcc-146">Pokud má vlastnost **PartnerEarnedCreditApplied** hodnotu true, mají přidružené náklady nárok na zvýhodněný kredit získaný partnerem.</span><span class="sxs-lookup"><span data-stu-id="2ebcc-146">When **PartnerEarnedCreditApplied** property is True, the associated cost has the benefit of the partner earned credit.</span></span> 

<span data-ttu-id="2ebcc-147">Pokud má vlastnost PartnerEarnedCreditApplied hodnotu false, přidružené náklady nevyhověly požadovanému nároku na kredit nebo zakoupená služba nemá nárok na kredit získaný partnerem.</span><span class="sxs-lookup"><span data-stu-id="2ebcc-147">When the PartnerEarnedCreditApplied property is False, the associated cost has not met the required eligibility for the credit or the service purchased is not eligible for partner earned credit.</span></span>

>[!NOTE] 
><span data-ttu-id="2ebcc-148">Obvykle se používání služeb v **cost management** zobrazuje za 8-24 hodin a KREDITy pec se zobrazí během 48 hodin od doby přístupu v Azure cost management.</span><span class="sxs-lookup"><span data-stu-id="2ebcc-148">Typically, usage for services takes 8-24 hours to appear in **Cost Management** and the PEC credits will appear within 48 hours from time of access in Azure Cost Management.</span></span>

5. <span data-ttu-id="2ebcc-149">Můžete také seskupit podle a filtrovat pomocí vlastnosti **PartnerEarnedCreditApplied** pomocí **Group by a přidat** funkce filtru pro přechod k podrobnostem o nákladech, které mají pec a náklady bez použití primárního řadiče PEC.</span><span class="sxs-lookup"><span data-stu-id="2ebcc-149">You can also group by, and filter by, the **PartnerEarnedCreditApplied** property using the **Group by and Add** filter features to drill into costs that have PEC and the costs that have no PEC applied.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2ebcc-150">Další kroky</span><span class="sxs-lookup"><span data-stu-id="2ebcc-150">Next steps</span></span>

- [<span data-ttu-id="2ebcc-151">Získaný kredit partnerů – přehled</span><span class="sxs-lookup"><span data-stu-id="2ebcc-151">Partner earned credit - overview</span></span>](partner-earned-credit.md)

- <span data-ttu-id="2ebcc-152">Podrobné příklady výpočtů vydaných kreditů pro partnery jsou umístěné na ceníku, ke kterému se můžete dostat prostřednictvím řídicího panelu partnerského centra (vyžaduje se přihlášení).</span><span class="sxs-lookup"><span data-stu-id="2ebcc-152">Detailed examples of partner earned credit calculations are located on the price list which you can reach through the Partner Center dashboard (sign-in required).</span></span>

- [<span data-ttu-id="2ebcc-153">Přejít na Azure Plan – Začínáme</span><span class="sxs-lookup"><span data-stu-id="2ebcc-153">Move to Azure plan - get started</span></span>](azure-plan-get-started.md)

- [<span data-ttu-id="2ebcc-154">Správa předplatných a prostředků v rámci plánu Azure</span><span class="sxs-lookup"><span data-stu-id="2ebcc-154">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="2ebcc-155">Odvolat nebo znovu nastavovat oprávnění správce pro předplatná Azure CSP</span><span class="sxs-lookup"><span data-stu-id="2ebcc-155">Revoke or re-instate admin privileges for Azure CSP subscriptions</span></span>](revoke-reinstate-csp.md)
