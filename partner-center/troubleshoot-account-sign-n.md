---
title: Řešení potíží s nastavením Partnerské centrum účtu nebo prodloužením platnosti MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Řešení potíží při pokusu o registraci v Partnerské centrum Odpovědi řeší problémy s způsoby platby, zapomenutím hesel a další.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4fc1a43b4d525d9221ac7e4db56f5f278404e3f5
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431751"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="8444a-104">Řešení potíží s nastavením účtu nebo prodloužením platnosti MPN</span><span class="sxs-lookup"><span data-stu-id="8444a-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="8444a-105">**Odpovídající role:** Globální správce | Správce partnera MPN</span><span class="sxs-lookup"><span data-stu-id="8444a-105">**Appropriate roles**: Global admin | MPN partner admin</span></span>
 
<span data-ttu-id="8444a-106">Tady je několik návrhů pro řešení běžných problémů, ke kterým dochází při nastavování Partnerské centrum účtu.</span><span class="sxs-lookup"><span data-stu-id="8444a-106">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="8444a-107">Co se stane, když migrujete z Partner Membership Center a nemůžete upravit žádná pole s informacemi o společnosti</span><span class="sxs-lookup"><span data-stu-id="8444a-107">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="8444a-108">V případech, kdy už vaše společnost existuje v Partnerské centrum (například účet Cloud Solution Provider (CSP), se zobrazí obrazovka jen pro čtení.</span><span class="sxs-lookup"><span data-stu-id="8444a-108">In cases where your company already has a presence in Partner Center (for example, a Cloud Solution Provider (CSP) account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="8444a-109">Na této obrazovce se zobrazí všechny informace o vaší společnosti, které existují v Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="8444a-109">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="8444a-110">Podrobnosti na této obrazovce nemůžete změnit.</span><span class="sxs-lookup"><span data-stu-id="8444a-110">You can't change the details on this screen.</span></span> <span data-ttu-id="8444a-111">Jedná se o návrh, a ne o chybu.</span><span class="sxs-lookup"><span data-stu-id="8444a-111">This is by design and not an error.</span></span>

<span data-ttu-id="8444a-112">Pokračujte tak, že **vyberete Přijmout** a pak vyberete **Pokračovat.**</span><span class="sxs-lookup"><span data-stu-id="8444a-112">To proceed, select **Accept**, and then select **Continue**.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="8444a-113">Pokud oddělení IT vypnulo možnost **Registrace pro Partnerské centrum**</span><span class="sxs-lookup"><span data-stu-id="8444a-113">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="8444a-114">Tato zpráva se zobrazí, protože virální uživatelé jsou zakázaní nebo je v tenantovi služby Azure Active Directory (AD) zakázaná virální registrace.</span><span class="sxs-lookup"><span data-stu-id="8444a-114">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure Active Directory (AD) tenant.</span></span> <span data-ttu-id="8444a-115">Globální správce účtu Azure AD může povolit požadované funkce spuštěním následujícího příkazu PowerShellu:</span><span class="sxs-lookup"><span data-stu-id="8444a-115">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="8444a-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="8444a-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="8444a-117">Další informace najdete v [samoobslužné zaregistrovat.](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="8444a-117">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="8444a-118">Zapomněli jste heslo</span><span class="sxs-lookup"><span data-stu-id="8444a-118">You forgot your password</span></span>

<span data-ttu-id="8444a-119">Pokud jste zapomněli své heslo, vyberte na přihlašovací stránce možnost **Nemáte přístup ke svému účtu?**.</span><span class="sxs-lookup"><span data-stu-id="8444a-119">If you have forgotten your password, on the sign-in page, select **Can't access your account?**.</span></span> <span data-ttu-id="8444a-120">Tato možnost umožňuje resetovat heslo nebo požádat globálního správce o přiřazení nových přihlašovacích údajů.</span><span class="sxs-lookup"><span data-stu-id="8444a-120">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="8444a-121">Na obrazovce Řekněte nám o vaší společnosti se zobrazí chyba Něco se pokazilo</span><span class="sxs-lookup"><span data-stu-id="8444a-121">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="8444a-122">Tato chybová zpráva se obvykle zobrazí, pokud na firemním telefonním čísle neúmyslně použijete speciální znaky, mezery nebo kód země.</span><span class="sxs-lookup"><span data-stu-id="8444a-122">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="8444a-123">Hodnota zadaná do pole Telefonní číslo může obsahovat maximálně 10 znaků.</span><span class="sxs-lookup"><span data-stu-id="8444a-123">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="8444a-124">Při nákupu platební karty se zobrazí chybová zpráva s oznámením, že vaše objednávka byla zamítnuta.</span><span class="sxs-lookup"><span data-stu-id="8444a-124">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="8444a-125">Ověřte své informace.</span><span class="sxs-lookup"><span data-stu-id="8444a-125">Please verify your information”</span></span>


<span data-ttu-id="8444a-126">Vždy používejte adresu odpovídající vaší platební kartě, a ne právnickou osobu.</span><span class="sxs-lookup"><span data-stu-id="8444a-126">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="8444a-127">Také se ujistěte, že je PSČ správné a odpovídá adrese, kterou používáte.</span><span class="sxs-lookup"><span data-stu-id="8444a-127">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="8444a-128">Chcete přepnout z offline platby na online způsob platby</span><span class="sxs-lookup"><span data-stu-id="8444a-128">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="8444a-129">Budete muset zrušit původní objednávku a znovu ji zakoupit pomocí upřednostňovaného způsobu platby.</span><span class="sxs-lookup"><span data-stu-id="8444a-129">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="8444a-130">Zrušení objednávky:</span><span class="sxs-lookup"><span data-stu-id="8444a-130">To cancel an order:</span></span>

1. <span data-ttu-id="8444a-131">Na řídicím Partnerské centrum vyberte kartu **Nabídky členství.**</span><span class="sxs-lookup"><span data-stu-id="8444a-131">In the Partner Center dashboard, select the **Membership Offers** tab.</span></span>

2. <span data-ttu-id="8444a-132">Vyberte **Zrušit objednávku.**</span><span class="sxs-lookup"><span data-stu-id="8444a-132">Select **Cancel order**</span></span>

3. <span data-ttu-id="8444a-133">Zobrazí se potvrzovací okno, které musíte potvrdit, abyste mohli zrušit počáteční objednávku.</span><span class="sxs-lookup"><span data-stu-id="8444a-133">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8444a-134">Další kroky</span><span class="sxs-lookup"><span data-stu-id="8444a-134">Next steps</span></span>

- [<span data-ttu-id="8444a-135">Správa účtu v Partnerském centru</span><span class="sxs-lookup"><span data-stu-id="8444a-135">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="8444a-136">Čtení souboru faktury a odsoučtu</span><span class="sxs-lookup"><span data-stu-id="8444a-136">How to read your bill and recon file</span></span>](read-your-bill.md)
