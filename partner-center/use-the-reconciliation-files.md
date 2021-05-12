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
ms.openlocfilehash: 755881d0bd96b9d601346ebb6271bd524c31d0a3
ms.sourcegitcommit: 837d3c5b52ab056b2b761cd85eb2426f56b62614
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/12/2021
ms.locfileid: "109794951"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Přečtěte si, jak číst položky řádků v souborech odsouhlasení partnerského centra.

**Příslušné role**: správce fakturace | Globální správce

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
4. V průvodci vyberte **typ souboru s oddělovači**. Pak vyberte **Další.**
5. V **poli Oddělovače** vyberte **Čárka**. (Pokud **je už** vybraná karta Tabulátor, můžete tuto možnost ponechat vybranou.) Pak vyberte **Další.**
6. V **poli Formát dat sloupce** vyberte **Date:MDY**. Pak vyberte **Další.**
7. V poli **Formát dat sloupce** vyberte Text **pro** všechny sloupce s množstvím dat. Pak vyberte **Finish** (Dokončit).

## <a name="download-reconciliation-files-programmatically"></a>Stažení souborů s vyrovnáním prostřednictvím kódu programu

Soubory pro sesouhlasení mohou být velmi velké a někdy se obtížně stahují. Pokud chcete stáhnout soubory s vyrovnáním prostřednictvím kódu programu, podívejte se [na stránku Získání řádových položek faktury.](/partner-center/develop/get-invoiceline-items)

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a>Pokud váš soubor překročí limit řádku v Excelu

Pokud si můžete stáhnout soubor s vyrovnáním, ale v Microsoft Excelu ho neotevřete, pravděpodobně to znamená, že soubor obsahuje více řádků, než Excel povolí. Pokud k tomu dojde, můžete soubor otevřít pomocí jednoho z následujících postupů.

### <a name="open-a-recon-file-in-power-bi"></a>Otevřete soubor odsoustavy v Power BI

1. Stáhněte si soubor s vyrovnáním běžným způsobem.
2. Stáhněte, nainstalujte a otevřete instanci Power BI.
3. Na Power BI **Domů** vyberte Získat **data**.
4. V seznamu **Běžných zdrojů dat** vyberte **Text/CSV.**
5. Po zobrazení výzvy otevřete soubor odsoustavy.

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a>Otevření souboru s rekonsekcemi v excelové kontingenční tabulce

1. Stáhněte si soubor s vyrovnáním běžným způsobem.
2. Otevřete nový soubor v aplikaci Microsoft Excel.
3. Na kartě **data** vyberte **získat data**, vyberte **ze souboru** a pak vyberte **text/CSV**.
4. Po zobrazení výzvy otevřete soubor rekognoskaci. Vaše data se zobrazí.
5. V rozevírací nabídce **načíst** vyberte **načíst do** a pak **OK**.
6. V dialogovém okně **importovat data** vyberte **sestavu kontingenční tabulka** a otevřete soubor.

## <a name="negative-amount-displayed"></a>Zobrazená záporná částka

V souboru pro odsouhlasení se může zobrazit záporná částka. Pravděpodobně to má jednu z následujících příčin:

- Nedávno jste zrušili nebo snížili počet licencí.
- Dostali jste kredit pro licenční smlouvu o úrovni služeb (SLA) nebo pro využití Azure.

Pokud chcete o této transakci získat další informace, zkontrolujte v souboru s vyrovnáním příslušný atribut typu poplatku.

## <a name="map-taxes-or-vat"></a>Mapování daní nebo DPH

K namapování daně nebo daně z přidané hodnoty (DPH) na fakturu:

- Sečtěte sloupec **daně** ze souboru založeného na licencích.
- Sečtěte sloupec **TaxAmount** ze souboru založeného na využití.

## <a name="itemize-reconciliation-files-by-partner"></a>Soubory pro odsouhlasení itemize podle partnera

Partneři v **nepřímém modelu** můžou použít tato další pole v souborech pro odsouhlasení založené na licencích i na základě využití k itemizeí souborů podle prodejce.

| ID MPN | Description |
| ------ | ----------- |
| ID MPN | Identifikátor Microsoft Partner Network (MPN) pro partnera poskytovatele Cloud Solution Provider (CSP) (přímý nebo nepřímý). |
| [ID MPN prodejce](#reseller-mpn-id) | [Identifikátor MPN prodejce záznamu pro předplatné](#reseller-mpn-id). Toto pole odpovídá ID prodejce uvedeného u konkrétního předplatného v partnerském centru. Zobrazuje se jenom v souborech s vyrovnáním pro partnery v nepřímém modelu. |

### <a name="reseller-mpn-id"></a>ID MPN prodejce

Pokud partner CSP prodá předplatné přímo zákazníkovi, jeho **ID MPN** se vyjádřuje dvakrát jako **ID MPN** i **ID MPN prodejce**.

Pokud má partner CSP prodejce bez **ID MPN,** nastaví se tato hodnota místo toho na **ID MPN** partnera.

Pokud partner CSP odebere **ID MPN** prodejce, tato hodnota se nastaví *na -1.*

Zobrazení nebo aktualizace **ID MPN prodejce:**

1. Přihlaste se do Partnerského centra.
2. V nabídce Partnerské centrum vyberte **Zákazníci.**
3. V seznamu vyberte zákazníka.
4. V nabídce zákazníka vyberte **Předplatná.**
5. V seznamu vyberte předplatné.
6. Výběrem **možnosti** Aktualizovat **změňte reseller (MPN ID).**

## <a name="next-steps"></a>Další kroky

- [Čtení souboru s vyúčtováním & odsoustavy](read-your-bill.md) 