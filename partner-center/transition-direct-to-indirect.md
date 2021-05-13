---
title: Přepnutí partnera s přímým vyúčtováním na nepřímého prodejce
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak může programový partner CSP Partnerské centrum k přechodu z partnera s přímým vyúčtováním na nepřímého prodejce.
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e57ae5a30e3ee4331ae509a0650d09baf4a82590
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854889"
---
# <a name="transition-from-cloud-solution-provider-csp-direct-bill-partner-to-csp-indirect-reseller"></a><span data-ttu-id="8a538-103">Přechod z partnera CSP (Cloud Solution Provider) s přímým vyúčtováním na nepřímého prodejce CSP</span><span class="sxs-lookup"><span data-stu-id="8a538-103">Transition from Cloud Solution Provider (CSP) direct bill partner to CSP indirect reseller</span></span>

<span data-ttu-id="8a538-104">**Odpovídající role:** Globální správce</span><span class="sxs-lookup"><span data-stu-id="8a538-104">**Appropriate roles**: Global admin</span></span>

>[!Note]
><span data-ttu-id="8a538-105">Tento článek je určený pro partnery s přímým vyúčtováním, kteří se rozhodli přejít na nepřímé prodejce.</span><span class="sxs-lookup"><span data-stu-id="8a538-105">This article is intended for direct bill partners who have decided to transition to indirect resellers.</span></span> <span data-ttu-id="8a538-106">I když jste se ale ještě explicitně nerozhodla, že se zaregistrují jako nepřímý [](direct-partner-new-requirements.md) prodejce, budou partneři s přímým vyúčtováním, kteří nesplňuje nové požadavky na program partnera CSP s přímým vyúčtováním, informováni Microsoft, že jejich možnosti přímého vyúčtování budou [omezené.](restricted-direct-bill-capabilities.md)</span><span class="sxs-lookup"><span data-stu-id="8a538-106">However, even if you have not made an explicit decision yet to enroll as an indirect reseller, direct bill partners who do not meet the new [requirements](direct-partner-new-requirements.md) for the CSP direct bill partner program will be informed by Microsoft when their [direct bill capabilities will be restricted](restricted-direct-bill-capabilities.md).</span></span>
<br><span data-ttu-id="8a538-107">Od ledna 2021 se přidá nový požadavek na výnosy.</span><span class="sxs-lookup"><span data-stu-id="8a538-107">As of January 2021, a new revenue requirement will be added.</span></span> <span data-ttu-id="8a538-108">Partneři zaregistrovaní jako partner s přímým vyúčtováním budou muset v průběhu předchozích 12 měsíců provést transakce s výnosy z programu Cloud Solution Provider minimálně 300 000 USD na úrovni globálního účtu partnera.</span><span class="sxs-lookup"><span data-stu-id="8a538-108">Partners enrolled as a direct bill partner will need to have transacted at least USD$300K in Cloud Solution Provider program revenue at a Partner Global Account level over the previous 12 months.</span></span>

<span data-ttu-id="8a538-109">Do programu nepřímého prodejce se budete moct zaregistrovat pomocí stávajícího tenanta s přímým vyúčtováním.</span><span class="sxs-lookup"><span data-stu-id="8a538-109">You will be able to enroll in the indirect reseller program using your existing direct bill tenant.</span></span>

## <a name="get-started"></a><span data-ttu-id="8a538-110">Začínáme</span><span class="sxs-lookup"><span data-stu-id="8a538-110">Get started</span></span>

1. <span data-ttu-id="8a538-111">Ujistěte se, že váš profil partnera Partnerské centrum a ID MPN jsou aktuální.</span><span class="sxs-lookup"><span data-stu-id="8a538-111">Make sure your partner profile in Partner Center and MPN ID are current.</span></span>

2. <span data-ttu-id="8a538-112">Přihlaste se Partnerské centrum jako globální správce tenanta s přímým vyúčtováním, který přecházíte na nepřímého prodejce.</span><span class="sxs-lookup"><span data-stu-id="8a538-112">Sign in to Partner Center as the global admin for the direct bill tenant you are transitioning to indirect reseller.</span></span>

   :::image type="content" source="images/direct/direct1.png" alt-text="Přehled":::

3. <span data-ttu-id="8a538-114">Zkontrolujte podrobnosti o partnerovi ve formuláři registrace.</span><span class="sxs-lookup"><span data-stu-id="8a538-114">Review your partner details on the enrollment form.</span></span>

   :::image type="content" source="images/direct/direct2a.png" alt-text="Zaregistrovat":::

4. <span data-ttu-id="8a538-116">Vyberte Zaregistrovat.</span><span class="sxs-lookup"><span data-stu-id="8a538-116">Select Enroll now.</span></span> <span data-ttu-id="8a538-117">Váš nepřímý prodejce bude používat stejného tenanta AAD, který používáte pro vaši přímou firmu.</span><span class="sxs-lookup"><span data-stu-id="8a538-117">Your indirect reseller business will use the same AAD tenant you use for your direct business.</span></span>

    > [!NOTE]
    > <span data-ttu-id="8a538-118">Na začátku bude tato nová možnost přechodu dostupná pro partnery od září do prosince.</span><span class="sxs-lookup"><span data-stu-id="8a538-118">Initially, this new transition capability will be available for partners with September to December anniversary dates.</span></span> <span data-ttu-id="8a538-119">Pokud mezi zářím a prosincem nemáte datum výročí, tuto možnost v tuto chvíli neuvidíte.</span><span class="sxs-lookup"><span data-stu-id="8a538-119">If you don"t have an anniversary date between September and December, you won't see the capability at this time.</span></span> <span data-ttu-id="8a538-120">Partneři s kalendářními daty výročí po prosinci 2018 budou upozorněni později, jakmile je tato funkce pro partnery povolená.</span><span class="sxs-lookup"><span data-stu-id="8a538-120">Partners with anniversary dates after December 2018 will be notified later once the feature is enabled for the partners.</span></span>

5. <span data-ttu-id="8a538-121">Po schválení registrace se znovu přihlaste Partnerské centrum přihlášení.</span><span class="sxs-lookup"><span data-stu-id="8a538-121">When your enrollment is approved, sign in to Partner Center again.</span></span>

    > [!NOTE]
    > <span data-ttu-id="8a538-122">Schválení je obvykle okamžité, ale může trvat až pět pracovních dnů.</span><span class="sxs-lookup"><span data-stu-id="8a538-122">While approval is usually immediate, it can take up to five business days.</span></span> <span data-ttu-id="8a538-123">Po schválení obdržíte oznámení na e-mailovou adresu, kterou jste zadali v primárním kontaktu ve formuláři registrace.</span><span class="sxs-lookup"><span data-stu-id="8a538-123">Once approved, you will receive a notification to the email address you have specified under primary contact in the enrollment form.</span></span> <span data-ttu-id="8a538-124">Stav registrace můžete také ověřit v části **Nastavení**  >  **Nastavení účtu**  >  **profil partnera** > informace o programu.</span><span class="sxs-lookup"><span data-stu-id="8a538-124">You can also check your enrollment status under **Settings** > **Account Settings** > **Partner Profile** > Program info.</span></span>

6. <span data-ttu-id="8a538-125">Na stránce s **přehledem** se zobrazí smlouva nepřímý prodejce.</span><span class="sxs-lookup"><span data-stu-id="8a538-125">On your **Overview** page, you will see the indirect reseller agreement.</span></span> <span data-ttu-id="8a538-126">Vyberte **přijmout a pokračovat**.</span><span class="sxs-lookup"><span data-stu-id="8a538-126">Select **Accept and continue**.</span></span> <span data-ttu-id="8a538-127">Tato akce povoluje možnosti nepřímých prodejců.</span><span class="sxs-lookup"><span data-stu-id="8a538-127">This action enables the indirect reseller capabilities.</span></span>

<span data-ttu-id="8a538-128">Když přijmete nepřímý prodejce, Všimněte si, že váš partnerský profil vás **identifikuje jako přímý a** nepřímý prodejce.</span><span class="sxs-lookup"><span data-stu-id="8a538-128">When you have accepted the indirect reseller agreement, notice that your Partner profile identifies you as **both** a direct bill and indirect reseller.</span></span>

