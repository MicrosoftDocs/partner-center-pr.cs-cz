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
ms.openlocfilehash: 8ba08d97f1d360eae5af1941ed36753addd24939
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441417"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="9a00c-103">Přidání více uživatelů na účet zákazníka vytvořením souboru. csv</span><span class="sxs-lookup"><span data-stu-id="9a00c-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="9a00c-104">**Příslušné role**</span><span class="sxs-lookup"><span data-stu-id="9a00c-104">**Appropriate roles**</span></span>

- <span data-ttu-id="9a00c-105">Globální správce</span><span class="sxs-lookup"><span data-stu-id="9a00c-105">Global admin</span></span>

<span data-ttu-id="9a00c-106">Přidejte více uživatelů na účet zákazníka najednou, a to tak, že do partnerského centra nahrajete datový soubor ve formátu textový soubor s oddělovači (. csv).</span><span class="sxs-lookup"><span data-stu-id="9a00c-106">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="9a00c-107">Ukázkový datový soubor si můžete stáhnout z partnerského centra a pak ho upravit pro vaše použití, nebo můžete vytvořit nový datový soubor pomocí datového modelu definovaného níže.</span><span class="sxs-lookup"><span data-stu-id="9a00c-107">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="9a00c-108">Požadavky na datové soubory</span><span class="sxs-lookup"><span data-stu-id="9a00c-108">Data file requirements</span></span>

<span data-ttu-id="9a00c-109">Chcete-li přidat více uživatelů k účtu zákazníka pomocí procesu hromadného nahrávání, je nutné splnit následující požadavky:</span><span class="sxs-lookup"><span data-stu-id="9a00c-109">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="9a00c-110">Musíte mít oprávnění globálního správce k účtu zákazníka;</span><span class="sxs-lookup"><span data-stu-id="9a00c-110">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="9a00c-111">Každý uživatel musí mít jedinečnou e-mailovou adresu, která se připojí k e-mailovým doménám zákazníka;</span><span class="sxs-lookup"><span data-stu-id="9a00c-111">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="9a00c-112">Můžete nahrávat až 100 záznamů najednou.</span><span class="sxs-lookup"><span data-stu-id="9a00c-112">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="9a00c-113">Pokud potřebujete přidat více než 100 uživatelů, vytvořte a nahrajte další datové soubory.</span><span class="sxs-lookup"><span data-stu-id="9a00c-113">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="9a00c-114">Všichni uživatelé musí být ve stejném geografickém **umístění**.</span><span class="sxs-lookup"><span data-stu-id="9a00c-114">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="9a00c-115">Zadejte pouze data popsaná níže.</span><span class="sxs-lookup"><span data-stu-id="9a00c-115">Enter only the data described below.</span></span> <span data-ttu-id="9a00c-116">Nadbytečné údaje způsobí selhání nahrávání.</span><span class="sxs-lookup"><span data-stu-id="9a00c-116">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="9a00c-117">V datovém souboru zadejte následující data:</span><span class="sxs-lookup"><span data-stu-id="9a00c-117">Enter the following data in the data file:</span></span>

| <span data-ttu-id="9a00c-118">**Název sloupce**</span><span class="sxs-lookup"><span data-stu-id="9a00c-118">**Column name**</span></span> | <span data-ttu-id="9a00c-119">**Popis**</span><span class="sxs-lookup"><span data-stu-id="9a00c-119">**Description**</span></span>  | <span data-ttu-id="9a00c-120">**Omezení**</span><span class="sxs-lookup"><span data-stu-id="9a00c-120">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="9a00c-121">Jméno</span><span class="sxs-lookup"><span data-stu-id="9a00c-121">First name</span></span>  | <span data-ttu-id="9a00c-122">Křestní jméno uživatele (volitelné pole)</span><span class="sxs-lookup"><span data-stu-id="9a00c-122">User's first name (optional field)</span></span>  | <span data-ttu-id="9a00c-123">50 – limit znaků</span><span class="sxs-lookup"><span data-stu-id="9a00c-123">50-character limit</span></span>  |
| <span data-ttu-id="9a00c-124">Příjmení</span><span class="sxs-lookup"><span data-stu-id="9a00c-124">Last name</span></span>  | <span data-ttu-id="9a00c-125">Poslední jméno uživatele (volitelné pole)</span><span class="sxs-lookup"><span data-stu-id="9a00c-125">User's last name (optional field)</span></span>  | <span data-ttu-id="9a00c-126">50 – limit znaků</span><span class="sxs-lookup"><span data-stu-id="9a00c-126">50-character limit</span></span>  |
| <span data-ttu-id="9a00c-127">Zobrazované jméno</span><span class="sxs-lookup"><span data-stu-id="9a00c-127">Display name</span></span>    | <span data-ttu-id="9a00c-128">Název zobrazený v partnerském centru (povinné pole)</span><span class="sxs-lookup"><span data-stu-id="9a00c-128">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="9a00c-129">50 – limit znaků</span><span class="sxs-lookup"><span data-stu-id="9a00c-129">50-character limit</span></span>                         |
| <span data-ttu-id="9a00c-130">E-mail</span><span class="sxs-lookup"><span data-stu-id="9a00c-130">Email</span></span>   | <span data-ttu-id="9a00c-131">Obchodní e-mailová adresa uživatele na zákaznické firmě (povinné pole)</span><span class="sxs-lookup"><span data-stu-id="9a00c-131">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="9a00c-132">Každý uživatel musí mít jedinečnou e-mailovou adresu.</span><span class="sxs-lookup"><span data-stu-id="9a00c-132">Each user must have a unique email address</span></span> |
| <span data-ttu-id="9a00c-133">Aktualizace stavu</span><span class="sxs-lookup"><span data-stu-id="9a00c-133">Status update</span></span>   | <span data-ttu-id="9a00c-134">Slouží k označení, zda byl záznam nového uživatele úspěšně vytvořen.</span><span class="sxs-lookup"><span data-stu-id="9a00c-134">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="9a00c-135">\*\*Ponechat prázdné\*\*</span><span class="sxs-lookup"><span data-stu-id="9a00c-135">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="9a00c-136">Další kroky</span><span class="sxs-lookup"><span data-stu-id="9a00c-136">Next steps</span></span>

- [<span data-ttu-id="9a00c-137">Postup přidání více uživatelů pro zákazníka</span><span class="sxs-lookup"><span data-stu-id="9a00c-137">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)