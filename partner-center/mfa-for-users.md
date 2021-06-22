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
ms.openlocfilehash: 9cdb83c8b58b75606275c9773cba79eba75d5d0d
ms.sourcegitcommit: 7cc83714e17337b472727819243f98c84ae181ba
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/22/2021
ms.locfileid: "112450797"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="7f947-103">Nastavení vícefaktorového ověřování pro uživatele</span><span class="sxs-lookup"><span data-stu-id="7f947-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="7f947-104">**Odpovídající role:** Globální správce</span><span class="sxs-lookup"><span data-stu-id="7f947-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="7f947-105">Mezi naše hlavní priority patří větší ochrana osobních údajů a zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="7f947-105">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="7f947-106">Víme, že nejlepší obranou je prevence a že jsme jen tak silná jako naše nejslabší propojení.</span><span class="sxs-lookup"><span data-stu-id="7f947-106">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="7f947-107">Proto potřebujeme, aby všichni v našem ekosystému jednaly a zajistili odpovídající ochranu zabezpečení.</span><span class="sxs-lookup"><span data-stu-id="7f947-107">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="7f947-108">Všem partnerům důrazně doporučujeme povolit vícefaktorové ověřování (MFA) pro své uživatele ve svém partnerském tenantovi.</span><span class="sxs-lookup"><span data-stu-id="7f947-108">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="7f947-109">Přidání vícefaktorového ověřování pro uživatele</span><span class="sxs-lookup"><span data-stu-id="7f947-109">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="7f947-110">Abyste tuto úlohu dokončili, musíte být globálním správcem vaší společnosti.</span><span class="sxs-lookup"><span data-stu-id="7f947-110">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="7f947-111">Je nejjednodušší povolit více ověřování pro uživatele při jejich přidávání do tenanta Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7f947-111">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="7f947-112">Přihlaste se [k Azure Portal](https://portal.azure.com) a pak přejděte na **Správa uživatelů.**</span><span class="sxs-lookup"><span data-stu-id="7f947-112">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="7f947-113">Vyberte **Multi-Factor Authentication**.</span><span class="sxs-lookup"><span data-stu-id="7f947-113">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="7f947-114">Vyberte uživatele, kterého chcete povolit, a pak vyberte **Povolit.**</span><span class="sxs-lookup"><span data-stu-id="7f947-114">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="7f947-115">Tím se pro tohoto uživatele povolí MFA.</span><span class="sxs-lookup"><span data-stu-id="7f947-115">This will enable MFA for this user.</span></span> <span data-ttu-id="7f947-116">Povoleno znamená, že při prvním přihlášení se uživateli zobrazí dotaz, jestli má nastavit více ověřování.</span><span class="sxs-lookup"><span data-stu-id="7f947-116">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="7f947-117">Následně se při přihlášení zobrazí dotaz, jestli jim má poslat kód, a to buď e-mailem, nebo textovou zprávou (v závislosti na tom, kterou si nastavili).</span><span class="sxs-lookup"><span data-stu-id="7f947-117">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/multi-factor-authentication/security-verification.png" alt-text="Určete, jak to ověřit.":::

>[!NOTE]
><span data-ttu-id="7f947-119">Pomocí výše **uvedeného** postupu můžete vynutit, aby uživatelé více ověřování mohli používat, a to výběrem **možnosti Vynutit**.</span><span class="sxs-lookup"><span data-stu-id="7f947-119">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="7f947-120">Další informace najdete v části [Povolení vícefaktorového](/azure/active-directory/authentication/howto-mfa-userstates)ověřování Azure pro uživatele pro zabezpečení událostí přihlášení.</span><span class="sxs-lookup"><span data-stu-id="7f947-120">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="7f947-121">Všichni uživatelé začínají na **Zakázáno.**</span><span class="sxs-lookup"><span data-stu-id="7f947-121">All users start out **Disabled**.</span></span> <span data-ttu-id="7f947-122">Když zaregistrujete uživatele do služby Multi-Factor Authentication Azure Active Directory, jejich stav se změní na **Povoleno.**</span><span class="sxs-lookup"><span data-stu-id="7f947-122">When you enroll users in per-user Azure Active Directory Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="7f947-123">Když se uživatelé povolí, přihlásí se a dokončí proces registrace, jejich stav se změní na **Vynucené.**</span><span class="sxs-lookup"><span data-stu-id="7f947-123">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="7f947-124">Další kroky</span><span class="sxs-lookup"><span data-stu-id="7f947-124">Next steps</span></span>

- [<span data-ttu-id="7f947-125">Přiřazování rolí a oprávnění uživatelům</span><span class="sxs-lookup"><span data-stu-id="7f947-125">Assign roles and permissions to users</span></span>](permissions-overview.md)