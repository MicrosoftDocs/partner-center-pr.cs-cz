---
title: Nejčastější dotazy k vydaným obchodním marketplacem Microsoftu
description: Získejte odpovědi na běžné otázky týkající se výběrů na komerčním webu Marketplace. Obsahuje odpovědi na důvody, proč se vaše tržby liší od očekávání.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: keferna
ms.author: keferna
ms.date: 09/11/2020
ms.openlocfilehash: 44bd7f488e3d4e79c45cb2746c7e2a6da449a310
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/19/2020
ms.locfileid: "92527771"
---
# <a name="common-questions-about-commercial-marketplace-payouts"></a>Běžné otázky k obchodním výběrům na webu Marketplace

Tento článek obsahuje odpovědi na nejčastější dotazy týkající se výběrů na komerčním webu Marketplace.

## <a name="earnings-incorrect-or-missing"></a>Nesprávné nebo chybějící výdělky

#### <a name="why-are-my-earnings-missing"></a>Proč moje příjmy chybí?

- Objednávka zákazníka možná ještě není způsobilá k výplatě. V případě objednávek jiných než podnikových zákazníků musí Microsoft nejprve přijmout platbu zákazníka, a teprve pak vydavatel získá nárok na příjem. V případě objednávek podnikových zákazníků budou vaše příjmy k dispozici 1–2 dny od data nákupní objednávky. Ověřte stav objednávky v [sestavách objednávek](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- V sestavě historie transakcí se nemusí zobrazovat příjmy z transakcí provedených před červencem 2019. Zkontrolujte historické výpisy ve [stažených informacích o platbách](https://partner.microsoft.com/dashboard/payouts/reports/incentiveexport).
- Podívejte se na [časový rámec cyklu](payment-thresholds-methods-timeframes.md) a zjistěte, kdy by se příjmy měly objevit v příkazu výběr.

#### <a name="why-is-my-earnings-amount-different-than-what-i-expected"></a>Proč se množství příjmů liší od toho, co jsem očekával?

- Pokud zákazník tuto objednávku zaplatil za částečně, bude vaše míra využití vycházet z částečně placené částky po odečtení poplatků a příslušné daně.
- Ověřte odpovědnost za daňové úhrady podle země. V případě zemí, ve kterých za odvod daní zodpovídá Microsoft, Microsoft vybírá a odečítá příslušné daně z příjmů vydavatelů. Částka transakce uvedená ve výpisu je částka po odečtení daní. Projděte si [podrobné informace o daních](tax-details-marketplace.md).
- SaaS a IaaS nabídky mají poplatky za zlevněnou agenturu na 10% místo na úrovni Standard 20%, takže se sazba příjmů 90%. Tato propagační akce platí do 30. června 2021.

**Další** materiály: [smlouvy o vydavateli komerčního tržiště](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Podrobnosti o](payout-policy-details.md)vydaných zásadách, [prahová hodnota platby, metoda a časový rámec](payment-thresholds-methods-timeframes.md), [který se zaplatí na komerčním webu Marketplace](marketplace-get-paid.md), [daňové detaily](tax-details-marketplace.md), [příkazy výběrů](payout-statement.md), [řídicí panel objednávky v komerčním obchodě](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="earnings-reconciliation"></a>Vypořádání příjmů
### <a name="how-do-i-reconcile-payout-statements-to-order-or-usage-reports-in-analytics"></a>Jak odsouhlasím výpisy plateb pro sestavy objednávek nebo využití v analýzách?
Použijte AssetID, ČísloObjednávky a ID položky řádku, které se zobrazují v sestavě historie transakcí vydaných položek s analytickými objednávkami a sestavami využití. Použít toto mapování:

- Payout Transaction History.AssetID = order.OrderID
- Payout Transaction History.OrderID & LineItem = Usage.UsageReferenceID [OrderID:LineItemID]

### <a name="how-do-i-know-when-to-expect-payments-for-my-customer-orders"></a>Jak zjistím, kdy mám očekávat platby za objednávky zákazníků?
- Nejprve pomocí své služby assetID ověřte objednávky zákazníků v [sestavách objednávek](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Podívejte se na kanál zákazníka pro předplatné zákazníka v [sestavě zákazníci](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/customer).
- V případě podnikových zákazníků se příjmy vydavatelů zobrazí v příkazu 1-2 dnů po datu nákupní objednávky.
- V případě nepodnikových zákazníků se příjmy vydavatelů zobrazí v prohlášení 1-2 dnů po přijetí platby zákazníkovi.

**Další** materiály: [příkazy výběrů](payout-statement.md), [řídicí panel objednávek v analýzách komerčního tržiště](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="payout-policies"></a>Zásady plateb

#### <a name="how-do-i-find-the-current-agency-fee-and-the-payout-rate"></a>Jak zjistím aktuální výši provize a výplaty?

- Projděte si smlouvu pro vydavatele na komerčním marketplace. Standardní provize je 20 %. SaaS Co-Sell způsobilých transakcí mají zlevněný poplatek s 10%. Informace o případných propagačních provizích najdete v oznámeních.
- V příkazu typu výběr určuje sazba za danou transakci skutečnou sazbu pro výběr.

#### <a name="when-can-i-expect-a-payment-from-microsoft-once-earnings-appear-on-my-statement"></a>Kdy můžu očekávat platbu od Microsoftu, jakmile se ve výpisu zobrazí příjmy?
- Jakmile budou vaše příjmy v nezpracovaném stavu, můžete zkontrolovat datum splatnosti a zjistit tak, ve kterém měsíci se zpracuje jejich platba. Po přípravě platby se stav vašeho vystavení změní na zpracováno.  Microsoft uvolňuje platby do 15. dne měsíce splatnosti.
- V případě objednávek placených kreditními kartami má společnost Microsoft platby za 30 dní až do doby, kdy je vyčerpána.

 **Další** materiály: [Smlouva o vydavateli komerčního tržiště](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Podrobnosti o](payout-policy-details.md)vydaných zásadách, [Podrobnosti o daních](tax-details-marketplace.md), [prahová hodnota platby, metoda a časový rámec](payment-thresholds-methods-timeframes.md)

## <a name="payments-and-adjustments"></a>Platby a úpravy

#### <a name="why-is-my-payment-missing"></a>Proč moje platba chybí?

- Ujistěte se, že stav vypsaných a daňový profil se na [stránce Přehled](https://partner.microsoft.com/dashboard/commercial-marketplace/overview)zobrazují jako *platné* .
- Možná jste nedosáhli minimální prahové hodnoty pro platbu. Abyste mohli přijmout platbu, příjmy musí dosahovat alespoň 50 USD.


#### <a name="how-do-i-set-my-account-to-not-receive-payment"></a>Návody nastavte můj účet na nepříjem plateb?
Platby můžete uchovávat v [profilu výběr](https://partner.microsoft.com/dashboard/commercial-marketplace/overview); jednoduše se podívejte na **blokování** . Společnost Microsoft bude mít za vás platbu, dokud neuvolníte blokování.

#### <a name="why-do-i-receive-in-a-different-currency-than-the-purchase-currency"></a>Proč mi platby přicházejí v jiné měně, než je měna použitá při nákupu?

Měna výplaty vychází z měny, kterou jste vybrali v platebním profilu. Měna použitá při nákupu vychází z měny, ve které zákazník zaplatil.

#### <a name="how-do-i-reconcile-adjustments"></a>Jak odsouhlasím vyrovnání?

Vyrovnání plateb představují opravy plateb za účelem kompenzačních vyrovnání například kvůli systémovým problémům. Ve výpisu plateb najdete důvod vyrovnání v poli Kód důvodu. Tato vyrovnání nejsou určená přímo pro jednotlivé transakce.

**Další** materiály: [Smlouva o vydavateli komerčního tržiště](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Podrobnosti o](payout-policy-details.md)vydaných zásadách, [Podrobnosti o daních](tax-details-marketplace.md), [prahová hodnota platby, metoda a časový rámec](payment-thresholds-methods-timeframes.md)

## <a name="taxes"></a>Daně

#### <a name="how-do-we-identify-tax-remit-responsibility-between-microsoft-or-publisher-in-the-payout-statement"></a>Jak ve výpisu plateb zjistíme, jestli je za odvod daní zodpovědný Microsoft, nebo vydavatel?

Ve stažené historii transakcí vyhledejte sloupec Tax model (Daňový model). V tomto sloupci se zobrazí MS Managed (Spravuje Microsoft) nebo ISV Managed (Spravují nezávislí výrobci softwaru). Informace o daňových pravidlech v konkrétních zemích a důsledcích pro výplaty najdete v [podrobných informacích o daních](tax-details-marketplace.md).

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Jak si můžu stáhnout formuláře pro daň z poplatků za služby?

Přejděte na stránku **Výplata plateb** a pak do části **Seznam plateb** . Pro platby, na které se vztahuje daň z poplatků za služby, se zobrazí odkaz na formulář pro daň z poplatků za služby.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Jak si můžu stáhnout formulář pro srážkovou daň ve formátu PDF?

Přejděte na stránku *Výplata plateb* a pak do části **Seznam plateb** . Vedle plateb se zobrazí odkaz na formulář pro srážkovou daň.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Kde najdu daňové formuláře ke konci roku?

Daňové formuláře ke konci roku můžete zobrazit na [profilové stránce](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage).

#### <a name="how-do-i-find-withholding-tax-for-a-transaction"></a>Jak zjistí srážkovou daň pro konkrétní transakci?
Srážkové dani podléhají vydavatelé z USA, kteří vyplnili formulář W-9. Srážková daň se počítá z měsíční výplaty.

**Další** materiály: [Smlouva o vydavateli komerčního tržiště](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Podrobnosti o](payout-policy-details.md) vydaných zásadách

## <a name="payout-statement-access"></a>Přístup k příkazu výběr

#### <a name="how-do-i-access-a-payout-statement"></a>Jak získám přístup k výpisu plateb?

1. Zkontrolujte své role. Abyste mohli získat přístup k výpisu plateb, musíte mít roli *finančního přispěvatele* nebo *vlastníka účtu* .
2. V pravém horním rohu vyberte ikonu **Výběr** , abyste zobrazili příkaz výběr. Vyberte si mezi **historií transakcí** , **platbami** a **stažením** .

**Další** materiály: [Výběr rolí a oprávnění](payout-statement.md#roles-and-permissions), [příkazů výběr](payout-statement.md) 

## <a name="payout-statement-report"></a>Sestava příkazu výběr

#### <a name="what-does-each-field-in-the-transaction-download-mean"></a>Co znamenají jednotlivá pole ve stažených informacích o transakcích?

Podrobný seznam atributů a jejich význam naleznete v tématu [Výběr příkazů](payout-statement.md) .

#### <a name="what-is-earning-status"></a>Co je stav příjmů?

Zobrazí se vaše tržby buď nezpracovaných, zpracovávaných, nebo odeslaných.

- **Nezpracované** – příjmy jsou v v úschově období až do data splatnosti.
- **Zpracované** – příjmy byly zralé a jsou připravené na měsíční platbu. Platby se uvolňují do 15. měsíce v měsíci.
- **Odeslané** – platba se úspěšně vydala do vaší banky na základě vašeho profilu vydaných.

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Jak si můžu stáhnout formuláře pro daň z poplatků za služby?

Přejděte na stránku **Výplata plateb** a pak do části **Seznam plateb** . Pro platby, na které se vztahuje daň z poplatků za služby, se zobrazí odkaz na formulář pro daň z poplatků za služby.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Návody stáhnout formulář pro srážkovou daň ve formátu PDF?

Přejděte na stránku **Výplata plateb** a pak do části **Seznam plateb** . Vedle plateb se zobrazí odkaz na formulář pro srážkovou daň.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Kde najdu daňové formuláře ke konci roku?

Daňové formuláře ke konci roku můžete zobrazit na [profilové stránce](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage).

**Další** materiály: [příkazy výběrů](payout-statement.md), [stažení Historie transakcí](payout-statement.md#transaction-history-download)

## <a name="historical-statements"></a>Historické příkazy

#### <a name="how-do-i-view-historical-information"></a>Návody zobrazit historické informace?

V historickém výpisu se zobrazí snímek údajů o platbách k říjnu 2019. Informace o výběrech se bohužel neaktualizují. Pokud chcete dostávat nejnovější informace, odešlete lístek podpory pro nejnovější data.

**Další** materiály: [příkazy výběrů](payout-statement.md), [stažení Historie transakcí](payout-statement.md#transaction-history-download)

## <a name="payout-export-api"></a>Exportovat rozhraní API pro výběr

#### <a name="how-do-i-download-payout-data"></a>Jak si můžu stáhnout údaje o platbách?

Použijte [rozhraní API pro výběr partnerů](https://apidocs.microsoft.com/services/partnerpayouts).

## <a name="next-steps"></a>Další kroky

- [Vyplácení na komerčním marketplace](marketplace-get-paid.md)
