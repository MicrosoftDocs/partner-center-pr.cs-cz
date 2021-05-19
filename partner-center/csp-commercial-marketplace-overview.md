---
title: Přehled – web CSP Marketplace
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se prodávat předplatitele předplatné SaaS (software jako služba) od nezávislých výrobců softwaru (ISV) na webu Marketplace.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7c18f69a62e8f8d126a0756911d2fbcdfdb85d8d
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147866"
---
# <a name="overview-of-the-commercial-marketplace-in-partner-center"></a>Přehled komerčního tržiště v partnerském centru

**Příslušné role**: globální správce

Partner v programu Cloud Solution Provider (CSP) umožňuje seskupit a prodávat produkty Microsoftu spolu s řešeními publikovanými nezávislými dodavateli softwaru (ISV) třetích stran. Díky tomu, že je možné rozčlenit řešení tímto způsobem, můžete lépe poskytovat koncovým zákazníkům a rozšířit své obchodní služby CSP.

Jako partner v programu CSP můžete použít Partnerské centrum k nákupu mnoha řešení ISV od komerčního tržiště Microsoftu. Tím a vašim zákazníkům získáte několik klíčových výhod:

- Přístup ke katalogu softwarových řešení optimalizovaných pro technologie a prostředí Microsoftu
- Zjednodušený servisní cyklus a zkracuje se na něj.
- Jedna integrace s rozhraními API partnerského centra (Tato integrace dále umožňuje přístup ke katalogu řešení ISV, snižuje náklady na provoz a strojírenství a zjednodušuje správu několika předplatných dodavatelů a fakturuje se přes jednoho poskytovatele.)
- Zjednodušené nasazení a zřizování v tenantovi Azure zákazníka (pro řešení založená na virtuálních počítačích).
- Omezuje možné problémy s přímým nákupem ISV nebo jejich vyřízením, konfigurací řešení a integrací a potřebou spravovat nebo konsolidovat opakované faktury od různých dodavatelů.

## <a name="overview-of-csp-offers-in-the-commercial-marketplace"></a>Přehled nabídek CSP na komerčním webu Marketplace

Pokud jste partnerem v programu CSP, existuje spousta komerčních aktivit na webu Marketplace, které můžete chtít provést s ohledem na nabídky ISV. Další informace o jednotlivých aktivitách najdete v následující tabulce.

|**Pokud chcete**  |**Oprávnění**   |
|:------------------------------------|:------------------|
|Zjistěte, jak zobrazit nebo vyhledat dostupné nabídky, ceny, podrobnosti o produktu nebo kontaktní informace vydavatele. | [Zjišťování nabídek](csp-commercial-marketplace-discover.md) | 
|Zjistěte, jak zakoupit a nasadit nabídku.   | [Nákup nabídek](csp-commercial-marketplace-purchase.md)   | 
|Zjistěte, jak zrušit nebo obnovit předplatné nebo přidat nebo odebrat licence.  | [Správa nabídek](csp-commercial-marketplace-manage.md) |
|Informace o tom, jak funguje fakturace nákupů na komerčním marketplace | [Principy fakturace](csp-commercial-marketplace-billing.md) |
|Informace o tom, kdo zodpovídá za jaké typy podpory nákupů isv | [Principy podpory](csp-commercial-marketplace-support.md) |
|Informace o kontraktech a zodpovědnostech partnerů CSP a isvů na komerčním marketplace | [Principy kontraktů](csp-commercial-marketplace-contracting.md) |

> [!NOTE]
> Tento přehled popisuje, jak mohou partneři v programu CSP používat některé funkce komerčního marketplace v Partnerské centrum. Na rozdíl od partnerů v programu CSP mají vydavatelé ISV jinou roli na marketplace. Mají také různé funkce komerčního marketplace, které jsou k dispozici v Partnerské centrum. Další informace o roli vydavatelů ISV najdete v tématu [Přehled komerčního marketplace Azure.](/azure/marketplace/partner-center-portal/commercial-marketplace-overview)

## <a name="where-to-complete-commercial-marketplace-activities"></a>Kde dokončit aktivity komerčního marketplace

Jako partner v programu CSP můžete řadu aktivit komerčního marketplace pro nabídky ISV SaaS provést přímo z řídicího panelu Partnerské centrum nebo pomocí [rozhraní API Partnerské centrum.](/partner-center/develop/) [](https://partner.microsoft.com/dashboard) K dokončení dalších aktivit na marketplace ale možná budete muset přejít na:

- Portál [Microsoft Azure pro správu](https://portal.azure.com/)

    Nebo

- Systém nebo web vydavatele isv jiného výrobce softwaru

Velká část toho, kam se můžete dostat k dokončení aktivit, začíná typem nabídky, kterou zvolíte. Partneři v programu CSP můžou v současné době používat dva typy nabídek s vydavateli ISV třetích stran:

1. Nabídky SaaS založené na licencích  
2. Nabídky založené na využití (včetně nabídek založených na virtuálních počítačích, kontejnerech nebo aplikacích Azure)

Další informace o tom, jak se fakturace mezi nabídkami založenými na licencích a nabídkami na základě využití liší, najdete v tématu [základy fakturace](billing-basics.md) .  

Další informace o tom, jak dokončit konkrétní aktivitu Marketplace pro nabídky ISV založené na licencích nebo použití, najdete v následujících tabulkách.

|**Pro nabídky na základě licencí nebo měřený SaaS od nezávislého výrobce softwaru**  |**Použití**  |
|:------------------------------------|:------------------|
|Zjišťování a hledání dostupných nabídek  | Rozhraní API pro řídicí panel nebo partnerské Centrum partnerského centra  |
|Nákup nabídky  | Rozhraní API pro řídicí panel nebo partnerské Centrum partnerského centra  |
|Nasazení zakoupené nabídky (nastavení účtu, Správa softwaru nebo nasazení v tenantovi AAD zákazníka)  | Systém nebo web vydavatele ISV  |
|Zrušení/obnovení předplatných nabídky nebo přidání nebo odebrání licencí | Rozhraní API pro řídicí panel nebo partnerské Centrum partnerského centra  |
|Vytvoření uživatelů nebo Správa oprávnění  | Systém nebo web vydavatele ISV  |

|**Pro nabídky založené na používání od nezávislého výrobce softwaru**  |**Použití**  |
|:------------------------------------|:------------------|
|Zjišťování a hledání dostupných nabídek  | Řídicí panel partnerského centra, rozhraní API partnerského centra nebo Azure Portal  |
|Nákup nabídky  | portál Azure  |
|Nasazení zakoupené nabídky (nastavení účtu, správa softwaru nebo nasazení v tenantovi AAD zákazníka)  | portál Azure  |
|Zrušení nebo prodloužení platnosti předplatných nabídek nebo přidání nebo odebrání licencí | portál Azure  |
|Vytvoření uživatelů nebo správa oprávnění  | portál Azure  |

## <a name="next-steps"></a>Další kroky

- [Zjišťování nebo zobrazení nabídek komerčního marketplace](csp-commercial-marketplace-discover.md)
- [Nákup nabídek komerčního marketplace](csp-commercial-marketplace-purchase.md)
