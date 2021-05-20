---
title: Správa rezervací Azure pro zákazníky
description: Zjistěte, jak spravovat rezervace Azure pro zákazníka, včetně zrušení rezervace, výměny rezervace nebo žádosti o refundaci.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 1184b199d6235dd1d16fe981000bae44b797f76a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149481"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a>Správa, zrušení, výměna nebo refundace Microsoft Azure rezervací pro zákazníky

**Odpovídající role:** Agent pro správu | Globální správce | Agent helpdesku | Sales agent | Správce správy uživatelů

Tento článek vysvětluje, jak spravovat rezervace Azure pro zákazníka, včetně zrušení rezervace, výměny rezervace nebo žádosti o refundaci.

> [!NOTE]
> Tento článek se týká jenom partnerů v Cloud Solution Provider (CSP). Zákazníci, kteří používají jiné typy předplatných (například předplatná s platbami, jednotlivá předplatná, Smlouva se zákazníkem Microsoftu nebo předplatná smlouva Enterprise), by si místo toho měli přečíst tuto dokumentaci k [rezervacím Azure.](/azure/cost-management-billing/reservations)

Pokud chcete spravovat rezervace Azure zákazníků po nákupu, vyberete zákazníka a rezervaci, které chcete spravovat v Partnerské centrum, a pak v této Azure Portal.

1. Pokud chcete začít, **vyberte** v nabídce Partnerské centrum zákazníky a pak vyberte zákazníka, jehož rezervace chcete spravovat. 

2. V nabídce stránky podrobností zákazníka vyberte **Rezervace Azure** a pak vyberte konkrétní rezervaci, kterou chcete spravovat.  

3. V **části** Akce vyberte **Spravovat** a přejděte na záznam rezervace zákazníka v Azure Portal. Na stránce s podrobnostmi o rezervaci postupujte podle následujících kroků a dokončete úlohy.  

    | **Výběr**   | **Do**    |
    |:-----------------------------|:-----------------|
    | **Přehled**   | View details of a customer's reservation, including expiration date, scope, and utilization data. **POZNÁMKA:** Výběrem **možnosti** Refundace vytvořte žádost o podporu k poměrné refundaci. Pokud **chcete vytvořit** žádost o podporu a vyměnit nevyužitou část období rezervace, vyberte Exchange.  
    | **Access Control (IAM)**   | Správa přístupu k informacím o rezervacích zákazníka|
    | **Konfigurace**   | Změňte rozsah rezervace nebo předplatné Azure, ke které je rezervace přidružená.    |
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
|5 nebo méně                         | No          | 100 %       | No                              | $50 000 USD   |
|5 nebo méně                         | Yes         | Poměrná  | No                              | 50 000 USD   |
|Více než 5                        | No          | Poměrná  | 12 %                             | 50 000 USD   |
|Více než 5                        | Yes         | Poměrná  | 12 %                             | 50 000 USD   |

### <a name="how-exchanges-work"></a>Jak fungují výměny 

Pokud zákazník chce koupit jinou rezervaci, než kterou od vás původně koupil, může požádat o výměnu. Výměna rezervace může být atraktivní alternativou ke zrušení rezervace, protože umožňuje zákazníkovi využít poměrnou refundaci k ceně nové rezervace. 

Na váš účet se připsá částka refundace zaceněnou podle objemu peněz, abyste zákazníkovi mohli nabídnout výměnu.

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Žádost o refundaci nebo výměnu jménem zákazníka

Pokud chcete vytvořit žádost o podporu o refundaci nebo výměnu jménem vašich zákazníků, vyberete zákazníka a rezervaci v Partnerské centrum a pak vytvoříte žádost o podporu v Azure Portal. 

>[!NOTE]
>Podpora Microsoftu agenti vás mohou požádat o poskytnutí ID rezervace a ID objednávky rezervace. Tyto informace najdete na stránce Vlastností **rezervace** v Azure Portal.

1. Pokud chcete začít, **vyberte** v nabídce Partnerské centrum zákazníky a pak vyberte zákazníka, který chce refundaci. 

2. Na stránce podrobností zákazníka vyberte **Rezervace Azure** a pak vyberte konkrétní rezervaci, u které chce zákazník vrátit peníze.  

3. V **části** Actions (Akce) **vyberte Refundace,** abyste v seznamu Azure Portal zákazníka a zahájili žádost o podporu.  

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
|Nákup rezervací Azure pomocí rozhraní API partnerského centra | [Informace Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) najdete v dokumentaci Partnerské centrum pro vývojáře.   |
|Dáváte zákazníkům oprávnění k nákupu vlastních rezervací Azure z předplatného, které jste pro ně zakoupili. | [Udělit zákazníkům oprávnění k nákupu vlastních rezervací Azure](give-customers-permission.md)   |