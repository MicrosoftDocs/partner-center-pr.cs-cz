---
title: Správa uživatelů a uživatelských licencí pro zákaznické účty
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se spravovat uživatele pro vaše zákazníky v partnerském centru, jako je vytváření uživatelských účtů, přidávání nebo odebírání uživatelských licencí, Resetování uživatelských hesel a odstraňování nebo obnovování uživatelských účtů.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: fb7906b006540ef939e443a21855488e9d2c36f9
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/01/2020
ms.locfileid: "96474066"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="680b2-103">Správa uživatelů a uživatelských licencí pro zákaznické účty</span><span class="sxs-lookup"><span data-stu-id="680b2-103">Manage users and user licenses for customer accounts</span></span>

<span data-ttu-id="680b2-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="680b2-104">**Appropriate roles**</span></span>

- <span data-ttu-id="680b2-105">Globální správce</span><span class="sxs-lookup"><span data-stu-id="680b2-105">Global admin</span></span>
- <span data-ttu-id="680b2-106">Správce správy uživatelů</span><span class="sxs-lookup"><span data-stu-id="680b2-106">User management admin</span></span>
- <span data-ttu-id="680b2-107">Agent správce</span><span class="sxs-lookup"><span data-stu-id="680b2-107">Admin agent</span></span>


<span data-ttu-id="680b2-108">Můžete vytvářet a odstraňovat nové uživatele v účtu zákazníka.</span><span class="sxs-lookup"><span data-stu-id="680b2-108">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="680b2-109">Můžete také obnovit jeden nebo více uživatelských účtů, které jste dříve odstranili během 30 dnů od odstranění.</span><span class="sxs-lookup"><span data-stu-id="680b2-109">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="680b2-110">Budou obnovena i předchozí přiřazení předplatného uživatele (za předpokladu, že jsou k dispozici jejich předchozí přidělení).</span><span class="sxs-lookup"><span data-stu-id="680b2-110">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="680b2-111">Když si koupíte nové předplatné pro zákazníka, zákazník by vám měl poskytnout seznam všech uživatelů, kteří budou potřebovat účty, jejich uživatelská oprávnění a to, které služby jednotliví uživatelé potřebují.</span><span class="sxs-lookup"><span data-stu-id="680b2-111">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

