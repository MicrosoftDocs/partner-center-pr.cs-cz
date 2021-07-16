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
# <a name="sample-application"></a>Ukázková aplikace

Ukázkové aplikace jsou vytvořeny v jazycích C# a JAVA a jsou k dispozici na [GitHub](https://github.com/partneranalytics)

- [Ukázková aplikace v jazyce C#](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [Ukázková aplikace JAVA](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

Můžete si vybrat, že se inspiraci z ukázkové aplikace a sestavíte svou vlastní aplikaci v jakémkoli jazyce.

Ukázková aplikace dosahuje následujících cílů:

- vygeneruje Token Azure Active Directory (Azure AD).
- Získá dostupné datové sady.
- Vytvoří dotazy definované uživatelem.
- Získá uživatelsky definované a systémové dotazy.
- Naplánuje sestavu.

Ukázková aplikace nepokrývá metodu volání rozhraní API pro jiné funkce. Proces volání jiných rozhraní API však zůstává stejný, jak je popsáno výše.

## <a name="how-to-run-the-application"></a>Spuštění aplikace

- Naklonujte úložiště do místního systému pomocí tohoto příkazu:

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> další pokyny najdete v souboru ProgrammaticExportSampleAppMPN/readme. md v [úložišti](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)GitHub.

- Pokud chcete aplikaci rychle spustit, aktualizujte ID klienta a tajný klíč klienta v **appsettings.Development.jsdne** .

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="Ilustrace kódu JSON pro vývoj AppSetting":::

Spuštění aplikace spustí místní webový server a otevře se stránka ( `https://localhost:44365/ProgrammaticExportSampleApp/sample` ).
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="Znázornění uživatelského rozhraní ukázkové aplikace":::

Tato stránka provede volání rozhraní API na server, který běží na místním počítači, a pak provede skutečná volání rozhraní API pro programové přístup.

## <a name="code-snippets"></a>Fragmenty kódu

Základní struktura kódu jazyka C# pro volání rozhraní API pro programové přístup je následující:
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Ilustrující fragment kódu":::

## <a name="next-steps"></a>Další kroky

[Rozhraní API pro přístup k datům služby partner Insights Analytics](insights-programmatic-analytics-available-api.md)
