---
title: Migrace předplatných Kaizala Pro na Microsoft 365
description: Zjistěte, jak migrovat předplatná Kaizala Pro na Microsoft 365 nebo verze Office 365. Další podrobnosti o přechodu zákazníků najdete v tomto článku.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 583e9c40bb8d161c30440f12331dc8dcbf3db417
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146421"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a>Migrace samostatných předplatných Kaizala Pro na Microsoft 365 nebo verze Office 365

**Odpovídající role:** Agent prodeje

Od 1. července 2020 Microsoft ukončí prodej samostatné služby Kaizala Pro. Zákazníci už nebudou moct po tomto datu kupovat nová předplatná Kaizala Pro a stávající předplatná Kaizala Pro se po vypršení jejich platnosti automaticky neobnoví.

Pokud chcete zajistit kontinuitu pro zákazníky, měli byste zákazníky, kteří mají vypršenou platnost samostatných předplatných Kaizala Pro, pře převodovat na podporovanou možnost SKU uvedenou níže. Doporučujeme přestěhovat zákazníky na nová předplatná před ročním datem ukončení předplatného, abyste se vyhnuli výpadkům služeb pro zákazníky.

Pokud používáte rozhraní API (CREST nebo Partnerské centrum), můžete zjistit předplatná, kterým vyprší platnost, vyhodnocením koncového data odběru spolu s vlastností automatického obnovení nastavenou na false: `auto renew = False` .

Předplatná E4 se nastaví na `auto renew=False` 1. července 2020. Zákazníky můžete kdykoli přesunout do nového plánu.

## <a name="kaizala-pro-standalone-replacement-plans"></a>Náhradní plány Kaizala Pro Standalone

S těmito novými plány mohou vaši zákazníci využívat novější funkce v Microsoft 365. Podrobnosti o cenách najdete v matici ceníku a seznamu nabídek v Partnerské centrum.

- [**Microsoft 365 for Business,**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2)včetně:  
   - Microsoft 365 Business Basic
   - Microsoft 365 Business Standard
   - Microsoft 365 Business Premium
    
- [**Microsoft 365 pro frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), včetně:
   - Microsoft 365 F3 (dříve Microsoft 365 F1) a Office 365 F3
    
- [**Microsoft 365 pro podniky**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), včetně: 
   - Office 365 E1
   - Microsoft 365 E3 a Office 365 E3
   - Microsoft 365 E5 a Office 365 E5

- [**Microsoft 365 pro vzdělávání**](https://www.microsoft.com/education/buy-license/microsoft365), včetně: 
    - Microsoft 365 a1 a Office 365 a1
    - Microsoft 365 a3 a Office 365 a3
    - Microsoft 365 a5 a Office 365 a5

## <a name="transition-customers-to-new-product-plans"></a>Přechod zákazníků na nové plány produktů

Microsoft neustále nabízí našim partnerům nové produkty a služby. V těchto případech možná budete muset upgradovat zákazníky na nové služby nebo migrovat své odběry z SKU, které se nakonec vypnou. Migrace zákazníků z vyřazených SKU do novějších vyžaduje následující kroky:

A. Koupit nové předplatné

B. Změna přiřazení licencí k aktuálním uživatelům

C. Zrušit staré předplatné


## <a name="migrate-your-customers-to-new-plans"></a>Migrace zákazníků na nové plány

### <a name="a-purchase-the-new-subscription"></a>A. Koupit nové předplatné

1. Pokud chcete nové předplatné koupit, vyberte v nabídce **Partnerské centrum** možnost **zákazníci**, vyberte zákazníka, kterého chcete přesunout, a pak vyberte **Přidat předplatná**.

2. Vyberte předplatné, které chcete z katalogu koupit (v tomto případě jednu z výše uvedených možností), zadejte počet licencí a pak vyberte **Odeslat**.

Váš zákazník by teď měl mít staré i nové předplatné, staré předplatné Kaizala pro a nové předplatné Target, třeba možnost 1 – Office 365 Enterprise F1.

### <a name="b-reassign-current-user-licenses"></a>B. Opětovné přiřazení aktuálních uživatelských licencí

1. Pokud chcete znovu přiřadit licence uživatelů zákazníka, v nabídce **Partnerské centrum** vyberte **Zákazníci,** vyberte zákazníka, který přesouváte, a pak vyberte Uživatelé a **licence.** Otevře se stránka Uživatelé a licence zákazníka.

2. Pokud chcete znovu přiřadit uživatelskou licenci, vyberte uživatele, který chcete znovu přiřadit, a pak vyberte **Spravovat licence.**

3. Na stránce **Spravovat licence** zrušte zaškrtnutí políčka Kaizala Pro Standalone license (Samostatná licence Kaizala Pro) a vyberte nový plán služby pro předplatné, do které zákazník přemísťuje.

4.  Vyberte **Odeslat**. Na potvrzovací stránce se zobrazí nová přiřazení licencí. Pokračujte stejným způsobem i pro ostatní uživatele, kteří potřebují přiřazení licencí.

### <a name="c-cancel-old-subscription"></a>C. Zrušení starého předplatného

Po přesunutí uživatelské licence na novou službu můžete vyřazené předplatné bezpečně zrušit na úrovni zákazníka.

1.  V **nabídce Partnerské centrum** vyberte **Zákazníci.** Vyberte zákazníka, jehož předplatné zrušíte.

2.  Na stránce s podrobnostmi o předplatném nastavte předplatné na **Pozastaveno.**

3.  Vyberte **Odeslat**.

Původní předplatné je pozastavené a nové předplatné je aktivní. Pozastavené předplatné bude po 120 dnech automaticky zrušeno. Za staré předplatné se zákazníkovi ne účtuly žádné další poplatky.
