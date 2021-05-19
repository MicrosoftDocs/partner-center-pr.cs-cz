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
ms.openlocfilehash: 152daadde25a9325937797f7a3daa90dfb59a9b4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150977"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="cbfcf-103">Přidání více uživatelů na účet zákazníka vytvořením souboru. csv</span><span class="sxs-lookup"><span data-stu-id="cbfcf-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="cbfcf-104">**Příslušné role**: globální správce</span><span class="sxs-lookup"><span data-stu-id="cbfcf-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="cbfcf-105">Přidejte více uživatelů na účet zákazníka najednou, a to tak, že do partnerského centra nahrajete datový soubor ve formátu textový soubor s oddělovači (. csv).</span><span class="sxs-lookup"><span data-stu-id="cbfcf-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="cbfcf-106">Ukázkový datový soubor si můžete stáhnout z partnerského centra a pak ho upravit pro vaše použití, nebo můžete vytvořit nový datový soubor pomocí datového modelu definovaného níže.</span><span class="sxs-lookup"><span data-stu-id="cbfcf-106">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="cbfcf-107">Požadavky na datové soubory</span><span class="sxs-lookup"><span data-stu-id="cbfcf-107">Data file requirements</span></span>

<span data-ttu-id="cbfcf-108">Chcete-li přidat více uživatelů k účtu zákazníka pomocí procesu hromadného nahrávání, je nutné splnit následující požadavky:</span><span class="sxs-lookup"><span data-stu-id="cbfcf-108">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="cbfcf-109">Musíte mít oprávnění globálního správce k účtu zákazníka;</span><span class="sxs-lookup"><span data-stu-id="cbfcf-109">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="cbfcf-110">Každý uživatel musí mít jedinečnou e-mailovou adresu, která se připojí k e-mailovým doménám zákazníka;</span><span class="sxs-lookup"><span data-stu-id="cbfcf-110">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="cbfcf-111">Můžete nahrávat až 100 záznamů najednou.</span><span class="sxs-lookup"><span data-stu-id="cbfcf-111">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="cbfcf-112">Pokud potřebujete přidat více než 100 uživatelů, vytvořte a nahrajte další datové soubory.</span><span class="sxs-lookup"><span data-stu-id="cbfcf-112">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="cbfcf-113">Všichni uživatelé musí být ve stejném geografickém **umístění**.</span><span class="sxs-lookup"><span data-stu-id="cbfcf-113">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="cbfcf-114">Zadejte pouze data popsaná níže.</span><span class="sxs-lookup"><span data-stu-id="cbfcf-114">Enter only the data described below.</span></span> <span data-ttu-id="cbfcf-115">Nadbytečné údaje způsobí selhání nahrávání.</span><span class="sxs-lookup"><span data-stu-id="cbfcf-115">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="cbfcf-116">V datovém souboru zadejte následující data:</span><span class="sxs-lookup"><span data-stu-id="cbfcf-116">Enter the following data in the data file:</span></span>

| <span data-ttu-id="cbfcf-117">**Název sloupce**</span><span class="sxs-lookup"><span data-stu-id="cbfcf-117">**Column name**</span></span> | <span data-ttu-id="cbfcf-118">**Popis**</span><span class="sxs-lookup"><span data-stu-id="cbfcf-118">**Description**</span></span>  | <span data-ttu-id="cbfcf-119">**Omezení**</span><span class="sxs-lookup"><span data-stu-id="cbfcf-119">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="cbfcf-120">Jméno</span><span class="sxs-lookup"><span data-stu-id="cbfcf-120">First name</span></span>  | <span data-ttu-id="cbfcf-121">Křestní jméno uživatele (volitelné pole)</span><span class="sxs-lookup"><span data-stu-id="cbfcf-121">User's first name (optional field)</span></span>  | <span data-ttu-id="cbfcf-122">50 – limit znaků</span><span class="sxs-lookup"><span data-stu-id="cbfcf-122">50-character limit</span></span>  |
| <span data-ttu-id="cbfcf-123">Příjmení</span><span class="sxs-lookup"><span data-stu-id="cbfcf-123">Last name</span></span>  | <span data-ttu-id="cbfcf-124">Poslední jméno uživatele (volitelné pole)</span><span class="sxs-lookup"><span data-stu-id="cbfcf-124">User's last name (optional field)</span></span>  | <span data-ttu-id="cbfcf-125">50 – limit znaků</span><span class="sxs-lookup"><span data-stu-id="cbfcf-125">50-character limit</span></span>  |
| <span data-ttu-id="cbfcf-126">Zobrazované jméno</span><span class="sxs-lookup"><span data-stu-id="cbfcf-126">Display name</span></span>    | <span data-ttu-id="cbfcf-127">Název zobrazený v Partnerské centrum (povinné pole)</span><span class="sxs-lookup"><span data-stu-id="cbfcf-127">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="cbfcf-128">Limit 50 znaků</span><span class="sxs-lookup"><span data-stu-id="cbfcf-128">50-character limit</span></span>                         |
| <span data-ttu-id="cbfcf-129">E-mail</span><span class="sxs-lookup"><span data-stu-id="cbfcf-129">Email</span></span>   | <span data-ttu-id="cbfcf-130">Obchodní e-mailová adresa uživatele ve společnosti zákazníka (povinné pole)</span><span class="sxs-lookup"><span data-stu-id="cbfcf-130">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="cbfcf-131">Každý uživatel musí mít jedinečnou e-mailovou adresu.</span><span class="sxs-lookup"><span data-stu-id="cbfcf-131">Each user must have a unique email address</span></span> |
| <span data-ttu-id="cbfcf-132">Aktualizace stavu</span><span class="sxs-lookup"><span data-stu-id="cbfcf-132">Status update</span></span>   | <span data-ttu-id="cbfcf-133">Slouží k určení, jestli se nový záznam uživatele úspěšně vytvořil.</span><span class="sxs-lookup"><span data-stu-id="cbfcf-133">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="cbfcf-134">\*\*Ponechte prázdné.\*\*</span><span class="sxs-lookup"><span data-stu-id="cbfcf-134">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="cbfcf-135">Další kroky</span><span class="sxs-lookup"><span data-stu-id="cbfcf-135">Next steps</span></span>

- [<span data-ttu-id="cbfcf-136">Přidání více uživatelů pro zákazníka</span><span class="sxs-lookup"><span data-stu-id="cbfcf-136">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)