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
ms.openlocfilehash: 2171e2b10101e99bdd8d415a936ba98af65c2a1b
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502566"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="6a5f9-104">Pokyny ke konsolidaci tenantů s regionální autorizací CSP</span><span class="sxs-lookup"><span data-stu-id="6a5f9-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="6a5f9-105">**Platí pro**</span><span class="sxs-lookup"><span data-stu-id="6a5f9-105">**Applies to**</span></span>

- <span data-ttu-id="6a5f9-106">Partnerské centrum pro Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="6a5f9-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="6a5f9-107">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="6a5f9-107">**Appropriate roles**</span></span>

- <span data-ttu-id="6a5f9-108">Globální správce</span><span class="sxs-lookup"><span data-stu-id="6a5f9-108">Global admin</span></span>
- <span data-ttu-id="6a5f9-109">Agent správce</span><span class="sxs-lookup"><span data-stu-id="6a5f9-109">Admin agent</span></span>

<span data-ttu-id="6a5f9-110">\[Některé informace se vztahují na předem vydaný produkt, který se před prodejem z komerčního vydání může podstatně upravit.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-110">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="6a5f9-111">Microsoft neposkytuje žádné záruky, výslovné ani předpokládané, týkající se zde uváděných informací.\]</span><span class="sxs-lookup"><span data-stu-id="6a5f9-111">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="6a5f9-112">Můžete konsolidovat klienty pro vaši firmu.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-112">You can consolidate tenants for your business.</span></span> <span data-ttu-id="6a5f9-113">Tyto pokyny slouží ke konsolidaci klientů pro různé země nebo oblasti.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-113">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="6a5f9-114">Musíte být vědomi všech zřízené předplatných a počty licencí pro každého ze svých zákazníků v účtu, ze kterého provádíte převod.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-114">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="6a5f9-115">V rámci tohoto procesu migrace se v rámci nového účtu centrálního CSP v rámci procesu migrace znovu zřídí stejné přesně stejné odběry se stejnými počty licencí.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-115">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="6a5f9-116">Pomocí funkce seznam pro export můžete vytvořit seznam zákazníků pro přesun do centralizovaného tenanta.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-116">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="6a5f9-117">Po dokončení konsolidace se nemůžete vrátit k předchozímu stavu tenanta.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-117">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="6a5f9-118">Může se také vyžadovat akce zákazníka.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-118">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="6a5f9-119">Příprava migrace</span><span class="sxs-lookup"><span data-stu-id="6a5f9-119">Prepare for migration</span></span>

- <span data-ttu-id="6a5f9-120">Přihlaste se k **partnerskému centru**  pomocí **přechodu** účtu (ten, který převedete na nový účet), a Projděte si všechny zákazníky a všechny služby zřízené pro tyto zákazníky.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-120">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="6a5f9-121">Odhlaste se z tohoto účtu.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-121">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="6a5f9-122">Migrace zákaznických účtů</span><span class="sxs-lookup"><span data-stu-id="6a5f9-122">Migrate customer accounts</span></span>

1. <span data-ttu-id="6a5f9-123">Přihlaste se k **partnerskému centru**  pomocí účtu **přechodu** (nového) (ten, na který přecházíte zákazníky).</span><span class="sxs-lookup"><span data-stu-id="6a5f9-123">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="6a5f9-124">Vyberte **Zákazníci**.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-124">Select **Customers**.</span></span>

3. <span data-ttu-id="6a5f9-125">Vyberte **požádat o vztah prodejce**.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-125">Select **Request a reseller relationship**.</span></span> <span data-ttu-id="6a5f9-126">Zobrazí se výchozí e-mailová zpráva, která se odešle vašim zákazníkům.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-126">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="6a5f9-127">Tato zpráva obsahuje adresu URL s ID organizace, které je pro nový účet partnerského centra jedinečné.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-127">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="6a5f9-128">**Akce zákazníka:** Ujistěte se, že každý z aktivních zákazníků, které chcete migrovat, navštíví tuto adresu URL.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-128">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="6a5f9-129">Při otevření adresy URL se zobrazí výzva, abyste se přihlásili na portál Office 365.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-129">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="6a5f9-130">Zákazník se přihlásí pomocí stejného ID organizace, které používají pro přístup k portálům pro správu Azure a Office 365.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-130">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="6a5f9-131">Po přihlášení se globální správce pro **účet zákazníka** vyzve k odeslání smlouvy, která poskytuje oprávnění delegovaného správce k novému účtu CSP.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-131">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="6a5f9-132">Pokud souhlasí, zákazník vybere zaškrtávací políčko a souhlasí s autorizací vztahu.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-132">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="6a5f9-133">Zákazníci se zobrazí v seznamu zákazníků partnera po odeslání smlouvy, jednu po jednu.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-133">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="6a5f9-134">Migrace předplatných na základě využití pro Office 365 a jiné než Azure</span><span class="sxs-lookup"><span data-stu-id="6a5f9-134">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="6a5f9-135">Jakmile zákazník smlouvu podepíše, můžete znovu vytvořit své odběry v rámci centralizovaného partnerského tenanta.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-135">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="6a5f9-136">Z **partnerského centra** vyberte **zákazníci**.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-136">From **Partner Center**, select **Customers**.</span></span>

3. <span data-ttu-id="6a5f9-137">Otevřete název společnosti pro zákazníka, kterého chcete migrovat.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-137">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="6a5f9-138">Vyberte **přidat odběr**.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-138">Select **Add subscription**.</span></span>

5. <span data-ttu-id="6a5f9-139">Přidejte správné předplatné a počty licencí z katalogu.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-139">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="6a5f9-140">Ověřte s informacemi, které jsou k dispozici v **přechodu z** partnerských účtů.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-140">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="seznam zákazníků":::

6. <span data-ttu-id="6a5f9-142">Vyberte **Odeslat.**</span><span class="sxs-lookup"><span data-stu-id="6a5f9-142">Select **Submit.**</span></span>

   <span data-ttu-id="6a5f9-143">Služby jsou nyní poskytovány zákazníkovi z **přechodu na** Partnerský účet.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-143">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="6a5f9-144">Zopakováním těchto kroků migrujte odběry pro všechny další zákazníky.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-144">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="6a5f9-145">Než budete pokračovat k další části, ujistěte se, že všechna předplatná zákazníka existující v rámci **přechodu z** partnerských účtů jsou znovu zřízena v rámci **přechodu na** Partnerský účet.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-145">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="6a5f9-146">Partneři musí pozastavit odběry při **přechodu z** účtu partnerského tenanta v partnerském centru, a to za stejný den, kdy se tato předplatná přecházejí a nastavují v rámci **přechodu na** účet partnerského tenanta v partnerském centru, aby se zajistilo dvojí vyúčtování.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-146">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="6a5f9-147">Žádosti o podporu budou odepřeny pro kredity z důvodu překrytí při fakturaci, ke kterému dojde z nesprávného zákazu **přechodu z** předplatných.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-147">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="6a5f9-148">Zakázání předplatných Office 365 v rámci přechodu z partnerského účtu</span><span class="sxs-lookup"><span data-stu-id="6a5f9-148">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="6a5f9-149">Zakázáním předplatného CSP v rámci **přechodu z** partnerských účtů zastavíte jakoukoli budoucí fakturaci.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-149">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="6a5f9-150">Nemusíte ručně zakázat předplatná Azure, protože předplatná Azure se během procesu migrace automaticky vypnou.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-150">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="6a5f9-151">Přihlaste se k **partnerskému centru** pomocí **přechodu z** účtu CSP a přejděte do seznamu zákazníků.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-151">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="6a5f9-152">Otevřete zákazníka s předplatnými, které chcete zakázat, a pak vyberte první nabídku, kterou chcete zakázat.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-152">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="6a5f9-153">Nastavte předplatné na **pozastaveno** a pak vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-153">Set the subscription to **suspended**, and then select **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="6a5f9-154">Pozastavení předplatného zajistí, že nedojde k dvojímu vyúčtování.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-154">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="6a5f9-155">V seznamu předplatných se zobrazí **pozastavené** předplatné.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-155">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="6a5f9-156">Tento postup opakujte pro všechna předplatná v rámci zákazníka.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-156">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="6a5f9-157">Ověřte, že je **pozastavená** všechna zobrazení.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-157">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="6a5f9-158">Vyberte dalšího zákazníka v seznamu a opakujte postup zakázání všech předplatných.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-158">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="6a5f9-159">Migrace předplatných na základě využití Azure</span><span class="sxs-lookup"><span data-stu-id="6a5f9-159">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="6a5f9-160">Na rozdíl od předplatných CSP pro Office 365 se nemusíte migrovat ručně pomocí Azure, předplatných CSP na základě využití.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-160">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="6a5f9-161">Služba Microsoft Azure Support migruje předplatná Azure a všechny nasazené služby nebo prostředky z **přechodu z** účtů prodejců CSP na **převod na** účet prodejce CSP.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-161">Microsoft Azure Support will migrate the Azure subscriptions and all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="6a5f9-162">Během tohoto přechodu nebudete mít k dispozici žádné přerušení služby pro zákazníka.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-162">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="6a5f9-163">Ujistěte se, že účty zákazníků, které budou mít migrované předplatné Azure, přijaly smlouvu, která bude přidružená k novému **přechodu na** účet CSP.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-163">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="6a5f9-164">Budete upozorněni na to, kteří zákaznické účty budou připravené k migraci, a poskytnout jim názvy společností.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-164">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="6a5f9-165">Microsoft migruje předplatné založené na využití Azure a upozorní vás, až se migrace dokončí.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-165">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="6a5f9-166">Musíte potvrdit, že předplatné Azure v rámci **přechodu z** účtu zprostředkovatele CSP je teď označené jako **pozastavené** v partnerském centru v části Předplatná zákazníka.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-166">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="6a5f9-167">Potvrďte, že předplatné Azure v rámci **přechodu na** účet poskytovatele CSP teď zobrazuje stav **aktivní** v partnerském centru v části Předplatná zákazníka.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-167">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="6a5f9-168">Zakázáním předplatných v rámci zákazníka se nezmění vzhled zákazníka v seznamu zákazníků.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-168">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="6a5f9-169">V tuto chvíli není k dispozici možnost odebrat zákazníky ze seznamu.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-169">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="6a5f9-170">Partneři by se měli vyhnout přidání předplatného zpátky těmto zákazníkům ze svých **přechodů z** účtu v budoucnu.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-170">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="6a5f9-171">Opakujte tyto kroky u všech předplatných ve všech vašich zákaznících, abyste zastavili budoucí poplatky za **Převod z** účtů.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-171">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="6a5f9-172">Partner dostane jednu konečnou fakturu s kreditem na počet nevyužitých dní mezi dnem zrušení a posledním dnem fakturačního období.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-172">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="6a5f9-173">Po uplynutí tohoto finálního fakturačního období nebudou vygenerovány žádné budoucí faktury.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-173">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="6a5f9-174">Další informace</span><span class="sxs-lookup"><span data-stu-id="6a5f9-174">Additional information</span></span>

- <span data-ttu-id="6a5f9-175">Zakázání předplatného z **převodu z** účtu CSP nemá vliv na službu koncového zákazníka, pokud byla služba zřízená z **přechodu na** účet CSP před zakázáním předplatného.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-175">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="6a5f9-176">Předplatná nelze použít u zákazníka a při pozastavení nebo zrušení negeneruje poplatky.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-176">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="6a5f9-177">V současné době neexistuje způsob, jak úplně odebrat zákazníka ze seznamu **zákazníků** .</span><span class="sxs-lookup"><span data-stu-id="6a5f9-177">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="6a5f9-178">Partneři musí pozastavit odběry při **přechodu z** účtu partnerského tenanta v partnerském centru. stejný den jsou tato předplatná přepnuta do a nastavena v rámci **přechodu na** účet, aby se zajistilo dvojí vyúčtování.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-178">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="6a5f9-179">Společnost Microsoft nebude podporovat žádosti o kredity z důvodu překrytí při fakturaci, ke kterému dojde z nesprávného nastavení **přechodu z** předplatných na pozastaveno.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-179">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="6a5f9-180">Zjednodušení migrace pomocí exportu</span><span class="sxs-lookup"><span data-stu-id="6a5f9-180">Simplify migration using Export</span></span>

<span data-ttu-id="6a5f9-181">Pomocí **funkce exportu** můžete zachytit odběry, které je třeba použít v nové konsolidované struktuře:</span><span class="sxs-lookup"><span data-stu-id="6a5f9-181">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="6a5f9-182">Pokud chcete zobrazit seznam zákazníků, vyberte **zákazníky** v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-182">Select **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="6a5f9-183">Otevřete požadované jméno zákazníka.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-183">Open the desired customer name.</span></span>

3. <span data-ttu-id="6a5f9-184">Na stránce **předplatná** vyberte **exportovat odběry** a exportujte tak podrobnosti předplatných do excelového souboru.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-184">On the **Subscriptions** page, select **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="6a5f9-185">Pomocí tohoto seznamu můžete znovu vytvořit odběry ve vašem novém konsolidovaném tenantovi.</span><span class="sxs-lookup"><span data-stu-id="6a5f9-185">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="6a5f9-186">Registrace rozhraní API</span><span class="sxs-lookup"><span data-stu-id="6a5f9-186">API registration</span></span>

<span data-ttu-id="6a5f9-187">Další informace o registraci rozhraní API najdete v tématu [nastavení přístupu k rozhraní API v partnerském centru](/partner-center/develop/set-up-api-access-in-partner-center).</span><span class="sxs-lookup"><span data-stu-id="6a5f9-187">For more information about API registration, see [Set up API access in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span></span>

## <a name="next-steps"></a><span data-ttu-id="6a5f9-188">Další kroky</span><span class="sxs-lookup"><span data-stu-id="6a5f9-188">Next steps</span></span>

- [<span data-ttu-id="6a5f9-189">Poskytovatel řešení cloudu a místní trhy a měny, kde můžete prodávat nabídky CSP</span><span class="sxs-lookup"><span data-stu-id="6a5f9-189">Cloud Solution Provider program regional markets and currencies where you can sell CSP offers</span></span>](regional-authorization-overview.md)
