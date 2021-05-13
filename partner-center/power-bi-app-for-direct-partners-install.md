---
title: Instalace analýzy partnerského centra pro Power BI
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Postupujte podle kroků v tomto článku a nainstalujte a zobrazte si ukázkovou aplikaci partner Center Analytics pro Power BI (pro přímé partnery v CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 15ee391d6b748b6499700aee321ff4abd85e75d2
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854481"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Instalace a vyzkoušení aplikace Analýzy v Partnerském centru pro Microsoft Power BI


**Příslušné role**: globální správce | Správce správy uživatelů | Prodejní agent | Agent správce

## <a name="before-you-begin"></a>Než začnete

Vyberte aplikaci, která je pro vaši firmu nejdůležitější, z následujícího seznamu dostupných Power BIch aplikací:

- [Přímý poskytovatel](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [Nepřímý poskytovatel](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [Nepřímý prodejce](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

Než nainstalujete verzi Preview partnerského centra pro analýzu, ujistěte se, že splňujete následující požadavky.

- Vyberte správnou aplikaci Power BI pro vaši firmu.

- Máte licenci Power BI pro.

- Máte oprávnění k instalaci aplikací šablon do svého tenanta.

- Můžete se přihlásit k Power BI.

- K [tenantovi Azure Active Directory vaší společnosti (Azure AD)](azure-active-directory-tenants-and-partner-center.md)se můžete přihlásit jako globální správce, agent pro správu nebo správce fakturace.

## <a name="to-install-the-app"></a>Instalace aplikace

1. V části výše vyberte zdrojový odkaz aplikace (přímý poskytovatel/nepřímý poskytovatel/nepřímý prodejce).

2. Vyberte **získat hned**. 

3. Odsouhlasení podmínek a ujednání výběrem možnosti **pokračovat**.

4. V části už máte účet? Vyberte **Přihlásit se**.

5. Na další stránce zadejte své uživatelské jméno a heslo Power BI a pak vyberte **Přihlásit se**.

6. Nainstalujte pracovní prostor zadáním názvu pracovního prostoru.

7. Nainstalované aplikace šablon najdete v části Aplikace.

8. Vyberte **Aplikace a** zvolte nainstalované aplikace.

9. Otevře se obrazovka Začínáme s novou aplikací.

10. Pokud se chcete připojit k datům, vyberte **Připojit.**

11. V automaticky **otevíraně otevřeném okně Připojit** k  Partnerské centrum Analytics ověřte, že je metoda ověřování nastavená na oAuth2, nebo v seznamu vyberte **oAuth2,** pokud není.  

> [!NOTE]  
>  Zobrazení tohoto okna může trvat několik minut.

12. Na stránce **Partnerské centrum Analytics Connector** se přihlaste pomocí globálního správce, agenta pro správu nebo přihlašovacích údajů správce fakturace pro tenanta Azure AD vaší společnosti a pak vyberte **Přihlásit se.**
 
13. Po zobrazení výzvy k zadání přístupu vyberte **Přijmout.** 

Jakmile je Partnerské centrum Analytics připojená k Power BI, začnou se načítat data. V závislosti na množství dat to může trvat až 10 minut. 

Po dokončení načítání dat můžete začít používat řídicí panel aplikace Partnerské centrum Analytics a sestavy v Power BI.

## <a name="next-steps"></a>Další kroky

[Zobrazení obchodních dat pomocí aplikace Partnerské centrum Analytics pro Microsoft Power BI](power-bi-app-for-direct-partners-use.md)
