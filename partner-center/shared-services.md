---
title: Přidat služby Azure partner Shared Services
description: Využijte Azure partner Shared Services k nákupu předplatných Azure pro vaše vlastní použití a k zajištění jednotné metody pro nákup, sledování a správu Azure.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: a59cf0b271a0ccf5fd5a1d8e3e85ff43818a3801
ms.sourcegitcommit: fe867be44de3479607be3309940b904d7ea9fc6e
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/06/2021
ms.locfileid: "102247708"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>Přidejte služby Azure partner Shared Services, aby partneři mohli koupit předplatné Azure pro vlastní použití.

 
**Příslušné role**

- Globální správce
- Agent správce
- Agent prodeje

Azure partner Shared Services je nový typ nabídky pro partnery v programu CSP, který umožňuje partnerům zakoupit si předplatné Azure pro vlastní použití.Vytvoří příležitost pro partnery, aby používali jednotnou metodu pro nákup, sledování a správu Azure společně s možností konsolidovat své licence na Azure a prodávat smlouvy s Microsoftem. U partnerských sdílených služeb Azure teď mají partneři stejnou flexibilitu při používání předplatných Azure ve zprostředkovateli CSP, protože jsou v aplikacích Microsoft smlouva Enterprise a web Direct, otevírá scénáře jako: vývoj a testovací prostředí, nasazují interní úlohy a hostuje sdílené služby nebo víceklientské aplikace.  

## <a name="create-the-shared-services-tenant"></a>Vytvoření tenanta sdílených služeb

1. Přejít na **Nastavení** nastavení  >  **účtu**  >  **sdílené služby**.

   :::image type="content" source="images/sharedservices2.png" alt-text="Nastavení účtu > sdílené služby":::

2. Pokud ještě nemáte tenanta sdílených služeb, klikněte na **vytvořit sdílené služby**.

   :::image type="content" source="images/sharedservices3.png" alt-text="Vytváření sdílených služeb":::

3. Tím se vytvoří tenant sdílených služeb a nakupují předplatné Azure CSP Shared Services, které se bude používat pro sdílené prostředky a interní úlohy.

   :::image type="content" source="images/sharedservices5.png" alt-text="Vytvoření tenanta a zakoupení předplatného":::

## <a name="about-the-azure--internalshared-services-offer"></a>O nabídce Azure-Internal/Shared Services

- Azure-Internal/Shared Services předplatné je nový typ nabídky Azure ve zprostředkovateli CSP, ke kterému se přistupoval prostřednictvím partnerského centra, které partneři získají k vlastnímu používání Azure.

- Předplatné Azure partner Shared Services má nárok a dá se použít k zakoupení služeb vzdálené instalace.

- Nabídku Azure-Internal/Shared Services lze použít pouze pro tenanta sdílených služeb.

- Primárním využitím předplatného Azure-Internal/Shared Services je, abyste mohli Azure používat pro vlastní účely vývoje. Sdílený tenant, který použijete k zřízení této nabídky, se nedá použít pro jiné služby, jako jsou licence na Office 365 nebo Dynamics.

- Předplatné můžete zrušit stejně jako jakékoli jiné předplatné. Přejít na **Nastavení**  >  **Zobrazit všechna nastavení**  >  **sdílené služby**. Vyberte předplatné Azure-Internal/Shared Services a zrušte ho.

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Přístup k podrobnostem o spotřebě Azure partner Shared Services

Na faktuře CSP a souboru pro odsouhlasení najdete spotřebu Azure. Bude obsažena jako součást Microsoft Azure položky řádku na faktuře. Podrobné informace o spotřebě budou k dispozici v souboru pro odsouhlasení s klientem vytvořeným pro tuto nabídku.

## <a name="azure-partner-shared-services-pricing"></a>Ceny za službu Azure partner Shared Services

Pokud chcete zobrazit nový soubor s cenami pro Azure partner Shared Services, přejděte na **prodej**  >  **ceny a nabídky** a vyberte ceník aktuální měsíc. V nadcházejících týdnech se uvolní také rozhraní API pro specifickou míru karet.

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Nabídky Marketplace a služby Azure partner Shared Services

Od 1. března 2019 již Azure partner Shared Services (APSS) už nepodporuje nabídky na webu Marketplace.

|**Podpora Marketplace**   |**APSS se podporuje do 1. března 2019**|**Od 1. března 2019**|
|---------------------------|:----------------------------|:-------------------|
|Přineste si vlastní licenci (BYOL) a bezplatné služby   | Ano   | Ne|
|Další nabídky na webu Marketplace třetích stran   | Ne   |Ne|

Partneři, kteří mají BYOL nebo bezplatné služby nasazené pomocí APSS, nebudou ovlivněny. od 1. března 2019 ale nebude moct koupit nové BYOL nebo bezplatné služby.

Aby bylo možné využít kompletní katalog nabízených nabídek Marketplace (ne jenom BYOL a bezplatné služby), doporučujeme, aby partneři CSP nasadili sdílené služby s použitím předplatných Azure web Direct.  Partneři CSP, kteří už dříve nasadili BYOL a bezplatné prostředky služeb z webu Marketplace a chtějí je dál používat a nasazovat další nabídky třetích stran, se doporučuje migrovat předplatné APSS na web přímo [migrací stávajících předplatných Azure](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).

Partneři, kteří plánují i nadále používat předplatné APSS po 1. březnu 2019 a chtějí nasadit nové [služby BYOL](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) třetích stran nebo bezplatné služby, můžou podle pokynů od nezávislých výrobců softwaru tyto informace nasadit do svých předplatných APSS.

## <a name="next-steps"></a>Další kroky

- [Prodej softwarových předplatných prostřednictvím CSP](csp-software-subscriptions.md)