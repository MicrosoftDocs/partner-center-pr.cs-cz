---
title: Nastavení vícefaktorového ověřování pro uživatele
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Zjistěte, jak nastavit zaměstnance pomocí MFA.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 5173526d0f65623311d5cd3a1061e8b9e93e9bb9
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151623"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="c0620-103">Nastavení vícefaktorového ověřování pro uživatele</span><span class="sxs-lookup"><span data-stu-id="c0620-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="c0620-104">**Odpovídající role:** Globální správce</span><span class="sxs-lookup"><span data-stu-id="c0620-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="c0620-105">Mezi naše hlavní priority patří větší ochrana osobních údajů a zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="c0620-105">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="c0620-106">Víme, že nejlepší obranou je prevence a že jsme jen tak silná jako naše nejslabší propojení.</span><span class="sxs-lookup"><span data-stu-id="c0620-106">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="c0620-107">Proto potřebujeme, aby všichni v našem ekosystému jednaly a zajistili, aby byla zajištěna odpovídající ochrana zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="c0620-107">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="c0620-108">Důrazně doporučujeme všem partnerům povolit vícefaktorové ověřování (MFA) pro uživatele ve svém partnerském tenantovi.</span><span class="sxs-lookup"><span data-stu-id="c0620-108">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="c0620-109">Přidání vícefaktorového ověřování pro uživatele</span><span class="sxs-lookup"><span data-stu-id="c0620-109">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="c0620-110">Abyste tuto úlohu dokončili, musíte být globálním správcem vaší společnosti.</span><span class="sxs-lookup"><span data-stu-id="c0620-110">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="c0620-111">Je nejjednodušší povolit více ověřování pro uživatele při jejich přidávání do tenanta Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c0620-111">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="c0620-112">Přihlaste se [k Azure Portal](https://portal.azure.com) a pak přejděte na **Správa uživatelů.**</span><span class="sxs-lookup"><span data-stu-id="c0620-112">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="c0620-113">Vyberte **Multi-Factor Authentication**.</span><span class="sxs-lookup"><span data-stu-id="c0620-113">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="c0620-114">Vyberte uživatele, kterého chcete povolit, a pak vyberte **Povolit.**</span><span class="sxs-lookup"><span data-stu-id="c0620-114">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="c0620-115">Tím se pro tohoto uživatele povolí MFA.</span><span class="sxs-lookup"><span data-stu-id="c0620-115">This will enable MFA for this user.</span></span> <span data-ttu-id="c0620-116">Povoleno znamená, že při prvním přihlášení se uživateli zobrazí dotaz, jestli má nastavit více ověřování.</span><span class="sxs-lookup"><span data-stu-id="c0620-116">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="c0620-117">Následně se při přihlášení zobrazí dotaz, jestli jim pošlete kód, a to buď e-mailem, nebo textovou zprávou (podle toho, které nastavení nastavili).</span><span class="sxs-lookup"><span data-stu-id="c0620-117">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Určení způsobu ověření":::

>[!NOTE]
><span data-ttu-id="c0620-119">Pomocí **stejného postupu** jako výše můžete vynutit, aby uživatelé mohli používat MFA, a vybrat **Vynutit**.</span><span class="sxs-lookup"><span data-stu-id="c0620-119">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="c0620-120">Další informace najdete v části [Povolení vícefaktorového ověřování Azure pro](/azure/active-directory/authentication/howto-mfa-userstates)uživatele pro zabezpečení událostí přihlášení.</span><span class="sxs-lookup"><span data-stu-id="c0620-120">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="c0620-121">Všichni uživatelé začínají na **Zakázáno.**</span><span class="sxs-lookup"><span data-stu-id="c0620-121">All users start out **Disabled**.</span></span> <span data-ttu-id="c0620-122">Když zaregistrujete uživatele do služby Multi-Factor Authentication Azure Active Directory, jejich stav se změní na **Povoleno.**</span><span class="sxs-lookup"><span data-stu-id="c0620-122">When you enroll users in per-user Azure Active Directory Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="c0620-123">Když se uživatelé s povoleným přihlášením a dokončí proces registrace, jejich stav se změní na **vynutilo**.</span><span class="sxs-lookup"><span data-stu-id="c0620-123">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="c0620-124">Další kroky</span><span class="sxs-lookup"><span data-stu-id="c0620-124">Next steps</span></span>

- [<span data-ttu-id="c0620-125">Přiřazování rolí a oprávnění uživatelům</span><span class="sxs-lookup"><span data-stu-id="c0620-125">Assign roles and permissions to users</span></span>](permissions-overview.md)