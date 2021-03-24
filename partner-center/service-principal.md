---
title: Instanční objekt služby Azure AD
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si, jak přidat instanční objekt k vašemu tenantovi služby Azure AD. To znamená, že přidání aplikace Azure AD (instančního objektu) v partnerském centru.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 6ef5373fd9a606cd25345cbe80a55f28fc1f753f
ms.sourcegitcommit: ec33c2352a9dd3e5a941f0f42ff1e8d256bb2399
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/24/2021
ms.locfileid: "105028464"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="24d43-104">Přidání aplikace Azure AD (instančního objektu) v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="24d43-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="24d43-105">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="24d43-105">**Appropriate roles**</span></span>

- <span data-ttu-id="24d43-106">Globální správce</span><span class="sxs-lookup"><span data-stu-id="24d43-106">Global admin</span></span>

<span data-ttu-id="24d43-107">V programu komerčního obchodu v partnerském centru teď můžete do svého účtu partnerského centra přidat aplikaci Azure AD (instanční objekt) jako uživatele.</span><span class="sxs-lookup"><span data-stu-id="24d43-107">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="24d43-108">(Dříve jste to mohli udělat v portál partnerů cloudu, nebo CPP.</span><span class="sxs-lookup"><span data-stu-id="24d43-108">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="24d43-109">Teď, když jste migrovali do partnerského centra, je účet CPP jen pro čtení.)</span><span class="sxs-lookup"><span data-stu-id="24d43-109">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="24d43-110">Instanční objekt je synonymem pro aplikaci Azure AD.</span><span class="sxs-lookup"><span data-stu-id="24d43-110">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="24d43-111">Přidat aplikaci Azure AD (instanční objekt)</span><span class="sxs-lookup"><span data-stu-id="24d43-111">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="24d43-112">Z řídicího panelu partnerského centra vyberte **Nastavení** a potom vyberte **Nastavení vývojáře**.</span><span class="sxs-lookup"><span data-stu-id="24d43-112">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="24d43-113">Vyberte **Uživatelé** a pak vyberte **Přidat aplikace Azure AD**.</span><span class="sxs-lookup"><span data-stu-id="24d43-113">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="24d43-114">Vyberte existující aplikaci Azure AD nebo vytvořte novou.</span><span class="sxs-lookup"><span data-stu-id="24d43-114">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="24d43-115">Pokud vytvoříte novou aplikaci Azure AD, zahrňte tyto informace:</span><span class="sxs-lookup"><span data-stu-id="24d43-115">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="24d43-116">**Adresa URL odpovědi**: adresa URL, kde se uživatelé můžou přihlásit k používání vaší aplikace Azure AD.</span><span class="sxs-lookup"><span data-stu-id="24d43-116">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="24d43-117">**Identifikátor URI ID aplikace**: logický identifikátor pro aplikaci Azure AD, který se zobrazí, když pošle žádost o jednotné přihlašování do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="24d43-117">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="24d43-118">**Role zabezpečení**: **správce** rolí (stejné jako role Owner v CPP) a **Developer** (stejné jako role Přispěvatel v CPP) platí pro program komerčního tržiště v partnerském centru a je možné ho přidružit k této aplikaci Azure AD.</span><span class="sxs-lookup"><span data-stu-id="24d43-118">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="24d43-119">Další kroky</span><span class="sxs-lookup"><span data-stu-id="24d43-119">Next steps</span></span>

- [<span data-ttu-id="24d43-120">Přehled komerčního tržiště v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="24d43-120">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)