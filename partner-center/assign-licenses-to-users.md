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
ms.openlocfilehash: fc208283e0ed8c0f164a44cc9bd70260b8671c6e
ms.sourcegitcommit: 22af0997d52a87417b62f44fb0a7d711bec77b35
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/19/2020
ms.locfileid: "92527790"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="5b3ce-103">Správa uživatelů a uživatelských licencí pro zákaznické účty</span><span class="sxs-lookup"><span data-stu-id="5b3ce-103">Manage users and user licenses for customer accounts</span></span>

<span data-ttu-id="5b3ce-104">**Platí pro**</span><span class="sxs-lookup"><span data-stu-id="5b3ce-104">**Applies to**</span></span>

- <span data-ttu-id="5b3ce-105">Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="5b3ce-105">Partner Center</span></span>

<span data-ttu-id="5b3ce-106">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="5b3ce-106">**Appropriate roles**</span></span>

- <span data-ttu-id="5b3ce-107">Globální správce</span><span class="sxs-lookup"><span data-stu-id="5b3ce-107">Global admin</span></span>
- <span data-ttu-id="5b3ce-108">Správce správy uživatelů</span><span class="sxs-lookup"><span data-stu-id="5b3ce-108">User management admin</span></span>
- <span data-ttu-id="5b3ce-109">Agent správce</span><span class="sxs-lookup"><span data-stu-id="5b3ce-109">Admin agent</span></span>
- <span data-ttu-id="5b3ce-110">Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="5b3ce-110">Sales agent</span></span>
- <span data-ttu-id="5b3ce-111">Agent helpdesku</span><span class="sxs-lookup"><span data-stu-id="5b3ce-111">Helpdesk agent</span></span>

<span data-ttu-id="5b3ce-112">Můžete vytvářet a odstraňovat nové uživatele v účtu zákazníka.</span><span class="sxs-lookup"><span data-stu-id="5b3ce-112">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="5b3ce-113">Můžete také obnovit jeden nebo více uživatelských účtů, které jste dříve odstranili během 30 dnů od odstranění.</span><span class="sxs-lookup"><span data-stu-id="5b3ce-113">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="5b3ce-114">Budou obnovena i předchozí přiřazení předplatného uživatele (za předpokladu, že jsou k dispozici jejich předchozí přidělení).</span><span class="sxs-lookup"><span data-stu-id="5b3ce-114">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="5b3ce-115">Když si koupíte nové předplatné pro zákazníka, zákazník by vám měl poskytnout seznam všech uživatelů, kteří budou potřebovat účty, jejich uživatelská oprávnění a to, které služby jednotliví uživatelé potřebují.</span><span class="sxs-lookup"><span data-stu-id="5b3ce-115">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

