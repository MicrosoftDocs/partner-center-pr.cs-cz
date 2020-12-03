---
title: Správa rezervací Azure pro zákazníky
description: Naučte se spravovat rezervace Azure pro zákazníka, včetně toho, jak zrušit rezervaci, vyměnit rezervaci nebo požádat o refundaci.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: c377fca3e38161258c836d14202ac4db21484526
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534756"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a>Správa, zrušení, výměna nebo refundace Microsoft Azure rezervacích pro zákazníky

**Příslušné role**

- Agent správce
- Globální správce
- Agent helpdesku
- Agent prodeje
- Správce správy uživatelů

Tento článek vysvětluje, jak spravovat rezervace Azure pro zákazníka, včetně toho, jak zrušit rezervaci, vyměnit rezervaci nebo požádat o refundaci.

> [!NOTE]
> Tento článek se týká jenom partnerů v programu Cloud Solution Provider (CSP). [Tuto dokumentaci k rezervacím Azure](/azure/cost-management-billing/reservations)by si měli přečíst zákazníci, kteří používají jiné typy předplatných (například, platby na základě průběžných plateb, jednotlivce, smlouvy o zákaznících Microsoftu nebo předplatná smlouva Enterprise).

Pokud chcete spravovat rezervace Azure pro zákazníky po nákupu, vyberte zákazníka a rezervaci, které chcete spravovat v partnerském centru, a pak v Azure Portal proveďte změny rezervace.

1. Začněte tím, že v nabídce partnerského centra vyberete **zákazníci** a pak vyberete zákazníka, jehož rezervace chcete spravovat. 

2. V nabídce Stránka podrobností zákazníka vyberte **rezervace Azure** a pak vyberte konkrétní rezervaci, kterou chcete spravovat.  

3. V části **Akce** vyberte **Spravovat** , pokud chcete přejít na záznam o rezervacích zákazníka v Azure Portal. Na stránce s podrobnostmi o rezervacích dokončete úlohy podle následujících kroků.  

    | **Výběr**   | **Schopn**    |
    |:-----------------------------|:-----------------|
    | **Přehled**   | Zobrazení podrobností o rezervacích zákazníka, včetně data vypršení platnosti, rozsahu a dat o využití **Poznámka:** Vyberte **refundaci** a vytvořte žádost o podporu s hodnocením pro nominální částku. Pokud chcete vytvořit žádost o podporu pro výměnu nevyužité části podmínky rezervace, vyberte **Exchange** .  
    | **Access Control (IAM)**   | Spravujte přístup k informacím o rezervacích zákazníka.|
    | **Konfigurace**   | Změňte rozsah rezervace nebo předplatné Azure, ke kterému je rezervace přidružená.    |
    | **Vlastnosti**   | Zobrazení vlastností rezervace a zkopírování do schránky ID rezervace a ID objednávky rezervace. **Poznámka:** Pokud požadujete podporu jménem zákazníka, může vám podpora vyžadovat ID rezervace a ID objednávky rezervace.    |
    | **Nová žádost o podporu**    | Požádat o požádejte o podporu od podpora Microsoftu.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Zrušení nebo výměna rezervace

Pokud se změní obchodní potřeby zákazníka v jakémkoli okamžiku, může chtít zrušit rezervaci a získat refundaci nebo vyměňovat částku za poměrnou refundaci rezervace, která se má použít k ceně nové rezervace.

V obou těchto scénářích vám Microsoft refundace za vás, takže můžete spravovat výsledné finanční transakce se zákazníky. Společnost Microsoft nekontaktuje zákazníky přímo o fakturaci, zrušení a refundaci.

### <a name="how-cancellations-work"></a>Jak ruší zrušení práce

Zákazníci si můžou kdykoliv požádat, aby rezervaci zrušili (částka refundace se omezené na $50 000 za rok). Zrušením rezervace umožníte zákazníkovi vracet množství zbývajících měsíců k rezervaci Azure za poplatek za předčasné ukončení. Zbývající poměrný zůstatek minus poplatek za předčasné ukončení se vrátí na váš účet, abyste mohli vrátit účet zákazníka. 

