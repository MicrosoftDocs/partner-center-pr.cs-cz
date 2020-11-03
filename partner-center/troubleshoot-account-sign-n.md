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
ms.openlocfilehash: d990a2cb4dcb69dfc76e8a4f0d40fd4912b4f8a0
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/19/2020
ms.locfileid: "92527732"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="a6e0b-104">Řešení potíží s nastavením účtu nebo problémy s obnovením MPN</span><span class="sxs-lookup"><span data-stu-id="a6e0b-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="a6e0b-105">**Platí pro**</span><span class="sxs-lookup"><span data-stu-id="a6e0b-105">**Applies to**</span></span>

- <span data-ttu-id="a6e0b-106">Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="a6e0b-106">Partner Center</span></span>
 
<span data-ttu-id="a6e0b-107">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="a6e0b-107">**Appropriate roles**</span></span>

- <span data-ttu-id="a6e0b-108">Globální správce</span><span class="sxs-lookup"><span data-stu-id="a6e0b-108">Global admin</span></span>
- <span data-ttu-id="a6e0b-109">Správce partnera MPN</span><span class="sxs-lookup"><span data-stu-id="a6e0b-109">MPN partner admin</span></span> 
 
<span data-ttu-id="a6e0b-110">Tady jsou některé návrhy řešení běžných potíží, které vznikají při nastavování účtu partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="a6e0b-110">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="a6e0b-111">Co se stane, když migrujete z partnerského centra členství a nemůžete upravovat žádná pole informací o společnosti</span><span class="sxs-lookup"><span data-stu-id="a6e0b-111">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="a6e0b-112">V případech, kdy už vaše společnost má přítomnost v partnerském centru (Řekněte mu účet CSP) – zobrazí se obrazovka, která je jen pro čtení.</span><span class="sxs-lookup"><span data-stu-id="a6e0b-112">In cases where your company already has a presence in Partner Center (say CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="a6e0b-113">Na této obrazovce se zobrazí všechny informace o vaší společnosti, které v partnerském centru existují.</span><span class="sxs-lookup"><span data-stu-id="a6e0b-113">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="a6e0b-114">Podrobnosti na této obrazovce nemůžete změnit.</span><span class="sxs-lookup"><span data-stu-id="a6e0b-114">You can't change the details on this screen.</span></span> <span data-ttu-id="a6e0b-115">Jedná se o návrh a nejedná se o chybu.</span><span class="sxs-lookup"><span data-stu-id="a6e0b-115">This is by design and not an error.</span></span>

<span data-ttu-id="a6e0b-116">Vyberte **přijmout** a **pokračovat** a pokračujte.</span><span class="sxs-lookup"><span data-stu-id="a6e0b-116">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="a6e0b-117">Pokud IT oddělení vypnulo **registraci v partnerském centru** .</span><span class="sxs-lookup"><span data-stu-id="a6e0b-117">If the IT department has turned off **sign up for Partner Center** .</span></span>

<span data-ttu-id="a6e0b-118">Tato zpráva se zobrazí, protože virové uživatele jsou zakázané, nebo protože je v tenantovi Azure AD zakázaná registrace viru.</span><span class="sxs-lookup"><span data-stu-id="a6e0b-118">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="a6e0b-119">Globální správce vašeho účtu Azure AD může povolit požadované funkce spuštěním následujícího příkazu PowerShellu:</span><span class="sxs-lookup"><span data-stu-id="a6e0b-119">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="a6e0b-120">**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="a6e0b-120">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="a6e0b-121">Další informace najdete v tématu věnovaném [registraci samoobslužných služeb](/azure/active-directory/users-groups-roles/directory-self-service-signup) .</span><span class="sxs-lookup"><span data-stu-id="a6e0b-121">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="a6e0b-122">Zapomněli jste heslo</span><span class="sxs-lookup"><span data-stu-id="a6e0b-122">You forgot your password</span></span>

<span data-ttu-id="a6e0b-123">Pokud jste zapomněli heslo, vyberte odkaz **nemáte přístup k účtu?** na přihlašovací stránce.</span><span class="sxs-lookup"><span data-stu-id="a6e0b-123">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="a6e0b-124">Tato možnost umožňuje resetovat heslo nebo požádat globálního správce, aby vám přiřadil nové přihlašovací údaje.</span><span class="sxs-lookup"><span data-stu-id="a6e0b-124">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-scree-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="a6e0b-125">V "Řekněte nám o vaší společnosti" Scree se zobrazí chyba "něco se pokazilo".</span><span class="sxs-lookup"><span data-stu-id="a6e0b-125">On the “Tell us about your company” scree, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="a6e0b-126">Tato chybová zpráva se obvykle zobrazuje, pokud nechtěně používáte v telefonním čísle vaší společnosti speciální znaky, mezery nebo kód země.</span><span class="sxs-lookup"><span data-stu-id="a6e0b-126">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="a6e0b-127">Hodnota zadaná v poli telefonní číslo může obsahovat jenom maximálně 10 znaků.</span><span class="sxs-lookup"><span data-stu-id="a6e0b-127">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="a6e0b-128">Nákup vaší platební karty obdržíte chybovou zprávu s oznámením, že vaše objednávka byla zamítnuta.</span><span class="sxs-lookup"><span data-stu-id="a6e0b-128">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="a6e0b-129">Ověřte prosím vaše informace.</span><span class="sxs-lookup"><span data-stu-id="a6e0b-129">Please verify your information”</span></span>


<span data-ttu-id="a6e0b-130">Vždy používejte adresu odpovídající vaší kreditní kartě, nikoli vaší právní entitu.</span><span class="sxs-lookup"><span data-stu-id="a6e0b-130">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="a6e0b-131">Také se ujistěte, že je poštovní směrovací číslo správné a odpovídá adrese, kterou používáte.</span><span class="sxs-lookup"><span data-stu-id="a6e0b-131">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="a6e0b-132">Chcete přepnout z offline platby na online způsob platby</span><span class="sxs-lookup"><span data-stu-id="a6e0b-132">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="a6e0b-133">Původní objednávku bude nutné zrušit a znovu zakoupit pomocí preferovaného způsobu platby.</span><span class="sxs-lookup"><span data-stu-id="a6e0b-133">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="a6e0b-134">Postup zrušení objednávky:</span><span class="sxs-lookup"><span data-stu-id="a6e0b-134">To cancel an order:</span></span>

1. <span data-ttu-id="a6e0b-135">Na řídicím panelu vyberte kartu **nabídky členství** .</span><span class="sxs-lookup"><span data-stu-id="a6e0b-135">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="a6e0b-136">Vyberte možnost **zrušit pořadí** .</span><span class="sxs-lookup"><span data-stu-id="a6e0b-136">Select **Cancel order**</span></span>

3. <span data-ttu-id="a6e0b-137">Zobrazí se potvrzovací okno, které je nutné potvrdit, aby bylo možné původní pořadí zrušit.</span><span class="sxs-lookup"><span data-stu-id="a6e0b-137">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a6e0b-138">Další kroky</span><span class="sxs-lookup"><span data-stu-id="a6e0b-138">Next steps</span></span>

- [<span data-ttu-id="a6e0b-139">Správa účtu v Partnerském centru</span><span class="sxs-lookup"><span data-stu-id="a6e0b-139">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="a6e0b-140">Jak číst váš soubor fakturace a rekognoskaci</span><span class="sxs-lookup"><span data-stu-id="a6e0b-140">How to read your bill and recon file</span></span>](read-your-bill.md)