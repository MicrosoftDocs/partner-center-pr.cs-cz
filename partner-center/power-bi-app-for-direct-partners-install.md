---
title: Instalace analýzy partnerského centra pro Power BI
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Postupujte podle kroků v tomto článku a nainstalujte a zobrazte si ukázkovou aplikaci partner Center Analytics pro Power BI (pro přímé partnery v CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 64467ec608c2ca87dbc2b7d5dfb02adb08f13c18
ms.sourcegitcommit: 0a6b1e6d845391539f54213efff00af4d23f028c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/14/2020
ms.locfileid: "92526999"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="7faf7-103">Instalace a vyzkoušení aplikace Analýzy v Partnerském centru pro Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="7faf7-103">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>

<span data-ttu-id="7faf7-104">**Platí pro**</span><span class="sxs-lookup"><span data-stu-id="7faf7-104">**Applies to**</span></span>

- <span data-ttu-id="7faf7-105">Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="7faf7-105">Partner Center</span></span>

<span data-ttu-id="7faf7-106">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="7faf7-106">**Appropriate roles**</span></span>
-   <span data-ttu-id="7faf7-107">Globální správce</span><span class="sxs-lookup"><span data-stu-id="7faf7-107">Global admin</span></span>
-   <span data-ttu-id="7faf7-108">Správce uživatelů</span><span class="sxs-lookup"><span data-stu-id="7faf7-108">User admin</span></span>
-   <span data-ttu-id="7faf7-109">Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="7faf7-109">Sales agent</span></span>
-   <span data-ttu-id="7faf7-110">Agent správce</span><span class="sxs-lookup"><span data-stu-id="7faf7-110">Admin agent</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="7faf7-111">Než začnete</span><span class="sxs-lookup"><span data-stu-id="7faf7-111">Before you begin</span></span>

<span data-ttu-id="7faf7-112">Vyberte aplikaci, která je pro vaši firmu nejdůležitější, z následujícího seznamu dostupných Power BIch aplikací:</span><span class="sxs-lookup"><span data-stu-id="7faf7-112">Select the application that is most relevant to your business from the following list of available Power BI apps:</span></span>
- [<span data-ttu-id="7faf7-113">Přímý poskytovatel</span><span class="sxs-lookup"><span data-stu-id="7faf7-113">Direct Provider</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [<span data-ttu-id="7faf7-114">Nepřímý poskytovatel</span><span class="sxs-lookup"><span data-stu-id="7faf7-114">Indirect Provider</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [<span data-ttu-id="7faf7-115">Nepřímý prodejce</span><span class="sxs-lookup"><span data-stu-id="7faf7-115">Indirect Reseller</span></span>](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

<span data-ttu-id="7faf7-116">Než nainstalujete verzi Preview partnerského centra pro analýzu, ujistěte se, že splňujete následující požadavky.</span><span class="sxs-lookup"><span data-stu-id="7faf7-116">Before you install the Partner Center Analytics app preview version, be sure that you meet the following requirements.</span></span>

- <span data-ttu-id="7faf7-117">Vyberte správnou aplikaci Power BI pro vaši firmu.</span><span class="sxs-lookup"><span data-stu-id="7faf7-117">You pick the correct Power BI app for your business.</span></span>

- <span data-ttu-id="7faf7-118">Máte licenci Power BI pro.</span><span class="sxs-lookup"><span data-stu-id="7faf7-118">You have a Power BI pro license.</span></span>

- <span data-ttu-id="7faf7-119">Máte oprávnění k instalaci aplikací šablon do svého tenanta.</span><span class="sxs-lookup"><span data-stu-id="7faf7-119">You have permissions to install template apps on your tenant.</span></span>

- <span data-ttu-id="7faf7-120">Můžete se přihlásit k Power BI.</span><span class="sxs-lookup"><span data-stu-id="7faf7-120">You can sign in to Power BI.</span></span>

- <span data-ttu-id="7faf7-121">K [tenantovi Azure Active Directory vaší společnosti (Azure AD)](azure-active-directory-tenants-and-partner-center.md)se můžete přihlásit jako globální správce, agent pro správu nebo správce fakturace.</span><span class="sxs-lookup"><span data-stu-id="7faf7-121">You can sign in as a global admin, admin agent, or billing admin to [your company's Azure Active Directory (Azure AD) tenant](azure-active-directory-tenants-and-partner-center.md).</span></span>

## <a name="to-install-the-app"></a><span data-ttu-id="7faf7-122">Instalace aplikace</span><span class="sxs-lookup"><span data-stu-id="7faf7-122">To install the app</span></span>

1. <span data-ttu-id="7faf7-123">V předchozí části klikněte na příslušný odkaz na zdroj aplikace (přímý poskytovatel/nepřímý poskytovatel/nepřímý prodejce).</span><span class="sxs-lookup"><span data-stu-id="7faf7-123">Click on the app source link given (Direct Provider/Indirect Provider/Indirect Reseller) in the above section.</span></span>

2. <span data-ttu-id="7faf7-124">Klikněte na **získat hned** .</span><span class="sxs-lookup"><span data-stu-id="7faf7-124">Click on **GET IT NOW** .</span></span> 

3. <span data-ttu-id="7faf7-125">Kliknutím na **pokračovat** souhlasíte s podmínkami a ujednáními.</span><span class="sxs-lookup"><span data-stu-id="7faf7-125">Agree terms and conditions by clicking **Continue** .</span></span>

4. <span data-ttu-id="7faf7-126">V části už máte účet? Vyberte **Přihlásit se** .</span><span class="sxs-lookup"><span data-stu-id="7faf7-126">Under Already have an account? select **Sign In** .</span></span>

5. <span data-ttu-id="7faf7-127">Na další stránce zadejte své uživatelské jméno a heslo Power BI a pak vyberte přihlásit se.</span><span class="sxs-lookup"><span data-stu-id="7faf7-127">On the next page, enter your Power BI user name and password and then select Sign In.</span></span>

6. <span data-ttu-id="7faf7-128">Nainstalujte pracovní prostor zadáním názvu pracovního prostoru.</span><span class="sxs-lookup"><span data-stu-id="7faf7-128">Install the workspace by providing the workspace name.</span></span>

7. <span data-ttu-id="7faf7-129">Nainstalovanou šablonu aplikace můžete najít v části aplikace.</span><span class="sxs-lookup"><span data-stu-id="7faf7-129">You can find the template apps installed under Apps Section.</span></span>

8. <span data-ttu-id="7faf7-130">Klikněte na aplikace a vyberte nainstalované aplikace.</span><span class="sxs-lookup"><span data-stu-id="7faf7-130">Click on Apps and choose the installed apps.</span></span>

9. <span data-ttu-id="7faf7-131">Začněte tím, že otevřete obrazovku nové aplikace.</span><span class="sxs-lookup"><span data-stu-id="7faf7-131">Get Started with your new app screen opens.</span></span>

10. <span data-ttu-id="7faf7-132">Pokud se chcete připojit k datům, klikněte na **připojit** .</span><span class="sxs-lookup"><span data-stu-id="7faf7-132">To connect to the data Click **Connect** .</span></span>

11. <span data-ttu-id="7faf7-133">V místním okně **připojit k partnerskému centru Analytics** ověřte, že je **metoda ověřování** nastavená na **oAuth2** , nebo vyberte **oAuth2** ze seznamu, pokud není.</span><span class="sxs-lookup"><span data-stu-id="7faf7-133">On the **Connect to Partner Center Analytics** pop-up window, verify that the **Authentication method** is set to **oAuth2** or select **oAuth2** from the list if it's not.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="7faf7-134">Zobrazení tohoto okna může trvat několik minut.</span><span class="sxs-lookup"><span data-stu-id="7faf7-134">This window may take a few minutes to appear.</span></span>

12. <span data-ttu-id="7faf7-135">Na stránce **konektor Datacenter Center Analytics** se přihlaste pomocí účtu globálního správce, agenta správce nebo přihlašovacích údajů správce fakturace pro TENANTA Azure AD vaší společnosti a pak vyberte **Přihlásit** se.</span><span class="sxs-lookup"><span data-stu-id="7faf7-135">On the **Partner Center Analytics Connector** page, sign in with global admin, admin agent, or billing admin credentials for your company's Azure AD tenant, and then select **Sign In** .</span></span>
 
13. <span data-ttu-id="7faf7-136">Po zobrazení výzvy k zadání přístupu vyberte **přijmout** .</span><span class="sxs-lookup"><span data-stu-id="7faf7-136">When prompted for access, select **Accept** .</span></span> 

<span data-ttu-id="7faf7-137">Jakmile je služba pro analýzu partnerského centra připojená k Power BI, začnou se data načíst.</span><span class="sxs-lookup"><span data-stu-id="7faf7-137">Once the Partner Center Analytics service is connected to Power BI, data will begin to load.</span></span> <span data-ttu-id="7faf7-138">V závislosti na množství dat může to trvat až 10 minut.</span><span class="sxs-lookup"><span data-stu-id="7faf7-138">Depending on the amount of data, this can take up to 10 minutes.</span></span> 

<span data-ttu-id="7faf7-139">Po načtení dat můžete začít používat řídicí panel aplikace a sestavy partnerského centra pro analytiky v Power BI.</span><span class="sxs-lookup"><span data-stu-id="7faf7-139">After the data finishes loading, you can start using the Partner Center Analytics app dashboard and reports in Power BI.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7faf7-140">Další kroky</span><span class="sxs-lookup"><span data-stu-id="7faf7-140">Next steps</span></span>

[<span data-ttu-id="7faf7-141">Zobrazení obchodních dat pomocí aplikace Datacenter Center Analytics pro Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="7faf7-141">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-use.md)