:::image type="content" source="images/direct/direct3.png" alt-text="Smlouva o nepřímý prodejce":::

> [!IMPORTANT]
> <span data-ttu-id="8a538-130">Po registraci jako nepřímý prodejce pomocí nové funkce není k dispozici možnost vrátit se zpět k přímému klientovi pouze s fakturací.</span><span class="sxs-lookup"><span data-stu-id="8a538-130">Once you enroll as an indirect reseller using the new capability, there is no option to roll back to a direct bill- only tenant.</span></span> <span data-ttu-id="8a538-131">Před registrací jako nepřímý prodejce prosím ověřte, že jste plně vyhodnotili své obchodní potřeby.</span><span class="sxs-lookup"><span data-stu-id="8a538-131">Please make sure that you fully evaluate your business needs before enrolling as an indirect reseller.</span></span>

## <a name="while-you-transition-from-direct-to-indirect-reseller"></a><span data-ttu-id="8a538-132">Při přechodu z přímého na nepřímý prodejce</span><span class="sxs-lookup"><span data-stu-id="8a538-132">While you transition from direct to indirect reseller</span></span>

<span data-ttu-id="8a538-133">V průběhu této fáze budete nadále spravovat požadavky vašich přímých zákazníků do předplatného, včetně fakturačního procesu.</span><span class="sxs-lookup"><span data-stu-id="8a538-133">During this phase, you will continue to manage your direct customers' subscription needs including the billing process.</span></span> <span data-ttu-id="8a538-134">Můžete také začít přijímat zákazníky od svého nepřímého poskytovatele a provozovat jako nepřímý prodejce.</span><span class="sxs-lookup"><span data-stu-id="8a538-134">You can also begin accepting customers from your Indirect provider and operating as an indirect reseller.</span></span>

:::image type="content" source="images/direct/direct4.png" alt-text="Máte přímý účet i nepřímý prodejce.":::

## <a name="find-an-indirect-provider"></a><span data-ttu-id="8a538-136">Vyhledání nepřímého poskytovatele</span><span class="sxs-lookup"><span data-stu-id="8a538-136">Find an indirect provider</span></span>

<span data-ttu-id="8a538-137">Po registraci se v levém navigačním panelu zobrazí odkaz na nepřímé poskytovatele.</span><span class="sxs-lookup"><span data-stu-id="8a538-137">After enrolling, a link to Indirect providers will appear in your left nav.</span></span> <span data-ttu-id="8a538-138">Jako nepřímý prodejce vytvoříte relaci s nepřímým poskytovatelem, který potom může zpracovávat vaše fakturace, koupit produkty pro vaše zákazníky a podporovat infrastrukturu.</span><span class="sxs-lookup"><span data-stu-id="8a538-138">As an indirect reseller you will establish a relationship with an indirect provider who then can handle your billing, purchase products for your customers, and support infrastructure.</span></span>

<span data-ttu-id="8a538-139">Různí nepřímá zprostředkovatelé nabízejí různé podpory a služby, takže byste měli vyhodnotit poskytovatele ve vaší oblasti, abyste zjistili, které z nich nejlépe vyhovují vašim potřebám.</span><span class="sxs-lookup"><span data-stu-id="8a538-139">Different indirect providers offer different support and services, so you should evaluate the providers in your area to determine which ones best meet your needs.</span></span> <span data-ttu-id="8a538-140">Obecně platí, že většina zprostředkovatelů bude:</span><span class="sxs-lookup"><span data-stu-id="8a538-140">Generally, most providers will:</span></span>

- <span data-ttu-id="8a538-141">Poskytování technického školení a pomoci</span><span class="sxs-lookup"><span data-stu-id="8a538-141">Provide you with technical training and assistance</span></span>
- <span data-ttu-id="8a538-142">Vaše produkty a služby vám pomůžou uvádět na trh.</span><span class="sxs-lookup"><span data-stu-id="8a538-142">Help you market your products and services</span></span>
- <span data-ttu-id="8a538-143">Spravujte svoje finanční a úvěrové smlouvy.</span><span class="sxs-lookup"><span data-stu-id="8a538-143">Manage your financing and credit terms</span></span>

