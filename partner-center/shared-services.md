---
title: Přidání Azure Partner Shared Services
description: Využijte Azure Partner Shared Services k nákupu předplatných Azure pro vlastní použití a jednotnou metodu nákupu, sledování a správy Azure.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: ffec50d53b50bdb6aa2690f1dfcc1bc7312cc3cb
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277296"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>Přidání Azure Partner Shared Services, aby si partneři mohli koupit předplatná Azure pro vlastní použití

**Odpovídající role:** Globální správce | Agent pro správu | Agent prodeje

Azure Partner Shared Services je nový typ nabídky pro partnery v programu CSP, který umožňuje partnerům nakupovat předplatná Azure pro vlastní použití.Kromě možnosti konsolidovat své licenční smlouvy a smlouvy o prodeji v Azure s Microsoftem dává partnerům příležitost používat jednotnou metodu nákupu, sledování a správy Azure. Díky Azure Partner Shared Services mají teď partneři stejnou flexibilitu při používání předplatných Azure v CSP jako v programech Microsoft smlouva Enterprise a Web Direct, a otevírají tak scénáře, jako jsou: vytváření vývojových a testovacích prostředí, nasazování interních úloh a hostování sdílených služeb nebo aplikací s více tenanty.  

## <a name="create-the-shared-services-tenant"></a>Vytvoření tenanta sdílených služeb

1. Přejděte na **Nastavení**  >  **Nastavení účtu Sdílené**  >  **služby**.

   :::image type="content" source="images/sharedservices2.png" alt-text="Nastavení účtu > sdílené služby":::

2. Pokud ještě tenanta sdílených služeb nemáte, klikněte na **Vytvořit sdílené služby.**

   :::image type="content" source="images/sharedservices3.png" alt-text="Vytvořte sdílené služby.":::

3. Tím se vytvoří tenant sdílených služeb a zakoupí se Azure CSP sdílené služby, které se použije pro sdílené prostředky a interní úlohy.

   :::image type="content" source="images/sharedservices5.png" alt-text="Vytvořte tenanta a zakupte předplatné.":::

## <a name="about-the-azure--internalshared-services-offer"></a>Informace o Azure - Internal/Shared Services nabídce

- Předplatné Azure - Internal/Shared Services nový typ nabídky Azure v PROGRAMU CSP, ke Partnerské centrum který partneři používají pro vlastní použití Azure.

- Azure Partner Shared Services předplatná jsou oprávněná a je možné ji použít k nákupu rozhraní RI.

- Nabídku Azure - Internal/Shared Services použít pouze na tenanta sdílených služeb.

- Primárním použitím předplatného Azure - Internal/Shared Services je, abyste mohli Azure používat pro vlastní účely vývoje. Sdílený tenant, který použijete ke zřízení této nabídky, se nemůže používat pro jiné služby, jako jsou licence Office 365 nebo Dynamics.

- Předplatné můžete zrušit stejně jako jakékoli jiné předplatné. Přejděte do **nastavení,**  >  **Zobrazit vše sdílené**  >  **služby**. Vyberte předplatné Azure - Internal/Shared Services a zrušte ho.

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Přístup Azure Partner Shared Services podrobnostem o spotřebě

Spotřebu Azure najdete na faktuře CSP a v souboru s vyrovnáním. Bude zahrnut jako součást Microsoft Azure položky na faktuře. Podrobné informace o spotřebě budou k dispozici v souboru s vyrovnáním zaznamenaného v tenantovi vytvořeném pro tuto nabídku.

## <a name="azure-partner-shared-services-pricing"></a>Azure Partner Shared Services ceny

Pokud chcete zobrazit nový soubor s cenami pro Azure Partner Shared Services, přejděte na **Sell**  >  **Pricing and offers (Prodejní** ceny a nabídky) a vyberte ceník pro aktuální měsíc. V nadcházejících týdnech bude také vydáno rozhraní API konkrétní karty sazeb.

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Nabídky a Azure Partner Shared Services Marketplace

Od 1. března 2019 Azure Partner Shared Services (APSS) už nepodporuje nabídky Marketplace.

|**Podpora Marketplace**   |**Podpora APSS před 1. březnem 2019**|**Po 1. březnu 2019**|
|---------------------------|:----------------------------|:-------------------|
|Použití vlastní licence (BYOL) a bezplatných služeb   | Yes   | No|
|Další nabídky třetích stran na marketplace   | No   |No|

Na partnery, kteří mají nasazené služby BYOL nebo bezplatné služby nasazené pomocí APSS, to nebude mít vliv. po 1. březnu 2019 ale nebudou moct nakupovat nové služby BYOL ani bezplatné služby.

Pokud chcete využít výhod plného katalogu dostupných nabídek Marketplace (nejen služeb BYOL a bezplatných služeb), doporučujeme partnerům CSP nasadit sdílené služby pomocí webových přímých předplatných Azure.  Partnerům CSP, kteří už dříve nasadili prostředky byOL a bezplatné služby třetích stran z Marketplace a chtějí je dál používat a nasazovat další nabídky třetích stran, se doporučuje migrovat předplatné APSS na web přímou migraci stávajících předplatných [Azure.](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)

Partneři, kteří po 1. březnu 2019 plánují dál používat předplatné APSS a chtějí nasadit nové služby [byOL](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) nebo bezplatné služby třetích stran, mohou postupovat podle pokynů od isvů a nasadit je do svých předplatných APSS.

## <a name="next-steps"></a>Další kroky

- [Prodej softwarových předplatných prostřednictvím CSP](csp-software-subscriptions.md)