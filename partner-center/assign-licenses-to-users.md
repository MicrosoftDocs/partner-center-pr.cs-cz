---
title: Správa uživatelů pro zákaznické účty
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Správa uživatelů pro zákazníky v Partnerské centrum – vytváření uživatelských účtů, přidávání nebo odebírání uživatelských licencí, resetování hesel a odstraňování nebo obnovení uživatelských účtů.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc896ec3ce16ab0f05a8131de14f573ad96a8141
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149889"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="2affb-103">Správa uživatelů a uživatelských licencí pro zákaznické účty</span><span class="sxs-lookup"><span data-stu-id="2affb-103">Manage users and user licenses for customer accounts</span></span> 

<span data-ttu-id="2affb-104">**Odpovídající role:** Globální správce | Správce správy uživatelů | Agent pro správu</span><span class="sxs-lookup"><span data-stu-id="2affb-104">**Appropriate roles**: Global admin | User management admin | Admin agent</span></span>


<span data-ttu-id="2affb-105">V účtu zákazníka můžete vytvářet a odstraňovat nové uživatele.</span><span class="sxs-lookup"><span data-stu-id="2affb-105">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="2affb-106">Můžete také obnovit jeden nebo více uživatelských účtů, které jste předtím odstranili do 30 dnů od odstranění.</span><span class="sxs-lookup"><span data-stu-id="2affb-106">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="2affb-107">Obnoví se také předchozí přiřazení předplatného uživatele (za předpokladu, že jsou k dispozici jeho předchozí přidělení).</span><span class="sxs-lookup"><span data-stu-id="2affb-107">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="2affb-108">Když zákazníkovi zakoupíte nová předplatná, měl by vám poskytnout seznam všech uživatelů, kteří budou potřebovat účty, jejich uživatelská oprávnění a služby, které každý uživatel potřebuje.</span><span class="sxs-lookup"><span data-stu-id="2affb-108">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

>[!NOTE]
><span data-ttu-id="2affb-109">V **části** Uživatelé a  licence na kartě Zákazník se zobrazují všichni uživatelé vytvoření v tenantovi konkrétního zákazníka, včetně uživatelů, kteří mají licence zakoupené od jiného partnera CSP nebo z jiného nákupního kanálu.</span><span class="sxs-lookup"><span data-stu-id="2affb-109">The **Users and licenses** section of **Customer** tab shows all users created in a specific customer’s tenant, including users that have licenses purchased from another CSP partner or from another purchasing channel.</span></span>

<span data-ttu-id="2affb-110">Odběry [můžete přiřadit více uživatelům](bulk-license-provisioning-for-multiple-users.md) najednou importem názvů pomocí souboru tabulky CSV [kompatibilního s Excelem.](adding-multiple-users-to-a-customer-account.md)</span><span class="sxs-lookup"><span data-stu-id="2affb-110">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="2affb-111">Vytvoření uživatelských účtů pro zákazníka</span><span class="sxs-lookup"><span data-stu-id="2affb-111">Create user accounts for a customer</span></span>

