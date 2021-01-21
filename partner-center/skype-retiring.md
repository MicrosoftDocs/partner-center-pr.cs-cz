---
title: Migrace některých předplatných Skypu pro firmy
description: Přečtěte si, jak a kdy se mají migrovat někteří zákazníci s vypršením platnosti předplatných služby Skype for Business Online Plan pro nové verze Office 365.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: c9ad5b1c0671ff1d27d25c6f92499b72d77e6c22
ms.sourcegitcommit: c40f826bb1143555bf3a1c2c806c34024f0f6019
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/02/2020
ms.locfileid: "92527218"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Migrace předplatných Online Skypu pro firmy (plán 1) na novější verze Office 365

**Platí pro**

- Partnerské centrum

Plán 1 pro Online Skype pro firmy bude vyřazený, platí od 1. srpna 2018. Po tomto datu si zákazníci už nebudou moct koupit nové předplatné pro Skype pro firmy Plan 1 a stávající odběry se po vypršení platnosti nebudou automaticky obnovovat a nenabídnou možnost obnovení. Na stránce s podrobnostmi o předplatném se stav předplatného pro Skype for Business Online plánu 1 změnil na "vyprší dne [Date]" z "automatické obnovy" v [datum] ".  

Chcete-li zajistit kontinuitu pro zákazníky, doporučujeme, abyste zákazníkům přešli do vypršení platnosti předplatného online plánu Skypu pro firmy na podporovanou možnost SKU, která je uvedená níže. Doporučujeme zákazníkům přesunout nové předplatné před uplynutím ročního koncového data předplatného, aby se předešlo výpadkům služby pro zákazníky. 

>[!NOTE]
>Plán 1 pro Online Skype pro firmy je vyřazený z komerčních i státních SKU.

Pokud používáte rozhraní API (buď CREST nebo Partnerská centra), najděte vypršení platnosti předplatného, a to společně s vlastností automaticky obnovit = false. Předplatné plánu 1 pro Skype pro firmy online se nastaví na hodnotu automaticky obnovit = false od 1. září 2018. Zákazníky můžete kdykoli přesunout do nového plánu. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Plán 1 pro nahrazení Online Skypu pro firmy

S novými plány můžou vaši zákazníci využívat výhod novějších funkcí a funkcí v Office 365. Podrobnosti o cenách najdete v seznamu ceníků a v tabulce seznam nabídek v partnerském centru. 

- Možnost 1: Office 365 Enterprise F1
- Možnost 2: Microsoft 365 Enterprise F1
- Možnost 3: jiné plány Office 365

|**Funkce**    |**Možnost 1**   |**Možnost 2**   |**Možnost 3**   |
|:-----------------|:-----------------|:-------------|:------------|
|Získejte všechny funkce zahrnuté v plánu 1 pro Skype for Business Online.|Ano   |Ano   |Ano   |
|IM a přítomnost |Ano   |Ano   |Ano   |
|Zvuk a video peer-to-peer přes IP adresu|Ano   |Ano   |Ano   
|Připojit schůzky jako ověřeného uživatele| Ano   |Ano   |Ano   |

## <a name="transition-customers-to-new-product-plans"></a>Přechod zákazníků na nové plány produktů

Microsoft neustále nabízí našim partnerům nové produkty a služby. V těchto případech možná budete muset upgradovat zákazníky na nové služby nebo migrovat své odběry z SKU, které se nakonec vypnou. Migrace zákazníků z vyřazených SKU do novějších vyžaduje následující kroky:

- Koupit nové předplatné
- Změna přiřazení licencí k aktuálním uživatelům
- Zrušit staré předplatné

### <a name="migrate-your-customers-to-new-plans"></a>Migrace zákazníků na nové plány

1. Pokud chcete nové předplatné koupit, vyberte v **nabídce partnerské Centrum** možnost **zákazníci**, vyberte zákazníka, kterého chcete přesunout, a pak vyberte **Přidat předplatná**.

2. Vyberte předplatné, které chcete z katalogu koupit (v tomto případě jednu z výše uvedených možností), zadejte počet licencí a pak vyberte **Odeslat**. 

Váš zákazník by teď měl mít staré i nové předplatné, staré předplatné online pro Skype pro firmy a nové předplatné Target, třeba možnost 1 – Office 365 Enterprise F1.

3. Pokud chcete znovu přiřadit licence uživatelů zákazníka, vyberte v nabídce **Partnerské centrum** možnost **zákazníci**, vyberte zákazníka, kterého přesouváte, a pak vyberte **Uživatelé a licence**. Otevře se stránka uživatelé a licence zákazníka.

4. Pokud chcete znovu přiřadit uživatelskou licenci, vyberte uživatele, kterého chcete znovu přiřadit, a pak vyberte **spravovat licence.**

5. Na stránce **spravovat licence** zrušte zaškrtnutí políčka licence pro Skype for Business Online Plan 1 a vyberte nový plán služby pro předplatné, na které se bude zákazník pohybovat.

6. Vyberte **Odeslat**. Stránka s potvrzením obsahuje seznam nových přiřazení licencí. Pokračujte stejným postupem pro ostatní uživatele, kteří potřebují přiřazení licencí.

Po přesunutí uživatelské licence na novou službu můžete zrušit vyřazené předplatné na úrovni zákazníka.

7. V nabídce **Partnerské centrum** vyberte **zákazníci**. Vyberte zákazníka, jehož předplatné rušíte.

8. Na stránce s podrobnostmi předplatného nastavte předplatné na **pozastaveno**.

9. Vyberte **Odeslat.**

Staré předplatné je pozastavené a nové předplatné je aktivní. Pozastavený odběr bude po 120 dnech automaticky zřízen. Zákazník nevzniká žádné další poplatky za původní předplatné.

