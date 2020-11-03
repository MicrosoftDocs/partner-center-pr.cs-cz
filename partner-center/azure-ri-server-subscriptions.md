---
title: Rezervace Azure & předplatných serveru
ms.topic: article
ms.date: 08/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si o příležitostech k získání, zřizování a správě rezervací Azure a předplatných serverů pro zákazníky v souvislosti se službou Cloud Solution Provider.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3c08e897a8f5d7c11b36627b0c24ad2da3f92329
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/22/2020
ms.locfileid: "92527340"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="1136d-103">Získání, zřízení, & Správa předplatných virtuálních počítačů Azure (rezervované instance) a předplatných serverů pro zákazníky</span><span class="sxs-lookup"><span data-stu-id="1136d-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>

<span data-ttu-id="1136d-104">Platí pro:</span><span class="sxs-lookup"><span data-stu-id="1136d-104">Applies to:</span></span>

- <span data-ttu-id="1136d-105">Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="1136d-105">Partner Center</span></span>

<span data-ttu-id="1136d-106">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="1136d-106">**Appropriate roles**</span></span>

- <span data-ttu-id="1136d-107">Agent správce</span><span class="sxs-lookup"><span data-stu-id="1136d-107">Admin agent</span></span>
- <span data-ttu-id="1136d-108">Globální správce</span><span class="sxs-lookup"><span data-stu-id="1136d-108">Global admin</span></span>
- <span data-ttu-id="1136d-109">Agent helpdesku</span><span class="sxs-lookup"><span data-stu-id="1136d-109">Helpdesk agent</span></span>
- <span data-ttu-id="1136d-110">Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="1136d-110">Sales agent</span></span>
- <span data-ttu-id="1136d-111">Správce správy uživatelů</span><span class="sxs-lookup"><span data-stu-id="1136d-111">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="1136d-112">Tento článek se týká jenom partnerů v programu Cloud Solution Provider (CSP).</span><span class="sxs-lookup"><span data-stu-id="1136d-112">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="1136d-113">[Tuto dokumentaci k rezervacím Azure](/azure/cost-management-billing/reservations)by si měli přečíst zákazníci, kteří používají jiné typy předplatných (například, platby na základě průběžných plateb, jednotlivce, smlouvy o zákaznících Microsoftu nebo předplatná smlouva Enterprise).</span><span class="sxs-lookup"><span data-stu-id="1136d-113">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="1136d-114">Co jsou rezervace Azure?</span><span class="sxs-lookup"><span data-stu-id="1136d-114">What are Azure Reservations?</span></span>

<span data-ttu-id="1136d-115">Azure Reservations vám pomůžou ušetřit peníze tím, že se předem platíte za jednoleté nebo tři roky virtuálních počítačů, SQL Database výpočetní kapacity, Azure Cosmos DB propustnosti nebo jiných prostředků Azure.</span><span class="sxs-lookup"><span data-stu-id="1136d-115">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="1136d-116">Předběžná platba vám umožní získat slevu na prostředky, které používáte.</span><span class="sxs-lookup"><span data-stu-id="1136d-116">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="1136d-117">Rezervace můžou významně snížit vaše virtuální počítače, výpočetní služby SQL Database, Azure Cosmos DB a další náklady na prostředky až do 72% ve srovnání s cenami průběžných plateb.</span><span class="sxs-lookup"><span data-stu-id="1136d-117">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="1136d-118">Rezervace poskytují slevu z faktury a neovlivňují běhový stav prostředků.</span><span class="sxs-lookup"><span data-stu-id="1136d-118">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="1136d-119">Další informace najdete v tématu [co je Azure reservations?](/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="1136d-119">For more information see [What are Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="1136d-120">Proč by si měli zákazníci koupit rezervaci?</span><span class="sxs-lookup"><span data-stu-id="1136d-120">Why should customers buy a reservation?</span></span>

<span data-ttu-id="1136d-121">Pokud mají zákazníci virtuální počítače, Azure Cosmos DB nebo databáze SQL, které se spouštějí po dlouhou dobu, je při nákupu rezervace k dispozici největší cenově výhodné možnosti.</span><span class="sxs-lookup"><span data-stu-id="1136d-121">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="1136d-122">Pokud například zákazník průběžně provozuje čtyři instance služby bez rezervace, budou se účtovat podle tarifů průběžných plateb.</span><span class="sxs-lookup"><span data-stu-id="1136d-122">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="1136d-123">Pokud si nakupují rezervaci pro tyto prostředky, okamžitě získají slevu za rezervaci.</span><span class="sxs-lookup"><span data-stu-id="1136d-123">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="1136d-124">Za tyto prostředky se už nebudou účtovat sazby pro průběžné platby.</span><span class="sxs-lookup"><span data-stu-id="1136d-124">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="1136d-125">Působivá nová nabídka Azure v CSP</span><span class="sxs-lookup"><span data-stu-id="1136d-125">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="1136d-126">Díky zavedení Azure Reservations a serverových předplatných pro svůj program CSP je Microsoft lepší, aby jeho partneři mohli řešit rychle rostoucí poptávku zákazníků, aby se zajistila cenově výhodné řešení pro podporu vysoce předvídatelných a trvalých cloudových úloh.</span><span class="sxs-lookup"><span data-stu-id="1136d-126">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="1136d-127">Program CSP umožňuje partnerům získat, zřídit a spravovat Azure Reservations a odběry serverů jménem komerčních zákazníků prostřednictvím partnerského centra Microsoftu a Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="1136d-127">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>

<span data-ttu-id="1136d-128">Partnerům v našem programu CSP nabízíme i informace o tom, jak můžou být zakoupeny rezervace Azure.</span><span class="sxs-lookup"><span data-stu-id="1136d-128">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="1136d-129">Partneři CSP můžou [koupit rezervace Azure jménem zákazníka](azure-reservations-buying.md) nebo můžou [zákazníkům dovolit koupit si své vlastní rezervace](give-customers-permission.md) z předchozího předplatného Azure, které si ho zakoupili.</span><span class="sxs-lookup"><span data-stu-id="1136d-129">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="1136d-130">Azure Reservations zákazníkům poskytuje flexibilitu virtualizace pro nejrůznější výpočetní řešení, včetně vývoje a testování, spouštění aplikací a rozšiřování datového centra.</span><span class="sxs-lookup"><span data-stu-id="1136d-130">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="1136d-131">[Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) například komerčním zákazníkům můžete ušetřit až 72% oproti průběžným nákupům Azure s průběžnými platbami, a to jednoduše tak, že ho zakoupíte nebo zachováte – virtuální počítač po dobu 1 nebo 3 roky.</span><span class="sxs-lookup"><span data-stu-id="1136d-131">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="1136d-132">Zákazníci se systémem Windows Server s Zvýhodněné hybridní využití Azure, kteří jsou součástí programu Software Assurance, budou moci ušetřit až 80% oproti sazbám průběžných plateb.</span><span class="sxs-lookup"><span data-stu-id="1136d-132">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="1136d-133">Díky nespárované kombinaci působivých cen a nespárované flexibilitě nasazení uvidí zákazníci nejlepší celkovou hodnotu, když zvolí Azure Reservations:</span><span class="sxs-lookup"><span data-stu-id="1136d-133">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="1136d-134">Rezervace Azure</span><span class="sxs-lookup"><span data-stu-id="1136d-134">Azure reservations</span></span>

- <span data-ttu-id="1136d-135">Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="1136d-135">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="1136d-136">Rezervace databáze SQL</span><span class="sxs-lookup"><span data-stu-id="1136d-136">SQL DB Reservations</span></span>
- <span data-ttu-id="1136d-137">Spravovaná instance SQL</span><span class="sxs-lookup"><span data-stu-id="1136d-137">SQL Managed Instance</span></span>
- <span data-ttu-id="1136d-138">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="1136d-138">Azure Cosmos DB</span></span>
- <span data-ttu-id="1136d-139">Azure SQL Data Warehouse</span><span class="sxs-lookup"><span data-stu-id="1136d-139">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="1136d-140">App Services</span><span class="sxs-lookup"><span data-stu-id="1136d-140">App Services</span></span>
- <span data-ttu-id="1136d-141">Rezervace jednotek Azure Databricks</span><span class="sxs-lookup"><span data-stu-id="1136d-141">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="1136d-142">Spravovaný disk</span><span class="sxs-lookup"><span data-stu-id="1136d-142">Managed Disk</span></span>
- <span data-ttu-id="1136d-143">Objekt blob bloku</span><span class="sxs-lookup"><span data-stu-id="1136d-143">Block blob</span></span>
- <span data-ttu-id="1136d-144">MySQL</span><span class="sxs-lookup"><span data-stu-id="1136d-144">MySQL</span></span>
- <span data-ttu-id="1136d-145">Průzkumník dat Azure</span><span class="sxs-lookup"><span data-stu-id="1136d-145">Azure Data explorer</span></span>
- <span data-ttu-id="1136d-146">MariaDB</span><span class="sxs-lookup"><span data-stu-id="1136d-146">MariaDB</span></span>
- <span data-ttu-id="1136d-147">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="1136d-147">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="1136d-148">Předplatná serveru</span><span class="sxs-lookup"><span data-stu-id="1136d-148">Server subscriptions</span></span>

- <span data-ttu-id="1136d-149">Windows Server</span><span class="sxs-lookup"><span data-stu-id="1136d-149">Windows Server</span></span>
- <span data-ttu-id="1136d-150">Licence CAL na službu Vzdálená plocha (VP)</span><span class="sxs-lookup"><span data-stu-id="1136d-150">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="1136d-151">SQL Server</span><span class="sxs-lookup"><span data-stu-id="1136d-151">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="1136d-152">Roční předplatná pro Linux ISV</span><span class="sxs-lookup"><span data-stu-id="1136d-152">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="1136d-153">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="1136d-153">SUSE Linux</span></span>
- <span data-ttu-id="1136d-154">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="1136d-154">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="1136d-155">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="1136d-155">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="1136d-156">Roční předplatná ISV</span><span class="sxs-lookup"><span data-stu-id="1136d-156">ISV annual subscriptions</span></span>

- <span data-ttu-id="1136d-157">Azure VMware Solution by CloudSimple</span><span class="sxs-lookup"><span data-stu-id="1136d-157">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="1136d-158">Začínáme</span><span class="sxs-lookup"><span data-stu-id="1136d-158">Getting started</span></span>

<span data-ttu-id="1136d-159">K tomu, abyste se seznámili s tím, jak můžete Azure Reservations umístit zákazníkům a co nejrychleji začít pracovat, doporučujeme následující postup, který vám pomůže zkontrolovat materiály připravenosti:</span><span class="sxs-lookup"><span data-stu-id="1136d-159">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="1136d-160">Projděte si přehled prezentací a přidružených webinářeů pro pozici a umístění zákaznické hodnoty.</span><span class="sxs-lookup"><span data-stu-id="1136d-160">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="1136d-161">Kontrola a pochopení moderní provozní příručky pro obchod</span><span class="sxs-lookup"><span data-stu-id="1136d-161">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="1136d-162">Přečtěte si nejčastější dotazy k předplatným Azure pro rezervované a serverové služby</span><span class="sxs-lookup"><span data-stu-id="1136d-162">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="1136d-163">Vysvětlení aktualizací Azure Reservations a předplatných serveru v [rozhraní API partnerského centra (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)</span><span class="sxs-lookup"><span data-stu-id="1136d-163">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="1136d-164">Zdroje a prostředky</span><span class="sxs-lookup"><span data-stu-id="1136d-164">Resources</span></span>

<span data-ttu-id="1136d-165">Níže je uvedený úplný seznam prostředků, které vám pomůžou rychle připojit Azure Reservations prostřednictvím partnerského centra:</span><span class="sxs-lookup"><span data-stu-id="1136d-165">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="1136d-166">Připravenost prodeje</span><span class="sxs-lookup"><span data-stu-id="1136d-166">Sales readiness</span></span>

- [<span data-ttu-id="1136d-167">Předplatná Azure Reservations a serveru s Zvýhodněné hybridní využití Azure přehled</span><span class="sxs-lookup"><span data-stu-id="1136d-167">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="1136d-168">Prodejní list</span><span class="sxs-lookup"><span data-stu-id="1136d-168">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="1136d-169">Nejčastější dotazy k partnerům pro Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="1136d-169">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="1136d-170">Nejčastější dotazy týkající se Azure Reservations a databáze SQL</span><span class="sxs-lookup"><span data-stu-id="1136d-170">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="1136d-171">Licence pro klientský přístup k vzdálené ploše (VP CAL) (oznámení)</span><span class="sxs-lookup"><span data-stu-id="1136d-171">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="1136d-172">Azure Reserved VM Instances (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="1136d-172">Azure Reserved VM Instances (Azure portal)</span></span>](/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="1136d-173">Předplatná serveru</span><span class="sxs-lookup"><span data-stu-id="1136d-173">Server Subscriptions</span></span>](csp-software-subscriptions.md)
- [<span data-ttu-id="1136d-174">Přehled SQL DB v Azure</span><span class="sxs-lookup"><span data-stu-id="1136d-174">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="1136d-175">Rezervace databáze SQL (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="1136d-175">SQL DB Reservations (Azure portal)</span></span>](/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="1136d-176">Azure Cosmos DB (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="1136d-176">Azure Cosmos DB (Azure portal)</span></span>](/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="1136d-177">Spravovaná instance SQL (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="1136d-177">SQL Managed Instance (Azure portal)</span></span>](/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="1136d-178">SUSE a Red Hat Enterprise Linux (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="1136d-178">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="1136d-179">Red Hat Linux v Azure</span><span class="sxs-lookup"><span data-stu-id="1136d-179">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="1136d-180">SUSE Linux v Azure</span><span class="sxs-lookup"><span data-stu-id="1136d-180">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="1136d-181">Linux v Azure</span><span class="sxs-lookup"><span data-stu-id="1136d-181">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="1136d-182">Přehled cen Azure</span><span class="sxs-lookup"><span data-stu-id="1136d-182">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="1136d-183">Cenová Kalkulačka Azure</span><span class="sxs-lookup"><span data-stu-id="1136d-183">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="1136d-184">Rezervace jednotek Azure Databricks</span><span class="sxs-lookup"><span data-stu-id="1136d-184">Azure Databricks unit reservations</span></span>](/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="1136d-185">Ceníky CSP: **Microsoft Azure rezervované instance** a ceníky pro **předplatné softwaru** se nachází na stránce [nabídky & cenového](https://partner.microsoft.com/pcv/sales) centra pro partnery.</span><span class="sxs-lookup"><span data-stu-id="1136d-185">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="1136d-186">Školení</span><span class="sxs-lookup"><span data-stu-id="1136d-186">Training</span></span>

<span data-ttu-id="1136d-187">Zaregistrujte se, abyste viděli [webinářey komerčních licencí](https://commercial-licensing.eventbuilder.com/FY2019_ALL) a události na vyžádání.</span><span class="sxs-lookup"><span data-stu-id="1136d-187">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>

<span data-ttu-id="1136d-188">Události na vyžádání licencování na vyžádání obsahují témata, jako například:</span><span class="sxs-lookup"><span data-stu-id="1136d-188">Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="1136d-189">Služby CSP Online Services, CSP Azure a obecné licenční aktualizace, včetně Azure (listopadu 2018)</span><span class="sxs-lookup"><span data-stu-id="1136d-189">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>
- <span data-ttu-id="1136d-190">Flexibilita velikosti instance & rezervované kapacity SQL DB (srpen 2018)</span><span class="sxs-lookup"><span data-stu-id="1136d-190">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>
- <span data-ttu-id="1136d-191">Předplatné serveru v CSP (červenec 2018)</span><span class="sxs-lookup"><span data-stu-id="1136d-191">Server Subscriptions in CSP (July 2018)</span></span>
- <span data-ttu-id="1136d-192">Přehled Azure Reservations CSP (květen 2018)</span><span class="sxs-lookup"><span data-stu-id="1136d-192">Azure Reservations Overview in CSP (May 2018)</span></span>

<span data-ttu-id="1136d-193">Další užitečné školení zahrnují [modul licencování Azure na univerzitě University](https://aka.ms/azure_partner_licensing).</span><span class="sxs-lookup"><span data-stu-id="1136d-193">Other useful training includes the [Azure Licensing Module on Partner University](https://aka.ms/azure_partner_licensing).</span></span>

### <a name="operations"></a><span data-ttu-id="1136d-194">Operace</span><span class="sxs-lookup"><span data-stu-id="1136d-194">Operations</span></span>

- <span data-ttu-id="1136d-195">[Moderní obchodní provozní příručka](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (aktualizovaná): komplexní průvodce vztahující se k klíčovým zásadám a provozním aspektům, jako jsou smlouvy, objednání prostřednictvím partnerského centra, faktury, podrobností o ceníku, motivů, souborů pro odsouhlasení, API/SDK, izolovaného prostoru a sdílených služeb Azure</span><span class="sxs-lookup"><span data-stu-id="1136d-195">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="1136d-196">Moderní nabídky dostupnost země a matice měna zákazníka</span><span class="sxs-lookup"><span data-stu-id="1136d-196">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="1136d-197">Prodej rezervovaných instancí Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="1136d-197">Sell Microsoft Azure Reserved Instances</span></span>](azure-reservations.md)
- [<span data-ttu-id="1136d-198">Nákup Microsoft Azure rezervací jménem vašich zákazníků</span><span class="sxs-lookup"><span data-stu-id="1136d-198">Buy Microsoft Azure reservations on behalf of your customers</span></span>](azure-reservations-buying.md)
- [<span data-ttu-id="1136d-199">Správa rezervací Azure jménem vašich zákazníků</span><span class="sxs-lookup"><span data-stu-id="1136d-199">Manage Azure reservations on behalf of your customers</span></span>](azure-reservations-manage.md)
- [<span data-ttu-id="1136d-200">Fakturace za rezervace Azure</span><span class="sxs-lookup"><span data-stu-id="1136d-200">Billing for Azure reservations</span></span>](azure-plan-billing.md)
- [<span data-ttu-id="1136d-201">Velikost virtuálního počítače pro maximální využití rezervace</span><span class="sxs-lookup"><span data-stu-id="1136d-201">VM sizing for maximum reservation usage</span></span>](azure-usage.md)
- [<span data-ttu-id="1136d-202">Rozhraní API partnerského centra (API/SDK)</span><span class="sxs-lookup"><span data-stu-id="1136d-202">Partner Center API (API/SDK)</span></span>](/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="1136d-203">Vzdálená plocha</span><span class="sxs-lookup"><span data-stu-id="1136d-203">Remote Desktop Services</span></span>](/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="1136d-204">Zvýhodněné hybridní využití Azure</span><span class="sxs-lookup"><span data-stu-id="1136d-204">Azure Hybrid Benefit</span></span>

<span data-ttu-id="1136d-205">[Zvýhodněné hybridní využití Azure](https://azure.microsoft.com/pricing/hybrid-benefit) vám pomůže získat větší hodnotu z licencí Windows serveru a ušetřit na virtuálních počítačích až \* 47 procent.</span><span class="sxs-lookup"><span data-stu-id="1136d-205">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="1136d-206">Výhody s licencemi na Windows Server Datacenter a Standard Edition, které jsou součástí programu Software Assurance, můžete využívat.</span><span class="sxs-lookup"><span data-stu-id="1136d-206">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="1136d-207">V závislosti na edici můžete licence převést nebo znovu použít k provozování virtuálních počítačů s Windows serverem v Azure a platit nižší základní výpočetní sazbu (sazby za virtuální počítače Linux).</span><span class="sxs-lookup"><span data-stu-id="1136d-207">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="1136d-208">Viz také [zvýhodněné hybridní využití Azure Nejčastější dotazy](https://azure.microsoft.com/pricing/hybrid-benefit/faq/) .</span><span class="sxs-lookup"><span data-stu-id="1136d-208">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="1136d-209">\* Skutečné úspory se můžou lišit v závislosti na oblasti, typu instance nebo využití.</span><span class="sxs-lookup"><span data-stu-id="1136d-209">\*Actual savings may vary based on region, instance type, or usage.</span></span>