1. <span data-ttu-id="2affb-112">Přihlaste se k Partnerské centrum [řídicího panelu.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="2affb-112">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="2affb-113">V Partnerské centrum vyberte **Zákazníci** a pak v seznamu zvolte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="2affb-113">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="2affb-114">V nabídce zákazníka vyberte **Uživatelé a licence.**</span><span class="sxs-lookup"><span data-stu-id="2affb-114">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="2affb-115">Pro každého uživatele, který přidáte, vyberte **Přidat předplatné** a vyplňte informace, včetně oprávnění a licencí.</span><span class="sxs-lookup"><span data-stu-id="2affb-115">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="2affb-116">**Uložte** změny.</span><span class="sxs-lookup"><span data-stu-id="2affb-116">**Save** your changes.</span></span>

5. <span data-ttu-id="2affb-117">Nezapomeňte si zaznamenat uživatelské jméno a dočasné heslo, které chcete uživateli odeslat.</span><span class="sxs-lookup"><span data-stu-id="2affb-117">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="2affb-118">Pokud přidáváte více uživatelů po jednom, použijte **možnost Přidat dalšího uživatele**.</span><span class="sxs-lookup"><span data-stu-id="2affb-118">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="2affb-119">Můžete také přidat více uživatelů najednou importem souboru tabulky .csv kompatibilního [s Excelem.](adding-multiple-users-to-a-customer-account.md)</span><span class="sxs-lookup"><span data-stu-id="2affb-119">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="2affb-120">Před odesláním e-mailu nebo tisku jmen a hesel z potvrzovací obrazovky můžete počkat, až s celou sadu skončíte.</span><span class="sxs-lookup"><span data-stu-id="2affb-120">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="2affb-121">Přiřazení nebo odebrání uživatelských licencí zákazníkovi</span><span class="sxs-lookup"><span data-stu-id="2affb-121">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="2affb-122">Následující postup se týká přidávání nebo odebírání uživatelských licencí pro produkty Microsoftu.</span><span class="sxs-lookup"><span data-stu-id="2affb-122">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="2affb-123">Pokud chcete přidat nebo odebrat uživatelské licence pro předplatná SaaS založená na licencích na komerčním marketplace, podívejte se na stránku Přidání nebo odebrání licencí [pro předplatné SaaS.](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)</span><span class="sxs-lookup"><span data-stu-id="2affb-123">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="2affb-124">Přihlaste se k Partnerské centrum [řídicího panelu.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="2affb-124">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="2affb-125">V Partnerské centrum vyberte **Zákazníci** a pak v seznamu zvolte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="2affb-125">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="2affb-126">V nabídce zákazníka vyberte **Uživatelé a licence.**</span><span class="sxs-lookup"><span data-stu-id="2affb-126">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="2affb-127">Vyberte v seznamu alespoň jednoho uživatele.</span><span class="sxs-lookup"><span data-stu-id="2affb-127">Choose one or more users from the list.</span></span> <span data-ttu-id="2affb-128">Pokud například zákazník právě zakoupil nové licence a vy jste je chtěli přiřadit lidem, kteří je  ještě nemají, můžete najít správnou skupinu pomocí možnosti Filtrovat uživatele podle.</span><span class="sxs-lookup"><span data-stu-id="2affb-128">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="2affb-129">Vyberte **Spravovat licence**.</span><span class="sxs-lookup"><span data-stu-id="2affb-129">Select **Manage licenses**.</span></span> <span data-ttu-id="2affb-130">Proveďte změny a pak **klikněte na Uložit.**</span><span class="sxs-lookup"><span data-stu-id="2affb-130">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="2affb-131">U [Azure Marketplace se](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)přiřazení licencí a aktivace spravují prostřednictvím nezávislého výrobce softwaru (ISV), který produkt publikoval.</span><span class="sxs-lookup"><span data-stu-id="2affb-131">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="2affb-132">Resetování hesla uživatele pro zákazníka</span><span class="sxs-lookup"><span data-stu-id="2affb-132">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="2affb-133">Přihlaste se k [řídicímu panelu](https://partner.microsoft.com/dashboard) pro Partnerské centrum.</span><span class="sxs-lookup"><span data-stu-id="2affb-133">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="2affb-134">V Partnerské centrum vyberte **Zákazníci** a pak v seznamu zvolte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="2affb-134">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="2affb-135">V nabídce zákazníka vyberte **Uživatelé a licence.**</span><span class="sxs-lookup"><span data-stu-id="2affb-135">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="2affb-136">Vyberte uživatele ze seznamu.</span><span class="sxs-lookup"><span data-stu-id="2affb-136">Choose the user from the list.</span></span>

4. <span data-ttu-id="2affb-137">V dolní části obrazovky vyberte **Resetovat heslo.**</span><span class="sxs-lookup"><span data-stu-id="2affb-137">At the bottom of the screen, select **Reset password**.</span></span> 

5. <span data-ttu-id="2affb-138">Odešlete nové dočasné heslo uživateli.</span><span class="sxs-lookup"><span data-stu-id="2affb-138">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="2affb-139">Odstranění uživatelských účtů pro zákazníka</span><span class="sxs-lookup"><span data-stu-id="2affb-139">Delete user accounts for a customer</span></span>

1. <span data-ttu-id="2affb-140">V **nabídce Partnerské centrum** vyberte **Zákazníci.**</span><span class="sxs-lookup"><span data-stu-id="2affb-140">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="2affb-141">V seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="2affb-141">Choose the customer from the list.</span></span>

2. <span data-ttu-id="2affb-142">V nabídce zákazníka vyberte **Uživatelé a licence.**</span><span class="sxs-lookup"><span data-stu-id="2affb-142">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="2affb-143">Vyberte uživatele ze seznamu.</span><span class="sxs-lookup"><span data-stu-id="2affb-143">Choose the user from the list.</span></span>

3. <span data-ttu-id="2affb-144">V dolní části obrazovky vyberte **Odstranit uživatelský účet**.</span><span class="sxs-lookup"><span data-stu-id="2affb-144">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="2affb-145">Pokud potřebujete tento účet obnovit, najdete ho  v seznamu Uživatelé a licence zákazníka na **kartě Odstranění** uživatelé.</span><span class="sxs-lookup"><span data-stu-id="2affb-145">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="2affb-146">K obnovení odstraněného uživatele máte 30 dní.</span><span class="sxs-lookup"><span data-stu-id="2affb-146">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="2affb-147">Obnovení odstraněných uživatelských účtů</span><span class="sxs-lookup"><span data-stu-id="2affb-147">Restore deleted user accounts</span></span>

1. <span data-ttu-id="2affb-148">V nabídce **Partnerské centrum** vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="2affb-148">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2. <span data-ttu-id="2affb-149">Vyberte **Uživatelé a licence**.</span><span class="sxs-lookup"><span data-stu-id="2affb-149">Select **Users and licenses**.</span></span>

3. <span data-ttu-id="2affb-150">Vyberte kartu **odstraněné uživatele ()** . V případě odstranění uživatelů, které lze obnovit, by mělo být přečteno **(1)** nebo vyšší.</span><span class="sxs-lookup"><span data-stu-id="2affb-150">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4. <span data-ttu-id="2affb-151">Zaškrtněte jedno nebo více políček Odstraněná uživatelé a pak vyberte **obnovit**.</span><span class="sxs-lookup"><span data-stu-id="2affb-151">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="2affb-152">Všechny vybrané uživatelské účty se znovu zobrazí na stránce **Uživatelé a licence** .</span><span class="sxs-lookup"><span data-stu-id="2affb-152">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2affb-153">Další kroky</span><span class="sxs-lookup"><span data-stu-id="2affb-153">Next steps</span></span>

- [<span data-ttu-id="2affb-154">Přiřazení licencí několika uživatelům nebo jejich odvolání</span><span class="sxs-lookup"><span data-stu-id="2affb-154">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

- [<span data-ttu-id="2affb-155">Vytvoření více uživatelů pro účet zákazníka</span><span class="sxs-lookup"><span data-stu-id="2affb-155">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)