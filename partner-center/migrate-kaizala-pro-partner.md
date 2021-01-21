---
title: Migrace předplatných Kaizala sady pro do Microsoft365
description: Naučte se migrovat předplatná Kaizala pro na verze Microsoft365 nebo Office 365. Přečtěte si tento článek, kde najdete další podrobnosti o přechodu zákazníků.
ms.topic: article
ms.service: partner-dashboard
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 0807931ae95b5c7d76f4ad33708cc8014412f55f
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/19/2020
ms.locfileid: "92527753"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft365-or-office-365-versions"></a>Migrace Kaizala pro samostatné odběry do verzí Microsoft365 nebo Office 365

Od 1. července 2020 společnost Microsoft ukončuje prodej samostatné služby Kaizala pro. Zákazníci už nebudou moct koupit nové předplatné Kaizala pro po tomto datu a stávající předplatné Kaizala pro se po uplynutí této doby nebudou automaticky obnovovat.

Chcete-li zajistit kontinuitu pro zákazníky, doporučujeme, abyste zákazníkům přešli do vypršení platnosti samostatného předplatného Kaizala pro s podporovanou možností SKU, která je uvedená níže. Doporučujeme zákazníkům přesunout nové předplatné před uplynutím ročního koncového data předplatného, aby se předešlo výpadkům služby pro zákazníky.

Pokud používáte rozhraní API (buď CREST nebo Partnerská centra), můžete zjistit platnost předplatných, a to tak, že vyhodnocujete koncové datum předplatného spolu s vlastností automatického obnovení nastavenou na hodnotu NEPRAVDA: `auto renew = False` .

Odběry E4 budou nastavené na `auto renew=False` 1. července 2020. Zákazníky můžete kdykoli přesunout do nového plánu.

## <a name="kaizala-pro-standalone-replacement-plans"></a>Samostatné plány nahrazení Kaizala pro

S novými plány můžou zákazníci využít výhod novějších funkcí a funkcí v Microsoft 365. Podrobnosti o cenách najdete v seznamu ceníků a v tabulce seznam nabídek v partnerském centru.

- [**Microsoft 365 pro firmy**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), včetně:  
   - Microsoft 365 Business Basic
   - Microsoft 365 Business Standard
   - Microsoft 365 Business Premium
    
- [**Microsoft 365 pro prvotní**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), včetně:
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

### <a name="b-reassign-current-user-licenses"></a>B. Změna přiřazení licencí k aktuálním uživatelům

1. Pokud chcete znovu přiřadit licence uživatelů zákazníka, vyberte v nabídce **Partnerské centrum** možnost **zákazníci**, vyberte zákazníka, kterého přesouváte, a pak vyberte **Uživatelé a licence**. Otevře se stránka uživatelé a licence zákazníka.

2. Pokud chcete znovu přiřadit uživatelskou licenci, vyberte uživatele, kterého chcete znovu přiřadit, a pak vyberte **spravovat licence**.

3. Na stránce **spravovat licence** zrušte zaškrtnutí políčka Kaizala pro samostatnou licenci a vyberte nový plán služby pro předplatné, na které se bude zákazník pohybovat.

4.  Vyberte **Odeslat**. Stránka s potvrzením obsahuje seznam nových přiřazení licencí. Pokračujte stejným postupem pro ostatní uživatele, kteří potřebují přiřazení licencí.

### <a name="c-cancel-old-subscription"></a>C. Zrušit staré předplatné

Po přesunutí uživatelské licence na novou službu můžete zrušit vyřazené předplatné na úrovni zákazníka.

1.  V nabídce **Partnerské centrum** vyberte **zákazníci**. Vyberte zákazníka, jehož předplatné rušíte.

2.  Na stránce s podrobnostmi předplatného nastavte předplatné na **pozastaveno**.

3.  Vyberte **Odeslat**.

Staré předplatné je pozastavené a nové předplatné je aktivní. Pozastavený odběr bude po 120 dnech automaticky zřízen. Zákazník nevzniká žádné další poplatky za původní předplatné.
