---
title: Použití souborů s vyrovnáním
ms.topic: article
ms.date: 03/26/2021
description: Přečtěte si o souborech odsouhlasení v Partnerské centrum a o tom, jak interpretovat podrobná zobrazení řádkové položky poplatků za dané fakturační období.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1a7d5f3169c4b338a07475a7e246e87841b8dcfb
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431562"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Zjistěte, jak číst řádkové položky v souborech Partnerské centrum odsouhlasení.

**Odpovídající role:** Správce fakturace | Globální správce

Soubory s vyrovnáním si můžete stáhnout z Partnerské centrum, kde najdete podrobné zobrazení jednotlivých poplatků ve fakturačním cyklu. Podrobnosti řádkové položky zahrnují poplatky za předplatná jednotlivých zákazníků a podrobné události (například střednědobé přidání licencí k předplatnému).

Informace o tom, jak číst **fakturu, najdete** v [tématu Čtení faktury.](read-your-bill.md)

## <a name="understand-reconciliation-file-fields"></a>Principy polí v souboru s vyrovnáním

- [Pole v souboru s vyrovnáním na základě licencí](license-based-recon-files.md)
- [Pole v souboru s vyrovnáním na základě využití](usage-based-recon-files.md)
- [Pole v souboru s vyrovnáním využití podle denní sazby](daily-rated-usage-recon-files.md)
- [Pole souboru se souborem odsouhlasení CSP pro jeden nákup](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Principy typů poplatků v souborech s vyrovnáním

Informace o typech poplatků v souborech s vyrovnáním (sloupec **ChargeType)** najdete v tématu Typy poplatků [za soubor s vyrovnáním.](recon-file-charge-types.md)

## <a name="fix-formatting-issues"></a>Oprava problémů s formátováním

V některých případech může soubor s vyrovnáním obsahovat problémy s formátováním. K tomuto problému může dojít například v případě, že není použito národní prostředí en-US.

Pokud chcete opravit všechny problémy s formátováním v souborech s vyrovnáním, postupujte podle těchto kroků:

1. Otevřete soubor s vyrovnáním (ve .csv) v Microsoft Excelu.
2. Vyberte první sloupec v souboru.
3. Otevřete Průvodce **převodem textu na sloupce.** Na pásu karet vyberte **Data** a pak **vyberte Text na Sloupce.**
4. V průvodci vyberte **Typ souboru s oddělovači.** Pak vyberte **Další.**
5. V **poli Oddělovače** vyberte **Čárka**. (Pokud **je už** vybraná karta Tabulátor, můžete tuto možnost ponechat vybranou.) Pak vyberte **Další.**
6. V **poli Formát dat sloupce** vyberte **Date:MDY**. Pak vyberte **Další.**
7. V poli **Formát dat sloupce** vyberte Text **pro** všechny sloupce s množstvím dat. Pak vyberte **Finish** (Dokončit).

## <a name="download-reconciliation-files-programmatically"></a>Stažení souborů s vyrovnáním prostřednictvím kódu programu

Soubory pro sesouhlasení mohou být velmi velké a někdy se obtížně stahují. Pokud chcete stáhnout soubory s vyrovnáním prostřednictvím kódu programu, podívejte se [na stránku Získání řádových položek faktury.](/partner-center/develop/get-invoiceline-items)

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a>Pokud váš soubor překročí limit řádku v Excelu

Pokud si můžete stáhnout soubor s vyrovnáním, ale v Microsoft Excelu ho neotevřete, pravděpodobně to znamená, že soubor obsahuje více řádků, než Excel povolí. Pokud k tomu dojde, můžete soubor otevřít pomocí jednoho z následujících postupů.

### <a name="open-a-recon-file-in-power-bi"></a>Otevřete soubor odsoustavy v Power BI

1. Stáhněte si soubor s vyrovnáním běžným způsobem.
2. Stáhněte, nainstalujte a otevřete instanci služby Microsoft Power BI.
3. Na kartě Power BI **Domů** vyberte **Získat data**.
4. V seznamu **Běžných zdrojů dat** vyberte **Text/CSV.**
5. Po zobrazení výzvy otevřete soubor odsoustavy.

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a>Otevření souboru s rekonsekcemi v kontingenční tabulce Excelu

1. Stáhněte si soubor s vyrovnáním běžným způsobem.
2. Otevřete nový soubor v Microsoft Excelu.
3. Na kartě **Data** vyberte Získat **data,** vyberte **Ze souboru a** pak vyberte **Text/CSV.**
4. Po zobrazení výzvy otevřete soubor odsoustavy. Zobrazí se vaše data.
5. V rozevírací **nabídce** Načíst vyberte **Načíst do** a pak vyberte **OK.**
6. V dialogovém **okně Importovat data** otevřete soubor **výběrem možnosti Sestava** kontingenční tabulky.

## <a name="negative-amount-displayed"></a>Zobrazené záporné množství

V souboru s vyrovnáním se může zobrazit záporná částka. Pravděpodobně to má jednu z následujících příčin:

- Nedávno jste zrušili nebo snížili počet licencí
- Obdrželi jste kredit na licenční smlouvu o službě (SLA) nebo na využití Azure.

Pokud chcete o této transakci získat další informace, zkontrolujte v souboru s vyrovnáním příslušný atribut typu poplatku.

## <a name="map-taxes-or-vat"></a>Mapové daně nebo DPH

Mapování daní nebo daně z přidané hodnoty (DIČ) na vaši fakturu:

- Sečte **sloupec** Daň ze souboru založeného na licencích.
- Sečte **sloupec TaxAmount** ze souboru založeného na využití.

## <a name="itemize-reconciliation-files-by-partner"></a>Položky souborů s vyrovnáním podle partnera

Partneři v **nepřímém modelu** mohou tato další pole použít v souborech odsouhlasení na základě licencí i na základě využití k položce souborů podle prodejce.

| ID MPN | Description |
| ------ | ----------- |
| ID MPN | Identifikátor Microsoft Partner Network (MPN) partnera Cloud Solution Provider (CSP) (přímý nebo nepřímý). |
| [ID MPN prodejce](#reseller-mpn-id) | Identifikátor [MPN prodejce záznamu pro předplatné](#reseller-mpn-id). Toto pole odpovídá ID prodejce uvedenému pro konkrétní předplatné v Partnerské centrum. Zobrazuje se jenom v souborech s vyrovnáním pro partnery v nepřímém modelu. |

### <a name="reseller-mpn-id"></a>ID MPN prodejce

Pokud partner CSP prodá předplatné přímo zákazníkovi, jeho **ID MPN** se vyjádřuje dvakrát, jako **ID MPN** i **ID MPN prodejce.**

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