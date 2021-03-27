---
title: Použití souborů odsouhlasení
ms.topic: article
ms.date: 03/26/2021
description: Přečtěte si informace o souborech pro odsouhlasení v partnerském centru a o tom, jak interpretovat detailní zobrazení položek poplatků za daný fakturační cyklus.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4a6a1455304f12e364d71e666cbd548821f8be55
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633892"
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

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a>Pokud soubor překračuje limit řádků v aplikaci Excel

Pokud si můžete stáhnout soubor pro odsouhlasení, ale nemůžete ho otevřít v Microsoft Excelu, pravděpodobně to znamená, že soubor obsahuje více řádků, než je Excel bude možné použít. Pokud k tomu dojde, můžete použít kterýkoli z následujících postupů k otevření souboru.

### <a name="open-a-recon-file-in-power-bi"></a>Otevřete soubor rekognoskaci v Power BI

1. Stáhněte soubor pro odsouhlasení obvyklým způsobem.
2. Stáhněte, nainstalujte a otevřete instanci Power BI.
3. Na kartě Power BI **Domů** vyberte **získat data**.
4. V seznamu **běžných zdrojů dat** vyberte **text/CSV**.
5. Po zobrazení výzvy otevřete soubor rekognoskaci.

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a>Otevření souboru rekognoskaci v kontingenční tabulce aplikace Excel

1. Stáhněte soubor pro odsouhlasení obvyklým způsobem.
2. Otevřete nový soubor v aplikaci Microsoft Excel.
3. Na kartě **data** vyberte **získat data**, vyberte **ze souboru** a pak vyberte **text/CSV**.
4. Po zobrazení výzvy otevřete soubor rekognoskaci. Vaše data se zobrazí.
5. V rozevírací nabídce **načíst** vyberte **načíst do** a pak **OK**.
6. V dialogovém okně **importovat data** vyberte **sestavu kontingenční tabulka** a otevřete soubor.

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