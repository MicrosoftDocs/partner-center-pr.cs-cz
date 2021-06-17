---
title: Nastavení velikosti virtuálního počítače Azure, která maximálně využívá rezervace
description: Zjistěte, jak při nákupu virtuálních rezervací virtuálního počítače (VM) podle potřeb vašich zákazníků Microsoft Azure jejich rezervace.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 2d8bc76e0da51abf433e49028445b398c6a1db31
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276990"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="3a5f7-103">Nastavení velikosti virtuálního počítače Microsoft Azure, která maximálně využívá rezervaci</span><span class="sxs-lookup"><span data-stu-id="3a5f7-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="3a5f7-104">**Odpovídající role:** Agent pro správu | Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="3a5f7-104">**Appropriate roles**: Admin agent | Sales agent</span></span>

<span data-ttu-id="3a5f7-105">Tento článek vysvětluje, jak velikost virtuálního počítače podle výpočetních potřeb vašich zákazníků při nákupu virtuálních Microsoft Azure za ně.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-105">This article explains how to size a virtual machine (VM) to your customers' computing needs when you buy Microsoft Azure reservations for them.</span></span>
 
> [!NOTE]
> <span data-ttu-id="3a5f7-106">Tento článek se týká jenom partnerů v Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="3a5f7-106">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="3a5f7-107">Zákazníci, kteří používají jiné typy předplatných (například předplatná s předplatným s předplatným s platbami, jednotlivá předplatná, Smlouva se zákazníkem Microsoftu nebo předplatná smlouva Enterprise), by si místo toho měli přečíst tuto dokumentaci k rezervacím [Azure.](/azure/cost-management-billing/reservations)</span><span class="sxs-lookup"><span data-stu-id="3a5f7-107">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="3a5f7-108">Určení velikosti virtuálního počítače pro rezervaci Azure zákazníka</span><span class="sxs-lookup"><span data-stu-id="3a5f7-108">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="3a5f7-109">Při Microsoft Azure rezervací jménem vašich zákazníků budete muset zvolit virtuální počítač s velikostí, která bude splňovat výpočetní potřeby zákazníka.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-109">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="3a5f7-110">Tyto informace najdete pomocí jedné z těchto metod:</span><span class="sxs-lookup"><span data-stu-id="3a5f7-110">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="3a5f7-111">Rozhraní API využití Azure</span><span class="sxs-lookup"><span data-stu-id="3a5f7-111">Azure utilization API</span></span>
- <span data-ttu-id="3a5f7-112">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="3a5f7-112">The Azure portal</span></span>
- <span data-ttu-id="3a5f7-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="3a5f7-113">Azure PowerShell</span></span>
- <span data-ttu-id="3a5f7-114">Rozhraní API Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="3a5f7-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="3a5f7-115">Pokyny pro použití každé z těchto metod jsou uvedené níže.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="3a5f7-116">Po zakoupení rezervace se sleva za rezervaci automaticky uplatňuje na virtuální počítače odpovídající atributům a množství rezervace.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="3a5f7-117">Rezervaci nemusíte přiřazovat k virtuálnímu počítače.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-117">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="3a5f7-118">Slevy za rezervace se nevztahují na klasické ani propagační virtuální počítače.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-118">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="3a5f7-119">Pokud chcete správně identifikovat typ a velikost virtuálního počítače, který chcete koupit jménem zákazníka, musíte použít jednu z níže popsaných metod, protože typ řady virtuálních Partnerské centrum v souborech pro sesouhlasení.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="3a5f7-120">Získání informací o velikosti virtuálního počítače pomocí rozhraní API pro využití Azure</span><span class="sxs-lookup"><span data-stu-id="3a5f7-120">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="3a5f7-121">Pomocí hodnoty atributu ServiceType z additionalInfo v odpovědi rozhraní API identifikujte velikost virtuálního počítače, který chcete koupit.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="3a5f7-122">Další informace najdete v [tématu Získání záznamů o využití Azure zákazníkem](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) v rozhraní PARTNERSKÉ CENTRUM [API.](/partner-center/develop/)</span><span class="sxs-lookup"><span data-stu-id="3a5f7-122">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="3a5f7-123">Získání informací o velikosti virtuálního počítače pomocí portál Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="3a5f7-123">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="3a5f7-124">V Partnerské centrum přejděte na stránku **zákazníci.**</span><span class="sxs-lookup"><span data-stu-id="3a5f7-124">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="3a5f7-125">Vyhledejte zákazníka, který chce koupit rezervace virtuálních počítače Azure, a pak výběrem šipky dolů rozbalte informace o zákazníkovi.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="3a5f7-126">Výběrem **Portál pro správu Microsoft Azure** otevřete záznam zákazníka v Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-126">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="3a5f7-127">V **nabídce portálu** vyberte Virtuální počítače a pak vyberte virtuální počítač, pro který chcete koupit rezervaci.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="3a5f7-128">Na stránce s podrobnostmi o virtuálním počítači vyhledejte informace o velikosti a oblasti, jak je znázorněno níže, a tyto informace použijte k zakoupení rezervace v Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-128">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="Informace o velikosti a oblasti na stránce podrobností.":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="3a5f7-130">Získání informací o velikosti virtuálního počítače pomocí Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="3a5f7-130">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="3a5f7-131">Pomocí informací na obrázku níže získejte umístění a velikost virtuálního počítače, pro který chcete koupit rezervaci.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-131">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="Umístění a velikost virtuálního počítače.":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="3a5f7-133">Získání informací o velikosti virtuálního počítače pomocí Azure Resource Manager (ARM) API</span><span class="sxs-lookup"><span data-stu-id="3a5f7-133">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="3a5f7-134">Pomocí armclient nebo rozhraní API ARM zavolejte klienta ARM pro virtuální počítač, pro který chcete koupit rezervaci.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-134">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="3a5f7-135">/subscriptions/ <Subscription ID> /resourceGroups/ <Resource group name> /providers/Microsoft.Compute/virtualMachines/ <VM Instance Name> ?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="3a5f7-135">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="3a5f7-136">Volání vrátí hodnoty pro **vmSize** a **location**, jak je znázorněno níže.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-136">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="Hodnota vmSize.":::
    :::image type="content" source="images/usage4.png" alt-text="hodnota umístění.":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="3a5f7-139">Ověření využití virtuálních počítače Azure a slevy za rezervaci</span><span class="sxs-lookup"><span data-stu-id="3a5f7-139">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="3a5f7-140">Po zakoupení rezervované instance virtuálního počítače Azure jménem zákazníka se sleva za placení za místo na virtuálním počítači automaticky použije na virtuální počítače, které odpovídají atributům a množství rezervace zákazníka.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-140">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="3a5f7-141">Pomocí jedné z následujících metod můžete ověřit využití rezervací zákazníka a zjistit, na které virtuální počítače se uplatňují slevy za rezervace:</span><span class="sxs-lookup"><span data-stu-id="3a5f7-141">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="3a5f7-142">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="3a5f7-142">The Azure portal</span></span>
