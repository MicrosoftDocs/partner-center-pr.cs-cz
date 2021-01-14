---
title: Získaný kredit partnerů pro spravované služby
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Seznamte se s tím, jak se počítá a hradí Microsoft partnerd Credit (PEC) pro spravované služby a jak zajistit, abyste měli nárok na to.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f274103feeadfa6fd135f99632f3013c29601972
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182405"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a><span data-ttu-id="1a763-103">Principy výpočtu a vyplácení kreditu získaného partnerem</span><span class="sxs-lookup"><span data-stu-id="1a763-103">How the partner earned credit is calculated and paid</span></span>

<span data-ttu-id="1a763-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="1a763-104">**Appropriate roles**</span></span>

- <span data-ttu-id="1a763-105">Globální správce</span><span class="sxs-lookup"><span data-stu-id="1a763-105">Global admin</span></span>
- <span data-ttu-id="1a763-106">Správce uživatelů</span><span class="sxs-lookup"><span data-stu-id="1a763-106">User admin</span></span>
- <span data-ttu-id="1a763-107">Agent správce</span><span class="sxs-lookup"><span data-stu-id="1a763-107">Admin agent</span></span>
- <span data-ttu-id="1a763-108">Správce fakturace</span><span class="sxs-lookup"><span data-stu-id="1a763-108">Billing admin</span></span>
- <span data-ttu-id="1a763-109">Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="1a763-109">Sales agent</span></span>

<span data-ttu-id="1a763-110">Získaný kredit partnerů pro spravované služby (PEC) rozpoznává a vyměňuje partnery, kteří mají nepřetržitou provozní kontrolu a správu částí, nebo celé prostředí Azure svých zákazníků.</span><span class="sxs-lookup"><span data-stu-id="1a763-110">Partner earned credit for managed services (PEC) recognizes and rewards partners that own the 24x7 IT operational control and management of parts of, or the entire, Azure environment of their customers.</span></span> <span data-ttu-id="1a763-111">Ve výchozím nastavení je ve zprostředkovateli CSP udělena potřebná přístupová práva k předplatnému zákazníka, což jim umožňuje provádět 24 × 7 provozní správu a kontrolu nad prostředky v rámci předplatného.</span><span class="sxs-lookup"><span data-stu-id="1a763-111">By default, in CSP, partners are granted the necessary access rights to the customer's subscription allowing them to perform 24 X 7 operational management and control of the resources on the subscription.</span></span> <span data-ttu-id="1a763-112">Další způsoby, jak zákazník může zřídit přístup pro transakčního partnera, je popsaný v následující části.</span><span class="sxs-lookup"><span data-stu-id="1a763-112">Additional ways in which customer can provision access for transacting partner is described in the following section.</span></span> <span data-ttu-id="1a763-113">Měsíční fakturovaná částka nezahrnuje kredit získaný partnerem.</span><span class="sxs-lookup"><span data-stu-id="1a763-113">The monthly invoice amount is net of partner earned credit.</span></span> <span data-ttu-id="1a763-114">Partneři můžou zobrazit podrobnosti o řadiči PEC na jejich měsíčním souboru rekognoskaci.</span><span class="sxs-lookup"><span data-stu-id="1a763-114">Partners can see the PEC details on their monthly recon file.</span></span> <span data-ttu-id="1a763-115">Další způsoby, jak může zákazník zřídit přístup pro transakčního partnera, najdete [v článku Správa předplatných a prostředků v plánu Azure](azure-plan-manage.md).</span><span class="sxs-lookup"><span data-stu-id="1a763-115">For additional ways in which a customer can provision access for the transacting partner, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="1a763-116">Také číst [obnovit oprávnění správce pro předplatná Azure CSP](revoke-reinstate-csp.md)</span><span class="sxs-lookup"><span data-stu-id="1a763-116">Also read [Reinstate admin privileges for Azure CSP subscriptions](revoke-reinstate-csp.md)</span></span>

## <a name="eligibility"></a><span data-ttu-id="1a763-117">Vznik</span><span class="sxs-lookup"><span data-stu-id="1a763-117">Eligibility</span></span>

<span data-ttu-id="1a763-118">Pro získání partnerského kreditu pro partnery (PEC) platí následující požadavky:</span><span class="sxs-lookup"><span data-stu-id="1a763-118">In order to receive the partner earned credit (PEC), the following requirements apply:</span></span> 

- <span data-ttu-id="1a763-119">Pro získání realizovaného kreditu za prostředky Azure, které spravujete, musíte mít aktivní smlouvu MPN a platnou roli řízení přístupu na základě role (RBAC).</span><span class="sxs-lookup"><span data-stu-id="1a763-119">You must have an active MPN agreement and valid role-based access control (RBAC) role to receive earned credit for the Azure assets you manage.</span></span>

- <span data-ttu-id="1a763-120">Musíte mít nepřetržitou provozní kontrolu a správu prostředků Azure zákazníka v CSP.</span><span class="sxs-lookup"><span data-stu-id="1a763-120">You must have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span> <span data-ttu-id="1a763-121">To znamená, že musíte mít oprávnění správce v předplatném Azure zákazníka, skupině prostředků Azure a prostředku Azure.</span><span class="sxs-lookup"><span data-stu-id="1a763-121">This means you must have admin privileges on the customer’s Azure subscription, Azure resource group, Azure resource.</span></span> <span data-ttu-id="1a763-122">V případě nepřímých zprostředkovatelů a jejich nepřímých prodejců budou mít nepřímý poskytovatel nárok na PEC, pokud je tento operační řízení buď nepřímým poskytovatelem, nebo nepřímým prodejcem.</span><span class="sxs-lookup"><span data-stu-id="1a763-122">In the case of indirect providers and their indirect resellers, the indirect provider will be eligible for PEC if either the indirect provider or the indirect reseller or both have this operational control.</span></span> <span data-ttu-id="1a763-123">Další informace najdete v tématu obnovení [oprávnění správce pro odběry CSP Azure](./revoke-reinstate-csp.md).</span><span class="sxs-lookup"><span data-stu-id="1a763-123">To learn more about this, see [Reinstate admin privileges for Azure CSP subscriptions](./revoke-reinstate-csp.md).</span></span>

- <span data-ttu-id="1a763-124">Kromě výše uvedených požadavků platí, že PEC se dá použít jenom pro služby uvedené v cenách Azure Plan spotřebování, které můžete exportovat na stránce s [cenami plánu Azure](https://partner.microsoft.com/commerce/sales) .</span><span class="sxs-lookup"><span data-stu-id="1a763-124">In addition to the requirements above, PEC is only applicable to services listed in the Azure plan consumption pricing, which you can export from the [Azure plan pricing](https://partner.microsoft.com/commerce/sales) page.</span></span>

- <span data-ttu-id="1a763-125">PEC se **nevztahuje** na tyto služby:</span><span class="sxs-lookup"><span data-stu-id="1a763-125">PEC is **not** applicable to the following services:</span></span>
    - <span data-ttu-id="1a763-126">Rezervace plánu Azure</span><span class="sxs-lookup"><span data-stu-id="1a763-126">Azure Plan reservations</span></span>
    - <span data-ttu-id="1a763-127">Produkty třetích stran identifikované jako třetí strana ve sloupci značky ceny spotřeby plánu Azure</span><span class="sxs-lookup"><span data-stu-id="1a763-127">Third-party products identified as Third Party in the Tags column of the Azure plan consumption price</span></span>
    - <span data-ttu-id="1a763-128">Produkty v ceníku webu Marketplace</span><span class="sxs-lookup"><span data-stu-id="1a763-128">Products in the Marketplace price list</span></span>
    - [<span data-ttu-id="1a763-129">Virtual Machines na místě Azure</span><span class="sxs-lookup"><span data-stu-id="1a763-129">Azure Spot Virtual Machines</span></span>](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- <span data-ttu-id="1a763-130">Řadič PEC se získal na úrovni prostředků Azure.</span><span class="sxs-lookup"><span data-stu-id="1a763-130">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="1a763-131">Pokud máte platný přístup buď na úrovni předplatného nebo skupiny prostředků, bude každý prostředek, který se zahrne do vyšší entity, získat PEC.</span><span class="sxs-lookup"><span data-stu-id="1a763-131">If you have valid access at either the subscription or resource group level, each resource that rolls up to the higher entity will earn PEC.</span></span>

- <span data-ttu-id="1a763-132">Podrobnosti o řadičích PEC jsou k dispozici také na stránce [Azure cost management](/azure/cost-management-billing/costs/get-started-partners) .</span><span class="sxs-lookup"><span data-stu-id="1a763-132">Details on PEC are also available on the [Azure Cost management](/azure/cost-management-billing/costs/get-started-partners) page.</span></span>

### <a name="calculation"></a><span data-ttu-id="1a763-133">Výpočet</span><span class="sxs-lookup"><span data-stu-id="1a763-133">Calculation</span></span>

<span data-ttu-id="1a763-134">PEC se počítá denně a je možné ji zobrazit v souboru denního využití a v souboru rekognoskaci pro měsíční fakturu.</span><span class="sxs-lookup"><span data-stu-id="1a763-134">PEC is calculated daily and can be viewed in the daily usage file and monthly invoice recon file.</span></span> <span data-ttu-id="1a763-135">Partner (nepřímý poskytovatel nebo nepřímý prodejce) musí mít přístup k celému dni (nepřetržitě), aby mohl získat PEC.</span><span class="sxs-lookup"><span data-stu-id="1a763-135">A partner (indirect provider or indirect reseller) must have access for the entire day (24x7) to ensure they earn PEC.</span></span> <span data-ttu-id="1a763-136">Na spravovaných prostředcích Azure se každý den počítá PEC.</span><span class="sxs-lookup"><span data-stu-id="1a763-136">PEC is calculated on a daily basis on the managed Azure assets.</span></span> <span data-ttu-id="1a763-137">Maximální počet řadičů PEC pro dané fakturační období (měsíc) je 15%.</span><span class="sxs-lookup"><span data-stu-id="1a763-137">The maximum PEC for a given billing period (Month) is 15%.</span></span> <span data-ttu-id="1a763-138">Partneři uchovávají trvalý privilegovaný přístup v průběhu měsíce (rozsah přístupu) a u všech oprávněných prostředků (rozsah přístupu) získají úplné PEC o 15%.</span><span class="sxs-lookup"><span data-stu-id="1a763-138">Partners retaining persistent privileged access through the month (span of access) and for all the eligible resources (scope of access) will earn full PEC of 15%.</span></span> <span data-ttu-id="1a763-139">Snížení rozsahu a rozpětí rozpětí bude mít za měsíc nižší sazbu PEC.</span><span class="sxs-lookup"><span data-stu-id="1a763-139">Scope and span reduction will result in lower PEC rate for the month.</span></span> <span data-ttu-id="1a763-140">Denní hodnocený soubor využití se denně zobrazuje na základě prostředku Azure, ať už se používá nebo ne.</span><span class="sxs-lookup"><span data-stu-id="1a763-140">Daily rated usage file shows on a daily basis on an Azure asset, whether PEC is applied or not.</span></span> <span data-ttu-id="1a763-141">Partneři taky můžou zaregistrovat výstrahy a monitorovat změny trvalého privilegovaného přístupu.</span><span class="sxs-lookup"><span data-stu-id="1a763-141">Partners can also enroll in alerts to monitor changes to persistent privileged access.</span></span>

## <a name="azure-cost-management"></a><span data-ttu-id="1a763-142">Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="1a763-142">Azure Cost Management</span></span>

<span data-ttu-id="1a763-143">Azure Cost Management (ACM) s využitím analýzy nákladů umožňuje jako partnera zobrazit náklady, které dostaly výhody PEC.</span><span class="sxs-lookup"><span data-stu-id="1a763-143">Azure Cost Management (ACM) using Cost Analysis enables you as a partner to view the costs that have received the benefit of PEC.</span></span>  

1. <span data-ttu-id="1a763-144">V [Azure Portal](https://portal.azure.com)se přihlaste ke svému partnerskému tenantovi a vyberte **cost management + fakturace**.</span><span class="sxs-lookup"><span data-stu-id="1a763-144">In the [Azure portal](https://portal.azure.com), sign into your partner tenant and select **Cost Management + Billing**.</span></span>

2. <span data-ttu-id="1a763-145">Vybrat **správu nákladů**</span><span class="sxs-lookup"><span data-stu-id="1a763-145">Select **Cost management**</span></span>

3. <span data-ttu-id="1a763-146">Vybrat **analýzu nákladů**</span><span class="sxs-lookup"><span data-stu-id="1a763-146">Select **Cost Analysis**</span></span>

   <span data-ttu-id="1a763-147">V zobrazení analýza nákladů se zobrazí náklady na fakturační účet pro všechny služby zakoupené a spotřebované v cenách, které platíte společnosti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1a763-147">The Cost Analysis view will display the costs for your billing account, for all the services purchased and consumed at the prices that you pay Microsoft.</span></span>

4. <span data-ttu-id="1a763-148">V rozevíracím seznamu v rozevíracím grafu vyberte **PartnerEarnedCreditApplied** , aby se zobrazily náklady s použitím pec.</span><span class="sxs-lookup"><span data-stu-id="1a763-148">Select **PartnerEarnedCreditApplied** in the drop down on a pivot chart to see costs that have PEC applied.</span></span> <span data-ttu-id="1a763-149">Pokud má vlastnost **PartnerEarnedCreditApplied** hodnotu true, mají přidružené náklady nárok na zvýhodněný kredit získaný partnerem.</span><span class="sxs-lookup"><span data-stu-id="1a763-149">When **PartnerEarnedCreditApplied** property is True, the associated cost has the benefit of the partner earned credit.</span></span> 

   <span data-ttu-id="1a763-150">Pokud má vlastnost PartnerEarnedCreditApplied hodnotu false, přidružené náklady nevyhověly požadovanému nároku na kredit nebo zakoupená služba nemá nárok na kredit získaný partnerem.</span><span class="sxs-lookup"><span data-stu-id="1a763-150">When the PartnerEarnedCreditApplied property is False, the associated cost has not met the required eligibility for the credit or the service purchased is not eligible for partner earned credit.</span></span>

   >[!NOTE] 
   ><span data-ttu-id="1a763-151">Obvykle se používání služeb v **cost management** zobrazuje za 8-24 hodin a KREDITy pec se zobrazí během 48 hodin od doby přístupu v Azure cost management.</span><span class="sxs-lookup"><span data-stu-id="1a763-151">Typically, usage for services takes 8-24 hours to appear in **Cost Management** and the PEC credits will appear within 48 hours from time of access in Azure Cost Management.</span></span>

5. <span data-ttu-id="1a763-152">Můžete také seskupit podle a filtrovat pomocí vlastnosti **PartnerEarnedCreditApplied** pomocí **Group by a přidat** funkce filtru pro přechod k podrobnostem o nákladech, které mají pec a náklady bez použití primárního řadiče PEC.</span><span class="sxs-lookup"><span data-stu-id="1a763-152">You can also group by, and filter by, the **PartnerEarnedCreditApplied** property using the **Group by and Add** filter features to drill into costs that have PEC and the costs that have no PEC applied.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1a763-153">Další kroky</span><span class="sxs-lookup"><span data-stu-id="1a763-153">Next steps</span></span>

- [<span data-ttu-id="1a763-154">Získaný kredit partnerů – přehled</span><span class="sxs-lookup"><span data-stu-id="1a763-154">Partner earned credit - overview</span></span>](partner-earned-credit.md)

- <span data-ttu-id="1a763-155">Podrobné příklady výpočtů vydaných kreditů pro partnery jsou umístěné na ceníku, ke kterému se můžete dostat prostřednictvím řídicího panelu partnerského centra (vyžaduje se přihlášení).</span><span class="sxs-lookup"><span data-stu-id="1a763-155">Detailed examples of partner earned credit calculations are located on the price list which you can reach through the Partner Center dashboard (sign-in required).</span></span>

- [<span data-ttu-id="1a763-156">Přejít na Azure Plan – Začínáme</span><span class="sxs-lookup"><span data-stu-id="1a763-156">Move to Azure plan - get started</span></span>](azure-plan-get-started.md)

- [<span data-ttu-id="1a763-157">Správa předplatných a prostředků v rámci plánu Azure</span><span class="sxs-lookup"><span data-stu-id="1a763-157">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="1a763-158">Odvolat nebo znovu nastavovat oprávnění správce pro předplatná Azure CSP</span><span class="sxs-lookup"><span data-stu-id="1a763-158">Revoke or re-instate admin privileges for Azure CSP subscriptions</span></span>](revoke-reinstate-csp.md)