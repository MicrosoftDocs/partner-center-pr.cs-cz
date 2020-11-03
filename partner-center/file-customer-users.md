---
title: Pole pro soubor. CSV pro import několika uživatelů pro účet zákazníka
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Pokud chcete přidat více uživatelů k účtu zákazníka, vytvořte soubor hodnot oddělených čárkami (. csv) s příslušnými poli.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 07a28e5310716f3df11caa36e51339e877e65627
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/03/2020
ms.locfileid: "92527107"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="afdb3-103">Přidání více uživatelů na účet zákazníka vytvořením souboru. csv</span><span class="sxs-lookup"><span data-stu-id="afdb3-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="afdb3-104">**Platí pro**</span><span class="sxs-lookup"><span data-stu-id="afdb3-104">**Applies to**</span></span>

- <span data-ttu-id="afdb3-105">Partnerské centrum</span><span class="sxs-lookup"><span data-stu-id="afdb3-105">Partner Center</span></span>

<span data-ttu-id="afdb3-106">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="afdb3-106">**Appropriate roles**</span></span>

- <span data-ttu-id="afdb3-107">Globální správce</span><span class="sxs-lookup"><span data-stu-id="afdb3-107">Global admin</span></span>

<span data-ttu-id="afdb3-108">Přidejte více uživatelů na účet zákazníka najednou, a to tak, že do partnerského centra nahrajete datový soubor ve formátu textový soubor s oddělovači (. csv).</span><span class="sxs-lookup"><span data-stu-id="afdb3-108">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="afdb3-109">Ukázkový datový soubor si můžete stáhnout z partnerského centra a pak ho upravit pro vaše použití, nebo můžete vytvořit nový datový soubor pomocí datového modelu definovaného níže.</span><span class="sxs-lookup"><span data-stu-id="afdb3-109">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="afdb3-110">Požadavky na datové soubory</span><span class="sxs-lookup"><span data-stu-id="afdb3-110">Data file requirements</span></span>

<span data-ttu-id="afdb3-111">Chcete-li přidat více uživatelů k účtu zákazníka pomocí procesu hromadného nahrávání, je nutné splnit následující požadavky:</span><span class="sxs-lookup"><span data-stu-id="afdb3-111">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="afdb3-112">Musíte mít oprávnění globálního správce k účtu zákazníka;</span><span class="sxs-lookup"><span data-stu-id="afdb3-112">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="afdb3-113">Každý uživatel musí mít jedinečnou e-mailovou adresu, která se připojí k e-mailovým doménám zákazníka;</span><span class="sxs-lookup"><span data-stu-id="afdb3-113">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="afdb3-114">Můžete nahrávat až 100 záznamů najednou.</span><span class="sxs-lookup"><span data-stu-id="afdb3-114">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="afdb3-115">Pokud potřebujete přidat více než 100 uživatelů, vytvořte a nahrajte další datové soubory.</span><span class="sxs-lookup"><span data-stu-id="afdb3-115">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="afdb3-116">Všichni uživatelé musí být ve stejném geografickém **umístění** .</span><span class="sxs-lookup"><span data-stu-id="afdb3-116">All users must be in the same geographic **Location** .</span></span>
- <span data-ttu-id="afdb3-117">Zadejte pouze data popsaná níže.</span><span class="sxs-lookup"><span data-stu-id="afdb3-117">Enter only the data described below.</span></span> <span data-ttu-id="afdb3-118">Nadbytečné údaje způsobí selhání nahrávání.</span><span class="sxs-lookup"><span data-stu-id="afdb3-118">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="afdb3-119">V datovém souboru zadejte následující data:</span><span class="sxs-lookup"><span data-stu-id="afdb3-119">Enter the following data in the data file:</span></span>

| <span data-ttu-id="afdb3-120">**Název sloupce**</span><span class="sxs-lookup"><span data-stu-id="afdb3-120">**Column name**</span></span> | <span data-ttu-id="afdb3-121">**Popis**</span><span class="sxs-lookup"><span data-stu-id="afdb3-121">**Description**</span></span>  | <span data-ttu-id="afdb3-122">**Omezení**</span><span class="sxs-lookup"><span data-stu-id="afdb3-122">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="afdb3-123">Jméno</span><span class="sxs-lookup"><span data-stu-id="afdb3-123">First name</span></span>  | <span data-ttu-id="afdb3-124">Křestní jméno uživatele (volitelné pole)</span><span class="sxs-lookup"><span data-stu-id="afdb3-124">User's first name (optional field)</span></span>  | <span data-ttu-id="afdb3-125">50 – limit znaků</span><span class="sxs-lookup"><span data-stu-id="afdb3-125">50-character limit</span></span>  |
| <span data-ttu-id="afdb3-126">Příjmení</span><span class="sxs-lookup"><span data-stu-id="afdb3-126">Last name</span></span>  | <span data-ttu-id="afdb3-127">Poslední jméno uživatele (volitelné pole)</span><span class="sxs-lookup"><span data-stu-id="afdb3-127">User's last name (optional field)</span></span>  | <span data-ttu-id="afdb3-128">50 – limit znaků</span><span class="sxs-lookup"><span data-stu-id="afdb3-128">50-character limit</span></span>  |
| <span data-ttu-id="afdb3-129">Zobrazovaný název</span><span class="sxs-lookup"><span data-stu-id="afdb3-129">Display name</span></span>    | <span data-ttu-id="afdb3-130">Název zobrazený v partnerském centru (povinné pole)</span><span class="sxs-lookup"><span data-stu-id="afdb3-130">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="afdb3-131">50 – limit znaků</span><span class="sxs-lookup"><span data-stu-id="afdb3-131">50-character limit</span></span>                         |
| <span data-ttu-id="afdb3-132">E-mail</span><span class="sxs-lookup"><span data-stu-id="afdb3-132">Email</span></span>   | <span data-ttu-id="afdb3-133">Obchodní e-mailová adresa uživatele na zákaznické firmě (povinné pole)</span><span class="sxs-lookup"><span data-stu-id="afdb3-133">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="afdb3-134">Každý uživatel musí mít jedinečnou e-mailovou adresu.</span><span class="sxs-lookup"><span data-stu-id="afdb3-134">Each user must have a unique email address</span></span> |
| <span data-ttu-id="afdb3-135">Aktualizace stavu</span><span class="sxs-lookup"><span data-stu-id="afdb3-135">Status update</span></span>   | <span data-ttu-id="afdb3-136">Slouží k označení, zda byl záznam nového uživatele úspěšně vytvořen.</span><span class="sxs-lookup"><span data-stu-id="afdb3-136">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="afdb3-137">\*\*Ponechat prázdné\*\*</span><span class="sxs-lookup"><span data-stu-id="afdb3-137">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="afdb3-138">Další kroky</span><span class="sxs-lookup"><span data-stu-id="afdb3-138">Next steps</span></span>

- [<span data-ttu-id="afdb3-139">Postup přidání více uživatelů pro zákazníka</span><span class="sxs-lookup"><span data-stu-id="afdb3-139">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)