- <span data-ttu-id="3a5f7-143">Rozhraní API využití Azure</span><span class="sxs-lookup"><span data-stu-id="3a5f7-143">Azure utilization API</span></span>

<span data-ttu-id="3a5f7-144">Pokyny pro použití každé z těchto metod jsou uvedené níže.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-144">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="3a5f7-145">Pouze rozhraní API využití Azure ukazuje, na který virtuální počítač se sleva uplatňuje.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-145">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="3a5f7-146">Ověření využití rezervací zákazníka v portál Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="3a5f7-146">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="3a5f7-147">V Partnerské centrum přejděte na stránku **zákazníci.**</span><span class="sxs-lookup"><span data-stu-id="3a5f7-147">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="3a5f7-148">Vyhledejte zákazníka, jehož slevu za rezervaci a využití chcete ověřit, a pak výběrem šipky dolů rozbalte informace o zákazníkovi.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-148">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="3a5f7-149">Výběrem **Portál pro správu Microsoft Azure** otevřete záznam zákazníka v Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-149">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="3a5f7-150">V **nabídce portálu** vyberte Rezervace a pak vyberte rezervaci, u které chcete zkontrolovat využití.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-150">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="3a5f7-151">Na stránce **Přehled** zkontrolujte graf využití rezervace, který ukazuje, jak velká část rezervace se použila na virtuální počítače.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-151">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="3a5f7-152">Data o využití mohou být zpožděna až o 8 hodin.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-152">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="3a5f7-153">a.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-153">a.</span></span> <span data-ttu-id="3a5f7-154">Pokud je využití rezervace 100 %, zákazník dostává všechny možné úspory, které může nákup rezervace poskytnout.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-154">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="3a5f7-155">b.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-155">b.</span></span> <span data-ttu-id="3a5f7-156">Pokud je využití rezervace 0 %, sleva se na žádný virtuální počítač nevyučuje.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-156">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="3a5f7-157">c.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-157">c.</span></span> <span data-ttu-id="3a5f7-158">Pokud je využití rezervace mezi 1 a 99 %, existují nevyužité výhody.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-158">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="3a5f7-159">Pokud se chcete této situaci vyhnout, před nákupem určete správnou velikost virtuálního počítače pro podporu výpočetních potřeb zákazníka.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-159">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="3a5f7-160">Ověření využití rezervací zákazníka pomocí rozhraní API pro využití Azure</span><span class="sxs-lookup"><span data-stu-id="3a5f7-160">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="3a5f7-161">Pouze rozhraní API využití Azure ukazuje, na který virtuální počítač se sleva uplatňuje.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-161">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="3a5f7-162">Pomocí rozhraní API pro využití Azure můžete získat data o využití rezervací a ověřit, že zákazník používá slevu za rezervaci, a zjistit, na které virtuální počítače (virtuální počítače) se sleva uplatňuje.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-162">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="3a5f7-163">Porovnejte příklad A s příkladem B a podívejte se, jak ověřit využití rezervací zákazníka.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-163">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Příklady využití rezervací":::

