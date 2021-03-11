---
title: Použití souborů odsouhlasení
ms.topic: article
ms.date: 03/10/2021
description: Přečtěte si informace o souborech pro odsouhlasení v partnerském centru a o tom, jak interpretovat detailní zobrazení položek poplatků za daný fakturační cyklus.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e6b9e466402d71c988729052bd72ba2346a9d977
ms.sourcegitcommit: 868f90c54f26a037eee29749c207a7316bb4b475
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/11/2021
ms.locfileid: "103022770"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Přečtěte si, jak číst položky řádků v souborech odsouhlasení partnerského centra.

**Příslušné role**

- Správce fakturace
- Globální správce

Soubory pro odsouhlasení si můžete stáhnout z partnerského centra, kde najdete podrobné zobrazení položek jednotlivých poplatků v rámci fakturačního cyklu. Podrobnosti o položkách na řádcích zahrnují poplatky za předplatné každého zákazníka a podrobné události (například přidání licencí do předplatného).

Informace o tom, jak si **fakturu** přečíst, najdete v tématu [Přečtěte si vyúčtování](read-your-bill.md).

## <a name="understand-reconciliation-file-fields"></a>Vysvětlení polí souboru odsouhlasení

- [Pole v souboru s vyrovnáním na základě licencí](license-based-recon-files.md)
- [Pole v souboru s vyrovnáním na základě využití](usage-based-recon-files.md)
- [Pole v souboru s vyrovnáním využití podle denní sazby](daily-rated-usage-recon-files.md)
- [Pole souborů odsouhlasení zprostředkovatele CSP v jednom čase](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Pochopení typů poplatků v souborech pro odsouhlasení

Chcete-li pochopit typy poplatků v souborech pro odsouhlasení (sloupec **ChargeType** ), podívejte se na téma [odsouhlasení typů poplatků za soubor](recon-file-charge-types.md).

## <a name="fix-formatting-issues"></a>Opravit problémy s formátováním

V některých případech může soubor pro odsouhlasení obsahovat problémy s formátováním. K tomuto problému může dojít například v případě, že se národní prostředí en-US nepoužívá.

Pomocí těchto kroků opravíte všechny problémy formátování souborů odsouhlasení:

1. Otevřete soubor pro odsouhlasení (ve formátu CSV) v aplikaci Microsoft Excel.
2. Vyberte první sloupec v souboru.
3. Otevřete **Průvodce převodem textu na sloupce**. Na pásu karet vyberte **data** a pak vyberte **text do sloupců**.
4. V průvodci vyberte **typ souboru s oddělovači**. Pak vyberte **Další**.
5. V poli **oddělovače** vyberte **čárka**. (Pokud je už vybraná **karta** , můžete tuto možnost nechat vybranou.) Pak vyberte **Další**.
6. V poli **Formát dat sloupce** vyberte **Datum: MDY**. Pak vyberte **Další**.
7. V poli **Formát dat sloupce** vyberte možnost **text** pro sloupce všech částek. Pak vyberte **Finish** (Dokončit).

## <a name="download-reconciliation-files-programmatically"></a>Stažení souborů pro odsouhlasení programově

Soubory pro odsouhlasení můžou být velmi velké a někdy je obtížné stáhnout. Chcete-li stáhnout soubory pro odsouhlasení programově, viz [získat řádky faktury](/partner-center/develop/get-invoiceline-items).

## <a name="map-taxes-or-vat"></a>Mapování daní nebo DPH

K namapování daně nebo daně z přidané hodnoty (DPH) na fakturu:

- Sečtěte sloupec **daně** ze souboru založeného na licencích.
- Sečtěte sloupec **TaxAmount** ze souboru založeného na využití.

## <a name="itemize-reconciliation-files-by-partner"></a>Soubory pro odsouhlasení itemize podle partnera

Partneři v **nepřímém modelu** můžou použít tato další pole v souborech pro odsouhlasení založené na licencích i na základě využití k itemizeí souborů podle prodejce.

| ID MPN | Description |
| ------ | ----------- |
| ID MPN | Identifikátor Microsoft Partner Network (MPN) pro partnera poskytovatele Cloud Solution Provider (CSP) (přímý nebo nepřímý). |
| [ID MPN prodejce](#reseller-mpn-id) | [Identifikátor MPN prodejce záznamu pro předplatné](#reseller-mpn-id). Toto pole odpovídá ID prodejce uvedeného u konkrétního předplatného v partnerském centru. Zobrazí se pouze v souborech pro odsouhlasení pro partnery v nepřímém modelu. |

### <a name="reseller-mpn-id"></a>ID MPN prodejce

Pokud partner CSP prodal předplatné přímo zákazníkovi, jejich **ID MPN** se uvádí dvakrát, jak **ID MPN** , tak **ID programu MPN prodejce**.

Pokud má partner CSP prodejce bez **ID MPN**, tato hodnota se místo toho nastaví na **ID MPN** partnera.

Pokud partner CSP odebere ID programu **MPN pro prodejce**, tato hodnota se nastaví na hodnotu *-1*.

Zobrazení nebo aktualizace **ID MPN prodejce**:

1. Přihlaste se do Partnerského centra.
2. V nabídce partnerské Centrum vyberte **zákazníci**.
3. Vyberte zákazníka ze seznamu.
4. V nabídce zákazník vyberte **odběry**.
5. Vyberte předplatné ze seznamu.
6. Pokud chcete změnit **prodejce (MPN ID)**, vyberte **aktualizovat** .

## <a name="next-steps"></a>Další kroky

- [Postup čtení souboru rekognoskaci vy& účtování](read-your-bill.md) 