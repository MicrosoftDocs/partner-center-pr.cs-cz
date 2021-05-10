---
title: Řešení potíží při nastavování účtu partnerského centra nebo potížích s obnovením MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Řešení potíží při pokusu o registraci v partnerském centru Odpoví na výzvy, které řeší způsoby platby, hesla forgetting a další.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f34adc57e668caecb69af37afc72b5153f667335
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686258"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="09460-104">Řešení potíží s nastavením účtu nebo problémy s obnovením MPN</span><span class="sxs-lookup"><span data-stu-id="09460-104">Troubleshoot account setup or MPN renewal issues</span></span>


<span data-ttu-id="09460-105">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="09460-105">**Appropriate roles**</span></span>

- <span data-ttu-id="09460-106">Globální správce</span><span class="sxs-lookup"><span data-stu-id="09460-106">Global admin</span></span>
- <span data-ttu-id="09460-107">Správce partnera MPN</span><span class="sxs-lookup"><span data-stu-id="09460-107">MPN partner admin</span></span>
 
<span data-ttu-id="09460-108">Tady jsou některé návrhy řešení běžných potíží, které vznikají při nastavování účtu partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="09460-108">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="09460-109">Co se stane, když migrujete z partnerského centra členství a nemůžete upravovat žádná pole informací o společnosti</span><span class="sxs-lookup"><span data-stu-id="09460-109">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="09460-110">V případech, kdy už vaše společnost má přítomnost v partnerském centru (například účet CSP) – zobrazí se obrazovka, která je jen pro čtení.</span><span class="sxs-lookup"><span data-stu-id="09460-110">In cases where your company already has a presence in Partner Center (for example, a CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="09460-111">Na této obrazovce se zobrazí všechny informace o vaší společnosti, které v partnerském centru existují.</span><span class="sxs-lookup"><span data-stu-id="09460-111">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="09460-112">Podrobnosti na této obrazovce nemůžete změnit.</span><span class="sxs-lookup"><span data-stu-id="09460-112">You can't change the details on this screen.</span></span> <span data-ttu-id="09460-113">Jedná se o návrh a nejedná se o chybu.</span><span class="sxs-lookup"><span data-stu-id="09460-113">This is by design and not an error.</span></span>

<span data-ttu-id="09460-114">Vyberte **přijmout** a **pokračovat** a pokračujte.</span><span class="sxs-lookup"><span data-stu-id="09460-114">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="09460-115">Pokud IT oddělení vypnulo **registraci v partnerském centru**</span><span class="sxs-lookup"><span data-stu-id="09460-115">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="09460-116">Tato zpráva se zobrazí, protože virové uživatele jsou zakázané, nebo protože je v tenantovi Azure AD zakázaná registrace viru.</span><span class="sxs-lookup"><span data-stu-id="09460-116">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="09460-117">Globální správce vašeho účtu Azure AD může povolit požadované funkce spuštěním následujícího příkazu PowerShellu:</span><span class="sxs-lookup"><span data-stu-id="09460-117">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="09460-118">**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="09460-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="09460-119">Další informace najdete v tématu věnovaném [registraci pro samoobslužné služby](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span><span class="sxs-lookup"><span data-stu-id="09460-119">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="09460-120">Zapomněli jste heslo</span><span class="sxs-lookup"><span data-stu-id="09460-120">You forgot your password</span></span>

<span data-ttu-id="09460-121">Pokud jste zapomněli heslo, vyberte odkaz **nemáte přístup k účtu?** na přihlašovací stránce.</span><span class="sxs-lookup"><span data-stu-id="09460-121">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="09460-122">Tato možnost umožňuje resetovat heslo nebo požádat globálního správce o přiřazení nových přihlašovacích údajů.</span><span class="sxs-lookup"><span data-stu-id="09460-122">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="09460-123">Na obrazovce Řekněte nám o vaší společnosti se zobrazí chyba Něco se pokazilo</span><span class="sxs-lookup"><span data-stu-id="09460-123">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="09460-124">Tato chybová zpráva se obvykle zobrazí, pokud na firemním telefonním čísle neúmyslně použijete speciální znaky, mezery nebo kód země.</span><span class="sxs-lookup"><span data-stu-id="09460-124">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="09460-125">Hodnota zadaná do pole Telefonní číslo může obsahovat maximálně 10 znaků.</span><span class="sxs-lookup"><span data-stu-id="09460-125">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="09460-126">Při nákupu platební karty se zobrazí chybová zpráva s oznámením, že vaše objednávka byla zamítnuta.</span><span class="sxs-lookup"><span data-stu-id="09460-126">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="09460-127">Ověřte své informace.</span><span class="sxs-lookup"><span data-stu-id="09460-127">Please verify your information”</span></span>


<span data-ttu-id="09460-128">Vždy používejte adresu odpovídající vaší platební kartě, a ne právnickou osobu.</span><span class="sxs-lookup"><span data-stu-id="09460-128">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="09460-129">Také se ujistěte, že je PSČ správné a odpovídá adrese, kterou používáte.</span><span class="sxs-lookup"><span data-stu-id="09460-129">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="09460-130">Chcete přepnout z offline platby na online způsob platby</span><span class="sxs-lookup"><span data-stu-id="09460-130">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="09460-131">Budete muset zrušit původní objednávku a znovu ji zakoupit pomocí upřednostňovaného způsobu platby.</span><span class="sxs-lookup"><span data-stu-id="09460-131">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="09460-132">Zrušení objednávky:</span><span class="sxs-lookup"><span data-stu-id="09460-132">To cancel an order:</span></span>

1. <span data-ttu-id="09460-133">Na **řídicím panelu** vyberte kartu Nabídky členství.</span><span class="sxs-lookup"><span data-stu-id="09460-133">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="09460-134">Vyberte **Zrušit objednávku.**</span><span class="sxs-lookup"><span data-stu-id="09460-134">Select **Cancel order**</span></span>

3. <span data-ttu-id="09460-135">Zobrazí se potvrzovací okno, které musíte potvrdit, abyste mohli zrušit počáteční objednávku.</span><span class="sxs-lookup"><span data-stu-id="09460-135">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="09460-136">Další kroky</span><span class="sxs-lookup"><span data-stu-id="09460-136">Next steps</span></span>

- [<span data-ttu-id="09460-137">Správa účtu v Partnerském centru</span><span class="sxs-lookup"><span data-stu-id="09460-137">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="09460-138">Čtení souboru faktury a odsoučtu</span><span class="sxs-lookup"><span data-stu-id="09460-138">How to read your bill and recon file</span></span>](read-your-bill.md)
