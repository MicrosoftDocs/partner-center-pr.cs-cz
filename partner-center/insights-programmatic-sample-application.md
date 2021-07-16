---
title: Ukázková aplikace
ms.topic: article
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Použijte ukázkovou aplikaci k vytvoření vlastní aplikace pro programové získání přístupu k datům o partner Insights.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: 6f334b9047c38e8b7763a4ba96d21d987c252682
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376382"
---
# <a name="sample-application"></a><span data-ttu-id="612b1-103">Ukázková aplikace</span><span class="sxs-lookup"><span data-stu-id="612b1-103">Sample Application</span></span>

<span data-ttu-id="612b1-104">Ukázkové aplikace jsou vytvořeny v jazycích C# a JAVA a jsou k dispozici na [GitHub](https://github.com/partneranalytics)</span><span class="sxs-lookup"><span data-stu-id="612b1-104">Sample applications are created in C# and JAVA languages and are available on [GitHub](https://github.com/partneranalytics)</span></span>

- [<span data-ttu-id="612b1-105">Ukázková aplikace v jazyce C#</span><span class="sxs-lookup"><span data-stu-id="612b1-105">C# Sample Application</span></span>](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [<span data-ttu-id="612b1-106">Ukázková aplikace JAVA</span><span class="sxs-lookup"><span data-stu-id="612b1-106">JAVA Sample Application</span></span>](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

<span data-ttu-id="612b1-107">Můžete si vybrat, že se inspiraci z ukázkové aplikace a sestavíte svou vlastní aplikaci v jakémkoli jazyce.</span><span class="sxs-lookup"><span data-stu-id="612b1-107">You can choose to take inspiration from the sample application and build your own application in any language.</span></span>

<span data-ttu-id="612b1-108">Ukázková aplikace dosahuje následujících cílů:</span><span class="sxs-lookup"><span data-stu-id="612b1-108">The sample application achieves the following objectives:</span></span>

- <span data-ttu-id="612b1-109">vygeneruje Token Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="612b1-109">Generates an Azure Active Directory (Azure AD) Token.</span></span>
- <span data-ttu-id="612b1-110">Získá dostupné datové sady.</span><span class="sxs-lookup"><span data-stu-id="612b1-110">Gets available datasets.</span></span>
- <span data-ttu-id="612b1-111">Vytvoří dotazy definované uživatelem.</span><span class="sxs-lookup"><span data-stu-id="612b1-111">Creates user defined queries.</span></span>
- <span data-ttu-id="612b1-112">Získá uživatelsky definované a systémové dotazy.</span><span class="sxs-lookup"><span data-stu-id="612b1-112">Gets user defined and system queries.</span></span>
- <span data-ttu-id="612b1-113">Naplánuje sestavu.</span><span class="sxs-lookup"><span data-stu-id="612b1-113">Schedules a report.</span></span>

<span data-ttu-id="612b1-114">Ukázková aplikace nepokrývá metodu volání rozhraní API pro jiné funkce.</span><span class="sxs-lookup"><span data-stu-id="612b1-114">The sample application doesn't cover the method of calling APIs for other functionalities.</span></span> <span data-ttu-id="612b1-115">Proces volání jiných rozhraní API však zůstává stejný, jak je popsáno výše.</span><span class="sxs-lookup"><span data-stu-id="612b1-115">However, the process of calling other APIs remains the same as outlined above.</span></span>

## <a name="how-to-run-the-application"></a><span data-ttu-id="612b1-116">Spuštění aplikace</span><span class="sxs-lookup"><span data-stu-id="612b1-116">How to run the application</span></span>

- <span data-ttu-id="612b1-117">Naklonujte úložiště do místního systému pomocí tohoto příkazu:</span><span class="sxs-lookup"><span data-stu-id="612b1-117">Clone the repository to a local system using this command:</span></span>

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> <span data-ttu-id="612b1-118">další pokyny najdete v souboru ProgrammaticExportSampleAppMPN/readme. md v [úložišti](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)GitHub.</span><span class="sxs-lookup"><span data-stu-id="612b1-118">For more instructions, refer to the ProgrammaticExportSampleAppMPN/README.md file in the GitHub [repository](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java).</span></span>

- <span data-ttu-id="612b1-119">Pokud chcete aplikaci rychle spustit, aktualizujte ID klienta a tajný klíč klienta v **appsettings.Development.jsdne** .</span><span class="sxs-lookup"><span data-stu-id="612b1-119">To quickly run the app, update the client id and client secret in the **appsettings.Development.json**</span></span>

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="Ilustrace kódu JSON pro vývoj AppSetting":::

<span data-ttu-id="612b1-121">Spuštění aplikace spustí místní webový server a otevře se stránka ( `https://localhost:44365/ProgrammaticExportSampleApp/sample` ).</span><span class="sxs-lookup"><span data-stu-id="612b1-121">Running the app will start a local web server and a page will open (`https://localhost:44365/ProgrammaticExportSampleApp/sample`).</span></span>
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="Znázornění uživatelského rozhraní ukázkové aplikace":::

<span data-ttu-id="612b1-123">Tato stránka provede volání rozhraní API na server, který běží na místním počítači, a pak provede skutečná volání rozhraní API pro programové přístup.</span><span class="sxs-lookup"><span data-stu-id="612b1-123">This page will make API calls to the webserver running on the local machine, which in turn will make the actual programmatic access API calls.</span></span>

## <a name="code-snippets"></a><span data-ttu-id="612b1-124">Fragmenty kódu</span><span class="sxs-lookup"><span data-stu-id="612b1-124">Code Snippets</span></span>

<span data-ttu-id="612b1-125">Základní struktura kódu jazyka C# pro volání rozhraní API pro programové přístup je následující:</span><span class="sxs-lookup"><span data-stu-id="612b1-125">The basic structure of the C# code for doing the programmatic access API calls is as follows:</span></span>
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Ilustrující fragment kódu":::

## <a name="next-steps"></a><span data-ttu-id="612b1-127">Další kroky</span><span class="sxs-lookup"><span data-stu-id="612b1-127">Next steps</span></span>

[<span data-ttu-id="612b1-128">Rozhraní API pro přístup k datům služby partner Insights Analytics</span><span class="sxs-lookup"><span data-stu-id="612b1-128">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)
