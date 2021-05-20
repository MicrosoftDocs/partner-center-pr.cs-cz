---
title: Propojení pracovního účtu pro přístup k Partnerské centrum
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Vytvořte pracovní účet, který pro propojení vaší společnosti s vaším Partnerské centrum účtem. Zaměstnanci ve vaší společnosti tak budou mít přístup k Partnerské centrum.
author: vinayks
ms.author: vinayks
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 11/25/2019
ms.openlocfilehash: a06a38ef9d96b4c2a1e95328d510eb2fd71ff0e3
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149838"
---
# <a name="create-a-work-account-that-links-your-company-to-your-partner-center-account"></a><span data-ttu-id="3148b-104">Vytvoření pracovního účtu, který pro propojení vaší společnosti s vaším Partnerské centrum účtem</span><span class="sxs-lookup"><span data-stu-id="3148b-104">Create a work account that links your company to your Partner Center account</span></span>

<span data-ttu-id="3148b-105">**Odpovídající role:** Globální správce | Správce správy uživatelů</span><span class="sxs-lookup"><span data-stu-id="3148b-105">**Appropriate roles**: Global admin | User management admin</span></span>

## <a name="why-you-need-a-work-account"></a><span data-ttu-id="3148b-106">Proč potřebujete pracovní účet</span><span class="sxs-lookup"><span data-stu-id="3148b-106">Why you need a work account</span></span>

<span data-ttu-id="3148b-107">Microsoft vyžaduje, abyste pracovní účet vaší společnosti propojují s novým Partnerské centrum účtem.</span><span class="sxs-lookup"><span data-stu-id="3148b-107">Microsoft requires you to link your company's work account to your new Partner Center account.</span></span> <span data-ttu-id="3148b-108">Tento odkaz umožňuje uživatelům vašeho účtu přihlásit se k Partnerské centrum pomocí uživatelských jmen a hesel svých pracovních účtů.</span><span class="sxs-lookup"><span data-stu-id="3148b-108">The link enables your account users to sign in to Partner Center with their work account user names and passwords.</span></span>

## <a name="the-work-account-email-address"></a><span data-ttu-id="3148b-109">E-mailová adresa pracovního účtu</span><span class="sxs-lookup"><span data-stu-id="3148b-109">The work account email address</span></span>

<span data-ttu-id="3148b-110">Váš pracovní účet nebo pracovní e-mail je e-mailová adresa, kterou vám poskytla vaše společnost.</span><span class="sxs-lookup"><span data-stu-id="3148b-110">Your work account or work email is the email address provided to you by your company.</span></span> <span data-ttu-id="3148b-111">E-mail pracovního účtu je obvykle ve formátu `you@yourcompany.com` .</span><span class="sxs-lookup"><span data-stu-id="3148b-111">A work account email is usually in the format `you@yourcompany.com`.</span></span> <span data-ttu-id="3148b-112">Osobní e-mailové adresy, jako je Hotmail, Gmail nebo Yahoo, nejsou pracovní e-maily a nelze je použít Partnerské centrum účtu.</span><span class="sxs-lookup"><span data-stu-id="3148b-112">Personal email addresses such as Hotmail, Gmail, or Yahoo aren't work email and can't be used for your Partner Center account.</span></span>

<span data-ttu-id="3148b-113">Pokud máte více než jednu platnou pracovní e-mailovou adresu, použijte tu, která je přidružená k ústředí společnosti, a ne oblastní oddělení, například místo adresy použijte `contoso.com` `contoso.uk` e-mail.</span><span class="sxs-lookup"><span data-stu-id="3148b-113">If you have more than one valid work email address, use the one that is associated to your Corporate Headquarters rather than the regional department, for example, use your `contoso.com` email rather than the `contoso.uk` address.</span></span>

> [!NOTE]  
> <span data-ttu-id="3148b-114">Než se rozhodnete použít existující pracovní účet, zamyslete se nad tím, kolik uživatelů v tomto účtu bude muset Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="3148b-114">Before you decide to use an existing work account, think about how many users in the account will need to work in Partner Center.</span></span> <span data-ttu-id="3148b-115">Pokud máte v účtu uživatele, kteří nebudou muset pracovat v Partnerské centrum, zvažte vytvoření nového účtu jenom pro uživatele, kteří budou potřebovat pracovat v Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="3148b-115">If you have users in the account who won't need to work in Partner Center, consider creating a new account for only those users who will need to work in the Partner Center.</span></span>

## <a name="not-sure-if-your-company-already-has-a-work-account"></a><span data-ttu-id="3148b-116">Nejste si jistí, jestli už vaše společnost má pracovní účet?</span><span class="sxs-lookup"><span data-stu-id="3148b-116">Not sure if your company already has a work account?</span></span>

<span data-ttu-id="3148b-117">Pokud si nejste jistí, jestli má vaše společnost pracovní účet, postupujte podle těchto kroků a proveďte kontrolu.</span><span class="sxs-lookup"><span data-stu-id="3148b-117">If you're not sure whether your company has a work account, follow these steps to check.</span></span> <span data-ttu-id="3148b-118">Pokud máte aktivní předplatné pro Microsoft Azure nebo Office 365, už máte pracovní účet.</span><span class="sxs-lookup"><span data-stu-id="3148b-118">If you have an active subscription to Microsoft Azure or Office 365, you already have a work account.</span></span>

