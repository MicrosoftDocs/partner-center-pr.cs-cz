---
title: Přizpůsobení připraveného prostředí zařízení
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Předtím, než dodáte nové zařízení zákazníka, můžete použít profily Windows autopilotu k přizpůsobení nebo předběžnému nastavení prostředí pro počáteční nastavení zařízení.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 12057d50e4456dd2450ff497e00c89a9afa5dc4d
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534981"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="bfa36-103">Přizpůsobení prostředí prvního spuštění nových zařízení s využitím profilů Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="bfa36-103">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="bfa36-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="bfa36-104">**Appropriate roles**</span></span>

- <span data-ttu-id="bfa36-105">Agent správce</span><span class="sxs-lookup"><span data-stu-id="bfa36-105">Admin agent</span></span>
- <span data-ttu-id="bfa36-106">Globální správce</span><span class="sxs-lookup"><span data-stu-id="bfa36-106">Global admin</span></span>
- <span data-ttu-id="bfa36-107">Agent prodeje</span><span class="sxs-lookup"><span data-stu-id="bfa36-107">Sales agent</span></span>
- <span data-ttu-id="bfa36-108">Správce správy uživatelů</span><span class="sxs-lookup"><span data-stu-id="bfa36-108">User management admin</span></span>

<span data-ttu-id="bfa36-109">Pokud spravujete zákaznická zařízení, možná budete muset pro uživatele zákazníka přizpůsobit integrované prostředí (OOBE).</span><span class="sxs-lookup"><span data-stu-id="bfa36-109">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="bfa36-110">Před dodáním zařízení zákazníkům a uplatněním nových profilů na zařízení, která si zákazníci už koupili, můžete předem nakonfigurovat nová zařízení pomocí profilů Windows autopilotu.</span><span class="sxs-lookup"><span data-stu-id="bfa36-110">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="bfa36-111">Všimněte si, že výrobci OEM začali včetně dodacího štítku na vnějším panelu zařízení autopilotu, který zobrazuje **ID kódu Product Key zařízení (PKID)**.</span><span class="sxs-lookup"><span data-stu-id="bfa36-111">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="bfa36-112">Tento jednorozměrný čárový kód poskytuje podřízeným partnerům způsob, jak registrovat zařízení pro autopilota, aniž by museli zařízení Unbox a získat ID zařízení alternativním způsobem.</span><span class="sxs-lookup"><span data-stu-id="bfa36-112">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="bfa36-113">Tento článek vysvětluje, jak vytvořit a použít profily autopilotu na zařízeních v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="bfa36-113">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="bfa36-114">Pokud ještě nejste obeznámeni s autopilotem, přečtěte si informace v těchto článcích:</span><span class="sxs-lookup"><span data-stu-id="bfa36-114">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="bfa36-115">Přehled Windows Autopilotu</span><span class="sxs-lookup"><span data-stu-id="bfa36-115">Overview of Windows Autopilot</span></span>](/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="bfa36-116">Referenční příručka k nasazení autopilotu</span><span class="sxs-lookup"><span data-stu-id="bfa36-116">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="bfa36-117">Přehled</span><span class="sxs-lookup"><span data-stu-id="bfa36-117">Overview</span></span>

<span data-ttu-id="bfa36-118">Pomocí funkce Windows Autopilot v partnerském centru můžete vytvořit vlastní profily, které se použijí na zákaznická zařízení.</span><span class="sxs-lookup"><span data-stu-id="bfa36-118">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="bfa36-119">Následující nastavení profilu byla k dispozici v době publikování tohoto článku:</span><span class="sxs-lookup"><span data-stu-id="bfa36-119">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="bfa36-120">Přeskočit nastavení ochrany osobních údajů.</span><span class="sxs-lookup"><span data-stu-id="bfa36-120">Skip privacy settings.</span></span> <span data-ttu-id="bfa36-121">Toto volitelné nastavení profilu autopilotu umožňuje organizacím, aby během procesu OOBE nežádali o nastavení ochrany osobních údajů.</span><span class="sxs-lookup"><span data-stu-id="bfa36-121">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="bfa36-122">V zařízení zakažte vytváření účtu místního správce.</span><span class="sxs-lookup"><span data-stu-id="bfa36-122">Disable local admin account creation on the device.</span></span> <span data-ttu-id="bfa36-123">Organizace se můžou rozhodnout, jestli uživatel, který má nastavení zařízení, musí mít po dokončení procesu přístup správce.</span><span class="sxs-lookup"><span data-stu-id="bfa36-123">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="bfa36-124">Automaticky nastaví zařízení pro práci nebo školu.</span><span class="sxs-lookup"><span data-stu-id="bfa36-124">Automatically set up device for work or school.</span></span> <span data-ttu-id="bfa36-125">Všechna zařízení zaregistrovaná pomocí automatického pilotního projektu se automaticky považují za pracovní nebo školní zařízení, takže se během procesu OOBE nebude zobrazovat výzva.</span><span class="sxs-lookup"><span data-stu-id="bfa36-125">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="bfa36-126">Přeskočit stránky nastavení registrace Cortany, OneDrive a OEM</span><span class="sxs-lookup"><span data-stu-id="bfa36-126">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="bfa36-127">Všechna zařízení zaregistrovaná pomocí automatického pilotního nasazení automaticky přeskočí tyto stránky během procesu spouštěného při prvním spuštění počítače.</span><span class="sxs-lookup"><span data-stu-id="bfa36-127">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="bfa36-128">Přeskočte si licenční smlouvu s koncovým uživatelem (EULA).</span><span class="sxs-lookup"><span data-stu-id="bfa36-128">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="bfa36-129">Od verze 1709 ve Windows 10 se můžou organizace rozhodnout přeskočit stránku EULA, která se zobrazí během procesu OOBE.</span><span class="sxs-lookup"><span data-stu-id="bfa36-129">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="bfa36-130">Důležité informace, které je třeba vzít v úvahu při přeskočení stránky EULA při instalaci systému Windows, najdete v článku o [neúspěšném odeslání služby Windows autopilot](#windows-autopilot-eula-dismissal) .</span><span class="sxs-lookup"><span data-stu-id="bfa36-130">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="bfa36-131">Pro správu profilů a zařízení platí následující oprávnění a omezení:</span><span class="sxs-lookup"><span data-stu-id="bfa36-131">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="bfa36-132">Partneři CSP můžou dál spravovat profily Autopilot pro stávající zákazníky, se kterými mají vztah na úrovni prodejce, a to i v případě, že jim zákazníci odebrali delegované oprávnění správce.</span><span class="sxs-lookup"><span data-stu-id="bfa36-132">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="bfa36-133">Pro zákazníky můžete spravovat existující zařízení, která jste přidali.</span><span class="sxs-lookup"><span data-stu-id="bfa36-133">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="bfa36-134">Nemůžete spravovat zařízení, která zákazník nahrál na Microsoft pro firmy nebo portál Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="bfa36-134">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="bfa36-135">Vytváření a Správa profilů pro Autopilot v partnerském centru</span><span class="sxs-lookup"><span data-stu-id="bfa36-135">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="bfa36-136">V partnerském centru můžete vytvořit profily nasazení Windows autopilot a použít je na zařízení.</span><span class="sxs-lookup"><span data-stu-id="bfa36-136">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="bfa36-137">Profily můžou vytvářet a používat jenom agenti pro správu.</span><span class="sxs-lookup"><span data-stu-id="bfa36-137">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="bfa36-138">Vytvoření nového profilu autopilotu</span><span class="sxs-lookup"><span data-stu-id="bfa36-138">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="bfa36-139">V nabídce partnerského centra vyberte **zákazníci** a pak vyberte zákazníka, pro který vytváříte profil pro autopilot.</span><span class="sxs-lookup"><span data-stu-id="bfa36-139">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="bfa36-140">Na stránce s podrobnostmi zákazníka vyberte **zařízení**.</span><span class="sxs-lookup"><span data-stu-id="bfa36-140">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="bfa36-141">V části **profily Windows autopilotu** vyberte **Přidat nový profil**.</span><span class="sxs-lookup"><span data-stu-id="bfa36-141">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="bfa36-142">Zadejte název a popis profilu a pak nakonfigurujte nastavení OOBE.</span><span class="sxs-lookup"><span data-stu-id="bfa36-142">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="bfa36-143">Vybírejte z těchto možností:</span><span class="sxs-lookup"><span data-stu-id="bfa36-143">Choose from:</span></span>  

   - <span data-ttu-id="bfa36-144">Přeskočit nastavení ochrany osobních údajů v instalačním programu</span><span class="sxs-lookup"><span data-stu-id="bfa36-144">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="bfa36-145">Zakázat účet místního správce v nastavení</span><span class="sxs-lookup"><span data-stu-id="bfa36-145">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="bfa36-146">Automaticky přeskočit stránky v instalačním programu</span><span class="sxs-lookup"><span data-stu-id="bfa36-146">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="bfa36-147">(Zahrnuje *automaticky výběr nastavení pracovní nebo školní* a *Přeskočit stránky pro nastavení registrace Cortany, OneDrive a OEM*)</span><span class="sxs-lookup"><span data-stu-id="bfa36-147">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="bfa36-148">Přeskočit licenční smlouvu s koncovým uživatelem (EULA)</span><span class="sxs-lookup"><span data-stu-id="bfa36-148">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="bfa36-149">Důležité informace, které je třeba vzít v úvahu při přeskočení stránky EULA při instalaci systému Windows, najdete v článku o [neúspěšném odeslání služby Windows autopilot](#windows-autopilot-eula-dismissal) .</span><span class="sxs-lookup"><span data-stu-id="bfa36-149">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="bfa36-150">Po dokončení vyberte **Odeslat** .</span><span class="sxs-lookup"><span data-stu-id="bfa36-150">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="bfa36-151">Použití profilu autopilotu u zákaznických zařízení</span><span class="sxs-lookup"><span data-stu-id="bfa36-151">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="bfa36-152">Níže uvedené pokyny předpokládají, že jste už přidali zařízení zákazníka do partnerského centra a že máte přístup k seznamu zařízení.</span><span class="sxs-lookup"><span data-stu-id="bfa36-152">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="bfa36-153">Pokud jste ještě nepřidali zařízení zákazníka, postupujte podle pokynů v části [Přidání zařízení na účet zákazníka](#add-devices-to-a-customers-account) a pak postupujte podle následujících pokynů.</span><span class="sxs-lookup"><span data-stu-id="bfa36-153">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="bfa36-154">Po vytvoření profilu autopilotu pro zákazníka ho můžete použít na zařízení zákazníka.</span><span class="sxs-lookup"><span data-stu-id="bfa36-154">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="bfa36-155">V nabídce partnerského centra vyberte **zákazníci** a potom vyberte zákazníka, pro který jste vytvořili profil pro autopilotu.</span><span class="sxs-lookup"><span data-stu-id="bfa36-155">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="bfa36-156">Na stránce s podrobnostmi zákazníka vyberte **zařízení**.</span><span class="sxs-lookup"><span data-stu-id="bfa36-156">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="bfa36-157">V části **použít profily na zařízení** vyberte skupiny zařízení nebo zařízení, do kterých chcete přidat profily, a pak vyberte **použít profil**.</span><span class="sxs-lookup"><span data-stu-id="bfa36-157">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="bfa36-158">Profil, který jste právě použili, se zobrazí ve sloupci **profil** .</span><span class="sxs-lookup"><span data-stu-id="bfa36-158">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="bfa36-159">Postupujte podle následujících kroků a ověřte, zda se profil na zařízení úspěšně použije.</span><span class="sxs-lookup"><span data-stu-id="bfa36-159">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="bfa36-160">a.</span><span class="sxs-lookup"><span data-stu-id="bfa36-160">a.</span></span>  <span data-ttu-id="bfa36-161">Připojte zařízení k síti a zapněte ho.</span><span class="sxs-lookup"><span data-stu-id="bfa36-161">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="bfa36-162">b.</span><span class="sxs-lookup"><span data-stu-id="bfa36-162">b.</span></span>  <span data-ttu-id="bfa36-163">Ověřte, zda se zobrazí příslušné obrazovky OOBE.</span><span class="sxs-lookup"><span data-stu-id="bfa36-163">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="bfa36-164">c.</span><span class="sxs-lookup"><span data-stu-id="bfa36-164">c.</span></span>  <span data-ttu-id="bfa36-165">Když se proces OOBE zastaví, resetujte zařízení do výchozího továrního nastavení, abyste ho připravili pro nového uživatele.</span><span class="sxs-lookup"><span data-stu-id="bfa36-165">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="bfa36-166">Odebrání profilu autopilotu ze zařízení zákazníka</span><span class="sxs-lookup"><span data-stu-id="bfa36-166">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="bfa36-167">V nabídce partnerského centra vyberte **zákazníci** a potom vyberte zákazníka, pro který jste vytvořili profil pro autopilotu.</span><span class="sxs-lookup"><span data-stu-id="bfa36-167">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="bfa36-168">Na stránce s podrobnostmi zákazníka vyberte **zařízení**.</span><span class="sxs-lookup"><span data-stu-id="bfa36-168">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="bfa36-169">V části **použít profily na zařízení** vyberte zařízení, ze kterých chcete profil odebrat, a pak vyberte **Odebrat profil**.</span><span class="sxs-lookup"><span data-stu-id="bfa36-169">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="bfa36-170">Když odeberete profil ze zařízení, profil ze seznamu se neodstraní.</span><span class="sxs-lookup"><span data-stu-id="bfa36-170">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="bfa36-171">Pokud chcete odstranit profil, postupujte podle pokynů v části [aktualizace nebo odstranění profilu autopilotu](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="bfa36-171">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="bfa36-172">Aktualizace nebo odstranění profilu autopilotu</span><span class="sxs-lookup"><span data-stu-id="bfa36-172">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="bfa36-173">Pokud chce zákazník změnit integrované prostředí po odeslání zařízení do těchto zařízení, můžete změnit profil v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="bfa36-173">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="bfa36-174">Jakmile se zařízení zákazníka připojí k Internetu, stáhne nejnovější verzi profilu během procesu OOBE.</span><span class="sxs-lookup"><span data-stu-id="bfa36-174">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="bfa36-175">I když zákazník obnoví zařízení do výchozího továrního nastavení, zařízení si znovu stáhne nejnovější verzi profilu během procesu OOBE.</span><span class="sxs-lookup"><span data-stu-id="bfa36-175">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="bfa36-176">V nabídce partnerského centra vyberte **zákazníci** a pak vyberte zákazníka, který požaduje, abyste změnili profil autopilotu.</span><span class="sxs-lookup"><span data-stu-id="bfa36-176">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="bfa36-177">Na stránce s podrobnostmi zákazníka vyberte **zařízení**.</span><span class="sxs-lookup"><span data-stu-id="bfa36-177">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="bfa36-178">V části **profily Windows autopilotu** vyberte profil, který potřebujete aktualizovat.</span><span class="sxs-lookup"><span data-stu-id="bfa36-178">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="bfa36-179">Proveďte požadované změny a pak vyberte **Odeslat**.</span><span class="sxs-lookup"><span data-stu-id="bfa36-179">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="bfa36-180">Chcete-li odstranit tento profil, vyberte možnost **Odstranit profil** v pravém horním rohu stránky.</span><span class="sxs-lookup"><span data-stu-id="bfa36-180">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="bfa36-181">Přidání zařízení do účtu zákazníka</span><span class="sxs-lookup"><span data-stu-id="bfa36-181">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="bfa36-182">Prodejní agenti a agenti pro správu můžou přidat zařízení k účtu zákazníka.</span><span class="sxs-lookup"><span data-stu-id="bfa36-182">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="bfa36-183">Než budete moct použít vlastní profily autopilotu na zákaznická zařízení, musíte mít přístup k seznamu zařízení zákazníka.</span><span class="sxs-lookup"><span data-stu-id="bfa36-183">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="bfa36-184">Pokud máte v plánu používat název výrobce OEM, sériové číslo a kombinaci modelů, pamatujte na tato omezení:</span><span class="sxs-lookup"><span data-stu-id="bfa36-184">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="bfa36-185">Tato řazená kolekce členů funguje jenom pro novější zařízení (například hodnoty hash 4k) a není podporovaná pro hodnoty hash 128B (RS2 a předchozí zařízení).</span><span class="sxs-lookup"><span data-stu-id="bfa36-185">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="bfa36-186">Registrace řazené kolekce členů rozlišuje velká a malá písmena, takže data v souboru se musí shodovat s názvy modelů a výrobců \**_přesně_* _, jak poskytuje poskytovatel OEM (poskytovatel hardwaru).</span><span class="sxs-lookup"><span data-stu-id="bfa36-186">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names \**_exactly_* _ as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="bfa36-187">Podle pokynů níže přidejte zařízení k účtu zákazníka v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="bfa36-187">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="bfa36-188">V nabídce partnerského centra vyberte _ *zákazníci*\* a pak vyberte zákazníka, jehož zařízení chcete spravovat.</span><span class="sxs-lookup"><span data-stu-id="bfa36-188">Select _ *Customers*\* from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="bfa36-189">Na stránce s podrobnostmi zákazníka vyberte **zařízení**.</span><span class="sxs-lookup"><span data-stu-id="bfa36-189">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="bfa36-190">V části **použít profily na zařízení** vyberte **Přidat zařízení**.</span><span class="sxs-lookup"><span data-stu-id="bfa36-190">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="bfa36-191">Zadejte název seznamu zařízení a pak vyberte **Procházet** a nahrajte seznam zákazníků (ve formátu souboru. csv) do partnerského centra.</span><span class="sxs-lookup"><span data-stu-id="bfa36-191">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="bfa36-192">Tento soubor. csv byste měli při nákupu zařízení přijmout.</span><span class="sxs-lookup"><span data-stu-id="bfa36-192">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="bfa36-193">Pokud jste neobdrželi soubor. csv, můžete si ho vytvořit sami podle kroků v části [Přidání zařízení do Windows autopilotu](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="bfa36-193">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="bfa36-194">Nahrajte soubor. csv a pak vyberte **Uložit**.</span><span class="sxs-lookup"><span data-stu-id="bfa36-194">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="bfa36-195">Pokud se vám při pokusu o nahrání souboru .csv zobrazí chybová zpráva, zkontrolujte formát souboru.</span><span class="sxs-lookup"><span data-stu-id="bfa36-195">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="bfa36-196">Můžete použít pouze hodnotu hash hardwaru nebo název výrobce OEM, sériové číslo a model (v uvedeném pořadí sloupců), případně ID produktu Windows.</span><span class="sxs-lookup"><span data-stu-id="bfa36-196">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="bfa36-197">K vytvoření seznamu zařízení můžete použít také ukázkový soubor. csv poskytnutý z odkazu vedle **Přidat zařízení** .</span><span class="sxs-lookup"><span data-stu-id="bfa36-197">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="bfa36-198">Váš soubor. csv by měl vypadat přibližně takto:</span><span class="sxs-lookup"><span data-stu-id="bfa36-198">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="bfa36-199">**Sériové číslo zařízení, ID produktu Windows, hodnota hash hardwaru, název výrobce, model zařízení**</span><span class="sxs-lookup"><span data-stu-id="bfa36-199">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="bfa36-200">**{Sériové},,, Microsoft Corporation, Surface notebooku**</span><span class="sxs-lookup"><span data-stu-id="bfa36-200">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="bfa36-201">V části název výrobce a model zařízení se rozlišují malá a velká písmena.</span><span class="sxs-lookup"><span data-stu-id="bfa36-201">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="bfa36-202">Pokud nevíte, jaká hodnota má být zadána pro název výrobce a model zařízení, můžete tuto akci spustit na zařízení a shromáždit správné hodnoty:</span><span class="sxs-lookup"><span data-stu-id="bfa36-202">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="bfa36-203">Neúspěšné přijetí smlouvy EULA pro Windows autopilot</span><span class="sxs-lookup"><span data-stu-id="bfa36-203">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="bfa36-204">DŮLEŽITÉ INFORMACE</span><span class="sxs-lookup"><span data-stu-id="bfa36-204">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="bfa36-205">Windows autopilot umožňuje nakonfigurovat vlastní instalace Windows na zařízeních, která spravujete pro vaše zákazníky.</span><span class="sxs-lookup"><span data-stu-id="bfa36-205">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="bfa36-206">Pokud k tomu má zákazník oprávnění, můžete potlačit nebo skrýt některé z nich, které se běžně uživatelům prezentují při nastavování Windows, včetně obrazovky EULA (licenční smlouva s koncovým uživatelem).</span><span class="sxs-lookup"><span data-stu-id="bfa36-206">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="bfa36-207">Pomocí této funkce, souhlasíte s tím, že potlačíte nebo skryjete všechny obrazovky, které jsou navržené tak, aby poskytovaly uživatelům upozornění, nebo přijetí podmínek znamená, že jste získali dostatečný souhlas a oprávnění od zákazníka ke skrytí podmínek a že jménem zákazníka (ať už je to organizace nebo jednotlivý uživatel), vyjádření souhlasu se všemi oznámeními a přijímají si podmínky, které platí pro vaše zákazníky.</span><span class="sxs-lookup"><span data-stu-id="bfa36-207">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="bfa36-208">To zahrnuje souhlas s podmínkami a ujednáními licence nebo oznámení, která by se uživateli zobrazovala, pokud jste ho potlačili nebo skryli pomocí tohoto nástroje.</span><span class="sxs-lookup"><span data-stu-id="bfa36-208">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="bfa36-209">Pokud zákazník nezískal licenci pro software od společnosti Microsoft nebo jejích licencovaných distributorů, nemusí na těchto zařízeních používat software Windows.</span><span class="sxs-lookup"><span data-stu-id="bfa36-209">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>