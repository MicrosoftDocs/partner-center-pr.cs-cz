---
title: Konsolidace tenanta regionální autorizace CSP
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Tyto pokyny slouží ke konsolidaci klientů pro různé země nebo oblasti. Sem patří postup migrace zákaznických účtů a zákaznických předplatných.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: d2168dcd60b8675a21960918dab49b778025fa51
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147577"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="d7fd2-104">Pokyny ke konsolidaci tenantů s regionální autorizací CSP</span><span class="sxs-lookup"><span data-stu-id="d7fd2-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="d7fd2-105">**Platí pro**: partnerské Centrum | Partnerské centrum pro Microsoft Cloud pro státní správu USA</span><span class="sxs-lookup"><span data-stu-id="d7fd2-105">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="d7fd2-106">**Příslušné role**: globální správce | Agent správce</span><span class="sxs-lookup"><span data-stu-id="d7fd2-106">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="d7fd2-107">\[Některé informace se vztahují na předem vydaný produkt, který se před prodejem z komerčního vydání může podstatně upravit.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-107">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="d7fd2-108">Microsoft neposkytuje žádné záruky, výslovné ani předpokládané, týkající se zde uváděných informací.\]</span><span class="sxs-lookup"><span data-stu-id="d7fd2-108">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="d7fd2-109">Můžete konsolidovat klienty pro vaši firmu.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-109">You can consolidate tenants for your business.</span></span> <span data-ttu-id="d7fd2-110">Tyto pokyny slouží ke konsolidaci klientů pro různé země nebo oblasti.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-110">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="d7fd2-111">Musíte být vědomi všech zřízené předplatných a počty licencí pro každého ze svých zákazníků v účtu, ze kterého provádíte převod.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-111">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="d7fd2-112">V rámci tohoto procesu migrace se v rámci nového účtu centrálního CSP v rámci procesu migrace znovu zřídí stejné přesně stejné odběry se stejnými počty licencí.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-112">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="d7fd2-113">Pomocí funkce seznam pro export můžete vytvořit seznam zákazníků pro přesun do centralizovaného tenanta.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="d7fd2-114">Po dokončení konsolidace se nemůžete vrátit k předchozímu stavu tenanta.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-114">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="d7fd2-115">Může se také vyžadovat akce zákazníka.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-115">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="d7fd2-116">Příprava migrace</span><span class="sxs-lookup"><span data-stu-id="d7fd2-116">Prepare for migration</span></span>

- <span data-ttu-id="d7fd2-117">Přihlaste se k **partnerskému centru**  pomocí **přechodu** účtu (ten, který převedete na nový účet), a Projděte si všechny zákazníky a všechny služby zřízené pro tyto zákazníky.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-117">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="d7fd2-118">Odhlaste se z tohoto účtu.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-118">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="d7fd2-119">Migrace zákaznických účtů</span><span class="sxs-lookup"><span data-stu-id="d7fd2-119">Migrate customer accounts</span></span>

1. <span data-ttu-id="d7fd2-120">Přihlaste se k **partnerskému centru**  pomocí účtu **přechodu** (nového) (ten, na který přecházíte zákazníky).</span><span class="sxs-lookup"><span data-stu-id="d7fd2-120">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="d7fd2-121">Vyberte **Zákazníci**.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-121">Select **Customers**.</span></span>

3. <span data-ttu-id="d7fd2-122">Vyberte **požádat o vztah prodejce**.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-122">Select **Request a reseller relationship**.</span></span> <span data-ttu-id="d7fd2-123">Zobrazí se výchozí e-mailová zpráva, která se odešle vašim zákazníkům.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-123">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="d7fd2-124">Tato zpráva obsahuje adresu URL s ID organizace, které je pro nový účet partnerského centra jedinečné.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-124">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="d7fd2-125">**Akce zákazníka:** Ujistěte se, že každý aktivní zákazník, kterého chcete migrovat, navštíví tuto adresu URL.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-125">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="d7fd2-126">Při otevírání adresy URL se zákazníkovi zobrazí výzva k přihlášení k portálu Office 365.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-126">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="d7fd2-127">Zákazník se přihlásí pomocí stejného ID organizace, které používá pro přístup k portálům pro správu Azure a Office 365.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-127">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="d7fd2-128">Po přihlášení se globálnímu  správci zákaznického účtu zobrazí výzva k odeslání smlouvy, která novému účtu CSP uděluje delegovaná oprávnění správce.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-128">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="d7fd2-129">Pokud zákazník souhlasí, zaškrtne políčko a souhlasí s autorizací relace.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-129">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="d7fd2-130">Zákazníci se po jednom odeslaní smlouvy zobrazí v seznamu zákazníků partnera.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-130">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="d7fd2-131">Migrace předplatných Office 365 a předplatných jiných než Azure založených na využití</span><span class="sxs-lookup"><span data-stu-id="d7fd2-131">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="d7fd2-132">Jakmile zákazník smlouvu podepíše, můžete znovu vytvořit jeho předplatná v rámci centralizovaného partnerského tenanta.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-132">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="d7fd2-133">V **Partnerské centrum** vyberte **Zákazníci.**</span><span class="sxs-lookup"><span data-stu-id="d7fd2-133">From **Partner Center**, select **Customers**.</span></span>

3. <span data-ttu-id="d7fd2-134">Otevřete název společnosti zákazníka, kterého chcete migrovat.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-134">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="d7fd2-135">Vyberte **Přidat předplatné.**</span><span class="sxs-lookup"><span data-stu-id="d7fd2-135">Select **Add subscription**.</span></span>

5. <span data-ttu-id="d7fd2-136">Přidejte správná předplatná a počty licencí z katalogu.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-136">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="d7fd2-137">Ověřte pomocí informací uvedených v části **Přechod z partnerských** účtů.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-137">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="seznam zákazníků":::

6. <span data-ttu-id="d7fd2-139">Vyberte **Odeslat.**</span><span class="sxs-lookup"><span data-stu-id="d7fd2-139">Select **Submit.**</span></span>

   <span data-ttu-id="d7fd2-140">Služby se teď zákazníkům poskytují z účtu **přechodu na** partnerský účet.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-140">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="d7fd2-141">Opakováním těchto kroků migrujte předplatná pro všechny další zákazníky.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-141">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="d7fd2-142">Než budete pokračovat k další části, ujistěte  se, že všechna zákaznická předplatná v části Přechod z partnerských účtů se znovu zř zda jsou v rámci účtu Přechod **na** partnera znovu zřízena.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-142">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="d7fd2-143">Partneři musí pozastavit  předplatná na účtu přechodu z partnerského tenanta v Partnerské centrum Partnerské centrum stejný  den, kdy se tato předplatná přenesou Partnerské centrum nastaví v rámci účtu přechodu na partnerského tenanta v Partnerské centrum, aby se zajistilo, že nedojde k dvojí fakturaci.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-143">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="d7fd2-144">Žádosti o podporu budou odepřeny pro kredity z důvodu překrytí při fakturaci, ke kterému dojde z nesprávného zákazu **přechodu z** předplatných.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-144">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="d7fd2-145">Zakázání předplatných Office 365 v rámci přechodu z partnerského účtu</span><span class="sxs-lookup"><span data-stu-id="d7fd2-145">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="d7fd2-146">Zakázáním předplatného CSP v rámci **přechodu z** partnerských účtů zastavíte jakoukoli budoucí fakturaci.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-146">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="d7fd2-147">Nemusíte ručně zakázat předplatná Azure, protože předplatná Azure se během procesu migrace automaticky vypnou.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-147">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="d7fd2-148">Přihlaste se k **partnerskému centru** pomocí **přechodu z** účtu CSP a přejděte do seznamu zákazníků.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-148">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="d7fd2-149">Otevřete zákazníka s předplatnými, které chcete zakázat, a pak vyberte první nabídku, kterou chcete zakázat.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-149">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="d7fd2-150">Nastavte předplatné na **pozastaveno** a pak vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-150">Set the subscription to **suspended**, and then select **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="d7fd2-151">Pozastavení předplatného zajistí, že nedojde k dvojímu vyúčtování.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-151">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="d7fd2-152">V seznamu předplatných se zobrazí **pozastavené** předplatné.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-152">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="d7fd2-153">Tento postup opakujte pro všechna předplatná v rámci zákazníka.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-153">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="d7fd2-154">Ověřte, že je **pozastavená** všechna zobrazení.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-154">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="d7fd2-155">Vyberte dalšího zákazníka v seznamu a opakujte postup zakázání všech předplatných.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-155">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="d7fd2-156">Migrace předplatných na základě využití Azure</span><span class="sxs-lookup"><span data-stu-id="d7fd2-156">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="d7fd2-157">Na rozdíl od předplatných CSP pro Office 365 se nemusíte migrovat ručně pomocí Azure, předplatných CSP na základě využití.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-157">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="d7fd2-158">Služba Microsoft Azure Support migruje předplatná Azure a všechny nasazené služby nebo prostředky z **přechodu z** účtů prodejců CSP na **převod na** účet prodejce CSP.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-158">Microsoft Azure Support will migrate the Azure subscriptions and all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="d7fd2-159">Během tohoto přechodu nebudete mít k dispozici žádné přerušení služby pro zákazníka.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-159">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="d7fd2-160">Ujistěte se, že účty zákazníků, které budou mít migrované předplatné Azure, přijaly smlouvu, která bude přidružená k novému **přechodu na** účet CSP.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-160">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="d7fd2-161">Budete upozorněni na to, kteří zákaznické účty budou připravené k migraci, a poskytnout jim názvy společností.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-161">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="d7fd2-162">Microsoft migruje předplatné založené na využití Azure a upozorní vás, až se migrace dokončí.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-162">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="d7fd2-163">Musíte potvrdit, že předplatné Azure v účtu prodejce Přechod  z **CSP** je teď označené jako pozastavené v Partnerské centrum v části Předplatná zákazníka.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-163">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="d7fd2-164">Ověřte, že předplatné Azure v **rámci** účtu prodejce Přechod  na CSP teď zobrazuje stav aktivní v Partnerské centrum v části Předplatná zákazníků.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-164">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="d7fd2-165">Zakázáním předplatných v rámci zákazníka se nezmění vzhled zákazníka v seznamu Zákazníci.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-165">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="d7fd2-166">V současné době není možné odebrat zákazníky ze seznamu.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-166">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="d7fd2-167">Partneři by se měli těmto zákazníkům v budoucnu vyhnout přidávání předplatných z **účtu,** který přechází z tohoto účtu.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-167">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="d7fd2-168">Opakujte tento postup pro všechna předplatná v rámci všech vašich zákazníků, abyste zastavili budoucí poplatky na účtech **přechodu** z účtu nebo účtů.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-168">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="d7fd2-169">Partner obdrží jednu konečnou fakturu s kreditem na počet nevyužitých dnů mezi dnem zrušení a posledním dnem fakturačního období.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-169">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="d7fd2-170">Po tomto konečném fakturačním období se nebudou generovat žádné budoucí faktury.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-170">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="d7fd2-171">Další informace</span><span class="sxs-lookup"><span data-stu-id="d7fd2-171">Additional information</span></span>

- <span data-ttu-id="d7fd2-172">Zakázání předplatného z účtu Přechod z **CSP** nemá vliv na službu koncového zákazníka, pokud byla služba zřízena z účtu Přechod na **CSP** před zakázáním předplatného.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-172">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="d7fd2-173">Předplatná nemůže zákazník používat a po pozastavení nebo zrušení negenerují poplatky.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-173">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="d7fd2-174">V současné době neexistuje způsob, jak zákazníka ze seznamu Zákazníků úplně **odebrat.**</span><span class="sxs-lookup"><span data-stu-id="d7fd2-174">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="d7fd2-175">Partneři musí pozastavit  předplatná na účtu tenanta přechodu z partnerského účtu Partnerské centrum ve stejný  den, kdy se tato předplatná přenesou na účet Přechod na Partnerské centrum nastaví je, aby se zajistilo, že nedojde k dvojí fakturaci.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-175">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="d7fd2-176">Microsoft nebude podporovat žádosti o kredity kvůli překrývání fakturace způsobené tím, že správně nenastaví přechod z **předplatných** na pozastavené.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-176">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="d7fd2-177">Zjednodušení migrace pomocí exportu</span><span class="sxs-lookup"><span data-stu-id="d7fd2-177">Simplify migration using Export</span></span>

<span data-ttu-id="d7fd2-178">Pomocí **funkce exportu** můžete zachytit odběry, které je třeba použít v nové konsolidované struktuře:</span><span class="sxs-lookup"><span data-stu-id="d7fd2-178">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="d7fd2-179">Pokud chcete zobrazit seznam zákazníků, vyberte **zákazníky** v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-179">Select **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="d7fd2-180">Otevřete požadované jméno zákazníka.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-180">Open the desired customer name.</span></span>

3. <span data-ttu-id="d7fd2-181">Na stránce **předplatná** vyberte **exportovat odběry** a exportujte tak podrobnosti předplatných do excelového souboru.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-181">On the **Subscriptions** page, select **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="d7fd2-182">Pomocí tohoto seznamu můžete znovu vytvořit odběry ve vašem novém konsolidovaném tenantovi.</span><span class="sxs-lookup"><span data-stu-id="d7fd2-182">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="d7fd2-183">Registrace rozhraní API</span><span class="sxs-lookup"><span data-stu-id="d7fd2-183">API registration</span></span>

<span data-ttu-id="d7fd2-184">Další informace o registraci rozhraní API najdete v tématu [nastavení přístupu k rozhraní API v partnerském centru](/partner-center/develop/set-up-api-access-in-partner-center).</span><span class="sxs-lookup"><span data-stu-id="d7fd2-184">For more information about API registration, see [Set up API access in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span></span>

## <a name="next-steps"></a><span data-ttu-id="d7fd2-185">Další kroky</span><span class="sxs-lookup"><span data-stu-id="d7fd2-185">Next steps</span></span>

- [<span data-ttu-id="d7fd2-186">Poskytovatel řešení cloudu a místní trhy a měny, kde můžete prodávat nabídky CSP</span><span class="sxs-lookup"><span data-stu-id="d7fd2-186">Cloud Solution Provider program regional markets and currencies where you can sell CSP offers</span></span>](regional-authorization-overview.md)
