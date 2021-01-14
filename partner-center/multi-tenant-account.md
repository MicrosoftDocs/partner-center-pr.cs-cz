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
ms.openlocfilehash: f9852b4e1c3997b82f744555db25fe64e1afc8ad
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182425"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="04a98-104">Přidání a správa několika tenantů v účtu partnerského centra</span><span class="sxs-lookup"><span data-stu-id="04a98-104">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="04a98-105">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="04a98-105">**Appropriate roles**</span></span>

- <span data-ttu-id="04a98-106">Globální správce</span><span class="sxs-lookup"><span data-stu-id="04a98-106">Global admin</span></span>
- <span data-ttu-id="04a98-107">Správce účtu</span><span class="sxs-lookup"><span data-stu-id="04a98-107">Account admin</span></span>

<span data-ttu-id="04a98-108">Tato funkce umožňuje spravovat více tenantů vaší společnosti a konsolidovat je do vašeho účtu v Partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="04a98-108">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="04a98-109">Existuje mnoho důvodů, proč možná budete muset ve svém účtu partnerského centra spravovat více tenantů Azure AD.</span><span class="sxs-lookup"><span data-stu-id="04a98-109">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="04a98-110">Příklad:</span><span class="sxs-lookup"><span data-stu-id="04a98-110">For example:</span></span>

- <span data-ttu-id="04a98-111">Vaše společnost si může koupit jinou společnost a vy chcete, aby zaměstnanci v nové firmě mohli používat Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="04a98-111">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="04a98-112">Chcete však, aby tyto dvě společnosti byly oddělené.</span><span class="sxs-lookup"><span data-stu-id="04a98-112">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="04a98-113">V takovém případě přiřadíte tenanta Azure AD nové společnosti k vašemu globálnímu účtu vašeho partnera (PGA).</span><span class="sxs-lookup"><span data-stu-id="04a98-113">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="04a98-114">Toto přidružení umožní uživatelům v obou společnostech pracovat v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="04a98-114">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="04a98-115">Pokud máte více než jednoho tenanta pro provozování vaší firmy (např. contoso.com, contoso.uk, contoso.in), můžete použít víceklientské prostředí, abyste je mohli spojit se stejným účtem počítače.</span><span class="sxs-lookup"><span data-stu-id="04a98-115">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="04a98-116">Fúze a akvizice vyžaduje, abyste pracovali s více než jedním klientem (např. Pokud společnost Contoso získá společnost Fabrikam, budete muset použít jak Constoso.com, tak Fabrikam.com příslušného tenanta).</span><span class="sxs-lookup"><span data-stu-id="04a98-116">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="04a98-117">Uživatelé ze všech tenantů by museli mít tyto možnosti:</span><span class="sxs-lookup"><span data-stu-id="04a98-117">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="04a98-118">Přístup k partnerským centrům pro školení, digitální stahování, MCP přidružení</span><span class="sxs-lookup"><span data-stu-id="04a98-118">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="04a98-119">Přiřadí se role partnerského centra, jako je například správce programu MPN, pobídka správce atd.</span><span class="sxs-lookup"><span data-stu-id="04a98-119">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="04a98-120">Přidat do svého účtu jiného tenanta Azure AD</span><span class="sxs-lookup"><span data-stu-id="04a98-120">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="04a98-121">Jako globální správce se přihlaste do [řídicího panelu](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="04a98-121">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="04a98-122">V ikoně **Nastavení** vyberte **Nastavení účtu** a pak vyberte **klienti**.</span><span class="sxs-lookup"><span data-stu-id="04a98-122">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="přidružit klienty"::: 

3. <span data-ttu-id="04a98-124">Vyberte **přidružit jiného tenanta služby AD** a určete tenanta, kterého chcete přidružit.</span><span class="sxs-lookup"><span data-stu-id="04a98-124">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="04a98-125">Jako globální správce se přihlaste ke klientovi, kterého chcete přidružit, a potvrďte přidružení.</span><span class="sxs-lookup"><span data-stu-id="04a98-125">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="potvrdit přidružení tenantů"::: 

5. <span data-ttu-id="04a98-127">Po potvrzení se zobrazí všechna oznámení o **sadě** .</span><span class="sxs-lookup"><span data-stu-id="04a98-127">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="04a98-128">Vyberte možnost **vrátit se ke správě tenanta** a uvidíte nově přidaný tenant.</span><span class="sxs-lookup"><span data-stu-id="04a98-128">Select **Return to tenant management** and you'll see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="04a98-129">Tenanta nemůžete přidružit k účtu, pokud je už přidružený k jinému účtu partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="04a98-129">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="04a98-130">Odebrání tenanta z účtu</span><span class="sxs-lookup"><span data-stu-id="04a98-130">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="04a98-131">Jako globální správce se přihlaste do [řídicího panelu](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="04a98-131">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="04a98-132">V ikoně **Nastavení** vyberte **nastavení účtu** – > tenantů a klikněte na kartu **partner** .</span><span class="sxs-lookup"><span data-stu-id="04a98-132">From the **Settings** icon, select **Account settings** -> Tenants and click on the **Partner** tab.</span></span>
 
3. <span data-ttu-id="04a98-133">Klikněte na odebrat pro tenanta, kterému chcete **Zrušit** přidružení.</span><span class="sxs-lookup"><span data-stu-id="04a98-133">Click **Remove** for the tenant you want to dissociate.</span></span>

4. <span data-ttu-id="04a98-134">Ruší tenant znamená, že uživatelé v tomto tenantovi už nebudou mít přístup k účtu partnerského centra a to může mít dopad na vaše kompetence.</span><span class="sxs-lookup"><span data-stu-id="04a98-134">Dissociating a tenant means that the users on that tenant will no longer have access to the Partner Center account, and this could have an impact on your competencies.</span></span> 

<span data-ttu-id="04a98-135">Tlačítko **Odebrat** je povolené pro všechny přidružené klienty, s výjimkou primárního tenanta a tenanta, ke kterému jste aktuálně přihlášení.</span><span class="sxs-lookup"><span data-stu-id="04a98-135">The **Remove** button is enabled for all associated tenants, except the primary tenant and the tenant which you are currently signed into.</span></span>

:::image type="content" source="images/disassociate.png" alt-text="klienti s tlačítkem odebrat":::
 

## <a name="next-steps"></a><span data-ttu-id="04a98-137">Další kroky</span><span class="sxs-lookup"><span data-stu-id="04a98-137">Next steps</span></span>

- [<span data-ttu-id="04a98-138">Přidávání uživatelů</span><span class="sxs-lookup"><span data-stu-id="04a98-138">Add users</span></span>](create-user-accounts-and-set-permissions.md)