<span data-ttu-id="680b2-112">[Odběry můžete přiřadit více uživatelům](bulk-license-provisioning-for-multiple-users.md) najednou pomocí importu názvů pomocí [souboru tabulky. csv kompatibilního s Excelem](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="680b2-112">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="680b2-113">Vytvoření uživatelských účtů pro zákazníka</span><span class="sxs-lookup"><span data-stu-id="680b2-113">Create user accounts for a customer</span></span>

1. <span data-ttu-id="680b2-114">Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="680b2-114">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="680b2-115">V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="680b2-115">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="680b2-116">V nabídce zákazník vyberte **Uživatelé a licence**.</span><span class="sxs-lookup"><span data-stu-id="680b2-116">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="680b2-117">Pro každého uživatele, kterého přidáte, vyberte **Přidat předplatné** a pak vyplňte informace, včetně oprávnění a licencí.</span><span class="sxs-lookup"><span data-stu-id="680b2-117">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="680b2-118">**Uložte** změny.</span><span class="sxs-lookup"><span data-stu-id="680b2-118">**Save** your changes.</span></span>

5. <span data-ttu-id="680b2-119">Nezapomeňte zaznamenat uživatelské jméno a dočasné heslo pro odeslání uživateli.</span><span class="sxs-lookup"><span data-stu-id="680b2-119">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="680b2-120">Pokud současně přidáváte více uživatelů, použijte **Přidat jiného uživatele**.</span><span class="sxs-lookup"><span data-stu-id="680b2-120">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="680b2-121">Můžete také přidat více uživatelů najednou [importováním souboru tabulky CSV kompatibilního s Excelem](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="680b2-121">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="680b2-122">Před odesláním e-mailu nebo tiskem názvů a hesel z potvrzovací obrazovky můžete počkat, dokud nedokončíte celou sadu.</span><span class="sxs-lookup"><span data-stu-id="680b2-122">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="680b2-123">Přidání nebo odebrání uživatelských licencí pro zákazníka</span><span class="sxs-lookup"><span data-stu-id="680b2-123">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="680b2-124">Následující postup platí pro přidání nebo odebrání uživatelských licencí pro produkty společnosti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="680b2-124">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="680b2-125">Pokud chcete přidat nebo odebrat uživatelské licence pro odběry SaaS založené na licencích na komerčním webu Marketplace, přečtěte si téma [Přidání nebo odebrání licencí pro předplatné SaaS](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span><span class="sxs-lookup"><span data-stu-id="680b2-125">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="680b2-126">Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="680b2-126">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="680b2-127">V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="680b2-127">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="680b2-128">V nabídce zákazník vyberte **Uživatelé a licence**.</span><span class="sxs-lookup"><span data-stu-id="680b2-128">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="680b2-129">Vyberte jednoho nebo více uživatelů ze seznamu.</span><span class="sxs-lookup"><span data-stu-id="680b2-129">Choose one or more users from the list.</span></span> <span data-ttu-id="680b2-130">Pokud například zákazník právě koupil nové licence a chtěli jste jim přiřadit lidi, kteří je ještě nemají, můžete k vyhledání správné skupiny použít možnost **filtrovat uživatele podle..** ..</span><span class="sxs-lookup"><span data-stu-id="680b2-130">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="680b2-131">Vyberte **spravovat licence**.</span><span class="sxs-lookup"><span data-stu-id="680b2-131">Select **Manage licenses**.</span></span> <span data-ttu-id="680b2-132">Proveďte změny a pak ho **uložte**.</span><span class="sxs-lookup"><span data-stu-id="680b2-132">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="680b2-133">U [Azure Marketplace produktů](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)se přiřazení licencí a aktivace spravují prostřednictvím nezávislého výrobce softwaru (ISV), který produkt zveřejnil.</span><span class="sxs-lookup"><span data-stu-id="680b2-133">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="680b2-134">Resetování hesla uživatele pro zákazníka</span><span class="sxs-lookup"><span data-stu-id="680b2-134">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="680b2-135">Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="680b2-135">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="680b2-136">V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="680b2-136">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3.  <span data-ttu-id="680b2-137">V nabídce zákazník vyberte **Uživatelé a licence**.</span><span class="sxs-lookup"><span data-stu-id="680b2-137">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="680b2-138">Vyberte uživatele ze seznamu.</span><span class="sxs-lookup"><span data-stu-id="680b2-138">Choose the user from the list.</span></span>

4.  <span data-ttu-id="680b2-139">V dolní části obrazovky vyberte **resetovat heslo**.</span><span class="sxs-lookup"><span data-stu-id="680b2-139">At the bottom of the screen, select **Reset password**.</span></span> 

5.  <span data-ttu-id="680b2-140">Poslat uživateli nové dočasné heslo.</span><span class="sxs-lookup"><span data-stu-id="680b2-140">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="680b2-141">Odstranění uživatelských účtů pro zákazníka</span><span class="sxs-lookup"><span data-stu-id="680b2-141">Delete user accounts for a customer</span></span>

1.  <span data-ttu-id="680b2-142">V nabídce **Partnerské centrum** vyberte **zákazníci**.</span><span class="sxs-lookup"><span data-stu-id="680b2-142">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="680b2-143">Vyberte zákazníka ze seznamu.</span><span class="sxs-lookup"><span data-stu-id="680b2-143">Choose the customer from the list.</span></span>

2.  <span data-ttu-id="680b2-144">V nabídce zákazník vyberte **Uživatelé a licence**.</span><span class="sxs-lookup"><span data-stu-id="680b2-144">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="680b2-145">Vyberte uživatele ze seznamu.</span><span class="sxs-lookup"><span data-stu-id="680b2-145">Choose the user from the list.</span></span>

3.  <span data-ttu-id="680b2-146">V dolní části obrazovky vyberte **Odstranit uživatelský účet**.</span><span class="sxs-lookup"><span data-stu-id="680b2-146">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="680b2-147">Pokud potřebujete tento účet obnovit, můžete ho najít na kartě **odstraněné uživatele** v seznamu **Uživatelé a licence** zákazníka.</span><span class="sxs-lookup"><span data-stu-id="680b2-147">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="680b2-148">K obnovení odstraněného uživatele máte 30 dní.</span><span class="sxs-lookup"><span data-stu-id="680b2-148">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="680b2-149">Obnovení odstraněných uživatelských účtů</span><span class="sxs-lookup"><span data-stu-id="680b2-149">Restore deleted user accounts</span></span>

1.  <span data-ttu-id="680b2-150">V nabídce **Partnerské centrum** vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="680b2-150">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2.  <span data-ttu-id="680b2-151">Vyberte **Uživatelé a licence**.</span><span class="sxs-lookup"><span data-stu-id="680b2-151">Select **Users and licenses**.</span></span>

3.  <span data-ttu-id="680b2-152">Vyberte kartu **odstraněné uživatele ()** . V případě odstranění uživatelů, které lze obnovit, by mělo být přečteno **(1)** nebo vyšší.</span><span class="sxs-lookup"><span data-stu-id="680b2-152">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4.  <span data-ttu-id="680b2-153">Zaškrtněte jedno nebo více políček Odstraněná uživatelé a pak vyberte **obnovit**.</span><span class="sxs-lookup"><span data-stu-id="680b2-153">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="680b2-154">Všechny vybrané uživatelské účty se znovu zobrazí na stránce **Uživatelé a licence** .</span><span class="sxs-lookup"><span data-stu-id="680b2-154">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="related-topics"></a><span data-ttu-id="680b2-155">Související témata</span><span class="sxs-lookup"><span data-stu-id="680b2-155">Related topics</span></span>


[<span data-ttu-id="680b2-156">Přiřazení licencí několika uživatelům nebo jejich odvolání</span><span class="sxs-lookup"><span data-stu-id="680b2-156">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

[<span data-ttu-id="680b2-157">Vytvoření více uživatelů pro účet zákazníka</span><span class="sxs-lookup"><span data-stu-id="680b2-157">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)