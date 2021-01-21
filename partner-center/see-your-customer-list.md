---
title: Správa seznamu zákazníků
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Záznamy zákazníků jsou mezi nejdůležitějšími informačními prostředky. Naučte se zobrazovat, Hledat, aktualizovat & informace o exportu v seznamu zákazníků partnerského centra.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 40df034e88a1bba7829d6f73e0fb970795a2a0dd
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 08/05/2020
ms.locfileid: "92527139"
---
# <a name="manage-your-customer-list---search-update-or-export-customers-in-partner-center"></a>Správa seznamu zákazníků – hledání, aktualizace nebo export zákazníků v partnerském centru

**Platí pro**

- Partnerské centrum
- Partnerské centrum pro Microsoft Cloud pro státní správu USA

Záznamy zákazníků jsou mezi nejdůležitějšími informačními prostředky v partnerském centru. Můžete hledat v databázi zákaznických účtů, exportovat celou zákaznickou databázi nebo exportovat podmnožinu, do formátu souboru hodnot oddělených čárkami (. csv) kompatibilním s Excelem. Informace o předplatných zákazníka taky můžete exportovat do souboru. csv.

Protokoly aktivit také poskytují exportovaná data o transakcích a akcích správy pro zákazníky. Další informace najdete v tématu [zobrazení protokolů aktivit zákazníků](activity-logs.md).

## <a name="search-for-a-customer"></a>Hledání zákazníka

1.  V nabídce **Partnerské centrum** vyberte **zákazníci**.
2.  Pokud chcete hledat zákazníka, zadejte do vyhledávacího pole název zákazníka nebo název domény.
3.  Vyberte **šipku dolů** na konci řádku zákazníka, abyste viděli své ID Microsoftu a jejich přidružené a rychlé odkazy na odběry a služby.

## <a name="update-a-customers-company-name"></a>Aktualizace názvu společnosti zákazníka

V nabídce **Partnerské centrum** vyberte **zákazníci**.
2.  Pokud chcete hledat zákazníka, zadejte do vyhledávacího pole název zákazníka nebo název domény.
3.  Vyberte **šipku dolů** na konci řádku zákazníka, abyste viděli své ID Microsoftu a jejich přidružené a rychlé odkazy na odběry a služby.
4.  V části informace o **fakturaci** zákazníka aktualizujte název společnosti. Když uložíte novou hodnotu, projeví se v seznamu zákazníků. Tím se změní jenom název faktury na společnost a hodnota seznamu zákazníků. Neprojeví se nikde jinde.

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

2. Vyberte **název společnosti** pro každého zákazníka. Otevře se stránka **předplatná** zákazníka se zobrazeným úplným seznamem předplatných produktů.

3. Vyberte **exportovat odběry**. Partner Center převede data předplatného zákazníka na soubor. csv a nahraje ho do výchozí složky pro stažení v počítači. Mezi datové sloupce patří následující:
   - **ID předplatného**;
   - **Předplatné**– název produktu pro předplatné;
   - **Množství**– počet zakoupených licencí;
   - **Stav**;
   - **Prodejce**– ID prodejce, který vlastní a spravuje předplatné.

> [!NOTE]  
> Další informace o správě předplatného najdete v tématu [předplatné zákazníka](customer-subscriptions.md).
