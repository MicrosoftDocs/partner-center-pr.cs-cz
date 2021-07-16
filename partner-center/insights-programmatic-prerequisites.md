---
title: Požadavky pro programové získání přístupu k analytickým datům
description: Požadavky pro programové získání přístupu k analytickým datům
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d4c39025aa3804435dd4d2359b93cd4a2e13ccc4
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376385"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a><span data-ttu-id="07eea-103">Požadavky pro programové získání přístupu k analytickým datům</span><span class="sxs-lookup"><span data-stu-id="07eea-103">Prerequisites to programmatically access analytics data</span></span>

<span data-ttu-id="07eea-104">**Příslušné role:** Globální správce | Správce MPN</span><span class="sxs-lookup"><span data-stu-id="07eea-104">**Appropriate roles:** Global admin | MPN admin</span></span>

<span data-ttu-id="07eea-105">Předtím, než budete moci programově získat přístup k datům o partner Insights Analytics, je nutné splnit následující požadavky.</span><span class="sxs-lookup"><span data-stu-id="07eea-105">Before you can programmatically access partner insights analytics data, you need to meet the following requirements.</span></span>

## <a name="mpn-program-enrollment"></a><span data-ttu-id="07eea-106">Registrace programu MPN</span><span class="sxs-lookup"><span data-stu-id="07eea-106">MPN Program enrollment</span></span>

<span data-ttu-id="07eea-107">Chcete-li získat přístup k datům služby partner Insights Analytics programově, je nutné se zaregistrovat v programu MPN a mít účet partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="07eea-107">To access partner insights analytics data programmatically, you need to be enrolled in the MPN program and have a Partner Center account.</span></span> <span data-ttu-id="07eea-108">Další informace o postupu najdete [v tématu Vytvoření účtu MPN v partnerském centru](mpn-create-a-partner-center-account.md) .</span><span class="sxs-lookup"><span data-stu-id="07eea-108">To learn how, see [Create an MPN account in Partner Center](mpn-create-a-partner-center-account.md)</span></span>

## <a name="create-azure-active-directory-aad-application"></a><span data-ttu-id="07eea-109">vytvořit aplikaci Azure Active Directory (AAD)</span><span class="sxs-lookup"><span data-stu-id="07eea-109">Create Azure Active Directory (AAD) application</span></span>

<span data-ttu-id="07eea-110">přihlašovací údaje pro běžné uživatele nelze použít pro programový přístup k datům partnerů Přehledy Analytics.</span><span class="sxs-lookup"><span data-stu-id="07eea-110">Regular user credentials cannot be used for programmatic access of Partner Insights Analytics data.</span></span> <span data-ttu-id="07eea-111">pro přístup k rozhraním api pro přístup k programování se musí vytvořit aplikace Azure Active Directory (AAD) společně s tajným klíčem (přístup uživatelů a aplikací).</span><span class="sxs-lookup"><span data-stu-id="07eea-111">An Azure Active Directory (AAD) application needs to be created along with a secret (application + user access) to access the programmatic access APIs.</span></span> <span data-ttu-id="07eea-112">Informace o tom, jak vytvořit aplikaci AAD a tajný klíč, najdete v tématu [rychlý Start: registrace aplikace pomocí Microsoft Identity Platform.](/azure/active-directory/develop/quickstart-register-app)   Pro přístup k rozhraní Microsoft Partner API se vyžaduje oprávnění.</span><span class="sxs-lookup"><span data-stu-id="07eea-112">To learn how to create an AAD application and secret, see [Quickstart: Register an application with the Microsoft identity platform.](/azure/active-directory/develop/quickstart-register-app) Permission is required to access Microsoft Partner API.</span></span> <span data-ttu-id="07eea-113">Další informace o tom, jak přidat oprávnění, najdete v tématu [ověřování rozhraní API pro partnery – partner](/partner/develop/api-authentication#application-and-user-access)</span><span class="sxs-lookup"><span data-stu-id="07eea-113">To learn how to add permission, see [Partner API authentication - Partner](/partner/develop/api-authentication#application-and-user-access)</span></span>

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a><span data-ttu-id="07eea-114">Přiřazení role ERV (Executive Report Viewer) uživateli</span><span class="sxs-lookup"><span data-stu-id="07eea-114">Assign Executive Report Viewer (ERV) role to the user</span></span>

<span data-ttu-id="07eea-115">Chcete-li získat přístup k datům pro analýzu partnerského Insights prostřednictvím kódu programu, měli byste mít manažera sestavy (ERV).</span><span class="sxs-lookup"><span data-stu-id="07eea-115">To access partner insights analytics data programmatically, you should have Executive Report Viewer (ERV).</span></span> <span data-ttu-id="07eea-116">informace o tom, jak přiřadit roli ERV uživateli, najdete v tématu [partnerským centrem Přehledy přístupu na základě role – partnerské centrum](insights-roles.md) .</span><span class="sxs-lookup"><span data-stu-id="07eea-116">To learn how to assign ERV role to the user, see [Partner Center Insights role-based access - Partner Center](insights-roles.md)</span></span>

## <a name="generate-an-aad-token"></a><span data-ttu-id="07eea-117">Vygenerovat token AAD</span><span class="sxs-lookup"><span data-stu-id="07eea-117">Generate an AAD token</span></span>

<span data-ttu-id="07eea-118">Je potřeba vygenerovat token AAD pomocí ID aplikace (klienta), tajného klíče klienta, vašeho uživatelského ID a hesla.   [Tady najdete](insights-programmatic-first-api-call.md#token-generation) postup pro vygenerování tokenu AAD.</span><span class="sxs-lookup"><span data-stu-id="07eea-118">You need to Generate an AAD token using the Application (client) ID, client secret, your user ID and password.  [Check here](insights-programmatic-first-api-call.md#token-generation) for steps to generate AAD token.</span></span>

> [!Note]
> <span data-ttu-id="07eea-119">Token je platný po dobu jedné hodiny.</span><span class="sxs-lookup"><span data-stu-id="07eea-119">The token is valid for one hour.</span></span>

## <a name="next-steps"></a><span data-ttu-id="07eea-120">Další kroky</span><span class="sxs-lookup"><span data-stu-id="07eea-120">Next steps</span></span>
[<span data-ttu-id="07eea-121">Programové přístupové paradigma</span><span class="sxs-lookup"><span data-stu-id="07eea-121">Programmatic access paradigm</span></span>](insights-programmatic-access-paradigm.md)