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
ms.openlocfilehash: caea2002b5edc2958c0af316762408e309bcf14a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151198"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="13637-103">Přidání a správa několika tenantů v účtu partnerského centra</span><span class="sxs-lookup"><span data-stu-id="13637-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="13637-104">**Příslušné role**: globální správce | Správce účtu</span><span class="sxs-lookup"><span data-stu-id="13637-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="13637-105">Tento článek popisuje, jak sloučit více tenantů Azure Active Directory (Azure AD) pro vaši společnost a pak je přidat a spravovat v účtu partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="13637-105">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="13637-106">K tomu je potřeba celá řada důvodů.</span><span class="sxs-lookup"><span data-stu-id="13637-106">There are many reasons to do so.</span></span> <span data-ttu-id="13637-107">Například:</span><span class="sxs-lookup"><span data-stu-id="13637-107">For example:</span></span>

- <span data-ttu-id="13637-108">Řekněme, že vaše společnost Contoso získala jinou společnost Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="13637-108">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="13637-109">Chcete, aby tyto dvě společnosti byly oddělené, ale chcete, aby noví zaměstnanci mohli používat Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="13637-109">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="13637-110">V takovém případě přidružíte tenanta Azure AD nové společnosti k globálnímu účtu vašeho partnera (PGA).</span><span class="sxs-lookup"><span data-stu-id="13637-110">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="13637-111">Toto přidružení umožňuje uživatelům v obou společnostech pracovat v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="13637-111">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="13637-112">Pokud svou firmu spustíte s více než jedním klientem (například *contoso.com*, *contoso.UK* a *contoso.in*), můžete pomocí víceklientské architektury seskupovat do stejného účtu počítače.</span><span class="sxs-lookup"><span data-stu-id="13637-112">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="13637-113">Pokud pokyny pro fúze a získání vyžadují, abyste mohli pracovat s klienty obou společností, použijte klienty *constoso.com* i *fabrikam.com* .</span><span class="sxs-lookup"><span data-stu-id="13637-113">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="13637-114">Uživatelé kteréhokoli klienta musí být schopni:</span><span class="sxs-lookup"><span data-stu-id="13637-114">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="13637-115">Přístup k partnerskému centru pro školení, digitální stahování nebo přidružení Microsoft Certified Professional (MCP)</span><span class="sxs-lookup"><span data-stu-id="13637-115">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="13637-116">Přiřadí se role partnerského centra, jako je například správce programu Microsoft Partner Network (MPN) nebo správce pobídek.</span><span class="sxs-lookup"><span data-stu-id="13637-116">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="13637-117">Přidání tenanta Azure AD ke svému účtu</span><span class="sxs-lookup"><span data-stu-id="13637-117">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="13637-118">Přihlaste se jako globální správce do [partnerského centra Microsoftu](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="13637-118">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="13637-119">V pravém horním rohu vyberte **Nastavení**, vyberte **Nastavení účtu** a pak vyberte **klienti**.</span><span class="sxs-lookup"><span data-stu-id="13637-119">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Snímek obrazovky s tlačítkem přidružit v podokně profilu Azure AD"::: 

1. <span data-ttu-id="13637-121">Vyberte **přidružit** a pak určete tenanta, kterého chcete přidružit.</span><span class="sxs-lookup"><span data-stu-id="13637-121">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="13637-122">Na příkazovém řádku se přihlaste jako globální správce k tenantovi, kterého chcete přidružit, a pak vyberte **Potvrdit.**</span><span class="sxs-lookup"><span data-stu-id="13637-122">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Snímek obrazovky s tlačítkem Potvrdit v podokně Potvrdit nové přidružení Azure AD"::: 

   <span data-ttu-id="13637-124">Po potvrzení přidružení se zobrazí zpráva **All set (Vše** nastaveno).</span><span class="sxs-lookup"><span data-stu-id="13637-124">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="13637-125">Pokud chcete zobrazit nově přidaného tenanta, vyberte **Return to tenant management (Vrátit se ke správě tenanta).**</span><span class="sxs-lookup"><span data-stu-id="13637-125">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="13637-126">Tenanta nemůžete přidružit k účtu, pokud už je přidružený k jinému Partnerské centrum účtu.</span><span class="sxs-lookup"><span data-stu-id="13637-126">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="13637-127">Odebrání tenanta z účtu</span><span class="sxs-lookup"><span data-stu-id="13637-127">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="13637-128">Přihlaste se jako globální správce k [Microsoft Partnerské centrum](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="13637-128">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="13637-129">V pravém horním rohu vyberte **ikonu Nastavení** a pak vyberte **Nastavení účtu**.</span><span class="sxs-lookup"><span data-stu-id="13637-129">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="13637-130">V levém podokně vyberte **Tenanti.**</span><span class="sxs-lookup"><span data-stu-id="13637-130">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="13637-131">V **části Spravovat tenanty Azure AD** vyberte **kartu** Partner.</span><span class="sxs-lookup"><span data-stu-id="13637-131">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="13637-132">Vedle **tenanta,** jehož přidružení chcete odebrat, vyberte Odebrat.</span><span class="sxs-lookup"><span data-stu-id="13637-132">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="Snímek obrazovky s aktuálními přidruženími tenantů a jejich odkazy Odebrat":::

   <span data-ttu-id="13637-134">Jak je znázorněno na  předchozím snímku obrazovky, odkazy Odebrat jsou povolené pro všechny přidružené tenanty s výjimkou primárního tenanta a tenanta, ke které jste aktuálně přihlášení.</span><span class="sxs-lookup"><span data-stu-id="13637-134">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="13637-135">Když odeberete tenanta, uživatelé v tomto tenantovi už nebudou mít přístup k účtu Partnerské centrum a odebrání může mít vliv na vaše kompetence.</span><span class="sxs-lookup"><span data-stu-id="13637-135">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="13637-136">Další kroky</span><span class="sxs-lookup"><span data-stu-id="13637-136">Next steps</span></span>

- [<span data-ttu-id="13637-137">Vytváření uživatelských účtů</span><span class="sxs-lookup"><span data-stu-id="13637-137">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






