---
title: Použití souborů odsouhlasení
ms.topic: article
ms.date: 06/08/2020
description: Přečtěte si informace o souborech pro odsouhlasení v partnerském centru a o tom, jak interpretovat detailní zobrazení položek poplatků za daný fakturační cyklus.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 98bfd9a9ce6f03ad62a830f05ba82f9b90268326
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/22/2020
ms.locfileid: "92527318"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Přečtěte si, jak číst položky řádků v souborech odsouhlasení partnerského centra.

Platí pro:

- Partnerské centrum
- Partnerské centrum pro Microsoft Cloud pro státní správu USA

Soubory pro odsouhlasení si můžete stáhnout z partnerského centra, kde najdete podrobné zobrazení položek jednotlivých poplatků v rámci fakturačního cyklu. Podrobnosti o položkách na řádcích zahrnují poplatky za předplatné každého zákazníka a podrobné události (například přidání licencí do předplatného).

Příslušné role:

- Správce fakturace
- Globální správce

Informace o tom, jak si **fakturu** přečíst, najdete v tématu [Přečtěte si vyúčtování](read-your-bill.md).

## <a name="understand-reconciliation-file-fields"></a>Vysvětlení polí souboru odsouhlasení

- [Pole souboru odsouhlasení založeného na licencích](license-based-recon-files.md)
- [Pole souboru odsouhlasení založeného na využití](usage-based-recon-files.md)
- [Pole souborů odsouhlasení podle denního hodnocení využití](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Pochopení typů poplatků v souborech pro odsouhlasení

Chcete-li pochopit typy poplatků v souborech pro odsouhlasení (sloupec **ChargeType** ), podívejte se na téma [odsouhlasení typů poplatků za soubor](recon-file-charge-types.md).

## <a name="fix-formatting-issues"></a>Opravit problémy s formátováním

V některých případech může soubor pro odsouhlasení obsahovat problémy s formátováním. K tomuto problému může dojít například v případě, že se národní prostředí en-US nepoužívá.

Pomocí těchto kroků opravíte všechny problémy formátování souborů odsouhlasení:

1. Otevřete soubor pro odsouhlasení (ve formátu CSV) v aplikaci Microsoft Excel.
2. Vyberte první sloupec v souboru.
3. Otevřete **Průvodce převodem textu na sloupce** . Na pásu karet vyberte **data** a pak vyberte **text do sloupců** .
4. V průvodci vyberte **typ souboru s oddělovači** . Pak vyberte **Další** .
5. V poli **oddělovače** vyberte **čárka** . (Pokud je už vybraná **karta** , můžete tuto možnost nechat vybranou.) Pak vyberte **Další** .
6. V poli **Formát dat sloupce** vyberte **Datum: MDY** . Pak vyberte **Další** .
7. V poli **Formát dat sloupce** vyberte možnost **text** pro sloupce všech částek. Pak vyberte **Finish** (Dokončit).

## <a name="download-reconciliation-files-programmatically"></a>Stažení souborů pro odsouhlasení programově

Soubory pro odsouhlasení můžou být velmi velké a někdy je obtížné stáhnout. Chcete-li stáhnout soubory pro odsouhlasení programově, viz [získat řádky faktury](/partner-center/develop/get-invoiceline-items).

## <a name="map-taxes-or-vat"></a>Mapování daní nebo DPH

K namapování daně nebo daně z přidané hodnoty (DPH) na fakturu:

- Sečtěte sloupec **daně** ze souboru založeného na licencích.
- Sečtěte sloupec **TaxAmount** ze souboru založeného na využití.

## <a name="itemize-reconciliation-files-by-partner"></a>Soubory pro odsouhlasení itemize podle partnera

Partneři v **nepřímém modelu** můžou použít tato další pole v souborech pro odsouhlasení založené na licencích i na základě využití k itemizeí souborů podle prodejce.

| ID MPN | Popis |
| ------ | ----------- |
| ID MPN | Identifikátor Microsoft Partner Network (MPN) pro partnera poskytovatele Cloud Solution Provider (CSP) (přímý nebo nepřímý). |
| [ID MPN prodejce](#reseller-mpn-id) | [Identifikátor MPN prodejce záznamu pro předplatné](#reseller-mpn-id). Toto pole odpovídá ID prodejce uvedeného u konkrétního předplatného v partnerském centru. Zobrazí se pouze v souborech pro odsouhlasení pro partnery v nepřímém modelu. |

### <a name="reseller-mpn-id"></a>ID MPN prodejce

Pokud partner CSP prodal předplatné přímo zákazníkovi, jejich **ID MPN** se uvádí dvakrát, jak **ID MPN** , tak **ID programu MPN prodejce** .

Pokud má partner CSP prodejce bez **ID MPN** , tato hodnota se místo toho nastaví na **ID MPN** partnera.

Pokud partner CSP odebere ID programu **MPN pro prodejce** , tato hodnota se nastaví na hodnotu *-1* .

Zobrazení nebo aktualizace **ID MPN prodejce** :

1. Přihlaste se do Partnerského centra.
2. V nabídce partnerské Centrum vyberte **zákazníci** .
3. Vyberte zákazníka ze seznamu.
4. V nabídce zákazník vyberte **odběry** .
5. Vyberte předplatné ze seznamu.
6. Pokud chcete změnit **prodejce (MPN ID)** , vyberte **aktualizovat** .