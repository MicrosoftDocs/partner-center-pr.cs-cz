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
ms.openlocfilehash: 022e7aabd0d850660f8236dce9a4fab9069af01b
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/31/2021
ms.locfileid: "106087123"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a><span data-ttu-id="fe7b1-103">Principy výpočtu a vyplácení kreditu získaného partnerem</span><span class="sxs-lookup"><span data-stu-id="fe7b1-103">How the partner earned credit is calculated and paid</span></span>

<span data-ttu-id="fe7b1-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="fe7b1-104">**Appropriate roles**</span></span>

- <span data-ttu-id="fe7b1-105">Globální správce</span><span class="sxs-lookup"><span data-stu-id="fe7b1-105">Global admin</span></span>
- <span data-ttu-id="fe7b1-106">Správce správy uživatelů</span><span class="sxs-lookup"><span data-stu-id="fe7b1-106">User management admin</span></span>
- <span data-ttu-id="fe7b1-107">Agent správce</span><span class="sxs-lookup"><span data-stu-id="fe7b1-107">Admin agent</span></span>
- <span data-ttu-id="fe7b1-108">Správce fakturace</span><span class="sxs-lookup"><span data-stu-id="fe7b1-108">Billing admin</span></span>
- <span data-ttu-id="fe7b1-109">Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="fe7b1-109">Sales agent</span></span>

<span data-ttu-id="fe7b1-110">Získaný kredit partnerů pro spravované služby (PEC) rozpoznává a vyměňuje partnery, kteří mají nepřetržitou provozní kontrolu a správu částí, nebo celé prostředí Azure svých zákazníků.</span><span class="sxs-lookup"><span data-stu-id="fe7b1-110">Partner earned credit for managed services (PEC) recognizes and rewards partners that own the 24x7 IT operational control and management of parts of, or the entire, Azure environment of their customers.</span></span> <span data-ttu-id="fe7b1-111">Ve výchozím nastavení je ve zprostředkovateli CSP udělena potřebná přístupová práva k předplatnému zákazníka, což jim umožňuje provádět 24 × 7 provozní správu a kontrolu nad prostředky v rámci předplatného.</span><span class="sxs-lookup"><span data-stu-id="fe7b1-111">By default, in CSP, partners are granted the necessary access rights to the customer's subscription allowing them to perform 24 X 7 operational management and control of the resources on the subscription.</span></span> <span data-ttu-id="fe7b1-112">Další způsoby, jak můžou zákazníci zřídit přístup k transakčním partnerům, jsou popsány v následující části.</span><span class="sxs-lookup"><span data-stu-id="fe7b1-112">Other ways in which customers can provision access for transacting partners is described in the following section.</span></span> <span data-ttu-id="fe7b1-113">Částka měsíční faktury je netto kredit získaný prostřednictvím partnerského serveru.</span><span class="sxs-lookup"><span data-stu-id="fe7b1-113">The monthly invoice amount is the net of the partner earned credit.</span></span> <span data-ttu-id="fe7b1-114">Partneři můžou zobrazit podrobnosti o řadiči PEC na jejich měsíčním souboru rekognoskaci.</span><span class="sxs-lookup"><span data-stu-id="fe7b1-114">Partners can see the PEC details on their monthly recon file.</span></span> <span data-ttu-id="fe7b1-115">Další způsoby, jak může zákazník zřídit přístup pro transakčního partnera, najdete [v článku Správa předplatných a prostředků v plánu Azure](azure-plan-manage.md).</span><span class="sxs-lookup"><span data-stu-id="fe7b1-115">For additional ways in which a customer can provision access for the transacting partner, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="fe7b1-116">Také číst [obnovit oprávnění správce pro předplatná Azure CSP](revoke-reinstate-csp.md)</span><span class="sxs-lookup"><span data-stu-id="fe7b1-116">Also read [Reinstate admin privileges for Azure CSP subscriptions](revoke-reinstate-csp.md)</span></span>

## <a name="eligibility"></a><span data-ttu-id="fe7b1-117">Vznik</span><span class="sxs-lookup"><span data-stu-id="fe7b1-117">Eligibility</span></span>

<span data-ttu-id="fe7b1-118">Pro získání partnerského kreditu pro partnery (PEC) platí následující požadavky:</span><span class="sxs-lookup"><span data-stu-id="fe7b1-118">In order to receive the partner earned credit (PEC), the following requirements apply:</span></span> 