<span data-ttu-id="5b3ce-116">[Odběry můžete přiřadit více uživatelům](bulk-license-provisioning-for-multiple-users.md) najednou pomocí importu názvů pomocí [souboru tabulky. csv kompatibilního s Excelem](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="5b3ce-116">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="5b3ce-117">Vytvoření uživatelských účtů pro zákazníka</span><span class="sxs-lookup"><span data-stu-id="5b3ce-117">Create user accounts for a customer</span></span>

1. <span data-ttu-id="5b3ce-118">Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="5b3ce-118">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="5b3ce-119">V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="5b3ce-119">From the Partner Center menu, select **Customers** , then choose a customer from the list.</span></span>

3. <span data-ttu-id="5b3ce-120">V nabídce zákazník vyberte **Uživatelé a licence** .</span><span class="sxs-lookup"><span data-stu-id="5b3ce-120">In the customer menu, select **Users and licenses** .</span></span>

4. <span data-ttu-id="5b3ce-121">Pro každého uživatele, kterého přidáte, vyberte **Přidat předplatné** a pak vyplňte informace, včetně oprávnění a licencí.</span><span class="sxs-lookup"><span data-stu-id="5b3ce-121">For each user you add, select **Add subscription** , then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="5b3ce-122">**Uložte** změny.</span><span class="sxs-lookup"><span data-stu-id="5b3ce-122">**Save** your changes.</span></span>

5. <span data-ttu-id="5b3ce-123">Nezapomeňte zaznamenat uživatelské jméno a dočasné heslo pro odeslání uživateli.</span><span class="sxs-lookup"><span data-stu-id="5b3ce-123">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="5b3ce-124">Pokud současně přidáváte více uživatelů, použijte **Přidat jiného uživatele** .</span><span class="sxs-lookup"><span data-stu-id="5b3ce-124">If you are adding multiple users one at a time use **Add another user** .</span></span>

7. <span data-ttu-id="5b3ce-125">Můžete také přidat více uživatelů najednou [importováním souboru tabulky CSV kompatibilního s Excelem](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="5b3ce-125">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="5b3ce-126">Před odesláním e-mailu nebo tiskem názvů a hesel z potvrzovací obrazovky můžete počkat, dokud nedokončíte celou sadu.</span><span class="sxs-lookup"><span data-stu-id="5b3ce-126">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="5b3ce-127">Přidání nebo odebrání uživatelských licencí pro zákazníka</span><span class="sxs-lookup"><span data-stu-id="5b3ce-127">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="5b3ce-128">Následující postup platí pro přidání nebo odebrání uživatelských licencí pro produkty společnosti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5b3ce-128">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="5b3ce-129">Pokud chcete přidat nebo odebrat uživatelské licence pro odběry SaaS založené na licencích na komerčním webu Marketplace, přečtěte si téma [Přidání nebo odebrání licencí pro předplatné SaaS](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span><span class="sxs-lookup"><span data-stu-id="5b3ce-129">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="5b3ce-130">Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="5b3ce-130">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="5b3ce-131">V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="5b3ce-131">From the Partner Center menu, select **Customers** , then choose a customer from the list.</span></span>

3. <span data-ttu-id="5b3ce-132">V nabídce zákazník vyberte **Uživatelé a licence** .</span><span class="sxs-lookup"><span data-stu-id="5b3ce-132">In the customer menu, select **Users and licenses** .</span></span>

4. <span data-ttu-id="5b3ce-133">Vyberte jednoho nebo více uživatelů ze seznamu.</span><span class="sxs-lookup"><span data-stu-id="5b3ce-133">Choose one or more users from the list.</span></span> <span data-ttu-id="5b3ce-134">Pokud například zákazník právě koupil nové licence a chtěli jste jim přiřadit lidi, kteří je ještě nemají, můžete k vyhledání správné skupiny použít možnost **filtrovat uživatele podle..** ..</span><span class="sxs-lookup"><span data-stu-id="5b3ce-134">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="5b3ce-135">Vyberte **spravovat licence** .</span><span class="sxs-lookup"><span data-stu-id="5b3ce-135">Select **Manage licenses** .</span></span> <span data-ttu-id="5b3ce-136">Proveďte změny a pak ho **uložte** .</span><span class="sxs-lookup"><span data-stu-id="5b3ce-136">Make your changes, then **Save** .</span></span>

> [!NOTE]
> <span data-ttu-id="5b3ce-137">U [Azure Marketplace produktů](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)se přiřazení licencí a aktivace spravují prostřednictvím nezávislého výrobce softwaru (ISV), který produkt zveřejnil.</span><span class="sxs-lookup"><span data-stu-id="5b3ce-137">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="5b3ce-138">Resetování hesla uživatele pro zákazníka</span><span class="sxs-lookup"><span data-stu-id="5b3ce-138">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="5b3ce-139">Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="5b3ce-139">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="5b3ce-140">V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="5b3ce-140">From the Partner Center menu, select **Customers** , then choose a customer from the list.</span></span>

3.  <span data-ttu-id="5b3ce-141">V nabídce zákazník vyberte **Uživatelé a licence** .</span><span class="sxs-lookup"><span data-stu-id="5b3ce-141">In the customer menu, select **Users and licenses** .</span></span> <span data-ttu-id="5b3ce-142">Vyberte uživatele ze seznamu.</span><span class="sxs-lookup"><span data-stu-id="5b3ce-142">Choose the user from the list.</span></span>

4.  <span data-ttu-id="5b3ce-143">V dolní části obrazovky vyberte **resetovat heslo** .</span><span class="sxs-lookup"><span data-stu-id="5b3ce-143">At the bottom of the screen, select **Reset password** .</span></span> 

5.  <span data-ttu-id="5b3ce-144">Poslat uživateli nové dočasné heslo.</span><span class="sxs-lookup"><span data-stu-id="5b3ce-144">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="5b3ce-145">Odstranění uživatelských účtů pro zákazníka</span><span class="sxs-lookup"><span data-stu-id="5b3ce-145">Delete user accounts for a customer</span></span>

1.  <span data-ttu-id="5b3ce-146">V nabídce **Partnerské centrum** vyberte **zákazníci** .</span><span class="sxs-lookup"><span data-stu-id="5b3ce-146">From the **Partner Center** menu, select **Customers** .</span></span> <span data-ttu-id="5b3ce-147">Vyberte zákazníka ze seznamu.</span><span class="sxs-lookup"><span data-stu-id="5b3ce-147">Choose the customer from the list.</span></span>

2.  <span data-ttu-id="5b3ce-148">V nabídce zákazník vyberte **Uživatelé a licence** .</span><span class="sxs-lookup"><span data-stu-id="5b3ce-148">In the customer menu, select **Users and licenses** .</span></span> <span data-ttu-id="5b3ce-149">Vyberte uživatele ze seznamu.</span><span class="sxs-lookup"><span data-stu-id="5b3ce-149">Choose the user from the list.</span></span>

3.  <span data-ttu-id="5b3ce-150">V dolní části obrazovky vyberte **Odstranit uživatelský účet** .</span><span class="sxs-lookup"><span data-stu-id="5b3ce-150">At the bottom of the screen, select **Delete user account** .</span></span>

<span data-ttu-id="5b3ce-151">Pokud potřebujete tento účet obnovit, můžete ho najít na kartě **odstraněné uživatele** v seznamu **Uživatelé a licence** zákazníka.</span><span class="sxs-lookup"><span data-stu-id="5b3ce-151">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="5b3ce-152">K obnovení odstraněného uživatele máte 30 dní.</span><span class="sxs-lookup"><span data-stu-id="5b3ce-152">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="5b3ce-153">Obnovení odstraněných uživatelských účtů</span><span class="sxs-lookup"><span data-stu-id="5b3ce-153">Restore deleted user accounts</span></span>

1.  <span data-ttu-id="5b3ce-154">V nabídce **Partnerské centrum** vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="5b3ce-154">From the **Partner Center** menu, select **Customers** , then choose the customer from the list.</span></span>

2.  <span data-ttu-id="5b3ce-155">Vyberte **Uživatelé a licence** .</span><span class="sxs-lookup"><span data-stu-id="5b3ce-155">Select **Users and licenses** .</span></span>

3.  <span data-ttu-id="5b3ce-156">Vyberte kartu **odstraněné uživatele ()** . V případě odstranění uživatelů, které lze obnovit, by mělo být přečteno **(1)** nebo vyšší.</span><span class="sxs-lookup"><span data-stu-id="5b3ce-156">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4.  <span data-ttu-id="5b3ce-157">Zaškrtněte jedno nebo více políček Odstraněná uživatelé a pak vyberte **obnovit** .</span><span class="sxs-lookup"><span data-stu-id="5b3ce-157">Select one or more of the deleted users' checkboxes and then select **Restore** .</span></span>

    <span data-ttu-id="5b3ce-158">Všechny vybrané uživatelské účty se znovu zobrazí na stránce **Uživatelé a licence** .</span><span class="sxs-lookup"><span data-stu-id="5b3ce-158">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="related-topics"></a><span data-ttu-id="5b3ce-159">Související témata</span><span class="sxs-lookup"><span data-stu-id="5b3ce-159">Related topics</span></span>


[<span data-ttu-id="5b3ce-160">Přiřazení licencí několika uživatelům nebo jejich odvolání</span><span class="sxs-lookup"><span data-stu-id="5b3ce-160">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

[<span data-ttu-id="5b3ce-161">Vytvoření více uživatelů pro účet zákazníka</span><span class="sxs-lookup"><span data-stu-id="5b3ce-161">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)