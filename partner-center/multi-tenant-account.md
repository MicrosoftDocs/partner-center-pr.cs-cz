---
title: Přidání dalších tenantů k účtu partnerského centra
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se přidávat, konsolidovat a spravovat více tenantů Azure AD v účtu partnerského centra. Seznamte se také s některými důvody, které byste mohli chtít udělat.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 22f85bda0a651559da1717ae1e5365da40d62aff
ms.sourcegitcommit: 8cb98de420f6ab5bb4cb3efc9007262c4d7d3327
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/12/2021
ms.locfileid: "98105544"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="e436d-104">Přidání a správa několika tenantů v účtu partnerského centra</span><span class="sxs-lookup"><span data-stu-id="e436d-104">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="e436d-105">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="e436d-105">**Appropriate roles**</span></span>

- <span data-ttu-id="e436d-106">Globální správce</span><span class="sxs-lookup"><span data-stu-id="e436d-106">Global admin</span></span>

<span data-ttu-id="e436d-107">Tato funkce umožňuje spravovat více tenantů vaší společnosti a konsolidovat je do vašeho účtu v Partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="e436d-107">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="e436d-108">Existuje mnoho důvodů, proč možná budete muset ve svém účtu partnerského centra spravovat více tenantů Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e436d-108">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="e436d-109">Například:</span><span class="sxs-lookup"><span data-stu-id="e436d-109">For example:</span></span>

- <span data-ttu-id="e436d-110">Vaše společnost si může koupit jinou společnost a vy chcete, aby zaměstnanci v nové firmě mohli používat Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="e436d-110">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="e436d-111">Chcete však, aby tyto dvě společnosti byly oddělené.</span><span class="sxs-lookup"><span data-stu-id="e436d-111">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="e436d-112">V takovém případě přiřadíte tenanta Azure AD nové společnosti k vašemu globálnímu účtu vašeho partnera (PGA).</span><span class="sxs-lookup"><span data-stu-id="e436d-112">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="e436d-113">Toto přidružení umožní uživatelům v obou společnostech pracovat v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="e436d-113">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="e436d-114">Pokud máte více než jednoho tenanta pro provozování vaší firmy (např. contoso.com, contoso.uk, contoso.in), můžete použít víceklientské prostředí, abyste je mohli spojit se stejným účtem počítače.</span><span class="sxs-lookup"><span data-stu-id="e436d-114">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="e436d-115">Fúze a akvizice vyžaduje, abyste pracovali s více než jedním klientem (např. Pokud společnost Contoso získá společnost Fabrikam, budete muset použít jak Constoso.com, tak Fabrikam.com příslušného tenanta).</span><span class="sxs-lookup"><span data-stu-id="e436d-115">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="e436d-116">Uživatelé ze všech tenantů by museli mít tyto možnosti:</span><span class="sxs-lookup"><span data-stu-id="e436d-116">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="e436d-117">Přístup k partnerským centrům pro školení, digitální stahování, MCP přidružení</span><span class="sxs-lookup"><span data-stu-id="e436d-117">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="e436d-118">Přiřadí se role partnerského centra, jako je například správce programu MPN, pobídka správce atd.</span><span class="sxs-lookup"><span data-stu-id="e436d-118">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="e436d-119">Přidat do svého účtu jiného tenanta Azure AD</span><span class="sxs-lookup"><span data-stu-id="e436d-119">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="e436d-120">Jako globální správce se přihlaste do [řídicího panelu](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="e436d-120">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="e436d-121">V ikoně **Nastavení** vyberte **Nastavení účtu** a pak vyberte **klienti**.</span><span class="sxs-lookup"><span data-stu-id="e436d-121">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="přidružit klienty"::: 

3. <span data-ttu-id="e436d-123">Vyberte **přidružit jiného tenanta služby AD** a určete tenanta, kterého chcete přidružit.</span><span class="sxs-lookup"><span data-stu-id="e436d-123">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="e436d-124">Jako globální správce se přihlaste ke klientovi, kterého chcete přidružit, a potvrďte přidružení.</span><span class="sxs-lookup"><span data-stu-id="e436d-124">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="potvrdit přidružení tenantů"::: 

5. <span data-ttu-id="e436d-126">Po potvrzení se zobrazí všechna oznámení o **sadě** .</span><span class="sxs-lookup"><span data-stu-id="e436d-126">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="e436d-127">Vyberte možnost **vrátit se ke správě tenanta** a uvidíte nově přidaný tenant.</span><span class="sxs-lookup"><span data-stu-id="e436d-127">Select **Return to tenant management** and you'll see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="e436d-128">Tenanta nemůžete přidružit k účtu, pokud je už přidružený k jinému účtu partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="e436d-128">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="e436d-129">Odebrání tenanta z účtu</span><span class="sxs-lookup"><span data-stu-id="e436d-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="e436d-130">Jako globální správce se přihlaste do [řídicího panelu](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="e436d-130">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="e436d-131">V ikoně **Nastavení** vyberte **nastavení účtu** – > tenantů a klikněte na kartu **partner** .</span><span class="sxs-lookup"><span data-stu-id="e436d-131">From the **Settings** icon, select **Account settings** -> Tenants and click on the **Partner** tab.</span></span>
 
3. <span data-ttu-id="e436d-132">Klikněte na odebrat pro tenanta, kterému chcete **Zrušit** přidružení.</span><span class="sxs-lookup"><span data-stu-id="e436d-132">Click **Remove** for the tenant you want to dissociate.</span></span>

4. <span data-ttu-id="e436d-133">Ruší tenant znamená, že uživatelé v tomto tenantovi už nebudou mít přístup k účtu partnerského centra a to může mít dopad na vaše kompetence.</span><span class="sxs-lookup"><span data-stu-id="e436d-133">Dissociating a tenant means that the users on that tenant will no longer have access to the Partner Center account, and this could have an impact on your competencies.</span></span> 

<span data-ttu-id="e436d-134">Tlačítko **Odebrat** je povolené pro všechny přidružené klienty, s výjimkou primárního tenanta a tenanta, ke kterému jste aktuálně přihlášení.</span><span class="sxs-lookup"><span data-stu-id="e436d-134">The **Remove** button is enabled for all associated tenants, except the primary tenant and the tenant which you are currently signed into.</span></span>

:::image type="content" source="images/disassociate.png" alt-text="klienti s tlačítkem odebrat":::
 

## <a name="next-steps"></a><span data-ttu-id="e436d-136">Další kroky</span><span class="sxs-lookup"><span data-stu-id="e436d-136">Next steps</span></span>

- [<span data-ttu-id="e436d-137">Přidávání uživatelů</span><span class="sxs-lookup"><span data-stu-id="e436d-137">Add users</span></span>](create-user-accounts-and-set-permissions.md)






