---
title: Přidání dalších tenantů k účtu partnerského centra
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se přidávat, konsolidovat a spravovat více tenantů Azure AD v účtu partnerského centra. Seznamte se také s některými důvody, které byste mohli chtít udělat.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b9379ce6b27a8ef6e5d6894a0630745794e04e04
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/19/2020
ms.locfileid: "92527751"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="4d37e-104">Přidání a správa několika tenantů v účtu partnerského centra</span><span class="sxs-lookup"><span data-stu-id="4d37e-104">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="4d37e-105">**Platí pro**</span><span class="sxs-lookup"><span data-stu-id="4d37e-105">**Applies to**</span></span>

- <span data-ttu-id="4d37e-106">Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="4d37e-106">Partner Center</span></span>

<span data-ttu-id="4d37e-107">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="4d37e-107">**Appropriate roles**</span></span>

- <span data-ttu-id="4d37e-108">Globální správce</span><span class="sxs-lookup"><span data-stu-id="4d37e-108">Global admin</span></span>

<span data-ttu-id="4d37e-109">Tato funkce umožňuje spravovat více tenantů vaší společnosti a konsolidovat je do vašeho účtu v Partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="4d37e-109">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="4d37e-110">Existuje mnoho důvodů, proč možná budete muset ve svém účtu partnerského centra spravovat více tenantů Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4d37e-110">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="4d37e-111">Příklad:</span><span class="sxs-lookup"><span data-stu-id="4d37e-111">For example:</span></span>

- <span data-ttu-id="4d37e-112">Vaše společnost si může koupit jinou společnost a vy chcete, aby zaměstnanci v nové firmě mohli používat Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="4d37e-112">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="4d37e-113">Chcete však, aby tyto dvě společnosti byly oddělené.</span><span class="sxs-lookup"><span data-stu-id="4d37e-113">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="4d37e-114">V takovém případě přiřadíte tenanta Azure AD nové společnosti k vašemu globálnímu účtu vašeho partnera (PGA).</span><span class="sxs-lookup"><span data-stu-id="4d37e-114">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="4d37e-115">Toto přidružení umožní uživatelům v obou společnostech pracovat v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="4d37e-115">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="4d37e-116">Pokud máte více než jednoho tenanta pro provozování vaší firmy (např. contoso.com, contoso.uk, contoso.in), můžete použít víceklientské prostředí, abyste je mohli spojit se stejným účtem počítače.</span><span class="sxs-lookup"><span data-stu-id="4d37e-116">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="4d37e-117">Fúze a akvizice vyžaduje, abyste pracovali s více než jedním klientem (např. Pokud společnost Contoso získá společnost Fabrikam, budete muset použít jak Constoso.com, tak Fabrikam.com příslušného tenanta).</span><span class="sxs-lookup"><span data-stu-id="4d37e-117">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="4d37e-118">Uživatelé ze všech tenantů by museli mít tyto možnosti:</span><span class="sxs-lookup"><span data-stu-id="4d37e-118">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="4d37e-119">Přístup k partnerským centrům pro školení, digitální stahování, MCP přidružení</span><span class="sxs-lookup"><span data-stu-id="4d37e-119">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="4d37e-120">Přiřadí se role partnerského centra, jako je například správce programu MPN, pobídka správce atd.</span><span class="sxs-lookup"><span data-stu-id="4d37e-120">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="4d37e-121">Přidat do svého účtu jiného tenanta Azure AD</span><span class="sxs-lookup"><span data-stu-id="4d37e-121">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="4d37e-122">Jako globální správce se přihlaste do [řídicího panelu](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="4d37e-122">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="4d37e-123">V ikoně **Nastavení** vyberte **Nastavení účtu** a pak vyberte **klienti** .</span><span class="sxs-lookup"><span data-stu-id="4d37e-123">From the **Settings** icon, select **Account settings** and then select **Tenants** .</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="přidružit klienty"::: 

3. <span data-ttu-id="4d37e-125">Vyberte **přidružit jiného tenanta služby AD** a určete tenanta, kterého chcete přidružit.</span><span class="sxs-lookup"><span data-stu-id="4d37e-125">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="4d37e-126">Jako globální správce se přihlaste ke klientovi, kterého chcete přidružit, a potvrďte přidružení.</span><span class="sxs-lookup"><span data-stu-id="4d37e-126">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="potvrdit přidružení tenantů"::: 

5. <span data-ttu-id="4d37e-128">Po potvrzení se zobrazí všechna oznámení o **sadě** .</span><span class="sxs-lookup"><span data-stu-id="4d37e-128">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="4d37e-129">Vyberte možnost **vrátit se ke správě tenanta** a zobrazí se nově přidaný tenant.</span><span class="sxs-lookup"><span data-stu-id="4d37e-129">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="4d37e-130">Tenanta nemůžete přidružit k účtu, pokud je už přidružený k jinému účtu partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="4d37e-130">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>

 
## <a name="next-steps"></a><span data-ttu-id="4d37e-131">Další kroky</span><span class="sxs-lookup"><span data-stu-id="4d37e-131">Next steps</span></span>

- [<span data-ttu-id="4d37e-132">Přidávání uživatelů</span><span class="sxs-lookup"><span data-stu-id="4d37e-132">Add users</span></span>](create-user-accounts-and-set-permissions.md)
