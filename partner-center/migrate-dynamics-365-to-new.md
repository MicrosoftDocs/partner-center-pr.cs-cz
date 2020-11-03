---
title: Migrace verze Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si, jak migrovat kvalifikované nabídky Dynamics 365 Business Edition do novějších verzí, než vyprší jejich platnost.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d441d121c28c2762d1f1c71d6f6a1e81d089f99c
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/17/2020
ms.locfileid: "92527030"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Migrace nabídek Dynamics 365 Business Edition na novější verze

**Platí pro**

- Partnerské centrum

**Příslušné role**
- Globální správce
- Správce uživatelů
- Agent správce
- Agent prodeje

Od 1. ledna 2019 se zákazníci s předplatným Dynamics 365 Business Edition už nemůžou prodloužit na tyto starší nabídky. existující odběry se po vypršení platnosti automaticky neobnoví. Na stránce s podrobnostmi o předplatném se stav předplatného změní na "vyprší dne [Date]" z "automatické obnovování v [datum]".

Chcete-li zajistit kontinuitu pro zákazníky, měli byste je přecházet s vypršením platnosti předplatných na podporovanou možnost, která je uvedena níže. Doporučujeme zákazníkům přesunout nové předplatné před uplynutím ročního koncového data předplatného, aby se předešlo výpadkům služby pro zákazníky.

Pokud používáte rozhraní API (buď CREST nebo Partnerská centra), můžete najít odběry, které vyhodnocuje datum ukončení předplatného spolu s vlastností automaticky obnovit = false. V případě 1. ledna 2019 budou předplatná nastavena na hodnotu automaticky obnovit = false. Zákazníky můžete kdykoli přesunout do nového plánu. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>Vyřazení obchodních edicí Dynamics 365

- Dynamics 365 pro finance a provoz, Business Edition
- Dynamics 365 pro členy týmu, verze Business Edition

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central – nové nabídky pro Dynamics 365 Business Edition

Díky novým nabídkám Dynamics Business Central můžou vaši zákazníci připojit své finanční služby, prodej, služby a operace, aby zjednodušily obchodní procesy, zlepšili interakce zákazníků a lépe rozhodovat. Dynamics 365 Business Central je cloudová a dostupná jenom prostřednictvím partnerů programu Cloud Solution Provider (CSP).
Zákazníci Dynamics 365 Business Edition mají nárok na zlevněné přechody na nové nabídky Business Central do 30. června 2020.

## <a name="transition-customers-to-new-product-plans"></a>Přechod zákazníků na nové plány produktů

 Přesun zákazníků z vyřazených SKU do novějšího vyžaduje následující kroky v tomto pořadí:

- Koupit nové předplatné
- Změna přiřazení licencí k aktuálním uživatelům
- Zrušit staré předplatné

## <a name="purchase-the-new-plan-for-your-customer"></a>Zakupte si nový plán pro zákazníka.

1. V levém navigačním panelu vyberte **zákazníky** a pak vyberte zákazníka, kterého chcete přesunout do nového předplatného.
2. Vyberte **přidat odběr** .
3. Vyberte předplatné, které chcete z katalogu koupit (v tomto případě jednu z výše uvedených možností), zadejte počet licencí a pak vyberte **Odeslat** . 

Zákazník teď bude mít původní předplatné i nový. Vaším dalším krokem je změna přiřazení licencí uživatelům zákazníka.

1. V levém navigačním panelu vyberte **zákazníky** a pak vyberte zákazníka, kterého přesouváte.
2. Vyberte **Uživatelé a licence** .
3. Pokud chcete uživateli přiřadit licenci, vyberte uživatele a pak vyberte **spravovat licence** . 
4. Na stránce **spravovat licence** zrušte zaškrtnutí políčka Dynamics 365 pro možnost plán služby Sales/zákazník Engagement z licence Basic (kvalifikovaná nabídka) a vyberte nový plán služby pro předplatné, na které se bude zákazník pohybovat. 
5. Vyberte **Odeslat** . To provedete pro každého uživatele, který bude tuto novou licenci potřebovat. 

Po přesunutí licencí do nového předplatného můžete zrušit původní předplatné. 

1. V levém navigačním panelu vyberte **zákazníky** a pak vyberte zákazníka, kterého přesouváte.
2. Na stránce s podrobnostmi předplatného nastavte původní předplatné na **pozastaveno** a vyberte **Odeslat** .

Staré předplatné je teď pozastavené a nové předplatné je aktivní. Pozastavený odběr bude po 120 dnech automaticky zřízen. Pro staré předplatné nepřijde váš zákazník žádné další poplatky.