Podrobnosti zrušení a poplatky najdete níže.


|**Datum zrušení**<br> denní   |**Použití**    |**Kredit**  |**Předčasné ukončení**<br> vyjádřen    |**Limit refundace** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 nebo méně                         | Ne          | 100 %       | Ne                              | $50 000 USD   |
|5 nebo méně                         | Ano         | Pro-hodnocené  | Ne                              | $50 000 USD   |
|Více než 5                        | Ne          | Pro-hodnocené  | 12 %                             | $50 000 USD   |
|Více než 5                        | Ano         | Pro-hodnocené  | 12 %                             | $50 000 USD   |

### <a name="how-exchanges-work"></a>Jak fungují funkce Exchange 

Pokud chce zákazník koupit jinou rezervaci, než kterou si původně koupili, může požádat o výměnu. Výměna rezervace může být zajímavou alternativou ke zrušení rezervace, protože umožňuje zákazníkovi použít částku poměrné refundace směrem k ceně nové rezervace. 

Částka průběžné refundace se účtuje na váš účet, abyste mohli zákazníka nabídnout na Exchangi.

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Požádat o refundaci nebo výměnu jménem zákazníka

Pokud chcete pokládat žádost o podporu pro refundaci nebo výměnu za vaše zákazníky, vyberte zákazníka a rezervaci v partnerském centru a pak vytvořte žádost o podporu v Azure Portal. 

>[!NOTE]
>Agenti podpora Microsoftu vás můžou požádat, abyste zadali ID rezervace a ID objednávky rezervace. Tyto informace najdete na stránce **vlastností** rezervace v Azure Portal.

1. Začněte tím, že v nabídce partnerského centra vyberete **zákazníci** a pak vyberete zákazníka, který požaduje refundaci. 

2. Na stránce s podrobnostmi zákazníka vyberte **rezervace Azure** a pak vyberte konkrétní rezervaci, kterou chce zákazník znovu vyfinancovat.  

3. V části **Akce** vyberte **refundace** , pokud chcete přejít na záznam o rezervacích zákazníka v Azure Portal a zahájit žádost o podporu.  

4. Na stránce **Nová žádost o podporu** postupujte podle následujících kroků a vyžádejte si refundaci. Po každém kroku vyberte **Další** . 

   |**Krok**                    |**Zvolené**    |
   |:---------------------------|:-----------------|
   |**1 Základy**                |Typ problému: fakturace  |
   |**2 problém**               |Typ problému: Správa rezervace Kategorie: výměn a refundace. |
   |**3 kontaktní informace**   |Vyberte Předvolby a zadejte požadované informace. 

5. Po dokončení vyberte **vytvořit** .

## <a name="azure-reservations-resources"></a>Prostředky rezervací Azure

|**Pro informace o**   |**Přečtěte si:**    |
|:-----------------------------|:-----------------|
|Přehled rezervací Azure v CSP  | [Prodej rezervovaných instancí Microsoft Azure](azure-reservations.md) |
|Nákup rezervací Azure pro vaše zákazníky v partnerském centru   | [Nákup rezervací Azure](azure-reservations-buying.md) |
|Určení správné velikosti virtuálního počítače a ověření využití virtuálního počítače zákazník   | [Změna velikosti virtuálního počítače pro maximální využití rezervace Azure](azure-usage.md)   |
|Nákup rezervací Azure pomocí rozhraní API partnerského centra | [Koupit Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) v dokumentaci pro vývojáře partnerského centra   |
|Udělení oprávnění zákazníkům k nákupu svých rezervací Azure z předplatného, které pro ně jste nakoupili. | [Poskytněte zákazníkům oprávnění k nákupu svých rezervací Azure.](give-customers-permission.md)   |