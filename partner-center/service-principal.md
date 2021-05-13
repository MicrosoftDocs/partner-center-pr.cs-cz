---
title: Objekt služby Azure AD
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak přidat objekt služby do tenanta Azure AD. To znamená přidání aplikace Azure AD (instančního objektu) do Partnerské centrum.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 7d12bb66574e6bcee60b2a1df1673dc9171fbee2
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854923"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="d624d-104">Přidání aplikace Azure AD (instančního objektu) v Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="d624d-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="d624d-105">**Odpovídající role:** Globální správce</span><span class="sxs-lookup"><span data-stu-id="d624d-105">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="d624d-106">V programu komerčního marketplace v Partnerské centrum teď můžete přidat aplikaci Azure AD (instanční objekt) jako uživatele ve vašem Partnerské centrum účtu.</span><span class="sxs-lookup"><span data-stu-id="d624d-106">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="d624d-107">(Dříve jste to mohli udělat ve svém portál partnerů cloudu neboli CPP.</span><span class="sxs-lookup"><span data-stu-id="d624d-107">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="d624d-108">Teď, když jste migroval do Partnerské centrum, je účet CPP jen pro čtení.)</span><span class="sxs-lookup"><span data-stu-id="d624d-108">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="d624d-109">Objekt služby je synonymem pro aplikaci Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d624d-109">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="d624d-110">Přidání aplikace Azure AD (objekt služby)</span><span class="sxs-lookup"><span data-stu-id="d624d-110">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="d624d-111">Na řídicím Partnerské centrum vyberte **Nastavení** a pak vyberte **Nastavení pro vývojáře.**</span><span class="sxs-lookup"><span data-stu-id="d624d-111">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="d624d-112">Vyberte **Uživatelé a** pak vyberte Přidat aplikace Azure **AD.**</span><span class="sxs-lookup"><span data-stu-id="d624d-112">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="d624d-113">Vyberte existující aplikaci Azure AD nebo vytvořte novou.</span><span class="sxs-lookup"><span data-stu-id="d624d-113">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="d624d-114">Pokud vytvoříte novou aplikaci Azure AD, zahrnte následující informace:</span><span class="sxs-lookup"><span data-stu-id="d624d-114">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="d624d-115">**Adresa URL odpovědi:** Adresa URL, na které se uživatelé mohou přihlásit, aby mohli používat vaši aplikaci Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d624d-115">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="d624d-116">**Identifikátor URI ID aplikace:** Logický identifikátor aplikace Azure AD, který se zobrazí při odeslání požadavku na jednotné přihlašování do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d624d-116">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="d624d-117">**Role zabezpečení:** Správce rolí **(totéž** jako role Vlastník v CPP) a Vývojář **(totéž** jako role Přispěvatel v CPP) se vztahují na program komerčního marketplace v Partnerské centrum a mohou být přidružené k této aplikaci Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d624d-117">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="d624d-118">Další kroky</span><span class="sxs-lookup"><span data-stu-id="d624d-118">Next steps</span></span>

- [<span data-ttu-id="d624d-119">Přehled komerčního marketplace v Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="d624d-119">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)