1. <span data-ttu-id="3148b-119">Přihlaste se na [Azure Portal](https://portal.azure.com).</span><span class="sxs-lookup"><span data-stu-id="3148b-119">Sign in to the [Azure portal](https://portal.azure.com).</span></span>

2. <span data-ttu-id="3148b-120">V Azure Active Directory vyberte Název domény a pak vyberte Názvy domén.</span><span class="sxs-lookup"><span data-stu-id="3148b-120">Select Azure Active Directory from the menu and then select Domain Names.</span></span>

3. <span data-ttu-id="3148b-121">Pokud už máte pracovní účet, zobrazí se váš název domény.</span><span class="sxs-lookup"><span data-stu-id="3148b-121">If you already have a work account, your domain name will be listed.</span></span>

<span data-ttu-id="3148b-122">Pokud vaše společnost ještě nemá pracovní účet, můžete si ji vytvořit během procesu registrace.</span><span class="sxs-lookup"><span data-stu-id="3148b-122">If your company doesn't already have a work account, you can create one during the enrollment process.</span></span>

<span data-ttu-id="3148b-123">Diagram níže popisuje kroky pro několik typických scénářů:</span><span class="sxs-lookup"><span data-stu-id="3148b-123">The diagram below provides steps for several typical scenarios:</span></span>

- <span data-ttu-id="3148b-124">určení, jestli máte pracovní účet</span><span class="sxs-lookup"><span data-stu-id="3148b-124">determine if you have a work account</span></span>
- <span data-ttu-id="3148b-125">určení způsobu přihlášení k pracovnímu účtu</span><span class="sxs-lookup"><span data-stu-id="3148b-125">determine how to sign into your work account</span></span>
- <span data-ttu-id="3148b-126">určení, jestli je potřeba vytvořit nový pracovní účet</span><span class="sxs-lookup"><span data-stu-id="3148b-126">determine if you need to create a new work account</span></span>

:::image type="content" source="images/onboardingAADFlow.png" lightbox="images/onboardingAADFlow.png" alt-text="Máte pracovní účet nebo ho potřebujete vytvořit?":::

<span data-ttu-id="3148b-128">Další informace o přidávání domén v Azure AD najdete v tématu [Přidání nebo přidružení domény ve službě Azure AD](/azure/active-directory/active-directory-add-domain) .</span><span class="sxs-lookup"><span data-stu-id="3148b-128">For more information about adding domains in Azure AD, see [Add or associate a domain in Azure AD](/azure/active-directory/active-directory-add-domain)</span></span>

## <a name="about-microsoft-azure"></a><span data-ttu-id="3148b-129">O Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="3148b-129">About Microsoft Azure</span></span>

<span data-ttu-id="3148b-130">Microsoft Azure je veřejná cloudová platforma, kterou můžou společnosti používat k sestavování, nasazování a správě aplikací napříč globální sítí datových center spravovaných Microsoftem.</span><span class="sxs-lookup"><span data-stu-id="3148b-130">Microsoft Azure is a public cloud platform that companies can use to build, deploy, and manage applications across a global network of Microsoft-managed datacenters.</span></span> <span data-ttu-id="3148b-131">Společnosti využívají Azure k vytváření virtuálních IT infrastruktury s virtuálními funkcemi nebo službami místo fyzických počítačů.</span><span class="sxs-lookup"><span data-stu-id="3148b-131">Companies use Azure to build a virtual IT infrastructure with virtual functions, or services, instead of physical machines.</span></span>

<span data-ttu-id="3148b-132">Když si koupíte předplatné Azure, nebudete mít v podstatě vyhrazené a zabezpečené místo ve veřejném cloudu Azure, ale nemusíte se zabývat podlahou v budově Office, která bude firemní fyzickou firmu.</span><span class="sxs-lookup"><span data-stu-id="3148b-132">When you purchase an Azure subscription, you're essentially renting a dedicated, secure space in the Azure public cloud, not too different from renting a floor in an office building to house your company's physical business.</span></span> <span data-ttu-id="3148b-133">K vlastníkovi budovy Office je vaše společnost tenant.</span><span class="sxs-lookup"><span data-stu-id="3148b-133">To the office building's owner, your company is a tenant.</span></span>

<span data-ttu-id="3148b-134">Pracovní účet Azure je vyhrazená a izolovaná virtuální reprezentace vaší společnosti ve veřejném cloudu Azure, která se vytvoří po přihlášení k odběru cloudové služby Microsoftu, jako je Azure, Microsoft Intune nebo Office 365.</span><span class="sxs-lookup"><span data-stu-id="3148b-134">An Azure work account is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span>

<span data-ttu-id="3148b-135">Váš pracovní účet je hostitelem uživatelů Azure AD a informací o nich – jejich hesla, data profilu, oprávnění atd.</span><span class="sxs-lookup"><span data-stu-id="3148b-135">Your work account hosts your Azure AD users and the information about them - their passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="3148b-136">Pracovní účet obsahuje také skupiny, aplikace a další informace, které se týkají společnosti a jejího zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="3148b-136">The work account also contains groups, applications, and other information pertaining to a company and its security.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3148b-137">Další kroky</span><span class="sxs-lookup"><span data-stu-id="3148b-137">Next steps</span></span>

- [<span data-ttu-id="3148b-138">Správa účtu v Partnerském centru</span><span class="sxs-lookup"><span data-stu-id="3148b-138">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="3148b-139">Sledovat stav ověřování</span><span class="sxs-lookup"><span data-stu-id="3148b-139">Track verification status</span></span>](verification-responses.md)