---
title: Nastavení vícefaktorového ověřování pro uživatele
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Naučte se, jak nastavit vaše zaměstnance na vícefaktorové ověřování.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f42c97be88a1a505f7e0ae9b8af0d4a9167d8447
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182371"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="acb83-103">Nastavení vícefaktorového ověřování pro uživatele</span><span class="sxs-lookup"><span data-stu-id="acb83-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="acb83-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="acb83-104">**Appropriate roles**</span></span>

- <span data-ttu-id="acb83-105">Globální správce</span><span class="sxs-lookup"><span data-stu-id="acb83-105">Global admin</span></span>

<span data-ttu-id="acb83-106">Vyšší zabezpečení ochrany osobních údajů a zabezpečení je z našich nejdůležitějších priorit.</span><span class="sxs-lookup"><span data-stu-id="acb83-106">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="acb83-107">Víme, že nejlepší obrana je prevence a že máme jenom silný, jako náš slabý odkaz.</span><span class="sxs-lookup"><span data-stu-id="acb83-107">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="acb83-108">Proto potřebujeme, aby všichni v našem ekosystému pracovali a zajistili správné fungování ochrany zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="acb83-108">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="acb83-109">Všem partnerům důrazně doporučujeme povolit vícefaktorové ověřování (MFA) pro své uživatele v partnerském tenantovi.</span><span class="sxs-lookup"><span data-stu-id="acb83-109">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="acb83-110">Přidání služby Multi-Factor Authentication pro uživatele</span><span class="sxs-lookup"><span data-stu-id="acb83-110">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="acb83-111">Abyste mohli dokončit tuto úlohu, musíte být globálním správcem vaší společnosti.</span><span class="sxs-lookup"><span data-stu-id="acb83-111">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="acb83-112">Je nejjednodušší povolit pro uživatele MFA při jejich přidávání do tenanta Azure AD.</span><span class="sxs-lookup"><span data-stu-id="acb83-112">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="acb83-113">Přihlaste se k [Azure Portal](https://portal.azure.com) a pak přejít ke **správě uživatelů**.</span><span class="sxs-lookup"><span data-stu-id="acb83-113">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="acb83-114">Vyberte **Multi-Factor Authentication**.</span><span class="sxs-lookup"><span data-stu-id="acb83-114">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="acb83-115">Vyberte uživatele, kterého chcete povolit, a pak vyberte **Povolit**.</span><span class="sxs-lookup"><span data-stu-id="acb83-115">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="acb83-116">Tato akce povolí MFA pro tohoto uživatele.</span><span class="sxs-lookup"><span data-stu-id="acb83-116">This will enable MFA for this user.</span></span> <span data-ttu-id="acb83-117">Povoleno znamená, že uživatel bude požádán o nastavení ověřování MFA při prvním přihlášení.</span><span class="sxs-lookup"><span data-stu-id="acb83-117">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="acb83-118">Po přihlášení se pak vyzve k poskytnutí kódu, který jim pošle e-mailem nebo textovou zprávou (v závislosti na tom, které nastavení).</span><span class="sxs-lookup"><span data-stu-id="acb83-118">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Určete, jak se má ověřit":::

>[!NOTE]
><span data-ttu-id="acb83-120">Uživatelům můžete **vyhovět** , aby používali vícefaktorové ověřování pomocí stejných kroků jako výše a **vynutili** výběr.</span><span class="sxs-lookup"><span data-stu-id="acb83-120">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="acb83-121">Pokud se chcete dozvědět víc, přečtěte si téma [povolení Multi-Factor Authentication Azure pro jednotlivé uživatele k zabezpečení přihlašovacích událostí](/azure/active-directory/authentication/howto-mfa-userstates).</span><span class="sxs-lookup"><span data-stu-id="acb83-121">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="acb83-122">Všichni uživatelé začínají **zakázáni**.</span><span class="sxs-lookup"><span data-stu-id="acb83-122">All users start out **Disabled**.</span></span> <span data-ttu-id="acb83-123">Když zaregistrujete uživatele v Multi-Factor Authentication Azure pro jednotlivé uživatele, jejich stav se změní na **povoleno**.</span><span class="sxs-lookup"><span data-stu-id="acb83-123">When you enroll users in per-user Azure Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="acb83-124">Když se uživatelé s povoleným přihlášením a dokončí proces registrace, jejich stav se změní na **vynutilo**.</span><span class="sxs-lookup"><span data-stu-id="acb83-124">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="acb83-125">Další kroky</span><span class="sxs-lookup"><span data-stu-id="acb83-125">Next steps</span></span>

- [<span data-ttu-id="acb83-126">Přiřazování rolí a oprávnění uživatelům</span><span class="sxs-lookup"><span data-stu-id="acb83-126">Assign roles and permissions to users</span></span>](permissions-overview.md)