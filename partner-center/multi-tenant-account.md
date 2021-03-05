---
title: Přidání tenantů k účtu partnerského centra
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se přidávat, konsolidovat nebo spravovat více tenantů Azure AD v účtu partnerského centra a zjistit, proč to budete chtít udělat.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124801"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="b7723-103">Přidání a správa několika tenantů v účtu partnerského centra</span><span class="sxs-lookup"><span data-stu-id="b7723-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="b7723-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="b7723-104">**Appropriate roles**</span></span>

- <span data-ttu-id="b7723-105">Globální správce</span><span class="sxs-lookup"><span data-stu-id="b7723-105">Global admin</span></span>
- <span data-ttu-id="b7723-106">Správce účtu</span><span class="sxs-lookup"><span data-stu-id="b7723-106">Account admin</span></span>

<span data-ttu-id="b7723-107">Tento článek popisuje, jak sloučit více tenantů Azure Active Directory (Azure AD) pro vaši společnost a pak je přidat a spravovat v účtu partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="b7723-107">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="b7723-108">K tomu je potřeba celá řada důvodů.</span><span class="sxs-lookup"><span data-stu-id="b7723-108">There are many reasons to do so.</span></span> <span data-ttu-id="b7723-109">Například:</span><span class="sxs-lookup"><span data-stu-id="b7723-109">For example:</span></span>

- <span data-ttu-id="b7723-110">Řekněme, že vaše společnost Contoso získala jinou společnost Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="b7723-110">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="b7723-111">Chcete, aby tyto dvě společnosti byly oddělené, ale chcete, aby noví zaměstnanci mohli používat Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="b7723-111">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="b7723-112">V takovém případě přidružíte tenanta Azure AD nové společnosti k globálnímu účtu vašeho partnera (PGA).</span><span class="sxs-lookup"><span data-stu-id="b7723-112">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="b7723-113">Toto přidružení umožňuje uživatelům v obou společnostech pracovat v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="b7723-113">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="b7723-114">Pokud svou firmu spustíte s více než jedním klientem (například *contoso.com*, *contoso.UK* a *contoso.in*), můžete pomocí víceklientské architektury seskupovat do stejného účtu počítače.</span><span class="sxs-lookup"><span data-stu-id="b7723-114">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="b7723-115">Pokud pokyny pro fúze a získání vyžadují, abyste mohli pracovat s klienty obou společností, použijte klienty *constoso.com* i *fabrikam.com* .</span><span class="sxs-lookup"><span data-stu-id="b7723-115">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="b7723-116">Uživatelé kteréhokoli klienta musí být schopni:</span><span class="sxs-lookup"><span data-stu-id="b7723-116">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="b7723-117">Přístup k partnerskému centru pro školení, digitální stahování nebo přidružení Microsoft Certified Professional (MCP)</span><span class="sxs-lookup"><span data-stu-id="b7723-117">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="b7723-118">Přiřadí se role partnerského centra, jako je například správce programu Microsoft Partner Network (MPN) nebo správce pobídek.</span><span class="sxs-lookup"><span data-stu-id="b7723-118">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="b7723-119">Přidání tenanta Azure AD ke svému účtu</span><span class="sxs-lookup"><span data-stu-id="b7723-119">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="b7723-120">Přihlaste se jako globální správce do [partnerského centra Microsoftu](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="b7723-120">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="b7723-121">V pravém horním rohu vyberte **Nastavení**, vyberte **Nastavení účtu** a pak vyberte **klienti**.</span><span class="sxs-lookup"><span data-stu-id="b7723-121">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Snímek obrazovky s tlačítkem přidružit v podokně profilu Azure AD"::: 

1. <span data-ttu-id="b7723-123">Vyberte **přidružit** a pak určete tenanta, kterého chcete přidružit.</span><span class="sxs-lookup"><span data-stu-id="b7723-123">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="b7723-124">Na příkazovém řádku se přihlaste jako globální správce do tenanta, kterého chcete přidružit, a pak vyberte **Potvrdit**.</span><span class="sxs-lookup"><span data-stu-id="b7723-124">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Snímek obrazovky s tlačítkem potvrdit v podokně potvrdit nové přidružení Azure AD"::: 

   <span data-ttu-id="b7723-126">Po potvrzení přidružení se zobrazí zpráva **všechna sada** .</span><span class="sxs-lookup"><span data-stu-id="b7723-126">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="b7723-127">Chcete-li zobrazit nově přidaného tenanta, vyberte možnost **vrátit se ke správě tenanta**.</span><span class="sxs-lookup"><span data-stu-id="b7723-127">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="b7723-128">Nemůžete přidružit klienta k účtu, pokud je už přidružený k jinému účtu partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="b7723-128">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="b7723-129">Odebrání tenanta z účtu</span><span class="sxs-lookup"><span data-stu-id="b7723-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="b7723-130">Přihlaste se jako globální správce do [partnerského centra Microsoftu](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="b7723-130">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="b7723-131">V pravém horním rohu vyberte ikonu **Nastavení** a pak vyberte **Nastavení účtu**.</span><span class="sxs-lookup"><span data-stu-id="b7723-131">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="b7723-132">V levém podokně vyberte možnost **klienti**.</span><span class="sxs-lookup"><span data-stu-id="b7723-132">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="b7723-133">V části **spravovat klienty Azure AD** vyberte kartu **partner** .</span><span class="sxs-lookup"><span data-stu-id="b7723-133">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="b7723-134">Vyberte **Odebrat** vedle tenanta, jehož přidružení chcete odebrat.</span><span class="sxs-lookup"><span data-stu-id="b7723-134">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="Snímek obrazovky aktuálních přidružení klientů a jejich odkazy pro odebrání":::

   <span data-ttu-id="b7723-136">Jak je znázorněno na předchozím snímku obrazovky, odkazy **Odebrat** jsou povolené pro všechny přidružené klienty, s výjimkou primárního tenanta a tenanta, ke kterému jste aktuálně přihlášení.</span><span class="sxs-lookup"><span data-stu-id="b7723-136">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="b7723-137">Když odeberete tenanta, uživatelé tohoto tenanta už nebudou mít přístup k účtu partnerského centra a odebrání můžou mít dopad na vaše kompetence.</span><span class="sxs-lookup"><span data-stu-id="b7723-137">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="b7723-138">Další kroky</span><span class="sxs-lookup"><span data-stu-id="b7723-138">Next steps</span></span>

- [<span data-ttu-id="b7723-139">Vytváření uživatelských účtů</span><span class="sxs-lookup"><span data-stu-id="b7723-139">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






