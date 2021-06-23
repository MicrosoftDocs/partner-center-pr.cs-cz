---
title: Odebrat vztah prodejce k zákazníkovi
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak můžou Microsoft Direct partner odebrat zákazníky ze svého seznamu, odebrat oprávnění delegovaného správce a přestat podporovat nebo kupovat zákazníky.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 83259f2f895be9ef34c55db5613ccfe6891a4424
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551465"
---
# <a name="how-to-remove-a-reseller-relationship-with-a-customer-in-partner-center"></a><span data-ttu-id="5c0d7-103">Odebrání vztahu se zákazníkem na úrovni prodejce v Partnerském centru</span><span class="sxs-lookup"><span data-stu-id="5c0d7-103">How to remove a reseller relationship with a customer in Partner Center</span></span>

<span data-ttu-id="5c0d7-104">**Příslušné role**: globální správce</span><span class="sxs-lookup"><span data-stu-id="5c0d7-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="5c0d7-105">Tento článek popisuje, jak odebrat vztah prodejce k zákazníkovi v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="5c0d7-105">This article describes how to remove a reseller relationship with a customer in Partner Center.</span></span>

<span data-ttu-id="5c0d7-106">Přímé partnery nebo nepřímá zprostředkovatelé: Pokud už se zákazníkem nepracujete, můžete relaci odebrat v partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="5c0d7-106">Direct partners or Indirect providers: if you're no longer transacting with a customer, you can remove the relationship in Partner Center.</span></span>

<span data-ttu-id="5c0d7-107">Odebrání vztahu má následující důsledky:</span><span class="sxs-lookup"><span data-stu-id="5c0d7-107">Removing a relationship has the following consequences:</span></span>

- <span data-ttu-id="5c0d7-108">Zákazník se odebere z vašeho seznamu zákazníků v Partnerském centru.</span><span class="sxs-lookup"><span data-stu-id="5c0d7-108">Removes the customer from your list of customers in Partner Center</span></span>
- <span data-ttu-id="5c0d7-109">Odebere vás ze [seznamu dostupných kontaktů podpory](assign-support-contacts.md) pro vašeho zákazníka.</span><span class="sxs-lookup"><span data-stu-id="5c0d7-109">Removes you from the [list of available support contacts](assign-support-contacts.md) for your customer</span></span>
- <span data-ttu-id="5c0d7-110">Zákazníkovi se odeberou delegovaná oprávnění správce.</span><span class="sxs-lookup"><span data-stu-id="5c0d7-110">Removes your delegation admin privileges for the customer</span></span>
- <span data-ttu-id="5c0d7-111">Nebudete pro zákazníka moct provádět další nákupy.</span><span class="sxs-lookup"><span data-stu-id="5c0d7-111">Prevents you from making future purchases for the customer</span></span>

## <a name="how-to-remove-a-relationship"></a><span data-ttu-id="5c0d7-112">Jak odebrat relaci</span><span class="sxs-lookup"><span data-stu-id="5c0d7-112">How to remove a relationship</span></span>

<span data-ttu-id="5c0d7-113">Pokud chcete relaci odebrat, budete muset zrušit rezervace rezervovaných instancí Azure, zrušit nákupy softwaru a všechny zbývající aktivní odběry nejdřív pozastavit.</span><span class="sxs-lookup"><span data-stu-id="5c0d7-113">To remove the relationship, you'll need to cancel Azure reserved instance (RI) reservations, cancel software purchases, and suspend any remaining active subscriptions first.</span></span>

1. <span data-ttu-id="5c0d7-114">**Pozastaví všechna aktivní předplatná.**</span><span class="sxs-lookup"><span data-stu-id="5c0d7-114">**Suspend any active subscriptions.**</span></span>

   1. <span data-ttu-id="5c0d7-115">V partnerském centru navštivte **zákazníky** a vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="5c0d7-115">From the Partner Center, go to **Customers** and select a customer</span></span>

   2. <span data-ttu-id="5c0d7-116">V části **předplatná** vyberte předplatné.</span><span class="sxs-lookup"><span data-stu-id="5c0d7-116">Under **Subscriptions**, select a subscription.</span></span>

   3. <span data-ttu-id="5c0d7-117">Vybrat **pozastaveno**</span><span class="sxs-lookup"><span data-stu-id="5c0d7-117">Select **Suspended**</span></span>

   4. <span data-ttu-id="5c0d7-118">Opakujte tyto kroky pro každé aktivní předplatné.</span><span class="sxs-lookup"><span data-stu-id="5c0d7-118">Repeat these steps for each active subscription.</span></span>

2. <span data-ttu-id="5c0d7-119">**Odeberte vztah v partnerském centru:**</span><span class="sxs-lookup"><span data-stu-id="5c0d7-119">**Remove the relationship in Partner Center:**</span></span>

   <span data-ttu-id="5c0d7-120">a.</span><span class="sxs-lookup"><span data-stu-id="5c0d7-120">a.</span></span> <span data-ttu-id="5c0d7-121">V partnerském centru klikněte na **zákazníci** a vyberte zákazníka.</span><span class="sxs-lookup"><span data-stu-id="5c0d7-121">From the Partner Center, go to **Customers** and select a customer.</span></span>

   <span data-ttu-id="5c0d7-122">b.</span><span class="sxs-lookup"><span data-stu-id="5c0d7-122">b.</span></span> <span data-ttu-id="5c0d7-123">Vyberte **účet**.</span><span class="sxs-lookup"><span data-stu-id="5c0d7-123">Select the **Account**.</span></span>

   <span data-ttu-id="5c0d7-124">c.</span><span class="sxs-lookup"><span data-stu-id="5c0d7-124">c.</span></span> <span data-ttu-id="5c0d7-125">Vyberte možnost **odebrat vztah prodejce**.</span><span class="sxs-lookup"><span data-stu-id="5c0d7-125">Select **Remove reseller relationship**.</span></span>

   > [!NOTE]
   > <span data-ttu-id="5c0d7-126">Pokud jsou nějaké odběry stále aktivní, odkaz **odebrat vztah prodejce** bude neaktivní.</span><span class="sxs-lookup"><span data-stu-id="5c0d7-126">If any subscriptions are still active, the **Remove reseller relationship** link will be inactive.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5c0d7-127">Další kroky</span><span class="sxs-lookup"><span data-stu-id="5c0d7-127">Next steps</span></span>

- [<span data-ttu-id="5c0d7-128">Vyžádat nebo znovu vytvořit relaci se zákazníkem</span><span class="sxs-lookup"><span data-stu-id="5c0d7-128">Request or re-establish a relationship with a customer</span></span>](request-a-relationship-with-a-customer.md)
