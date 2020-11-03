---
title: Nastavení velikosti virtuálního počítače Azure, která maximálně využívá rezervace
description: Naučte se, jak velikost virtuálního počítače (VM) nastavit na výpočetní požadavky vašich zákazníků při nákupu Microsoft Azure rezervacích.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: e6c4e3e7a68de720f586754703308a447d7d30c1
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/22/2020
ms.locfileid: "92527338"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="e12dc-103">Nastavení velikosti virtuálního počítače Microsoft Azure, která maximálně využívá rezervaci</span><span class="sxs-lookup"><span data-stu-id="e12dc-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="e12dc-104">**Platí pro**</span><span class="sxs-lookup"><span data-stu-id="e12dc-104">**Applies to**</span></span>

- <span data-ttu-id="e12dc-105">Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="e12dc-105">Partner Center</span></span>
- <span data-ttu-id="e12dc-106">portál Azure</span><span class="sxs-lookup"><span data-stu-id="e12dc-106">Azure portal</span></span>
- <span data-ttu-id="e12dc-107">Partneři v programu CSP</span><span class="sxs-lookup"><span data-stu-id="e12dc-107">Partners in the CSP program</span></span>
 
> [!NOTE]
> <span data-ttu-id="e12dc-108">Tento článek se týká jenom partnerů v programu Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="e12dc-108">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="e12dc-109">[Tuto dokumentaci k rezervacím Azure](/azure/cost-management-billing/reservations)by si měli přečíst zákazníci, kteří používají jiné typy předplatných (například, platby na základě průběžných plateb, jednotlivce, smlouvy o zákaznících Microsoftu nebo předplatná smlouva Enterprise).</span><span class="sxs-lookup"><span data-stu-id="e12dc-109">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="e12dc-110">Určení velikosti virtuálního počítače pro rezervaci Azure zákazníka</span><span class="sxs-lookup"><span data-stu-id="e12dc-110">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="e12dc-111">Při nákupu Microsoft Azure rezervacích jménem vašich zákazníků budete muset vybrat velikost virtuálního počítače, aby splňovala výpočetní požadavky zákazníka.</span><span class="sxs-lookup"><span data-stu-id="e12dc-111">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="e12dc-112">Tyto informace můžete najít pomocí jedné z těchto metod:</span><span class="sxs-lookup"><span data-stu-id="e12dc-112">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="e12dc-113">Rozhraní API využití Azure</span><span class="sxs-lookup"><span data-stu-id="e12dc-113">Azure utilization API</span></span>
- <span data-ttu-id="e12dc-114">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="e12dc-114">The Azure portal</span></span>
- <span data-ttu-id="e12dc-115">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="e12dc-115">Azure PowerShell</span></span>
- <span data-ttu-id="e12dc-116">Rozhraní API pro Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="e12dc-116">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="e12dc-117">Pokyny k používání každé z těchto metod jsou uvedeny níže.</span><span class="sxs-lookup"><span data-stu-id="e12dc-117">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="e12dc-118">Po zakoupení rezervované slevy se sleva pro rezervaci automaticky použije na virtuální počítače, které odpovídají atributům a množstvím rezervace.</span><span class="sxs-lookup"><span data-stu-id="e12dc-118">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="e12dc-119">Nemusíte přiřazovat rezervaci k virtuálnímu počítači.</span><span class="sxs-lookup"><span data-stu-id="e12dc-119">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="e12dc-120">Slevy za rezervace se nevztahují na klasické nebo propagační virtuální počítače.</span><span class="sxs-lookup"><span data-stu-id="e12dc-120">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="e12dc-121">Pokud chcete správně identifikovat typ a velikost virtuálního počítače, který se má koupit jménem zákazníka, musíte použít jednu z níže popsaných metod, protože typ řady virtuálních počítačů se v souborech pro odsouhlasení partnerského centra nezobrazuje správně.</span><span class="sxs-lookup"><span data-stu-id="e12dc-121">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="e12dc-122">Získání informací o velikosti virtuálních počítačů pomocí rozhraní API využití Azure</span><span class="sxs-lookup"><span data-stu-id="e12dc-122">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="e12dc-123">Použijte hodnotu pro atribut ServiceType z additionalInfo v odpovědi rozhraní API k identifikaci velikosti virtuálního počítače, který se má koupit.</span><span class="sxs-lookup"><span data-stu-id="e12dc-123">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="e12dc-124">Další informace najdete v tématu [získání záznamů o využití zákazníka pro Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) v [PARTNERSKÉM centru rozhraní API](/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="e12dc-124">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="e12dc-125">Získání informací o velikosti virtuálních počítačů pomocí portál Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="e12dc-125">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="e12dc-126">V partnerském centru přejdete na stránku **Customers** .</span><span class="sxs-lookup"><span data-stu-id="e12dc-126">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="e12dc-127">Najděte zákazníka, který chce koupit rezervace virtuálních počítačů Azure, a potom výběrem šipky dolů rozbalte informace o zákazníkovi.</span><span class="sxs-lookup"><span data-stu-id="e12dc-127">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="e12dc-128">Výběrem **portál pro správu Microsoft Azure** otevřete záznam zákazníka v Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="e12dc-128">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="e12dc-129">V nabídce portál vyberte **virtuální počítače** a potom vyberte virtuální počítač, pro který chcete zakoupit rezervaci.</span><span class="sxs-lookup"><span data-stu-id="e12dc-129">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="e12dc-130">Na stránce Podrobnosti o virtuálním počítači Najděte informace o velikosti a oblasti, jak je znázorněno níže, a tyto informace použijte k nákupu rezervace v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="e12dc-130">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="Informace o velikosti a oblasti na stránce podrobností":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="e12dc-132">Získání informací o velikosti virtuálních počítačů pomocí Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="e12dc-132">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="e12dc-133">K získání umístění a velikosti virtuálního počítače, pro který chcete zakoupit rezervaci, použijte informace na obrázku níže.</span><span class="sxs-lookup"><span data-stu-id="e12dc-133">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="Umístění a velikost virtuálního počítače":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="e12dc-135">Získání informací o velikosti virtuálních počítačů pomocí rozhraní API pro Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="e12dc-135">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="e12dc-136">Pomocí rozhraní API ARMClient nebo ARM volejte klienta ARM pro virtuální počítač, pro který chcete zakoupit rezervaci.</span><span class="sxs-lookup"><span data-stu-id="e12dc-136">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="e12dc-137">/Subscriptions/ <Subscription ID> /ResourceGroups/ <Resource group name> /providers/Microsoft.COMPUTE/virtualMachines/ <VM Instance Name> ? API-Version = 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="e12dc-137">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="e12dc-138">Volání vrátí hodnoty pro **vmSize** a **Location** , jak je znázorněno níže.</span><span class="sxs-lookup"><span data-stu-id="e12dc-138">The call returns the values for **vmSize** and **location** , as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="hodnota vmSize":::
    :::image type="content" source="images/usage4.png" alt-text="Hodnota umístění":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="e12dc-141">Ověření využití virtuálních počítačů Azure a slevy za rezervaci</span><span class="sxs-lookup"><span data-stu-id="e12dc-141">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="e12dc-142">Po zakoupení rezervované instance virtuálního počítače Azure jménem zákazníka se sleva za platbu za místo na virtuálním počítači automaticky aplikuje na virtuální počítače, které odpovídají atributům a množství rezervací zákazníka.</span><span class="sxs-lookup"><span data-stu-id="e12dc-142">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="e12dc-143">Pomocí jedné z následujících metod si můžete ověřit využití rezervace zákazníka a zjistit, na které virtuální počítače se vztahují slevy na rezervace:</span><span class="sxs-lookup"><span data-stu-id="e12dc-143">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="e12dc-144">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="e12dc-144">The Azure portal</span></span>
- <span data-ttu-id="e12dc-145">Rozhraní API využití Azure</span><span class="sxs-lookup"><span data-stu-id="e12dc-145">Azure utilization API</span></span>

<span data-ttu-id="e12dc-146">Pokyny k používání každé z těchto metod jsou uvedeny níže.</span><span class="sxs-lookup"><span data-stu-id="e12dc-146">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="e12dc-147">Jenom rozhraní API využití Azure ukazuje, na který virtuální počítač se sleva aplikuje.</span><span class="sxs-lookup"><span data-stu-id="e12dc-147">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="e12dc-148">Ověření využití rezervace zákazníka v portál Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="e12dc-148">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="e12dc-149">V partnerském centru přejdete na stránku **Customers** .</span><span class="sxs-lookup"><span data-stu-id="e12dc-149">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="e12dc-150">Vyhledejte zákazníka, jehož zlevněnou slevu a využití chcete ověřit, a potom výběrem šipky dolů rozbalte informace o zákazníkovi.</span><span class="sxs-lookup"><span data-stu-id="e12dc-150">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="e12dc-151">Výběrem **portál pro správu Microsoft Azure** otevřete záznam zákazníka v Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="e12dc-151">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="e12dc-152">V nabídce portálu vyberte možnost **rezervace** a pak vyberte rezervaci, pro kterou chcete zjistit využití.</span><span class="sxs-lookup"><span data-stu-id="e12dc-152">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="e12dc-153">Na stránce **Přehled** ověřte graf využití rezervace, který ukazuje, jak velká část rezervace byla aplikována na virtuální počítače.</span><span class="sxs-lookup"><span data-stu-id="e12dc-153">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="e12dc-154">Data o využití se můžou zpozdit až o 8 hodin.</span><span class="sxs-lookup"><span data-stu-id="e12dc-154">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="e12dc-155">a.</span><span class="sxs-lookup"><span data-stu-id="e12dc-155">a.</span></span> <span data-ttu-id="e12dc-156">Pokud je využití rezervace 100%, zákazník získá veškerou možnou úsporu, kterou může koupit rezervace.</span><span class="sxs-lookup"><span data-stu-id="e12dc-156">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="e12dc-157">b.</span><span class="sxs-lookup"><span data-stu-id="e12dc-157">b.</span></span> <span data-ttu-id="e12dc-158">Pokud je využití rezervace 0%, sleva se nepoužije na žádný virtuální počítač.</span><span class="sxs-lookup"><span data-stu-id="e12dc-158">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="e12dc-159">c.</span><span class="sxs-lookup"><span data-stu-id="e12dc-159">c.</span></span> <span data-ttu-id="e12dc-160">Pokud je využití rezervace v rozmezí od 1 do 99%, nevyužité výhody.</span><span class="sxs-lookup"><span data-stu-id="e12dc-160">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="e12dc-161">Abyste se vyhnuli této situaci, před provedením nákupu určete správnou velikost virtuálního počítače pro podporu výpočetních potřeb zákazníků.</span><span class="sxs-lookup"><span data-stu-id="e12dc-161">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="e12dc-162">Ověření využití rezervace zákazníka pomocí rozhraní API využití Azure</span><span class="sxs-lookup"><span data-stu-id="e12dc-162">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="e12dc-163">Jenom rozhraní API využití Azure ukazuje, na který virtuální počítač se sleva aplikuje.</span><span class="sxs-lookup"><span data-stu-id="e12dc-163">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="e12dc-164">Data o využití rezervace můžete získat pomocí rozhraní API využití Azure, abyste ověřili, že zákazník získává slevu za rezervaci, a zobrazí, na kterých virtuálních počítačích se sleva vztahuje.</span><span class="sxs-lookup"><span data-stu-id="e12dc-164">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="e12dc-165">Porovnejte příklad A s příkladem B, abyste viděli, jak ověřit využití rezervace zákazníka.</span><span class="sxs-lookup"><span data-stu-id="e12dc-165">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Příklady použití rezervací":::

- <span data-ttu-id="e12dc-167">ReservationId identifikuje rezervaci Azure, která se použila k uplatnění slevy na virtuální počítač.</span><span class="sxs-lookup"><span data-stu-id="e12dc-167">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="e12dc-168">consumptionMeter je MeterId pro virtuální počítač, na kterém je nastavená sleva rezervace.</span><span class="sxs-lookup"><span data-stu-id="e12dc-168">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="e12dc-169">ReservationMeter ukazuje náklady $0 od použití slevy rezervace.</span><span class="sxs-lookup"><span data-stu-id="e12dc-169">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="e12dc-170">Další informace najdete v tématu [získání záznamů o využití zákazníka pro Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) v [PARTNERSKÉM centru rozhraní API](/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="e12dc-170">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="e12dc-171">Náklady na software, jako je například Microsoft Windows Server, nejsou aktuálně zahrnuté v ceně rezervovaného virtuálního počítače a zobrazí se jako samostatné položky řádku v záznamu objednávky a na faktuře.</span><span class="sxs-lookup"><span data-stu-id="e12dc-171">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="e12dc-172">Pokud ale má zákazník zvýhodněné hybridní využití Azure, náklady na software se nepoužijí.</span><span class="sxs-lookup"><span data-stu-id="e12dc-172">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="e12dc-173">Další informace najdete v tématu [náklady na software systému Windows, které nejsou součástí rezervovaných instancí](/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="e12dc-173">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="e12dc-174">Prostředky rezervací Azure</span><span class="sxs-lookup"><span data-stu-id="e12dc-174">Azure reservations resources</span></span>

|<span data-ttu-id="e12dc-175">**Pro informace o**</span><span class="sxs-lookup"><span data-stu-id="e12dc-175">**For information about**</span></span>   |<span data-ttu-id="e12dc-176">**Přečtěte si:**</span><span class="sxs-lookup"><span data-stu-id="e12dc-176">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="e12dc-177">Přehled rezervací Azure v CSP</span><span class="sxs-lookup"><span data-stu-id="e12dc-177">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="e12dc-178">Prodej Microsoft Azure rezervovaných instancí virtuálních počítačů</span><span class="sxs-lookup"><span data-stu-id="e12dc-178">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="e12dc-179">Nákup rezervací Azure pro vaše zákazníky v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="e12dc-179">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="e12dc-180">Nákup rezervací Azure</span><span class="sxs-lookup"><span data-stu-id="e12dc-180">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="e12dc-181">Správa rezervací Azure v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="e12dc-181">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="e12dc-182">Správa rezervací Azure v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="e12dc-182">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="e12dc-183">Nákup rezervací Azure v Azure Portal</span><span class="sxs-lookup"><span data-stu-id="e12dc-183">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="e12dc-184">[Platba za virtuální počítače s Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) v nápovědě k Azure</span><span class="sxs-lookup"><span data-stu-id="e12dc-184">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="e12dc-185">Správa rezervací Azure v Azure Portal</span><span class="sxs-lookup"><span data-stu-id="e12dc-185">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="e12dc-186">[Správa rezervovaných instancí virtuálních počítačů](/azure/billing/billing-manage-reserved-vm-instance) v nápovědě k Azure</span><span class="sxs-lookup"><span data-stu-id="e12dc-186">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="e12dc-187">Nákup rezervací Azure pomocí rozhraní API partnerského centra</span><span class="sxs-lookup"><span data-stu-id="e12dc-187">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="e12dc-188">[Koupit Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) v dokumentaci pro vývojáře partnerského centra</span><span class="sxs-lookup"><span data-stu-id="e12dc-188">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="e12dc-189">Udělení oprávnění zákazníkům k nákupu svých rezervací Azure z předplatného, které pro ně jste nakoupili.</span><span class="sxs-lookup"><span data-stu-id="e12dc-189">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="e12dc-190">Poskytněte zákazníkům oprávnění k nákupu svých rezervací Azure.</span><span class="sxs-lookup"><span data-stu-id="e12dc-190">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |