---
title: Migrace Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak migrovat kvalifikované nabídky Dynamics 365 Business Edition na novější verze před vypršením jejich platnosti.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8232ab165ea68ebefdfbb30f3ac52c907e1b7278
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151521"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Migrace nabídek Dynamics 365 Business Edition na novější verze

**Odpovídající role:** Globální správce | Správce správy uživatelů | Agent správy | Agent prodeje

Od 1. ledna 2019 se zákazníci s předplatným Dynamics 365 Business Edition už nebudou moci v těchto starších verzích nabídek prodlužovat. stávající předplatná se po vypršení jejich platnosti automaticky neobnoví. Na stránce s podrobnostmi o předplatném se stav předplatného změní na Platnost vyprší [datum]" z "Automatické prodloužení platnosti k [datum]".

Pokud chcete zajistit kontinuitu pro zákazníky, měli byste uživatele s předplatným s vypršenou platnosti přejít na podporovanou možnost uvedenou níže. Doporučujeme přestěhovat zákazníky na nová předplatná před ročním datem ukončení předplatného, abyste se vyhnuli výpadkům služeb pro zákazníky.

Pokud používáte rozhraní API (CREST nebo Partnerské centrum), můžete zjistit vypršení platnosti odběrů vyhodnocením koncového data odběru spolu s vlastností auto renew = False. 1. ledna 2019 budou 1. ledna 2019 sporná předplatná nastavená na auto renew=False. Zákazníky můžete kdykoli přesunout do nového plánu. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>Vyřazení edicí Dynamics 365 Business Edition

- Dynamics 365 for Finance and Operations, edice Business
- Dynamics 365 for Team Members, edice Business

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central – nové nabídky Dynamics 365 Business Edition

S novými nabídkami Dynamics Business Central mohou vaši zákazníci propojit své finanční prostředky, prodej, službu a provoz a zjednodušit tak obchodní procesy, zlepšit interakce se zákazníky a lépe se rozhodovat. Dynamics 365 Business Central je cloudová a dostupná pouze prostřednictvím partnerů Cloud Solution Provider (CSP).
Zákazníci Dynamics 365 Business Edition mají nárok na zvýhodněné převodní ceny pro nové nabídky Business Central do 30. června 2020.

## <a name="transition-customers-to-new-product-plans"></a>Převod zákazníků na nové produktové plány

 Přesun zákazníků z vyřazených SKU na novější vyžaduje následující kroky v tomto pořadí:

- Zakoupení nového předplatného
- Opětovné přiřazení aktuálních uživatelských licencí
- Zrušení starého předplatného

## <a name="purchase-the-new-plan-for-your-customer"></a>Nákup nového plánu pro zákazníka

1. V **levém** navigačním panelu vyberte Zákazníci a pak vyberte zákazníka, kterého chcete přesunout do nového předplatného.
2. Vyberte **Přidat předplatné.**
3. Vyberte předplatné, které chcete zakoupit z katalogu (v tomto případě jednu z výše uvedených možností), zadejte počet licencí a pak vyberte **Odeslat.** 

Váš zákazník teď bude mít staré i nové předplatné. Dalším krokem je opětovné přiřazení licencí uživatelům zákazníka.

1. V **levém** navigačním panelu vyberte Zákazníci a pak vyberte zákazníka, který přesouváte.
2. Vyberte **Uživatelé a licence.**
3. Pokud chcete přiřadit licenci uživateli znovu, vyberte uživatele a pak vyberte **Spravovat licence.** 
4. Na  stránce Spravovat licence zrušte zaškrtnutí políčka Dynamics 365 for Sales/ Customer Engagement Plan (Plán Dynamics 365 for Customer Engagement z licence basic (kvalifikovaná nabídka) a vyberte nový plán služby pro předplatné, do které zákazník přechází. 
5. Vyberte **Odeslat**. To budete dělat pro každého uživatele, který potřebuje novou licenci. 

Po přesunu licencí do nového předplatného můžete staré předplatné zrušit. 

1. V **levém** navigačním panelu vyberte Zákazníci a pak vyberte zákazníka, který přesouváte.
2. Na stránce podrobností o předplatném nastavte staré předplatné na **Pozastaveno** a vyberte **Odeslat.**

Původní předplatné je teď pozastavené a nové předplatné je aktivní. Pozastavené předplatné bude po 120 dnech automaticky zrušeno. Za staré předplatné se zákazníkovi ne účtut žádné další poplatky.
