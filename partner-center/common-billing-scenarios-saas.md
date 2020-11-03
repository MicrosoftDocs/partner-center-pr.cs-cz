---
title: Fakturace – SaaS transakce založené na licencích
ms.topic: article
ms.date: 05/05/2020
description: Přečtěte si o běžných scénářích fakturace v partnerském centru pro transakce založené na licencích a SaaS (software-as-a-Service).
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3d63e8345bf127cb91f1812193b1f0311cd569b3
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/14/2020
ms.locfileid: "92527681"
---
# <a name="common-billing-scenarios-for-license-based-saas-transactions-in-partner-center"></a>Běžné scénáře fakturace pro transakce SaaS založené na licencích v partnerském centru

**Příslušné role**

- Agent správce
- Správce fakturace
- Agent helpdesku
- Agent prodeje


Tyto příklady [běžných fakturačních scénářů](common-billing-scenarios.md) se vztahují na předplatné na základě licenčního softwaru jako služby (SaaS) v partnerském centru.

## <a name="convert-a-free-trial-saas-subscription-to-a-paid-subscription"></a>Převod bezplatného zkušebního předplatného SaaS na placené předplatné

Tento scénář popisuje fakturaci za obnovení předplatného bezplatné zkušební verze SaaS na základě licence. Obnovení na konci bezplatné zkušební doby převede bezplatnou zkušební verzi na placené předplatné.

V tomto příkladu jste si zakoupili bezplatnou zkušební verzi předplatného SaaS založeného na licencích (software jako služba) na 10. června. Tato bezplatná zkušební verze se po skončení bezplatné zkušební doby automaticky obnoví jako placené předplatné.

Soubory rekognoskaci budou zahrnovat následující poplatky:

| Datum nákupu | Počáteční datum platby | Koncové datum zpoplatnění | Jednotková cena | Množství jednotek | Total amount | Typ poplatku | Popis předplatného |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | $0 | 1 | $0 | Nová | Bezplatná zkušební verze |
| 07/10/2019 | 07/10/2019 | 08/09/2019 | $2 | 1 | $2 | Obnovit | Placené předplatné |

## <a name="cancel-a-free-trial-saas-subscription"></a>Zrušení bezplatného zkušebního předplatného SaaS

> [!TIP]
> Předplatné bezplatné zkušební verze SaaS na základě licence můžete kdykoli zrušit, a to i během bezplatné zkušební doby.

V tomto scénáři jste si zakoupili předplatné bezplatné zkušební verze SaaS na základě licencí od 1. července a pak ho okamžitě zrušili v partnerském centru.

Soubor rekognoskaci bude obsahovat následující poplatky:

| Datum nákupu | Počáteční datum platby | Koncové datum zpoplatnění | Jednotková cena | Množství jednotek | Total amount | Typ poplatku | Popis předplatného |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | $0 | 11 | $0 | Nová | Bezplatná zkušební verze |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | $0 | 11 | $0 | Zrušit | Bezplatná zkušební verze |

## <a name="convert-custom-meter-saas-subscription-to-another-sku"></a>Převod předplatného Custom měřič SaaS na jinou SKU

Tento scénář popisuje, jak převést vlastní předplatné měřiče SaaS z jedné skladové jednotky (SKU) na jinou SKLADOVOU položku pro stejný produkt ve stejném datu.

V tomto scénáři jste v rámci produktu zakoupili jednu skladovou jednotku (stříbrné) a převedli ji na jinou dostupnou SKU (bronz) v rámci tohoto produktu ve stejném datu.

Soubor rekognoskaci bude obsahovat následující poplatky:

| Datum nákupu | Skladová položka | Počáteční datum platby | Koncové datum zpoplatnění | Jednotková cena | Množství jednotek | Total amount | Typ poplatku | Popis předplatného |
| ------------- | ----------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Silver | 06/10/2019 | 06/10/2019 | $20 | 1 | $20 | Nová | Předplatné Custom měřič SaaS |
| 06/10/2019 | Silver | 06/10/2019 | 06/10/2019 | $20 | 1 | -$20 | Převést | Poměrné přeúčtování pro vlastní předplatné měřičů SaaS |
| 06/10/2019 | Bronzová | 06/10/2019 | 06/10/2019 | $10 | 1 | $10 | Převést | Předplatné Custom měřič SaaS |

## <a name="purchase-and-cancel-a-customer-meter-saas-subscription-on-same-date"></a>Nákup a zrušení předplatného měření zákazníka SaaS ve stejném datu

Tento scénář popisuje fakturaci pro předplatné měřiče zákazníka, které jste zakoupili a zrušili prostřednictvím Azure Portal ve stejné datum.

V tomto scénáři jste si zakoupili vlastní předplatné měření SaaS na Azure Portal. Pak jste zrušili předplatné na stejné datum.

| Datum nákupu | Skladová položka | Počáteční datum platby | Koncové datum zpoplatnění | Jednotková cena | Množství jednotek | Total amount | Typ poplatku | Popis předplatného |
| ------------- | ------------- |----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Bronzová | 06/10/2019 | 06/10/2019 | $10 | 1 | $10 | Nová | Předplatné Custom měřič SaaS |
| 06/10/2019 | Bronzová | 06/10/2019 | 06/10/2019 | $10 | 1 | -$10 | CancelImmediate | Předplatné Custom měřič SaaS |
