---
title: Správa seznamu zákazníků
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Záznamy zákazníků patří mezi nejdůležitější informační prostředky. Zjistěte, jak zobrazit, hledat, aktualizovat & exportovat informace ze seznamu Partnerské centrum zákazníků.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6e73aa98e0cfaf82521a5fe63e34ebf0b44363fb
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854498"
---
# <a name="manage-your-customer-list---search-update-or-export-customers-in-partner-center"></a>Správa seznamu zákazníků – vyhledávání, aktualizace nebo export zákazníků v Partnerské centrum

**Platí pro**: Partnerské centrum | Partnerské centrum pro Microsoft Cloud for US Government

**Odpovídající role:** Agent pro správu | Globální správce

Záznamy zákazníků patří mezi nejdůležitější informační prostředky v Partnerské centrum. Můžete prohledávat databázi zákaznických účtů, exportovat celou databázi zákazníků nebo exportovat podmnožinu do formátu souboru s oddělovači kompatibilního s Excelem (CSV). Informace o předplatných zákazníka můžete také exportovat do souboru .csv.

Protokoly aktivit také poskytují exportovatelná data o transakcích a akcích správy pro zákazníky. Další informace najdete v tématu [Zobrazení protokolů aktivit zákazníků.](activity-logs.md)

## <a name="search-for-a-customer"></a>Vyhledání zákazníka

1. V **nabídce Partnerské centrum** vyberte **Zákazníci.**
2. Pokud chcete vyhledat zákazníka, zadejte do vyhledávacího pole jméno zákazníka nebo název domény.
3. Výběrem **šipky dolů** na konci řádku zákazníka zobrazíte jeho ID Microsoftu a přidružené rychlé odkazy na předplatná a služby.

## <a name="update-a-customers-company-name"></a>Aktualizace názvu společnosti zákazníka

V **nabídce Partnerské centrum** vyberte **Zákazníci.**
2. Pokud chcete vyhledat zákazníka, zadejte do vyhledávacího pole jméno zákazníka nebo název domény.
3. Výběrem **šipky dolů** na konci řádku zákazníka zobrazíte jeho ID Microsoftu a přidružené rychlé odkazy na předplatná a služby.
4. V části **Bill-to information (Vyúčtování)** zákazníka aktualizujte název společnosti. Když uložíte novou hodnotu, projeví se v seznamu zákazníků. Tím se změní jenom název faktury na společnost a hodnota seznamu zákazníků. Neprojeví se nikde jinde.

## <a name="export-your-customer-list"></a>Exportovat seznam zákazníků

1. V nabídce **Partnerské centrum** vyberte **zákazníci**.
2. Vyberte **exportovat zákazníky**.

   Partner Center převede úplný seznam zákazníků na soubor. csv a nahraje ho do výchozí složky pro stažení v počítači. Můžete také exportovat podmnožiny zákaznických dat. Mezi datové sloupce patří následující:

   - **ID Microsoftu**;
   - **Název společnosti**;
   - **Název primární domény**;
   - **Vztah**– obchodní vztah partnera ke každému uvedenému zákazníkovi.

    V partnerském centru se ve výchozím nastavení exportuje celý seznam zákazníků bez ohledu na jeho délku. Můžete také vyhledat seznam zákazníků podle názvu společnosti nebo domény a exportovat tuto podmnožinu dat.

3. Pokud jste nepřímý poskytovatel, můžete si seznam zákazníků filtrovat pomocí nepřímého prodejce. V seznamu vyberte **filtrovat podle nepřímý prodejce** a pak zvolte prodejce.


## <a name="export-customer-subscription-information"></a>Export informací o předplatném zákazníka

1. V nabídce **Partnerské centrum** vyberte **zákazníci**.

2. Vyberte **název společnosti** pro každého zákazníka. Otevře se stránka **Předplatná** zákazníka s úplným seznamem předplatných produktů.

3. Vyberte **Exportovat předplatná.** Partnerské centrum data předplatného zákazníka do souboru .csv a nahraje je do výchozí složky pro stahování ve vašem počítači. Mezi datové sloupce patří:
   - **ID předplatného;**
   - **Předplatné**– název produktu pro předplatné;
   - **Quantity**(Množství) – počet zakoupených licencí
   - **Stav;**
   - **Reseller**– ID prodejce, který vlastní a spravuje předplatné.

> [!NOTE]  
> Další informace o správě předplatných najdete v tématu [Předplatná zákazníků.](customer-subscriptions.md)