- <span data-ttu-id="3a5f7-165">ReservationId identifikuje rezervaci Azure, která se použila k použití slevy na virtuální počítač.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-165">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="3a5f7-166">consumptionMeter je MeterId pro virtuální počítač, na který se uplatňuje sleva za rezervaci.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-166">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="3a5f7-167">ReservationMeter zobrazuje náklady 0 USD od použití slevy za rezervaci.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-167">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="3a5f7-168">Další informace najdete v [tématu Získání záznamů o využití Azure zákazníkem](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) v rozhraní PARTNERSKÉ CENTRUM [API.](/partner-center/develop/)</span><span class="sxs-lookup"><span data-stu-id="3a5f7-168">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="3a5f7-169">Náklady na software, jako je Například Microsoft Windows Server, nejsou aktuálně zahrnuté v ceně rezervace virtuálního počítače a zobrazí se jako samostatné řádkové položky v záznamu objednávky a na faktuře.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-169">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="3a5f7-170">Pokud má ale zákazník Zvýhodněné hybridní využití Azure, náklady na software se neuplatní.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-170">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="3a5f7-171">Další informace najdete v tématu [Náklady na software Windows, které nejsou součástí rezervovaných instancí](/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="3a5f7-171">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="next-steps"></a><span data-ttu-id="3a5f7-172">Další kroky</span><span class="sxs-lookup"><span data-stu-id="3a5f7-172">Next steps</span></span>

|<span data-ttu-id="3a5f7-173">**Informace o**</span><span class="sxs-lookup"><span data-stu-id="3a5f7-173">**For information about**</span></span>   |<span data-ttu-id="3a5f7-174">**Přečtěte si:**</span><span class="sxs-lookup"><span data-stu-id="3a5f7-174">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="3a5f7-175">Přehled rezervací Azure v CSP</span><span class="sxs-lookup"><span data-stu-id="3a5f7-175">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="3a5f7-176">Prodej Microsoft Azure rezervovaných instancí virtuálních počítače</span><span class="sxs-lookup"><span data-stu-id="3a5f7-176">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="3a5f7-177">Nákup rezervací Azure pro zákazníky v Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="3a5f7-177">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="3a5f7-178">Nákup rezervací Azure</span><span class="sxs-lookup"><span data-stu-id="3a5f7-178">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="3a5f7-179">Správa rezervací Azure v Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="3a5f7-179">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="3a5f7-180">Správa rezervací Azure v Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="3a5f7-180">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="3a5f7-181">Nákup rezervací Azure v Azure Portal</span><span class="sxs-lookup"><span data-stu-id="3a5f7-181">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="3a5f7-182">[Platba předem pro virtuální počítače s Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) v nápovědě Azure</span><span class="sxs-lookup"><span data-stu-id="3a5f7-182">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="3a5f7-183">Správa rezervací Azure v Azure Portal</span><span class="sxs-lookup"><span data-stu-id="3a5f7-183">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="3a5f7-184">[Správa rezervovaných instancí virtuálních počítače v](/azure/billing/billing-manage-reserved-vm-instance) nápovědě Azure</span><span class="sxs-lookup"><span data-stu-id="3a5f7-184">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="3a5f7-185">Nákup rezervací Azure pomocí rozhraní PARTNERSKÉ CENTRUM API</span><span class="sxs-lookup"><span data-stu-id="3a5f7-185">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="3a5f7-186">[Informace Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) najdete v dokumentaci Partnerské centrum pro vývojáře.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-186">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="3a5f7-187">Dáváte zákazníkům oprávnění k nákupu vlastních rezervací Azure z předplatného, které jste pro ně zakoupili.</span><span class="sxs-lookup"><span data-stu-id="3a5f7-187">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="3a5f7-188">Udělit zákazníkům oprávnění k nákupu vlastních rezervací Azure</span><span class="sxs-lookup"><span data-stu-id="3a5f7-188">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |