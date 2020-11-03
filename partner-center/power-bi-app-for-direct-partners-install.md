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
ms.openlocfilehash: 64467ec608c2ca87dbc2b7d5dfb02adb08f13c18
ms.sourcegitcommit: 0a6b1e6d845391539f54213efff00af4d23f028c
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/14/2020
ms.locfileid: "92526999"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Instalace a vyzkoušení aplikace Analýzy v Partnerském centru pro Microsoft Power BI

**Platí pro**

- Partnerské centrum

**Příslušné role**
-   Globální správce
-   Správce uživatelů
-   Agent prodeje
-   Agent správce

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

1. V předchozí části klikněte na příslušný odkaz na zdroj aplikace (přímý poskytovatel/nepřímý poskytovatel/nepřímý prodejce).

2. Klikněte na **získat hned** . 

3. Kliknutím na **pokračovat** souhlasíte s podmínkami a ujednáními.

4. V části už máte účet? Vyberte **Přihlásit se** .

5. Na další stránce zadejte své uživatelské jméno a heslo Power BI a pak vyberte přihlásit se.

6. Nainstalujte pracovní prostor zadáním názvu pracovního prostoru.

7. Nainstalovanou šablonu aplikace můžete najít v části aplikace.

8. Klikněte na aplikace a vyberte nainstalované aplikace.

9. Začněte tím, že otevřete obrazovku nové aplikace.

10. Pokud se chcete připojit k datům, klikněte na **připojit** .

11. V místním okně **připojit k partnerskému centru Analytics** ověřte, že je **metoda ověřování** nastavená na **oAuth2** , nebo vyberte **oAuth2** ze seznamu, pokud není. 

> [!NOTE]  
>  Zobrazení tohoto okna může trvat několik minut.

12. Na stránce **konektor Datacenter Center Analytics** se přihlaste pomocí účtu globálního správce, agenta správce nebo přihlašovacích údajů správce fakturace pro TENANTA Azure AD vaší společnosti a pak vyberte **Přihlásit** se.
 
13. Po zobrazení výzvy k zadání přístupu vyberte **přijmout** . 

Jakmile je služba pro analýzu partnerského centra připojená k Power BI, začnou se data načíst. V závislosti na množství dat může to trvat až 10 minut. 

Po načtení dat můžete začít používat řídicí panel aplikace a sestavy partnerského centra pro analytiky v Power BI.

## <a name="next-steps"></a>Další kroky

[Zobrazení obchodních dat pomocí aplikace Datacenter Center Analytics pro Microsoft Power BI](power-bi-app-for-direct-partners-use.md)