<span data-ttu-id="8a538-144">Vyhledejte v seznamu oficiálních [zprostředkovatelů nepřímých od Microsoftu](https://partnercenter.microsoft.com/partner/find-a-provider).</span><span class="sxs-lookup"><span data-stu-id="8a538-144">Search the list of official [Microsoft indirect providers](https://partnercenter.microsoft.com/partner/find-a-provider).</span></span>

<span data-ttu-id="8a538-145">Další informace najdete v informacích  [o partnerech s nepřímými poskytovateli.](indirect-reseller-tasks-in-partner-center.md)</span><span class="sxs-lookup"><span data-stu-id="8a538-145">Learn more, read  [Partner with indirect providers](indirect-reseller-tasks-in-partner-center.md)</span></span>

## <a name="accept-a-partnership-invitation-from-your-indirect-provider"></a><span data-ttu-id="8a538-146">Přijetí pozvánky k partnerství od nepřímého poskytovatele</span><span class="sxs-lookup"><span data-stu-id="8a538-146">Accept a partnership invitation from your indirect provider</span></span>

<span data-ttu-id="8a538-147">Když najdete nepřímého poskytovatele pro partnery, navázání partnerství s nepřímým poskytovatelem v Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="8a538-147">When you find an indirect provider to partner with, establish a partnership with the indirect provider in Partner Center.</span></span>

<span data-ttu-id="8a538-148">Nepřímý poskytovatel, který vyberete, vám pošle e-mailem odkaz na pozvánku k partnerství, který vás na jeho pozvánku v Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="8a538-148">The indirect provider you select will send you in email a partnership invitation link that will take you to their invitation in Partner Center.</span></span> <span data-ttu-id="8a538-149">Ujistěte se, že se globální správce přihlásí k Partnerské centrum a že následuje odkaz na pozvánku.</span><span class="sxs-lookup"><span data-stu-id="8a538-149">Be sure your global admin signs in to Partner Center and follows the invitation link.</span></span> <span data-ttu-id="8a538-150">Když pozvánku přijmete, název poskytovatele se zobrazí v seznamu nepřímých poskytovatelů.</span><span class="sxs-lookup"><span data-stu-id="8a538-150">When you accept the invitation, the provider's name will appear in your indirect provider list.</span></span>

## <a name="acquire-new-customers-as-indirect-reseller"></a><span data-ttu-id="8a538-151">Získání nových zákazníků jako nepřímý prodejce</span><span class="sxs-lookup"><span data-stu-id="8a538-151">Acquire new customers as indirect reseller</span></span>

<span data-ttu-id="8a538-152">Vy i váš nepřímý poskytovatel musíte mít se zákazníky vztah prodejce.</span><span class="sxs-lookup"><span data-stu-id="8a538-152">Both you and your indirect provider need to have reseller relationships with customers.</span></span> <span data-ttu-id="8a538-153">Tyto vztahy s prodejcem umožňují spravovat předplatná a služby zákazníka jejich jménem.</span><span class="sxs-lookup"><span data-stu-id="8a538-153">These reseller relationships enable you to manage a customer's subscriptions and services on their behalf.</span></span> <span data-ttu-id="8a538-154">Pokud chcete získat nového zákazníka, který má existujícího tenanta Azure AD, můžete zákazníka pozvat, aby ve stejnou chvíli vytvořil vztah prodejce s vaším i vaším poskytovatelem.</span><span class="sxs-lookup"><span data-stu-id="8a538-154">To acquire a new customer who has an existing Azure AD tenant, you can invite the customer to establish a reseller relationship with both you and your provider at the same time.</span></span>

<span data-ttu-id="8a538-155">Vytvoření pozvánky nepřímého prodejce:</span><span class="sxs-lookup"><span data-stu-id="8a538-155">To create an indirect reseller invitation:</span></span>

1. <span data-ttu-id="8a538-156">V **levém navigačním** panelu Partnerské centrum možnost Nepřímí poskytovatelé.</span><span class="sxs-lookup"><span data-stu-id="8a538-156">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="8a538-157">Vyberte **Pozvat nové zákazníky,** aby pozvat zákazníka, aby navázání vztahu prodejce současně s vám i nepřímým poskytovatelem.</span><span class="sxs-lookup"><span data-stu-id="8a538-157">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="8a538-158">Poskytovatel musí mít se zákazníkem vztah prodejce, aby mohl odesílat objednávky jménem zákazníka, když chce zákazník koupit nová předplatná nebo přidat nové licence do stávajících předplatných.</span><span class="sxs-lookup"><span data-stu-id="8a538-158">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

3. <span data-ttu-id="8a538-159">Na další stránce zkontrolujte koncept e-mailové zprávy.</span><span class="sxs-lookup"><span data-stu-id="8a538-159">On the next page, review the draft email message.</span></span> <span data-ttu-id="8a538-160">Koncept zprávy můžete otevřít e-mailem nebo můžete zprávu zkopírovat do schránky a vložit ji do e-mailu.</span><span class="sxs-lookup"><span data-stu-id="8a538-160">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="8a538-161">Upravte text v e-mailu tak, abyste řekli, co potřebujete, ale nezapomeňte přidat odkaz tak, jak je přizpůsobený pro připojení zákazníka přímo k vašemu účtu i účtu poskytovatele.</span><span class="sxs-lookup"><span data-stu-id="8a538-161">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="8a538-162">Potom vyberte **Done** (Hotovo).</span><span class="sxs-lookup"><span data-stu-id="8a538-162">Then select **Done**.</span></span>

5. <span data-ttu-id="8a538-163">Po tom, co vám zákazník autorizuje a poskytovatele, aby byli prodejci záznamů, budete mít oprávnění správce ke správě svých předplatných, licencí a uživatelů jménem a váš nepřímý poskytovatel bude moci odesílat objednávky jménem.</span><span class="sxs-lookup"><span data-stu-id="8a538-163">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>
6. <span data-ttu-id="8a538-164">Pokud chcete spravovat účet, služby, uživatele a licence zákazníka, rozbalte záznam zákazníka tak, že vyberete šipku dolů v blízkosti jeho názvu.</span><span class="sxs-lookup"><span data-stu-id="8a538-164">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

<span data-ttu-id="8a538-165">Na rozdíl od přímých partnerů pro fakturaci nemůžou nepřímo prodejci vytvářet klienty Azure AD pro své nové zákazníky v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="8a538-165">Unlike direct bill partners, indirect resellers can't create Azure AD tenants for their new customers in Partner Center.</span></span> <span data-ttu-id="8a538-166">Poskytovatel vytvoří tenanta a zadá vám jako nepřímý prodejce pro tohoto zákazníka.</span><span class="sxs-lookup"><span data-stu-id="8a538-166">Your provider will create the tenant and will specify you as the indirect reseller for this customer.</span></span> <span data-ttu-id="8a538-167">Tím se zajistí, že se zákazník zobrazí v seznamu zákazníků v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="8a538-167">This ensures that the customer will appear in your customer list in Partner Center.</span></span>

>[!Note]
><span data-ttu-id="8a538-168">K vytvoření nákupu pro zákazníky, kteří získají jako nepřímý prodejce, nebudete moci využívat možnost přímé faktury.</span><span class="sxs-lookup"><span data-stu-id="8a538-168">You will not be able to use your direct bill capability to create purchases for customers you acquire as an indirect reseller.</span></span>

## <a name="managing-your-direct-bill-customers-and-your-indirect-reseller-customers"></a><span data-ttu-id="8a538-169">Správa zákazníků s přímým účtováním a zákazníky nepřímých prodejců</span><span class="sxs-lookup"><span data-stu-id="8a538-169">Managing your direct bill customers and your indirect reseller customers</span></span>

<span data-ttu-id="8a538-170">Zákazníkům s přímým účtováním můžete spravovat různé zákazníky a nepřímými prodejci.</span><span class="sxs-lookup"><span data-stu-id="8a538-170">You manage your direct bill customers and your indirect reseller customers differently.</span></span>

### <a name="direct-bill-customers-things-you-wont-do-as-an-indirect-reseller"></a><span data-ttu-id="8a538-171">Zákazníci s přímým účtováním (věci, které neuděláte jako nepřímý prodejce)</span><span class="sxs-lookup"><span data-stu-id="8a538-171">Direct bill customers (things you won't do as an indirect reseller)</span></span>

- <span data-ttu-id="8a538-172">Vytvoření objednávek pro produkty</span><span class="sxs-lookup"><span data-stu-id="8a538-172">Create orders for products</span></span>
- <span data-ttu-id="8a538-173">Správa rezervací Azure</span><span class="sxs-lookup"><span data-stu-id="8a538-173">Manage Azure reservations</span></span>
- <span data-ttu-id="8a538-174">Správa historie jejich objednávek</span><span class="sxs-lookup"><span data-stu-id="8a538-174">Manage their order history</span></span>
- <span data-ttu-id="8a538-175">Koupit software</span><span class="sxs-lookup"><span data-stu-id="8a538-175">Purchase software</span></span>
- <span data-ttu-id="8a538-176">Fakturovat zákazníky přímo</span><span class="sxs-lookup"><span data-stu-id="8a538-176">Bill customers directly</span></span>

### <a name="indirect-reseller-customers"></a><span data-ttu-id="8a538-177">Nepřímý prodejci pro zákazníky</span><span class="sxs-lookup"><span data-stu-id="8a538-177">Indirect reseller customers</span></span>

- <span data-ttu-id="8a538-178">Váš nepřímý poskytovatel objednávek produktů pro vaše zákazníky</span><span class="sxs-lookup"><span data-stu-id="8a538-178">Your indirect provider orders products for your customers</span></span>
- <span data-ttu-id="8a538-179">Správa licencí a uživatelů pro zákazníky</span><span class="sxs-lookup"><span data-stu-id="8a538-179">Manage customers' licenses and users</span></span>
- <span data-ttu-id="8a538-180">Zpracování obnovení předplatného</span><span class="sxs-lookup"><span data-stu-id="8a538-180">Handle subscription renewals</span></span>

### <a name="to-identify-customers-that-you-acquired-as-a-direct-bill-partner"></a><span data-ttu-id="8a538-181">Identifikace zákazníků, které jste získali jako přímého partnera pro fakturaci</span><span class="sxs-lookup"><span data-stu-id="8a538-181">To identify customers that you acquired as a direct bill partner</span></span>

1. <span data-ttu-id="8a538-182">Vyberte **Zákazníci**.</span><span class="sxs-lookup"><span data-stu-id="8a538-182">Select **Customers**.</span></span>

2. <span data-ttu-id="8a538-183">Vyberte zákazníka, pro který chcete zobrazit podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="8a538-183">Select a customer to view their details.</span></span>

3. <span data-ttu-id="8a538-184">Pokud je tento zákazník ten, kterého jste získali jako přímý účet pro fakturaci, zobrazí se vám možnosti pro **Přidání** nebo **zobrazení produktů** a jejich odběry se zobrazí.</span><span class="sxs-lookup"><span data-stu-id="8a538-184">If this customer is one you acquired as a direct bill partner, you will see options to **add** or **view products** and you will see their subscriptions.</span></span>

4. <span data-ttu-id="8a538-185">Pokud s váma zákazník má vztah nepřímého prodejce, nebudou tyto možnosti k dispozici.</span><span class="sxs-lookup"><span data-stu-id="8a538-185">If the customer has an indirect reseller relationship with you, those options will not be available.</span></span>

## <a name="move-your-direct-bill-customers-to-your-indirect-provider"></a><span data-ttu-id="8a538-186">Přesun zákazníků s přímým vyúčtováním na nepřímého poskytovatele</span><span class="sxs-lookup"><span data-stu-id="8a538-186">Move your direct bill customers to your indirect provider</span></span>

<span data-ttu-id="8a538-187">Váš nepřímý poskytovatel nemůže odesílat objednávky nebo stávající převody předplatných stávajícím zákazníkům s přímým vyúčtováním, dokud s nimi nemají vztah prodejce.</span><span class="sxs-lookup"><span data-stu-id="8a538-187">Your indirect provider cannot submit orders or existing subscription transfers for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="8a538-188">K navázání vztahu prodejce mezi vaším nepřímým poskytovatelem a vaším stávajícím zákazníkem s přímým vyúčtováním můžete použít jednu z následujících metod:</span><span class="sxs-lookup"><span data-stu-id="8a538-188">To establish the reseller relationship between your indirect provider and your existing direct bill customer, you can use one of the following methods:</span></span>

- [<span data-ttu-id="8a538-189">Rozšíření vztahu prodejce</span><span class="sxs-lookup"><span data-stu-id="8a538-189">Reseller relationship extension</span></span>](#reseller-relationship-extension)

- [<span data-ttu-id="8a538-190">Odeslání pozvánky nepřímého prodejce zákazníkovi</span><span class="sxs-lookup"><span data-stu-id="8a538-190">Send an indirect reseller invitation to the customer</span></span>](#send-an-indirect-reseller-invitation-to-the-customer)

<span data-ttu-id="8a538-191">Podrobný přehled tohoto podrobného procesu najdete v dokumentu Přímý na [nepřímý přechod.](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span><span class="sxs-lookup"><span data-stu-id="8a538-191">You can find a detailed overview of the step-by-step process in the [Direct to indirect transition document](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span></span>

### <a name="reseller-relationship-extension"></a><span data-ttu-id="8a538-192">Rozšíření vztahu prodejce</span><span class="sxs-lookup"><span data-stu-id="8a538-192">Reseller relationship extension</span></span>

<span data-ttu-id="8a538-193">Pomocí funkce rozšíření vztahu prodejce můžete vytvořit vztah prodejce mezi stávajícími zákazníky s přímým vyúčtováním a nepřímým poskytovatelem pomocí Partnerské centrum Dashboard.</span><span class="sxs-lookup"><span data-stu-id="8a538-193">You can use the reseller relationship extension feature to establish reseller relationship between your existing direct bill customers and your indirect provider using Partner Center Dashboard.</span></span> <span data-ttu-id="8a538-194">Než funkci začnete používat, mějte na vědomí následující:</span><span class="sxs-lookup"><span data-stu-id="8a538-194">Before using the feature, note the following:</span></span>

- <span data-ttu-id="8a538-195">Tato funkce je dostupná jenom pro partnery s přímým vyúčtováním, kteří přechádují a stanou se nepřímými prodejci, kteří dokončili registraci [nepřímého prodejce.](#get-started)</span><span class="sxs-lookup"><span data-stu-id="8a538-195">This feature is only available to direct bill partners who are transitioning to become an indirect reseller have completed the [indirect reseller enrollment](#get-started).</span></span>

- <span data-ttu-id="8a538-196">Tuto funkci můžete použít jenom u stávajících zákazníků s přímým vyúčtováním.</span><span class="sxs-lookup"><span data-stu-id="8a538-196">You can only apply this feature to existing direct bill customers.</span></span> <span data-ttu-id="8a538-197">Nelze ho použít pro zákazníky [s nepřímým prodejcem.](#acquire-new-customers-as-indirect-reseller)</span><span class="sxs-lookup"><span data-stu-id="8a538-197">It is not applicable to [indirect reseller customers](#acquire-new-customers-as-indirect-reseller).</span></span>

- <span data-ttu-id="8a538-198">Můžete vybrat pouze nepřímého poskytovatele, pro kterého jste přijali [pozvánku partnera od nepřímého poskytovatele](#accept-a-partnership-invitation-from-your-indirect-provider).</span><span class="sxs-lookup"><span data-stu-id="8a538-198">You can only select an indirect provider for which you have [accepted a partner invitation from your indirect provider](#accept-a-partnership-invitation-from-your-indirect-provider).</span></span>

- <span data-ttu-id="8a538-199">Kopie informací o vyúčtování, které máte pro tohoto zákazníka, bude k dispozici nepřímému poskytovateli.</span><span class="sxs-lookup"><span data-stu-id="8a538-199">A copy of the bill-to info you have for this customer will be made available to the indirect provider.</span></span> <span data-ttu-id="8a538-200">K informacím o vyúčtování se můžete dostat na stránku Account (Účet) pro tohoto zákazníka na Partnerské centrum Řídicí panel.</span><span class="sxs-lookup"><span data-stu-id="8a538-200">You can access the bill-to info by accessing the Account page for this customer in Partner Center Dashboard.</span></span>

    > [!NOTE]
    > <span data-ttu-id="8a538-201">Pomocí funkce rozšíření vztahu prodejce souhlasíte se sdílením informací o fakturách, které pro tohoto zákazníka máte, s nepřímým poskytovatelem.</span><span class="sxs-lookup"><span data-stu-id="8a538-201">By using the reseller relationship extension feature, you consent to sharing the bill-to info you have for this customer with the indirect provider.</span></span>

- <span data-ttu-id="8a538-202">Vašemu nepřímému poskytovateli nebudou udělena [delegovaná oprávnění správce](customers-revoke-admin-privileges.md) pro tenanta zákazníka.</span><span class="sxs-lookup"><span data-stu-id="8a538-202">Your indirect provider will not be provided with [delegated administration privileges](customers-revoke-admin-privileges.md) to the customer tenant.</span></span> <span data-ttu-id="8a538-203">Pokud váš nepřímý poskytovatel vyžaduje delegovaná oprávnění pro správu, musíte zákazníkovi místo toho poslat pozvánku nepřímého prodejce.</span><span class="sxs-lookup"><span data-stu-id="8a538-203">If your indirect provider requires delegated administration privileges, you must send an indirect reseller invitation to the customer instead.</span></span>

- <span data-ttu-id="8a538-204">Po navázání vztahu prodejce se nepřímý poskytovatel zobrazí jako partner CSP na stránce vztahy s partnery v [centru pro správu Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/partners) a [Microsoft Store pro firmy](/microsoft-store/work-with-partner-microsoft-store-business).</span><span class="sxs-lookup"><span data-stu-id="8a538-204">Once the reseller relationship is established, the indirect provider will appear as a CSP partner to the customer under the Partner Relationships page in [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/partners) and [Microsoft Store for Business](/microsoft-store/work-with-partner-microsoft-store-business).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="8a538-205">Aby nedocházelo k nejasnostem a nepochopení, jste si smluvní partnerskou smlouvou informovali o souhlasu zákazníka s přímým vyúčtováním a získat souhlas s tím, než použijete funkci rozšíření relace k vytvoření vztahu prodejce mezi stávajícím zákazníkem s přímým fakturací a nepřímým poskytovatelem.</span><span class="sxs-lookup"><span data-stu-id="8a538-205">To avoid confusion and misunderstanding, you are contractually obliged by your partner agreement to inform and obtain consent from the direct bill customer before you use the relationship extension feature to establish reseller relationship between an existing direct bill customer and an indirect provider.</span></span>

<span data-ttu-id="8a538-206">Pokud chcete tuto funkci použít u stávajícího tenanta zákazníka:</span><span class="sxs-lookup"><span data-stu-id="8a538-206">To use this feature on an existing customer tenant:</span></span>

1. <span data-ttu-id="8a538-207">Přihlaste se do partnerského centra jako **Agent pro správu**.</span><span class="sxs-lookup"><span data-stu-id="8a538-207">Log in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="8a538-208">Na **stránce zákazníci** vyberte existujícího zákazníka a kliknutím na ikonu **rychlých odkazů** rozbalte souhrnné zobrazení zákazníka.</span><span class="sxs-lookup"><span data-stu-id="8a538-208">In the **Customers page**, select an existing customer and click on its **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="8a538-209">V části **nepřímé zprostředkovatele** klikněte na **přenést zákazníka u nepřímého poskytovatele**.</span><span class="sxs-lookup"><span data-stu-id="8a538-209">Under **Indirect provider(s)**, click **Transfer customer on an indirect provider**.</span></span>

    :::image type="content" source="images/direct/direct5-1.png" alt-text="Přenést zákazníka na nepřímý poskytovatel":::

4. <span data-ttu-id="8a538-211">V místním dialogovém okně vyberte **nepřímý zprostředkovatel** , který chcete, aby se zákazníkem zobrazoval vztah prodejce.</span><span class="sxs-lookup"><span data-stu-id="8a538-211">In the pop-up dialog, select the **Indirect Provider** you would like to have reseller relationship with the customer.</span></span>

5. <span data-ttu-id="8a538-212">Klikněte na **Uložit a pokračujte**.</span><span class="sxs-lookup"><span data-stu-id="8a538-212">Click **Save and continue**.</span></span>

6. <span data-ttu-id="8a538-213">Ověřte, zda se vybraný nepřímý zprostředkovatel zobrazuje v části **nepřímá zprostředkovatelé**.</span><span class="sxs-lookup"><span data-stu-id="8a538-213">Verify the selected indirect provider shows up under **Indirect provider(s)**.</span></span>

    :::image type="content" source="images/direct/direct5-2.png" alt-text="Seznam nepřímých poskytovatelů":::

### <a name="send-an-indirect-reseller-invitation-to-the-customer"></a><span data-ttu-id="8a538-215">Odeslání pozvánky k nepřímému prodejci zákazníkovi</span><span class="sxs-lookup"><span data-stu-id="8a538-215">Send an indirect reseller invitation to the customer</span></span>

<span data-ttu-id="8a538-216">Váš nepřímý poskytovatel nemůže odesílat objednávky pro vaše stávající zákazníky s přímým účtováním, dokud nebudou mít k těmto zákazníkům vztah prodejce.</span><span class="sxs-lookup"><span data-stu-id="8a538-216">Your indirect provider cannot submit orders for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="8a538-217">Pokud chcete zřídit vztah prodejce mezi stávajícími zákazníky a vaším nepřímým poskytovatelem, pozvěte zákazníka pomocí nepřímých pozvání prodejce.</span><span class="sxs-lookup"><span data-stu-id="8a538-217">To establish the reseller relationship between your existing customers and your indirect provider, invite the customer using an indirect reseller invitation.</span></span>

1. <span data-ttu-id="8a538-218">Výběr **nepřímých zprostředkovatelů** z partnerského centra s levou navigací</span><span class="sxs-lookup"><span data-stu-id="8a538-218">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="8a538-219">Vyberte **pozvat nové zákazníky** a pozvat zákazníka k navázání vztahu prodejce s vámi i nepřímým poskytovatelem ve stejnou dobu.</span><span class="sxs-lookup"><span data-stu-id="8a538-219">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="8a538-220">Poskytovatel musí mít k vašemu zákazníkovi vztah prodejce, aby mohl odeslat objednávky jménem zákazníka, pokud chce zákazník koupit nové předplatné nebo přidat nové licence k existujícím předplatným.</span><span class="sxs-lookup"><span data-stu-id="8a538-220">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

    :::image type="content" source="images/direct/direct6.png" alt-text="Pozvání nových zákazníků":::

3. <span data-ttu-id="8a538-222">Na další stránce zkontrolujte koncept e-mailové zprávy.</span><span class="sxs-lookup"><span data-stu-id="8a538-222">On the next page, review the draft email message.</span></span> <span data-ttu-id="8a538-223">Koncept zprávy můžete otevřít e-mailem nebo můžete zprávu zkopírovat do schránky a vložit ji do e-mailu.</span><span class="sxs-lookup"><span data-stu-id="8a538-223">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="8a538-224">Upravte text v e-mailu tak, abyste řekli, co potřebujete, ale nezapomeňte přidat odkaz tak, jak je přizpůsobený pro připojení zákazníka přímo k vašemu účtu i účtu poskytovatele.</span><span class="sxs-lookup"><span data-stu-id="8a538-224">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="8a538-225">Potom vyberte **Done** (Hotovo).</span><span class="sxs-lookup"><span data-stu-id="8a538-225">Then select **Done**.</span></span>

5. <span data-ttu-id="8a538-226">Jakmile zákazník udělí vám a vašemu poskytovateli oprávnění k záznamu, budete mít oprávnění správce ke správě jejich předplatných, licencí a uživatelů jejich jménem a nepřímý poskytovatel bude moct odesílat objednávky jejich jménem.</span><span class="sxs-lookup"><span data-stu-id="8a538-226">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>

6. <span data-ttu-id="8a538-227">Pokud chcete spravovat účet zákazníka, služby, uživatele a licence, rozbalte záznam zákazníka výběrem šipky dolů vedle jeho jména.</span><span class="sxs-lookup"><span data-stu-id="8a538-227">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

### <a name="microsoft-customer-agreement-acceptance"></a><span data-ttu-id="8a538-228">Smlouva se zákazníkem Microsoftu přijetí</span><span class="sxs-lookup"><span data-stu-id="8a538-228">Microsoft Customer Agreement acceptance</span></span>

<span data-ttu-id="8a538-229">Smlouva o službách Microsoft Cloud platná do 31. ledna 2020.</span><span class="sxs-lookup"><span data-stu-id="8a538-229">Microsoft Cloud Agreement is valid until January 31, 2020.</span></span> <span data-ttu-id="8a538-230">Po tomto datu musí všichni zákazníci, stávající i noví, podepsat novou [Smlouva se zákazníkem Microsoftu](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="8a538-230">After that date, all customers, existing and new, must sign the new [Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span> <span data-ttu-id="8a538-231">Pro přechádující zákazníky, pokud:</span><span class="sxs-lookup"><span data-stu-id="8a538-231">For transitioning customers, if:</span></span>

- <span data-ttu-id="8a538-232">**Zákazník ještě nepřijal Smlouva se zákazníkem Microsoftu.**</span><span class="sxs-lookup"><span data-stu-id="8a538-232">**Customer has not accepted Microsoft Customer Agreement yet**</span></span>

   <span data-ttu-id="8a538-233">Obraťte se na nepřímého poskytovatele, aby zákazník [přijal Smlouva se zákazníkem Microsoftu](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="8a538-233">Please work with Indirect Provider to have customer [accept the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

- <span data-ttu-id="8a538-234">**Zákazník s Smlouva se zákazníkem Microsoftu přijal přístup prostřednictvím centra Microsoft 365 pro správu.**</span><span class="sxs-lookup"><span data-stu-id="8a538-234">**Customer has accepted Microsoft Customer Agreement with you through the Microsoft 365 Admin Center**</span></span>

   <span data-ttu-id="8a538-235">Přijetí se zachová po na navázatí vztahu prodejce s nepřímým poskytovatelem.</span><span class="sxs-lookup"><span data-stu-id="8a538-235">The acceptance will be retained once the reseller relationship is established with the Indirect Provider.</span></span> <span data-ttu-id="8a538-236">Není nic, co byste měli udělat.</span><span class="sxs-lookup"><span data-stu-id="8a538-236">There is nothing you need to do.</span></span>

- <span data-ttu-id="8a538-237">**Zákazník s Smlouva se zákazníkem Microsoftu prostřednictvím ověření partnerem**</span><span class="sxs-lookup"><span data-stu-id="8a538-237">**Customer has accepted Microsoft Customer Agreement with you through partner attestation**</span></span>

   <span data-ttu-id="8a538-238">Přijetí se nezachová.</span><span class="sxs-lookup"><span data-stu-id="8a538-238">The acceptance will not be retained.</span></span> <span data-ttu-id="8a538-239">Obraťte se na nepřímého poskytovatele [a aktualizujte souhlas zákazníka v Partnerské centrum](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span><span class="sxs-lookup"><span data-stu-id="8a538-239">Please work with Indirect Provider to [update the customer's acceptance in Partner Center](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span></span>

## <a name="transfer-existing-direct-bill-subscriptions-to-indirect-provider"></a><span data-ttu-id="8a538-240">Převod stávajících předplatných s přímým vyúčtováním na nepřímého poskytovatele</span><span class="sxs-lookup"><span data-stu-id="8a538-240">Transfer existing direct bill subscriptions to indirect provider</span></span>

<span data-ttu-id="8a538-241">V rámci nepřímého modelu CSP nemají nepřímí prodejci fakturační vztahy s Microsoftem.</span><span class="sxs-lookup"><span data-stu-id="8a538-241">Under CSP indirect model, indirect resellers do not have billing relationships with Microsoft.</span></span> <span data-ttu-id="8a538-242">Místo toho nepřímí prodejci získali předplatná pro své zákazníky prostřednictvím svých nepřímých poskytovatelů.</span><span class="sxs-lookup"><span data-stu-id="8a538-242">Instead, indirect resellers obtain subscriptions for their customers through their indirect providers.</span></span> <span data-ttu-id="8a538-243">Při přechodu z přímého poštovního partnera na nepřímý prodejce budete potřebovat přenést existující předplatná, která máte jako přímého dodavatele, do svého nepřímého poskytovatele.</span><span class="sxs-lookup"><span data-stu-id="8a538-243">While transitioning from direct bill partner to indirect reseller, you need to transfer the existing subscriptions you have as the direct bill partner to your indirect provider.</span></span> <span data-ttu-id="8a538-244">K tomu můžete použít funkci převodu předplatného pro samoobslužné partnery v řídicím panelu partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="8a538-244">You can use the self-served subscription transfer feature in Partner Center Dashboard to do so.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="8a538-245">Požadavky</span><span class="sxs-lookup"><span data-stu-id="8a538-245">Prerequisites</span></span>

- <span data-ttu-id="8a538-246">Tato funkce je k dispozici jenom pro přechod partnerů, kteří dokončili nepřímý zápis prodejce pomocí svých stávajících partnerských tenantů pro klienty s přímým přístupem.</span><span class="sxs-lookup"><span data-stu-id="8a538-246">This feature is only available to transitioning partners who have completed the indirect reseller enrollment using their existing direct bill partner tenants.</span></span>

- <span data-ttu-id="8a538-247">Před převodem předplatných přidružených k danému zákazníkovi musí přechod partner přesunout zákazníka na nepřímýho poskytovatele.</span><span class="sxs-lookup"><span data-stu-id="8a538-247">Before transferring subscriptions associated with a given customer, the transitioning partner must move the customer to an indirect provider.</span></span>

- <span data-ttu-id="8a538-248">Zákazník musí [přijmout smlouvu o zákaznících Microsoftu prostřednictvím nepřímého poskytovatele](#microsoft-customer-agreement-acceptance).</span><span class="sxs-lookup"><span data-stu-id="8a538-248">Customer must have [accepted Microsoft Customer Agreement through the Indirect Provider](#microsoft-customer-agreement-acceptance).</span></span>

### <a name="how-to-transition-to-indirect-reseller-status"></a><span data-ttu-id="8a538-249">Přechod na stav nepřímý prodejce</span><span class="sxs-lookup"><span data-stu-id="8a538-249">How to transition to indirect reseller status</span></span>

<span data-ttu-id="8a538-250">Tato funkce je 4 kroky procesu, kde:</span><span class="sxs-lookup"><span data-stu-id="8a538-250">The feature is a 4-step process, where:</span></span>

- <span data-ttu-id="8a538-251">Přechodná partner vytvoří požadavek na převod předplatného.</span><span class="sxs-lookup"><span data-stu-id="8a538-251">The transitioning partner creates a subscription transfer request.</span></span> <span data-ttu-id="8a538-252">Požadavek obsahuje jedno nebo více stávajících předplatných přidružených ke stejnému zákazníkovi a je adresováno nepřímému poskytovateli.</span><span class="sxs-lookup"><span data-stu-id="8a538-252">The request contains one or more existing subscriptions associated with the same customer and is addressed to an indirect provider.</span></span>

- <span data-ttu-id="8a538-253">Nepřímý poskytovatel kontroluje a přijímá (nebo odmítne) žádost o přenos.</span><span class="sxs-lookup"><span data-stu-id="8a538-253">The indirect provider reviews and accepts (or reject) the transfer request.</span></span>

- <span data-ttu-id="8a538-254">Nepřímý poskytovatel ověří, jestli je žádost o přenos dokončená.</span><span class="sxs-lookup"><span data-stu-id="8a538-254">The indirect provider verifies that the transfer request is complete.</span></span>

- <span data-ttu-id="8a538-255">Přechodná partner ověří, jestli je žádost o přenos dokončená.</span><span class="sxs-lookup"><span data-stu-id="8a538-255">The transitioning partner verifies that the transfer request is complete.</span></span>

### <a name="transitioning-partner"></a><span data-ttu-id="8a538-256">Přechod k partnerovi</span><span class="sxs-lookup"><span data-stu-id="8a538-256">Transitioning partner</span></span>

> [!NOTE]
> <span data-ttu-id="8a538-257">K přenosu stávajících předplatných do nepřímého poskytovatele můžete také použít [rozhraní API a sadu SDK pro partnery](/partner-center/develop/manage-customers) .</span><span class="sxs-lookup"><span data-stu-id="8a538-257">You can also use [Partner Center API/SDK](/partner-center/develop/manage-customers) to transfer the existing subscriptions to your indirect provider.</span></span>
>
> - [<span data-ttu-id="8a538-258">Získání způsobilosti pro převod předplatných zákazníka</span><span class="sxs-lookup"><span data-stu-id="8a538-258">Get a customer's subscriptions transfer eligibility</span></span>](/partner-center/develop/get-customer-s-subscriptions-transfer-eligibility)
> - [<span data-ttu-id="8a538-259">Vytvoření převodu pro zákazníka</span><span class="sxs-lookup"><span data-stu-id="8a538-259">Create a customer's transfer</span></span>](/partner-center/develop/create-a-transfer)
> - [<span data-ttu-id="8a538-260">Odvolání převodu pro zákazníka</span><span class="sxs-lookup"><span data-stu-id="8a538-260">Withdraw a customer's transfer</span></span>](/partner-center/develop/withdraw-a-transfer)
> - [<span data-ttu-id="8a538-261">Potvrzení převodu pro zákazníka</span><span class="sxs-lookup"><span data-stu-id="8a538-261">Accept a customer's transfer</span></span>](/partner-center/develop/accept-a-transfer)
> - [<span data-ttu-id="8a538-262">Odmítnout přenos zákazníka</span><span class="sxs-lookup"><span data-stu-id="8a538-262">Reject a Customer's transfer</span></span>](/partner-center/develop/reject-a-transfer)
> - [<span data-ttu-id="8a538-263">Získání převodů zákazníka</span><span class="sxs-lookup"><span data-stu-id="8a538-263">Get a customer's transfers</span></span>](/partner-center/develop/get-all-of-a-customer-s-transfers)
> - [<span data-ttu-id="8a538-264">Získat podrobnosti o přenosu podle ID</span><span class="sxs-lookup"><span data-stu-id="8a538-264">Get transfer details by id</span></span>](/partner-center/develop/get-transfer-by-id)

### <a name="transitioning-partner---create-transfer-request"></a><span data-ttu-id="8a538-265">Převod partnera – vytvoření žádosti o přenos</span><span class="sxs-lookup"><span data-stu-id="8a538-265">Transitioning partner - create transfer request</span></span>

<span data-ttu-id="8a538-266">Postup při vytváření žádosti o převod jako převádění partnera:</span><span class="sxs-lookup"><span data-stu-id="8a538-266">To create a transfer request as the transitioning partner:</span></span>

1. <span data-ttu-id="8a538-267">Přihlaste se do partnerského centra jako **Agent pro správu**.</span><span class="sxs-lookup"><span data-stu-id="8a538-267">Log in to Partner Center as an **Admin Agent**.</span></span>

2. <span data-ttu-id="8a538-268">Na stránce **zákazníci** vyberte zamýšleného zákazníka a kliknutím na ikonu Rychlé odkazy rozbalte souhrnné zobrazení zákazníka.</span><span class="sxs-lookup"><span data-stu-id="8a538-268">In the **Customers** page, select the intended customer and click on the Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="8a538-269">V **části Nepřímí poskytovatelé** ověřte, že je uvedený zamýšlený nepřímý poskytovatel.</span><span class="sxs-lookup"><span data-stu-id="8a538-269">Under **Indirect provider(s)**, confirm that the intended indirect provider is listed.</span></span>

4. <span data-ttu-id="8a538-270">Klikněte **na Zobrazit předplatná.**</span><span class="sxs-lookup"><span data-stu-id="8a538-270">Click **View Subscriptions**.</span></span>

5. <span data-ttu-id="8a538-271">Na stránce **Předplatná** vyhledejte **Předplatná Transfer**.</span><span class="sxs-lookup"><span data-stu-id="8a538-271">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

6. <span data-ttu-id="8a538-272">V **části Převod předplatného** klikněte na **Požádat o převod předplatného.**</span><span class="sxs-lookup"><span data-stu-id="8a538-272">Under **Subscription Transfer**, click **Request subscription transfer**.</span></span>

    :::image type="content" source="images/direct/direct8.png" alt-text="Žádost o převod předplatného":::

7. <span data-ttu-id="8a538-274">V dialogovém okně žádosti o převod vyberte jedno nebo více předplatných, která chcete převést.</span><span class="sxs-lookup"><span data-stu-id="8a538-274">In the transfer request dialog, select one or more subscriptions to be transferred.</span></span>

    :::image type="content" source="images/direct/direct9.png" alt-text="Vytvoření žádosti o převod":::

8. <span data-ttu-id="8a538-276">Klikněte na **Vytvořit**.</span><span class="sxs-lookup"><span data-stu-id="8a538-276">Click **Create**.</span></span>

9. <span data-ttu-id="8a538-277">V části Převod předplatného se zobrazí aktivní **žádost o převod předplatného.**</span><span class="sxs-lookup"><span data-stu-id="8a538-277">An active subscription transfer request will appear under **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct10.png" alt-text="Seznam žádostí o převod":::

10. <span data-ttu-id="8a538-279">Informujte nepřímého poskytovatele, že jste pro tohoto poskytovatele vytvořili žádost o převod předplatného.</span><span class="sxs-lookup"><span data-stu-id="8a538-279">Inform your indirect provider that you have created a subscription transfer request to them.</span></span>

### <a name="indirect-provider---accept-transfer-request"></a><span data-ttu-id="8a538-280">Nepřímý poskytovatel – přijetí žádosti o převod</span><span class="sxs-lookup"><span data-stu-id="8a538-280">Indirect provider - accept transfer request</span></span>

<span data-ttu-id="8a538-281">Kontrola a přijetí žádosti o převod jako nepřímý poskytovatel:</span><span class="sxs-lookup"><span data-stu-id="8a538-281">To review and accept a transfer request as the indirect provider:</span></span>

1. <span data-ttu-id="8a538-282">Přihlaste se k Partnerské centrum **jako agent pro** správu nebo **prodejní agent.**</span><span class="sxs-lookup"><span data-stu-id="8a538-282">Log in to Partner Center as an **Admin** Agent or **Sales Agent**.</span></span>

2. <span data-ttu-id="8a538-283">Na stránce **Zákazníci** vyberte zamýšleného zákazníka a kliknutím na jeho ikonu Rychlé odkazy rozbalte souhrnné zobrazení zákazníka.</span><span class="sxs-lookup"><span data-stu-id="8a538-283">In the **Customers** page, select the intended customer and click on its Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="8a538-284">V **části Nepřímí prodejci** potvrďte, že je uvedený přecházující partner.</span><span class="sxs-lookup"><span data-stu-id="8a538-284">Under **Indirect reseller(s)**, confirm the transitioning partner is listed.</span></span>

4. <span data-ttu-id="8a538-285">Klikněte **na Zobrazit předplatná.**</span><span class="sxs-lookup"><span data-stu-id="8a538-285">Click **View Subscriptions**.</span></span>

5. <span data-ttu-id="8a538-286">Na stránce **Předplatná** vyhledejte **Předplatná Transfer**.</span><span class="sxs-lookup"><span data-stu-id="8a538-286">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

    :::image type="content" source="images/direct/direct11.png" alt-text="Zobrazení žádosti o převod":::

6. <span data-ttu-id="8a538-288">V **části Převod předplatného** klikněte na žádost o převod, která se má zkontrolovat.</span><span class="sxs-lookup"><span data-stu-id="8a538-288">Under **Subscription Transfer**, click on the transfer request to review.</span></span>

7. <span data-ttu-id="8a538-289">Podle **potřeby klikněte** na Přijmout **(nebo** Odmítnout).</span><span class="sxs-lookup"><span data-stu-id="8a538-289">Click **Accept** (or **Reject**) as appropriate.</span></span>

    :::image type="content" source="images/direct/direct12.png" alt-text="Přijmout žádost o přenos":::

8. <span data-ttu-id="8a538-291">Počkejte, až se žádost o přenos dokončí.</span><span class="sxs-lookup"><span data-stu-id="8a538-291">Wait for the transfer request to complete.</span></span>

### <a name="indirect-provider---verify-transfer-request-is-complete"></a><span data-ttu-id="8a538-292">Nepřímý Zprostředkovatel – ověření žádosti o přenos je dokončeno</span><span class="sxs-lookup"><span data-stu-id="8a538-292">Indirect provider - verify transfer request is complete</span></span>

1. <span data-ttu-id="8a538-293">Po úspěšném dokončení žádosti o přenos ověřte, že se předplatná zobrazí v části **předplatná**.</span><span class="sxs-lookup"><span data-stu-id="8a538-293">After the transfer request is completed successfully, verify that you can see the subscriptions appear under **Subscriptions**.</span></span>

2. <span data-ttu-id="8a538-294">Informujte tohoto přecházejícího partnera.</span><span class="sxs-lookup"><span data-stu-id="8a538-294">Inform the transitioning partner.</span></span>

### <a name="transitioning-partner---verify-transfer-request-is-complete"></a><span data-ttu-id="8a538-295">Přechod k partnerovi – ověření žádosti o přenos je dokončené.</span><span class="sxs-lookup"><span data-stu-id="8a538-295">Transitioning partner - verify transfer request is complete</span></span>

<span data-ttu-id="8a538-296">Převedený partner by měl provádět tyto akce:</span><span class="sxs-lookup"><span data-stu-id="8a538-296">The transitioning partner should do the following:</span></span>

1. <span data-ttu-id="8a538-297">Přihlaste se k partnerskému centru jako **Agent pro správu** nebo **agenta prodeje**.</span><span class="sxs-lookup"><span data-stu-id="8a538-297">Sign into Partner Center as an **Admin Agent** or **Sales Agent**.</span></span>

2. <span data-ttu-id="8a538-298">Na stránce **zákazníci** vyberte zamýšleného zákazníka a kliknutím na ikonu **Rychlé odkazy** rozbalte souhrnné zobrazení zákazníka.</span><span class="sxs-lookup"><span data-stu-id="8a538-298">In the **Customers** page, select the intended customer and click on the **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="8a538-299">Klikněte na **Zobrazit předplatná**.</span><span class="sxs-lookup"><span data-stu-id="8a538-299">Click **View Subscriptions**.</span></span>

4. <span data-ttu-id="8a538-300">Na stránce **předplatná** vyhledejte **přenos předplatného**.</span><span class="sxs-lookup"><span data-stu-id="8a538-300">In the **Subscriptions** page, look for **Subscription Transfer**.</span></span>

5. <span data-ttu-id="8a538-301">Ověřte, zda je žádost o přenos označena jako **Úplná**.</span><span class="sxs-lookup"><span data-stu-id="8a538-301">Verify that the transfer request is marked as **Complete**.</span></span>

6. <span data-ttu-id="8a538-302">Ověřte, že odběry se na stránce **předplatná** již nezobrazuje jako aktivní:</span><span class="sxs-lookup"><span data-stu-id="8a538-302">Verify that the subscription(s) no longer appear as active in the **Subscriptions** page:</span></span>

   1. <span data-ttu-id="8a538-303">Pokud se jedná o předplatné Azure (MS-AZR-0145P), nebude se už v seznamu zobrazovat.</span><span class="sxs-lookup"><span data-stu-id="8a538-303">If this is an Azure subscription (MS-AZR-0145P), it will no longer be listed.</span></span>

   2. <span data-ttu-id="8a538-304">Pokud se jedná o předplatné založené na licencích (Office 365, Dynamics, Intune), zobrazí se v seznamu stav **pozastaveno**.</span><span class="sxs-lookup"><span data-stu-id="8a538-304">If this is a license-based subscription (Office 365, Dynamics, Intune), it will be listed with state as **Suspended**.</span></span>

   :::image type="content" source="images/direct/direct13.png" alt-text="Předplatné pozastaveno":::

### <a name="considerations"></a><span data-ttu-id="8a538-306">Požadavky</span><span class="sxs-lookup"><span data-stu-id="8a538-306">Considerations</span></span>

- <span data-ttu-id="8a538-307">**ID předplatného bude po přenosu jiné.**</span><span class="sxs-lookup"><span data-stu-id="8a538-307">**Subscription ID will be different after transfer.**</span></span> <span data-ttu-id="8a538-308">Pokud se jedná o předplatné Azure (MS-AZR-0145P), bude mít navíc ID předplatného Azure, které se zachová od předchozího vlastníka a zobrazí se na portálu pro správu Azure.</span><span class="sxs-lookup"><span data-stu-id="8a538-308">If it is an Azure subscription (MS-AZR-0145P), additionally, it will have an Azure Subscription ID, which is retained from the previous owner, and will appear in the Azure management portal.</span></span>

- <span data-ttu-id="8a538-309">**Na stejné předplatné nemůže odkazovat více požadavků na přenos.**</span><span class="sxs-lookup"><span data-stu-id="8a538-309">**The same subscription cannot be referenced by multiple transfer requests.**</span></span> <span data-ttu-id="8a538-310">Po vytvoření žádosti o přenos, která zahrnuje existující předplatné, nemůžete vytvořit další požadavky na přenos, včetně stejného předplatného, až do chvíle, kdy se první požadavek na přenos zruší.</span><span class="sxs-lookup"><span data-stu-id="8a538-310">After you have created a transfer request, which includes an existing subscription, you cannot create additional transfer requests including the same subscription, until the first transfer request is canceled.</span></span>

- <span data-ttu-id="8a538-311">**Doplňky pro předplatná založená na licencích se musí převést společně se svým základním předplatným.**</span><span class="sxs-lookup"><span data-stu-id="8a538-311">**Add-ons for license-based subscriptions must be transferred along with their base subscription.**</span></span> <span data-ttu-id="8a538-312">Pokud při vytváření žádosti o převod vyberete existující předplatné s jedním nebo více doplňky, do žádosti o převod se automaticky zahrnou doplňky.</span><span class="sxs-lookup"><span data-stu-id="8a538-312">When creating a transfer request, if you pick an existing subscription with one or more add-ons, the add-ons will automatically be included in the transfer request.</span></span>

- <span data-ttu-id="8a538-313">**Změny počtu licencí v předplatném se ve stávající žádosti o převod neprojeví.**</span><span class="sxs-lookup"><span data-stu-id="8a538-313">**License count changes to a subscription will not be reflected in existing transfer request.**</span></span> <span data-ttu-id="8a538-314">Po vytvoření žádosti o převod, která zahrnuje stávající předplatné, byste se měli vyhnout aktualizaci počtu licencí předplatného (nebo přidružených doplňků).</span><span class="sxs-lookup"><span data-stu-id="8a538-314">After you have created a transfer request which includes an existing subscription, you should avoid updating the license quantity of the subscription (or associated addons).</span></span> <span data-ttu-id="8a538-315">Pokud tak neučiníte, nové množství se v žádosti o převod neprojeví.</span><span class="sxs-lookup"><span data-stu-id="8a538-315">If you do so, the new quantity will not be reflected in the transfer request.</span></span> <span data-ttu-id="8a538-316">Jakmile nepřímý poskytovatel přijme žádost o převod, bude mít výsledné předplatné staré množství.</span><span class="sxs-lookup"><span data-stu-id="8a538-316">After the indirect provider accepts the transfer request, the resultant subscription will have the old quantity.</span></span> <span data-ttu-id="8a538-317">Pokud chcete nové množství převést na nepřímého poskytovatele, musíte zrušit stávající žádost o převod a znovu vytvořit novou.</span><span class="sxs-lookup"><span data-stu-id="8a538-317">If you wish for the new quantity to be transferred to the indirect provider, you must cancel the existing transfer request and recreate a new one.</span></span>

- <span data-ttu-id="8a538-318">**Ne všechny nákupy je možné převést pomocí samoobslužných převodů předplatného.**</span><span class="sxs-lookup"><span data-stu-id="8a538-318">**Not all purchases can be transferred using self-served subscription transfer.**</span></span> <span data-ttu-id="8a538-319">V současné době můžete pomocí této funkce přenášet pouze předplatná O365 a předplatná Azure PAYG (MS-AZR-0145P).</span><span class="sxs-lookup"><span data-stu-id="8a538-319">Currently, you can only transfer O365 subscriptions and Azure PAYG subscriptions (MS-AZR-0145P) using this feature.</span></span> <span data-ttu-id="8a538-320">Ostatní nákupy, včetně plánů Azure, rezervovaných instancí Azure, předplatných založených na termínech a předplatných SaaS pro Azure Marketplace se nepodporují.</span><span class="sxs-lookup"><span data-stu-id="8a538-320">Other purchases including Azure Plans, Azure Reserved Instances, Term-based Subscriptions and SaaS subscriptions for Azure Marketplace are not supported.</span></span> <span data-ttu-id="8a538-321">Na stránce odeslání žádosti o převod se zobrazí důvod, proč předplatné není možné převést.</span><span class="sxs-lookup"><span data-stu-id="8a538-321">You will see a reason why a subscription cannot be transferred in the submit transfer request page.</span></span> <span data-ttu-id="8a538-322">Pokud chcete tato předplatná [](create-a-new-subscription.md#suspend-or-cancel-a-subscription) převést, musíte zrušit stávající předplatné a zakoupit novou nabídku pro zákazníka prostřednictvím nepřímého poskytovatele.</span><span class="sxs-lookup"><span data-stu-id="8a538-322">To transfer these subscriptions, you will need to [cancel the existing subscription](create-a-new-subscription.md#suspend-or-cancel-a-subscription) and purchase new offer for customer through Indirect Provider.</span></span>

- <span data-ttu-id="8a538-323">**Nelze testovat pomocí prostředí sandboxu.**</span><span class="sxs-lookup"><span data-stu-id="8a538-323">**Cannot be tested using sandbox environment.**</span></span>

## <a name="enroll-for-indirect-reseller-incentives"></a><span data-ttu-id="8a538-324">Registrace pro pobídky nepřímých prodejců</span><span class="sxs-lookup"><span data-stu-id="8a538-324">Enroll for indirect reseller incentives</span></span>

<span data-ttu-id="8a538-325">Po úspěšné registraci jako nepřímý prodejce ve stávajícím tenantovi partnera s přímým vyúčtováním obdržíte během 30 dnů pozvánku k registraci do pobídek nepřímých prodejců.</span><span class="sxs-lookup"><span data-stu-id="8a538-325">After you have successfully enrolled as an indirect reseller on your existing direct bill partner tenant, you will receive an invitation to enroll for indirect reseller incentive within 30 days.</span></span> <span data-ttu-id="8a538-326">Pozvánka je založená na partnerském účtu MPN, který je aktuálně přidružený k vašemu tenantovi partnera CSP.</span><span class="sxs-lookup"><span data-stu-id="8a538-326">The invitation is based on the partner MPN account that is currently associated with your CSP partner tenant.</span></span> <span data-ttu-id="8a538-327">Pozvánka se pošle na e-mailovou adresu přidruženou k partnerskému účtu MPN.</span><span class="sxs-lookup"><span data-stu-id="8a538-327">The invitation will be sent to the email address associated with the partner MPN account.</span></span>

<span data-ttu-id="8a538-328">Máte taky nárok na registraci k programům pro přímé vyúčtování pomocí stejného partnerského tenanta.</span><span class="sxs-lookup"><span data-stu-id="8a538-328">You are also eligible to enroll for direct bill incentive programs with that same partner tenant.</span></span> <span data-ttu-id="8a538-329">Programy musíte spravovat samostatně.</span><span class="sxs-lookup"><span data-stu-id="8a538-329">You must manage the programs separately.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8a538-330">Další kroky</span><span class="sxs-lookup"><span data-stu-id="8a538-330">Next steps</span></span>

- [<span data-ttu-id="8a538-331">Další informace o tom, jak se stát nepřímým prodejcem</span><span class="sxs-lookup"><span data-stu-id="8a538-331">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)
- [<span data-ttu-id="8a538-332">Nové požadavky poskytovatele CSP Direct partner</span><span class="sxs-lookup"><span data-stu-id="8a538-332">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)
- [<span data-ttu-id="8a538-333">Omezené přímé možnosti fakturace</span><span class="sxs-lookup"><span data-stu-id="8a538-333">Restricted direct bill capabilities</span></span>](restricted-direct-bill-capabilities.md)
