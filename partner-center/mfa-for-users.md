---
title: Nastavení vícefaktorového ověřování pro uživatele
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Naučte se, jak nastavit zaměstnance pomocí vícefaktorového ověřování.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 37373c032dc34315c0e3274987805d7518d0b595
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276599"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="8e99e-103">Nastavení vícefaktorového ověřování pro uživatele</span><span class="sxs-lookup"><span data-stu-id="8e99e-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="8e99e-104">**Příslušné role**: globální správce</span><span class="sxs-lookup"><span data-stu-id="8e99e-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="8e99e-105">Vyšší zabezpečení ochrany osobních údajů a zabezpečení je z našich nejdůležitějších priorit.</span><span class="sxs-lookup"><span data-stu-id="8e99e-105">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="8e99e-106">Víme, že nejlepší obrana je prevence a že máme jenom silný, jako náš slabý odkaz.</span><span class="sxs-lookup"><span data-stu-id="8e99e-106">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="8e99e-107">Proto potřebujeme, aby všichni v našem ekosystému pracovali a zajistili správné fungování ochrany zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="8e99e-107">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="8e99e-108">Všem partnerům důrazně doporučujeme povolit vícefaktorové ověřování (MFA) pro své uživatele v partnerském tenantovi.</span><span class="sxs-lookup"><span data-stu-id="8e99e-108">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="8e99e-109">Přidání služby Multi-Factor Authentication pro uživatele</span><span class="sxs-lookup"><span data-stu-id="8e99e-109">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="8e99e-110">Abyste mohli dokončit tuto úlohu, musíte být globálním správcem vaší společnosti.</span><span class="sxs-lookup"><span data-stu-id="8e99e-110">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="8e99e-111">Je nejjednodušší povolit pro uživatele MFA při jejich přidávání do tenanta Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8e99e-111">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="8e99e-112">Přihlaste se k [Azure Portal](https://portal.azure.com) a pak přejít ke **správě uživatelů**.</span><span class="sxs-lookup"><span data-stu-id="8e99e-112">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="8e99e-113">Vyberte **Multi-Factor Authentication**.</span><span class="sxs-lookup"><span data-stu-id="8e99e-113">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="8e99e-114">Vyberte uživatele, kterého chcete povolit, a pak vyberte **Povolit**.</span><span class="sxs-lookup"><span data-stu-id="8e99e-114">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="8e99e-115">Tato akce povolí MFA pro tohoto uživatele.</span><span class="sxs-lookup"><span data-stu-id="8e99e-115">This will enable MFA for this user.</span></span> <span data-ttu-id="8e99e-116">Povoleno znamená, že uživatel bude požádán o nastavení ověřování MFA při prvním přihlášení.</span><span class="sxs-lookup"><span data-stu-id="8e99e-116">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="8e99e-117">Po přihlášení se pak vyzve k poskytnutí kódu, který jim pošle e-mailem nebo textovou zprávou (v závislosti na tom, které nastavení).</span><span class="sxs-lookup"><span data-stu-id="8e99e-117">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Určete, jak se má ověřit.":::

>[!NOTE]
><span data-ttu-id="8e99e-119">Uživatelům můžete **vyhovět** , aby používali vícefaktorové ověřování pomocí stejných kroků jako výše a **vynutili** výběr.</span><span class="sxs-lookup"><span data-stu-id="8e99e-119">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="8e99e-120">Pokud se chcete dozvědět víc, přečtěte si téma [povolení Multi-Factor Authentication Azure pro jednotlivé uživatele k zabezpečení přihlašovacích událostí](/azure/active-directory/authentication/howto-mfa-userstates).</span><span class="sxs-lookup"><span data-stu-id="8e99e-120">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="8e99e-121">Všichni uživatelé začínají **zakázáni**.</span><span class="sxs-lookup"><span data-stu-id="8e99e-121">All users start out **Disabled**.</span></span> <span data-ttu-id="8e99e-122">Když uživatele zaregistrujete v Multi-Factor Authentication Azure Active Directory pro jednotlivé uživatele, jejich stav se změní na **povoleno**.</span><span class="sxs-lookup"><span data-stu-id="8e99e-122">When you enroll users in per-user Azure Active Directory Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="8e99e-123">Když se uživatelé s povoleným přihlášením a dokončí proces registrace, jejich stav se změní na **vynutilo**.</span><span class="sxs-lookup"><span data-stu-id="8e99e-123">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="8e99e-124">Další kroky</span><span class="sxs-lookup"><span data-stu-id="8e99e-124">Next steps</span></span>

- [<span data-ttu-id="8e99e-125">Přiřazování rolí a oprávnění uživatelům</span><span class="sxs-lookup"><span data-stu-id="8e99e-125">Assign roles and permissions to users</span></span>](permissions-overview.md)