- <span data-ttu-id="fe7b1-119">Pro získání realizovaného kreditu za prostředky Azure, které spravujete, musíte mít aktivní smlouvu MPN a platnou roli řízení přístupu na základě role (RBAC).</span><span class="sxs-lookup"><span data-stu-id="fe7b1-119">You must have an active MPN agreement and valid role-based access control (RBAC) role to receive earned credit for the Azure assets you manage.</span></span>

- <span data-ttu-id="fe7b1-120">Musíte mít nepřetržitou provozní kontrolu a správu prostředků Azure zákazníka v CSP.</span><span class="sxs-lookup"><span data-stu-id="fe7b1-120">You must have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span> <span data-ttu-id="fe7b1-121">To znamená, že musíte mít oprávnění správce v předplatném Azure zákazníka, skupině prostředků Azure a prostředku Azure.</span><span class="sxs-lookup"><span data-stu-id="fe7b1-121">This means you must have admin privileges on the customer’s Azure subscription, Azure resource group, Azure resource.</span></span> <span data-ttu-id="fe7b1-122">V případě nepřímých zprostředkovatelů a jejich nepřímých prodejců budou mít nepřímý poskytovatel nárok na PEC, pokud je tento operační řízení buď nepřímým poskytovatelem, nebo nepřímým prodejcem.</span><span class="sxs-lookup"><span data-stu-id="fe7b1-122">In the case of indirect providers and their indirect resellers, the indirect provider will be eligible for PEC if either the indirect provider or the indirect reseller or both have this operational control.</span></span> <span data-ttu-id="fe7b1-123">Další informace najdete v tématu obnovení [oprávnění správce pro odběry CSP Azure](./revoke-reinstate-csp.md).</span><span class="sxs-lookup"><span data-stu-id="fe7b1-123">To learn more about this, see [Reinstate admin privileges for Azure CSP subscriptions](./revoke-reinstate-csp.md).</span></span>

- <span data-ttu-id="fe7b1-124">Kromě výše uvedených požadavků platí, že PEC se dá použít jenom pro služby uvedené v cenách Azure Plan spotřebování, které můžete exportovat na stránce s [cenami plánu Azure](https://partner.microsoft.com/commerce/sales) .</span><span class="sxs-lookup"><span data-stu-id="fe7b1-124">In addition to the requirements above, PEC is only applicable to services listed in the Azure plan consumption pricing, which you can export from the [Azure plan pricing](https://partner.microsoft.com/commerce/sales) page.</span></span>

- <span data-ttu-id="fe7b1-125">PEC se **nevztahuje** na tyto služby:</span><span class="sxs-lookup"><span data-stu-id="fe7b1-125">PEC is **not** applicable to the following services:</span></span>
    - <span data-ttu-id="fe7b1-126">Rezervace plánu Azure</span><span class="sxs-lookup"><span data-stu-id="fe7b1-126">Azure Plan reservations</span></span>
    - <span data-ttu-id="fe7b1-127">Produkty třetích stran identifikované jako třetí strana ve sloupci značky ceny spotřeby plánu Azure</span><span class="sxs-lookup"><span data-stu-id="fe7b1-127">Third-party products identified as Third Party in the Tags column of the Azure plan consumption price</span></span>
    - <span data-ttu-id="fe7b1-128">Produkty v ceníku webu Marketplace</span><span class="sxs-lookup"><span data-stu-id="fe7b1-128">Products in the Marketplace price list</span></span>
    - [<span data-ttu-id="fe7b1-129">Virtual Machines na místě Azure</span><span class="sxs-lookup"><span data-stu-id="fe7b1-129">Azure Spot Virtual Machines</span></span>](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- <span data-ttu-id="fe7b1-130">Řadič PEC se získal na úrovni prostředků Azure.</span><span class="sxs-lookup"><span data-stu-id="fe7b1-130">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="fe7b1-131">Pokud máte platný přístup buď na úrovni předplatného nebo skupiny prostředků, bude každý prostředek, který se zahrne do vyšší entity, získat PEC.</span><span class="sxs-lookup"><span data-stu-id="fe7b1-131">If you have valid access at either the subscription or resource group level, each resource that rolls up to the higher entity will earn PEC.</span></span>

- <span data-ttu-id="fe7b1-132">Podrobnosti o řadičích PEC jsou k dispozici také na stránce [Azure cost management](/azure/cost-management-billing/costs/get-started-partners) .</span><span class="sxs-lookup"><span data-stu-id="fe7b1-132">Details on PEC are also available on the [Azure Cost management](/azure/cost-management-billing/costs/get-started-partners) page.</span></span>

### <a name="calculation"></a><span data-ttu-id="fe7b1-133">Výpočet</span><span class="sxs-lookup"><span data-stu-id="fe7b1-133">Calculation</span></span>

<span data-ttu-id="fe7b1-134">PEC se počítá denně a je možné ji zobrazit v souboru denního využití a v souboru rekognoskaci pro měsíční fakturu.</span><span class="sxs-lookup"><span data-stu-id="fe7b1-134">PEC is calculated daily and can be viewed in the daily usage file and monthly invoice recon file.</span></span> <span data-ttu-id="fe7b1-135">Partner (nepřímý poskytovatel nebo nepřímý prodejce) musí mít přístup k celému dni (nepřetržitě), aby mohl získat PEC.</span><span class="sxs-lookup"><span data-stu-id="fe7b1-135">A partner (indirect provider or indirect reseller) must have access for the entire day (24x7) to ensure they earn PEC.</span></span> <span data-ttu-id="fe7b1-136">Na spravovaných prostředcích Azure se každý den počítá PEC.</span><span class="sxs-lookup"><span data-stu-id="fe7b1-136">PEC is calculated on a daily basis on the managed Azure assets.</span></span> <span data-ttu-id="fe7b1-137">Partneři uchovávají trvalý privilegovaný přístup v průběhu měsíce (rozsah přístupu) a u všech oprávněných prostředků (rozsah přístupu) získají úplný řadič PEC.</span><span class="sxs-lookup"><span data-stu-id="fe7b1-137">Partners retaining persistent privileged access through the month (span of access) and for all the eligible resources (scope of access) will earn full PEC.</span></span> <span data-ttu-id="fe7b1-138">Snížení rozsahu a rozpětí rozpětí bude mít za měsíc nižší sazbu PEC.</span><span class="sxs-lookup"><span data-stu-id="fe7b1-138">Scope and span reduction will result in lower PEC rate for the month.</span></span> <span data-ttu-id="fe7b1-139">Denní hodnocený soubor využití se denně zobrazuje na základě prostředku Azure, ať už se používá nebo ne.</span><span class="sxs-lookup"><span data-stu-id="fe7b1-139">Daily rated usage file shows on a daily basis on an Azure asset, whether PEC is applied or not.</span></span> <span data-ttu-id="fe7b1-140">Partneři taky můžou zaregistrovat výstrahy a monitorovat změny trvalého privilegovaného přístupu.</span><span class="sxs-lookup"><span data-stu-id="fe7b1-140">Partners can also enroll in alerts to monitor changes to persistent privileged access.</span></span>

## <a name="azure-cost-management"></a><span data-ttu-id="fe7b1-141">Správa nákladů v Azure</span><span class="sxs-lookup"><span data-stu-id="fe7b1-141">Azure Cost Management</span></span>

<span data-ttu-id="fe7b1-142">Azure Cost Management (ACM) s využitím analýzy nákladů umožňuje jako partnera zobrazit náklady, které dostaly výhody PEC.</span><span class="sxs-lookup"><span data-stu-id="fe7b1-142">Azure Cost Management (ACM) using Cost Analysis enables you as a partner to view the costs that have received the benefit of PEC.</span></span>  

1. <span data-ttu-id="fe7b1-143">V [Azure Portal](https://portal.azure.com)se přihlaste ke svému partnerskému tenantovi a vyberte **cost management + fakturace**.</span><span class="sxs-lookup"><span data-stu-id="fe7b1-143">In the [Azure portal](https://portal.azure.com), sign into your partner tenant and select **Cost Management + Billing**.</span></span>

2. <span data-ttu-id="fe7b1-144">Vybrat **správu nákladů**</span><span class="sxs-lookup"><span data-stu-id="fe7b1-144">Select **Cost management**</span></span>

3. <span data-ttu-id="fe7b1-145">Vybrat **analýzu nákladů**</span><span class="sxs-lookup"><span data-stu-id="fe7b1-145">Select **Cost Analysis**</span></span>

   <span data-ttu-id="fe7b1-146">V zobrazení analýza nákladů se zobrazí náklady na fakturační účet pro všechny služby zakoupené a spotřebované v cenách, které platíte společnosti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="fe7b1-146">The Cost Analysis view will display the costs for your billing account, for all the services purchased and consumed at the prices that you pay Microsoft.</span></span>

4. <span data-ttu-id="fe7b1-147">V rozevíracím seznamu v kontingenčním grafu vyberte **PartnerEarnedCreditApplied** , aby se zobrazily náklady s použitím pec.</span><span class="sxs-lookup"><span data-stu-id="fe7b1-147">Select **PartnerEarnedCreditApplied** in the drop-down list on a pivot chart to see costs that have PEC applied.</span></span> <span data-ttu-id="fe7b1-148">Pokud má vlastnost **PartnerEarnedCreditApplied** hodnotu true, mají přidružené náklady nárok na zvýhodněný kredit získaný partnerem.</span><span class="sxs-lookup"><span data-stu-id="fe7b1-148">When **PartnerEarnedCreditApplied** property is True, the associated cost has the benefit of the partner earned credit.</span></span> 

   <span data-ttu-id="fe7b1-149">Pokud má vlastnost PartnerEarnedCreditApplied hodnotu false, přidružené náklady nevyhověly požadovanému nároku na kredit nebo zakoupená služba nemá nárok na kredit získaný partnerem.</span><span class="sxs-lookup"><span data-stu-id="fe7b1-149">When the PartnerEarnedCreditApplied property is False, the associated cost has not met the required eligibility for the credit or the service purchased is not eligible for partner earned credit.</span></span>

   >[!NOTE] 
   ><span data-ttu-id="fe7b1-150">Obvykle se používání služeb v **cost management** zobrazuje za 8-24 hodin a KREDITy pec se zobrazí během 48 hodin od doby přístupu v Azure cost management.</span><span class="sxs-lookup"><span data-stu-id="fe7b1-150">Typically, usage for services takes 8-24 hours to appear in **Cost Management** and the PEC credits will appear within 48 hours from time of access in Azure Cost Management.</span></span>

5. <span data-ttu-id="fe7b1-151">Můžete také seskupit podle a filtrovat pomocí vlastnosti **PartnerEarnedCreditApplied** pomocí **Group by a přidat** funkce filtru pro přechod k podrobnostem o nákladech, které mají pec a náklady bez použití primárního řadiče PEC.</span><span class="sxs-lookup"><span data-stu-id="fe7b1-151">You can also group by, and filter by, the **PartnerEarnedCreditApplied** property using the **Group by and Add** filter features to drill into costs that have PEC and the costs that have no PEC applied.</span></span>

## <a name="next-steps"></a><span data-ttu-id="fe7b1-152">Další kroky</span><span class="sxs-lookup"><span data-stu-id="fe7b1-152">Next steps</span></span>

- [<span data-ttu-id="fe7b1-153">Získaný kredit partnerů – přehled</span><span class="sxs-lookup"><span data-stu-id="fe7b1-153">Partner earned credit - overview</span></span>](partner-earned-credit.md)

- <span data-ttu-id="fe7b1-154">Podrobné příklady výpočtů vydaných kreditů partnerů najdete v ceníku, ke kterému se můžete dostat prostřednictvím řídicího panelu partnerského centra (vyžaduje se přihlášení).</span><span class="sxs-lookup"><span data-stu-id="fe7b1-154">Detailed examples of partner earned credit calculations are located on the price list that you can reach through the Partner Center dashboard (sign in required).</span></span>

- [<span data-ttu-id="fe7b1-155">Přejít na Azure Plan – Začínáme</span><span class="sxs-lookup"><span data-stu-id="fe7b1-155">Move to Azure plan - get started</span></span>](azure-plan-get-started.md)

- [<span data-ttu-id="fe7b1-156">Správa předplatných a prostředků v rámci plánu Azure</span><span class="sxs-lookup"><span data-stu-id="fe7b1-156">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="fe7b1-157">Odvolat nebo obnovit oprávnění správce pro předplatná Azure CSP</span><span class="sxs-lookup"><span data-stu-id="fe7b1-157">Revoke or reinstate admin privileges for Azure CSP subscriptions</span></span>](revoke-reinstate-csp.md)
