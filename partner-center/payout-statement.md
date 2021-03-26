---
title: Výpisy plateb
description: Další informace o příkazech výběr a souhrnech a o tom, jak zobrazit a exportovat platební data z partnerského centra Microsoftu
ms.subservice: partnercenter-marketplace-publisher
ms.service: marketplace
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 3/22/2021
ms.openlocfilehash: afe9793e3a1ef9c0e3e8ecba6d1c3419b7e16604
ms.sourcegitcommit: 700150044ea4f1a0b96cb4caeb97d7197da29ef6
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/25/2021
ms.locfileid: "105549239"
---
# <a name="payout-statements"></a>Výpisy plateb

**Příslušné role:**

- Správce účtu
- Globální správce

**Příkaz Výběr** nabízí přehled o vašich výběrech z nabídek prodávaných prostřednictvím komerčního tržiště. Zobrazuje transakční historii příjmů, odhaduje vaši další platbu a znázorňuje trendy plateb. Můžete si také stáhnout historii transakcí a výpisy plateb. V tomto článku se dozvíte, jak získat přístup k příkazu pro výběr, a k různým stránkám výběr a ke stažení dostupným v partnerském centru.

>[!NOTE]
>Zobrazí se pouze data pro MPN ID a programy, ke kterým jste přidruženi. Pokud chcete zobrazit další data, spolupracujte se správcem účtu s oprávněním. 

## <a name="roles-and-permissions"></a>Role a oprávnění

Chcete-li získat přístup k příkazu typu výběr, je nutné přiřadit roli **vlastníka účtu** nebo **finančního přispěvatele** .

| Sestavy/stránky | Vlastník účtu | Manažer | Vývojář | Obchodní Přispěvatel | Přispěvatel pro finance | Obchodník |
| --- | --- | --- | --- | --- | --- | --- |
| Sestava pořízení (včetně dat téměř v reálném čase) | Může zobrazit | Může zobrazit | Bez přístupu | Bez přístupu | Může zobrazit | Bez přístupu |
| Sestava nebo odpovědi zpětné vazby | Může zobrazit a odeslat názor. | Může zobrazit a odeslat názor. | Může zobrazit a odeslat názor. | Bez přístupu | Bez přístupu | Může zobrazit a odeslat názor. |
| Sestava stavu (včetně dat téměř v reálném čase) | Může zobrazit | Může zobrazit | Může zobrazit | Může zobrazit | Bez přístupu | Bez přístupu |
| Sestava využití | Může zobrazit | Může zobrazit | Může zobrazit | Může zobrazit | Bez přístupu | Bez přístupu |
| Účet pro výběr | Může aktualizovat | Bez přístupu | Bez přístupu | Bez přístupu | Může aktualizovat | Bez přístupu |
| Daňový profil | Může aktualizovat | Bez přístupu | Bez přístupu | Bez přístupu | Může aktualizovat | Bez přístupu |
| Přehled plateb | Může zobrazit | Bez přístupu | Bez přístupu | Bez přístupu | Může zobrazit | Bez přístupu |
|

## <a name="access-your-payout-statement"></a>Přístup k příkazu výběr

Přihlaste se k [partnerskému centru](https://partner.microsoft.com/dashboard/home) a v pravém horním rohu obrazovky vyberte ikonu výběr, abyste měli přístup k těmto různým souhrnům:

- Historie transakcí
- Platby
- Exportovat data

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Ukazuje ikonu Výběr v pravém horním rohu portálu partnerského centra.":::

[Rozhraní API pro výběr partnerů](https://apidocs.microsoft.com/services/partnerpayouts) můžete použít také k připojení a získání transakcí výběrů a platebních údajů přímo.


## <a name="transaction-history"></a>Historie transakcí

Na stránce **historie transakcí** se zobrazuje souhrn příjmů, odhad další platby a trend a podíl plateb za posledních 36 měsíců. Z této části si také můžete stáhnout podrobnosti o transakcích.<br><br>Tato sestava zobrazuje všechny příjmy, které mají nárok na výběr, včetně dosud neodeslaných plateb. Tržby mají nárok na výběr, když ISV dokončí všechny bankovní a daňové informace v partnerském centru, vygenerovala >$50, účet ISV je aktivní a zákazník se účtuje (pro transakce EA) nebo platba byla přijata (pro transakce, které nejsou EA).

:::image type="content" source="images/payouts/transaction-overview.png" alt-text="Přehled transakcí":::

- **Příjmy zaslaly tento rok** – celkové tržby a rozpis výdělků, které byly placené a budou vypláceny v nadcházejícím měsíci.
- **Odhadované platební měsíc** – očekávané tržby v nadcházejících měsících.
- **Trend a trend plateb** – měsíční výnosy a částky plateb za posledních 36 měsíců.
- **Stáhnout** – podrobnosti o transakci si stáhněte ve formátu. csv nebo. TSV.

Pomocí výběru rozsahu kalendářních dat v pravém horním rohu stránky můžete vyfiltrovat výstup stránky, aby se zobrazily poslední 3, 6, 12 nebo 36 měsíců. Případně vyberte vlastní rozsah kalendářních dat až do 36 měsíců. Výchozí rozsah kalendářních dat je 12 měsíců. Můžete také filtrovat podle ID registrace, programu, ID platby, typu odblokování, páky a stavu. Data jsou k dispozici pro aktuální fiskální rok (1. června 30) a předchozí dva fiskální roky.

:::image type="content" source="images/payouts/search-filter.png" alt-text="Vyhledávací filtr v pravém horním rohu stránky.":::

Chcete-li zobrazit další podrobnosti o objektu k dispozici, vyberte šipku dolů na pravé straně stránky. Tím se zobrazí páčka, objem výnosů, produkt a zákazník. Pokud z nějakého důvodu není k dispozici některá z těchto dat, ale potřebujete k ní přístup, obraťte se na podporu. Pokud je výsledkem vyrovnání výsledek úpravy, a ne transakce, pole produkt a zákazník se nezobrazí.

### <a name="transaction-history-summary"></a>Souhrn historie transakcí

Tím se zobrazí informace o převádění, včetně původu z produktů, které se prodávají, stavu a odhadované platební měsíce.

:::image type="content" source="images/payouts/transaction-history.png" alt-text="Historie transakcí.":::

- **Datum výpočtu** – datum nákupu.
- **Typ** vlastnictví – typ přijetí, jako je například prodej, Rabat nebo souběžná op.
- **Celková částka** – částka za netto Na komerčním webu Marketplace to znamená po odečtení standardního poplatku za Marketplace.
- **Stav** – obsahuje tři možnosti:
    - **Nadcházející** – příjmy jsou v nevyřízeném období chlazení.
    - **Zpracované** – příjmy se připravují na další platbu.
    - **Odeslané** – příjmy byly placené.
- **Odhadovaný měsíční měsíc** – měsíc, ve kterém se mají platby zaplatit. Další informace najdete v [Další části](#estimated-payment-month) .

Transakce se zobrazí, jakmile transakce splňuje podmínky pro výběr. Informace o tom, proč možná nemáte nějaké nebo neočekávané tržby, najdete v tématu [běžné otázky o výběrech na komerčním webu Marketplace](payout-faq.md#why-are-my-earnings-missing).

#### <a name="estimated-payment-month"></a>Odhadovaný měsíc platby

Stránka historie transakcí nyní obsahuje tabulku zobrazující odhadované částky plateb za několik následujících měsíců. Tyto informace můžete také zobrazit a stáhnout v části Historie transakcí a export sestavy souhrnu. Tyto informace usnadňují sladění a platební projekce.

Odhadovaný měsíc platby se vypočítá na základě pravidel konfigurace programu a časových os a zpracovává se v nejbližším nebo nadcházejícím platebním cyklu.

Odhadovaný platební měsíc je aktuálně k dispozici pro všechny typy vyloučení s výjimkou souběžného op, který se zobrazí jako **nepoužitelné**. V případě zisků do 1. července 2020 se odhadované platební měsíc zobrazí jako **nedostupné**.

Příklad očekávaného měsíčního měsíce je uveden v následující tabulce.

| Month (Měsíc) | Částka |
| ------ | :-----------: |
|  SEP-2020 |  $7 273,99   |
|  Říjen – 2020 | $8 692,30  |
|  Listopadu – 2020 | $107,89  |

Odhadovaná částka se může lišit od skutečné částky z nejrůznějších důvodů:

- Přepočítání stavu: Pokud se přepočítá zisky, skutečná částka bude odlišná.
- Úpravy: skutečná hodnota se liší v závislosti na úpravách, které nastaly nebo byly odeslány.
- Změna pravidel: Změna pravidel může odrážet přepočítání v rámci skutečné placené částky
- Splatné: Pokud dojde k selhání platby, skutečná částka se může lišit.

Všimněte si, že vaše platba se vydává v předpokládaném měsíci, pokud jsou splněné prahové hodnoty a podmínky pro nárok na platbu v programu. Tato pravidla zahrnují, ale nejsou omezená na následující seznam:

- Váš daňový profil musí být aktuální.
- Vaše tržby musí splňovat nebo překročit prahovou hodnotu minimálního příjmu definovanou v Průvodci programem.
- Výběr je zablokovaný: Pokud na stránce přiřazení profilů vyberete možnost podržet moji platbu.
- Není k dispozici nástroj pro výběr: platba nebo daňový profil není dokončen.

### <a name="transaction-history-download"></a>Stažení Historie transakcí

Pokud se chcete podívat na další podrobnosti o objektu, vyberte **Stáhnout** v horní části stránky. Následující tabulka vysvětluje jednotlivé sloupce v sestavě.

>[!NOTE]
>Export historie transakcí má dvě nová pole, která jsou od srpna 2020:
>
>- **lastPaymentCurrency**  Měna, ve které byla přijata poslední platba, ve všech MPNs, ke kterým má partner aktuálně přihlášený přístup. Pokud se nepřijme žádná platba, poslední platební měna bude US dolarů.
>- **earningAmountInLastPaymentCurrency**  Částka využitá v poslední platební měně

| Název sloupce | Popis | Použitelnost pro pobídkové programy/tržiště |
| --- | --- | --- |
| agreementEndDate | Koncové datum smlouvy | Motivace – jenom některé programy |
| agreementNumber | Číslo smlouvy | Motivace – jenom některé programy |
| agreementStartDate | Počáteční datum smlouvy | Motivace – jenom některé programy |
| calculationDate | Datum výpočtu v systému | Vše |
| claimId | Jedinečný identifikátor pro deklaraci identity | Motivace – jenom některé programy |
| customerCountry | Země nebo oblast zákazníka | tržišť |
| customerEmail |  |  |
| customerName | Může být prázdné | Jenom motivační programy (výjimka: OEM) a tržiště. V případě transakcí CSP zobrazí tržiště název CSP. |
| customerTenantId |  |  |
| distributorId | Identifikátor distributora | Motivace – jenom některé programy |
| Distributor | Název distributora | Motivace – jenom některé programy |
| earningAmount | Peněžní částka v původní transakční měně | Vše |
| earningAmountInLastPaymentCurrency | Peněžní částka v poslední platební měně (pole bude prázdné, pokud se nezaplatily žádné předchozí platby) |  |
| earningAmountUSD | Množství využité v USD | Vše |
| earningDate | Datum přijetí | Vše |
| earningExchangeRate | Směnný kurz použitý k zobrazení odpovídajících částek v USD | Vše |
| earningId | Jedinečný identifikátor pro každý z nich | Vše |
| earningRate | Míra pobídek uplatňovaná na částku transakce pro vygenerování výnosu | Vše |
| earningType | Indikuje, že se jedná o poplatek, Rabat, co-op, prodej atd. | Vše |
| exchangeRateDate | Datum směnného kurzu použité k výpočtu EarningAmount USD | Vše |
| externalReferenceId | Jedinečný identifikátor programu | Programy přímých plateb (pobídek a Marketplace) |
| externalReferenceIdLabel | Popisek jedinečného identifikátoru | Programy přímých plateb (pobídek a Marketplace) |
| instantRebateAmount |  |  |
| invoiceDate |  |  |
| invoiceNumber | Číslo faktury (platí jenom pro Enterprise) | Motivace a Marketplace – jenom některé programy |
| lastPaymentCurrency | Poslední platební měna (pole bude prázdné, pokud se nezaplatila žádná předchozí platba) |  |
| páka | Označuje obchodní pravidlo pro vyloučení. | Vše |
| LicensingProgramName | Název licenčního programu |  |
| LineItemId | Jednotlivý řádek na faktuře zákazníka |  |
| localProviderSeller | Místní poskytovatel/prodejce záznamu |  |
| Měsíc splatnosti | Odhadovaný měsíc platby | Vše |
| OrderId | Má vztah k faktuře zákazníka.  | tržišť |
| parentProductId | Jedinečný identifikátor nadřazeného produktu Pokud pro transakci není k dispozici nadřazený produkt, pak ID nadřazeného produktu = ID produktu. | tržišť |
| parentProductName | Název nadřazeného produktu Pokud pro transakci není k dispozici nadřazený produkt, pak název nadřazeného produktu = název produktu. | tržišť |
| participantId | Primární identita partnera v rámci programu | Vše |
| participantIdType | Převážně ID programu pro pobídkové programy a prodejce, pokud se jedná o tržiště | Vše |
| účastník | Název partnerského partnera | Vše |
| partnerCountryCode | Umístění/země/oblast pro partnerský partner | Vše |
| partNumber | Bude vždy prázdné | Některé aplikace a tržiště |
| paymentId | Jedinečný identifikátor pro korelaci všech transakcí v sestavě transakce s určitou platbou v sestavě platby | Vše |
| paymentStatus | Stav platby | Vše |
| paymentStatusDescription | Popisný popis stavu platby | Vše |
| productId | Jedinečný identifikátor produktu | tržišť |
| NázevVýrobku | Název produktu propojený s transakcí | Vše |
| productType | Typ produktu, jako je aplikace, doplněk nebo hra | tržišť |
| Kód programu | Řetězec, který se má mapovat s názvem programu |  |
| programName | Motivace/uložení názvu programu | Vše |
| purchaseOrderCoverageEndDate | Bude vždy prázdné | Pobídkový program – CRI |
| purchaseOrderCoverageStartDate | Bude vždy prázdné | Pobídkový program – CRI |
| purchaseOrderType | Bude vždy prázdné | Pobídkový program – CRI |
| purchaseTypeCode | Bude vždy prázdné | Pobídkový program – CRI |
| quantity | Liší se v závislosti na programu. Indikuje fakturované množství transakčních programů. | Vše |
| reasonCode |  |  |
| resellerCountry |  |  |
| resellerId | Identifikátor prodejce | Motivace – jenom některé programy |
| proprodejce | Jméno prodejce |  |
| SkuId | ID skladové položky, jak je definováno během publikování. Nabídka může mít mnoho SKU, ale SKU může být přidruženo pouze k jedné nabídce. Motivace – jenom některé programy |  |
| storeFee | Množství, které Microsoft zachovává jako poplatek za zpřístupnění aplikace nebo doplňku ve Storu | tržišť |
| subscriptionEndDate | Datum ukončení předplatného | Motivace – jenom některé programy |
| subscriptionId | Identifikátor předplatného přidružený k zákazníkovi | Motivace – jenom některé programy |
| subscriptionStartDate | Počáteční datum odběru | Motivace – jenom některé programy |
| taxCity |  |  |
| taxCountry |  |  |
| taxRemitModel | Strana odpovědná za přebírání daní (prodej, použití nebo DPH/GST daně) | tržišť |
| taxRemitted | Množství poplatků za daň (prodej, použití nebo DPH/GST) | tržišť |
| taxState | Stav zákazníka |  |
| taxZipCode | Poštovní směrovací číslo zákazníka |  |
| tpan | Indikuje síť AD třetí strany. | jenom reklamy Marketplace |
| transactionAmount | Částka transakce v původní měně transakce na základě toho, které z nich se vygenerovaly | Vše |
| transactionAmountUSD | Částka transakce v USD | Vše |
| transactionCountryCode | Kód země/oblasti, ve kterém se transakce stala |  |
| transactionCurrency | Měna, ve které došlo k původní transakci zákazníka (nejedná se o měnu umístění partnera) | Vše |
| transactionDate | Datum transakce Užitečné pro programy, kde mnoho transakcí přispívá k jednomu z nich | Vše |
| transactionExchangeRate | Datum směnného kurzu použité k zobrazení odpovídající částky transakce v USD | Vše |
| transactionId | Jedinečný identifikátor pro transakci | Vše |
| transactionPaymentMethod | Platební nástroj zákazníka, který se používá pro transakci, jako je karta, fakturace mobilních dopravců nebo PayPal | tržišť |
| transactionType | Typ transakce, například nákup, refundace, Storno nebo vrácení peněz | tržišť |
| workload | Úloha | Motivace – jenom některé programy |
|

### <a name="transaction-adjustment-codes"></a>Kódy úprav transakcí

V následující tabulce jsou uvedeny kódy důvodů pro úpravy a jejich popisy.

|**Kód důvodu**   |**Popis**   |
|------------------|:-------------------------------------|
| Dodržování předpisů AR | Úprava, která snižuje tržby, když partner nehradí faktury společnosti Microsoft na čase. |
| Výměna souběžných op | Úprava, která přenáší zisky souběžnosti do jiné doby nebo převede zisky v rámci OP na rabat. |
| Úprava OPS | Úprava, která opravuje chyby výpočtů systému Microsoft. |
| Úprava OPS – nesprávný výpočet společnosti Microsoft | Úprava, která opravuje nepravdivé výpočty. |
| Úprava OPS – Microsoft nesprávný zápis | Úprava pro neodpovídající výpočty související se zápisem. |
| Mapování partnerů (předplatné) MCI/CSP | Úprava, která opravuje chybné zarovnání předplatného. |
| Výjimka zásad | Úprava, která přepíše pravidlo programu.  |
| Tržby za předchozí období | Úprava příjmů mimo aktuální období zisků. |

## <a name="payments"></a>Platby

Stránka s **platbami** detailně popisuje peníze, které jste získali od Microsoftu. Zobrazuje také, kdy a kolik vám bude placeno.

>[!Note]
> Aby bylo možné výsledek vyhodnotit, vaše výtěžek musí dosáhnout [prahové hodnoty pro platbu](payment-thresholds-methods-timeframes.md) $50. Další informace najdete v tématu [smlouva Microsoft Publisher](https://go.microsoft.com/fwlink/?LinkID=699560).

:::image type="content" source="images/payouts/payments-overview.png" alt-text="Obrazovka s přehledem plateb":::

- **Celkem za tento rok** – celková částka za tento rok, v amerických dolarech, pro všechny vaše programy.
- **Další odhadovaná platba** – jediná další platba, kterou jste udělali (i když už brzy přijdete), v amerických dolarech.
- **Poslední platba** – částka (v amerických dolarech), název programu a program vaší poslední platby.
- **Platba podle zdroje** – množství plateb (v amerických dolarech), za program za posledních 12 měsíců.

### <a name="payments-list"></a>Seznam plateb

Tabulka **Seznam plateb** zobrazuje placené a nedokončené platby. Informace o daních poplatků za službu si můžete stáhnout ve formátu PDF a zobrazit detaily o vzdávkách pro danou platbu.

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="Exportovat historii transakcí":::

- **Placené** – všechny platby se úspěšně odeslaly. V rozevírací nabídce vyberte rok, který chcete filtrovat podle plateb vydaných v daném roce.
- **Čeká na vyřízení** – nadcházející platby.
- **Daň za poplatek za službu (formulář PDF)** – je dostupná pro platby, na které se vztahuje daň za poplatek za službu. Daně za poplatky za služby jsou uvedené v **dalších daních**.
- **Zobrazení** – přesměruje na historii transakcí se seznamem výdělků zahrnutých do platby.

Informace o tom, proč možná nemáte nějaké nebo neočekávané tržby, najdete v tématu [běžné otázky o výběrech na komerčním webu Marketplace](payout-faq.md#why-are-my-earnings-missing).

### <a name="payment-status"></a>Stav platby

Následující tabulka popisuje různé stavy vystavení.

| Stav vystavení | Důvod | Je vyžadována akce partnera? |
| --- | --- | --- |
| Nezpracované | Zisk má nárok na platbu. Zůstane v tomto stavu pro období chlazení, jak je definováno v Průvodci programu pro program pobídek. | No |
| Nadcházející | Platební objednávka vygenerovala nevyřízené interní recenze před zpracováním platby. | No |
| Nevyřízená daňová faktura | Vaše daňová faktura je neúplná nebo neplatná. | Abyste mohli platit, musíte si nejdřív aktualizovat svou daňovou fakturu. |
| Zamítnuto během revize | Platba byla během revize odmítnuta. | Podrobnosti získáte od podpory Microsoftu. |
| Neúspěšný | Platba se nezdařila z důvodu chyby systému společnosti Microsoft. | Podrobnosti získáte od podpory Microsoftu. |
| Rozpracované | Platba probíhá. | No |
| Nesprávná platba | Recouping platby probíhá. | No |
| Odesláno | Platba byla odeslána do vaší banky. | No |
| Opětovného zpracování | V platbě došlo k systémové chybě společnosti Microsoft a probíhá její přepracování. | No |
| Reversed | Platba byla stornována vaší bankou a bude odeslána znovu v dalším platebním cyklu. | No |
| Daňová faktura odmítnuta | Vaše daňová faktura byla během revize odmítnuta. Všechny probíhající platby budou pozastaveny, dokud se nedokončí kontrola daňové faktury. | Podrobnosti získáte od podpory Microsoftu. |
| Daňová faktura pod kontrolou | Vaše daňové faktury se přezkoumávají. Po schválení daňové faktury se vaše platba uvolní. | No |
| Zamítnuto | Platba byla odmítnuta vaší bankou. | Podrobnosti získáte od své banky. |
|

### <a name="payments-download"></a>Stažení plateb

 Následující tabulka vysvětluje jednotlivé sloupce v sestavě. Pokud chcete zobrazit další podrobnosti o platbách, vyberte **Stáhnout** v horní části stránky s platbami.

| Název sloupce | Popis |
| --- | --- |
| participantID | Primární identita partnera v rámci programu |
| participantIDType | Obvykle ID programu pro motivaci programů a ID prodejců pro aplikace ze Storu |
| účastník | Název partnerského partnera |
| programName | Pobídek/uložit název programu |
| vytvořené | Množství realizované v měně za tento program/participantID |
| earnedUSD | Množství získané pro ID programu/účastníka v USD |
| withheldTax | Množství sražené daně v měně za program/participantID |
| salesTax | Celková částka DPH v platbě za program/participantID (platí jenom pro programy pobídek) |
| serviceFeeTax | Celková částka serviceFeeTax v platbě k měně pro program/participantID (platí pro programy pro Store a Azure Marketplace) |
| totalPayment | Celková platba v místní měně s výjimkou srážkové daně a zahrnutí DPH (Pokud je k dispozici) pro program/participantID |
| currencyCode | Plaťte podle kódu měny |
| paymentMethod | Metoda použitá pro placení partnera, například přenos elektronické banky, dobropis |
| paymentID | Jedinečný identifikátor pro platbu Toto číslo je obvykle viditelné v bankovním výpisu (platí pouze pro platby SAP). |
| paymentStatus | Stav platby |
| paymentStatusDescription | Popisný popis stavu platby |
| paymentDate | Platba data byla odeslána od společnosti Microsoft. |
|

## <a name="export-data"></a>Exportovat data

Stránka **exportovat data** se neaktualizuje sama na sebe. Je možné, že budete muset stránku aktualizovat ručně, aby se zobrazila nejnovější data. Výběrem ze tří karet můžete exportovat **historii transakcí**, **platby**, **souhrn transakcí** nebo **historické příkazy**.

Váš filtr může mít za následek **nedostupnou chybu dat** . K tomu může dojít, pokud jste opustili výchozí časové období, které jste vybrali po dobu tří měsíců, a pak jste si vybrali ID platby z vybírání, které je mimo tuto dobu. Pokud k tomu dojde, rozbalte své časové období a zkuste to znovu.

Tady je ukázka exportu plateb:

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="Sestava exportu plateb.":::

### <a name="historical-statements"></a>Historické příkazy

Souhrn **exportu dat** také poskytuje přístup k historickým příkazům.

> [!NOTE]
> Historický příkaz je snímek a není aktualizován. Obraťte se prosím na [podporu](https://partner.microsoft.com/support/v2/?stage=1) a v případě potřeby požádejte o nejnovější data.

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="Exportujte historické příkazy.":::

- Historie transakcí od 1. července 2019 se zpracovává samostatně a používá jiná pole z pozdějších sestav historie.
- Starší historie transakcí obsahuje sloupec s názvem "vyhrazeno", který odpovídá sloupci "příjmy" v moderní historii, s tím rozdílem, že vylučuje všechny příjmy se stavem se rovná "odeslané platby".
- Filtry, jako jsou 3M, 6 min nebo 12M, se nebudou vztahovat na oddíl historická prohlášení.

### <a name="historical-statement-downloads"></a>Stažení historických příkazů

Následující tabulka vysvětluje jednotlivé sloupce v historických příkazech.

| Název pole | Description |
| --- | --- |
| Zdroj výnosů | Zdroj výnosů na základě toho, kde transakce proběhla, například Microsoft Store, úložiště Windows Phone, Windows Store 8 nebo inzerce |
| ID objednávky | Jedinečný identifikátor objednávky Toto ID umožňuje identifikovat nákupní transakce s příslušnými transakcemi, které nepatří do nákupních transakcí, jako jsou refundace nebo vratek. Obě budou mít stejné ID objednávky. Také pokud je účtován poplatek za rozdělení, u kterého bylo použito více způsobů platby pro jeden nákup, umožňuje propojit transakce nákupu. |
| ID transakce | Jedinečný identifikátor transakce. |
| Datum a čas transakce | Datum a čas, kdy došlo k transakci (UTC). |
| ID nadřazeného produktu | Jedinečný identifikátor nadřazeného produktu Pokud pro transakci není k dispozici nadřazený produkt, pak ID nadřazeného produktu = ID produktu. |
| ID produktu | Jedinečný identifikátor produktu |
| Název nadřazeného produktu | Název nadřazeného produktu Pokud pro transakci není k dispozici nadřazený produkt, pak název nadřazeného produktu = název produktu. |
| Název produktu | Název produktu |
| Typ produktu | Typ produktu, jako je aplikace, doplněk nebo hra |
| Množství | Když je zdroj výnosů Microsoft Store pro firmy, množství představuje počet zakoupených licencí. U všech ostatních zdrojů příjmů bude množství vždy 1. I v případě, že jedna transakce je rozdělena na dvě řádkové položky, protože byly použity dvě různé metody platby, zobrazí se v každé položce řádku množství 1. |
| Transaction Type (Typ transakce) | Typ transakce, například nákup, refundace, Storno nebo vrácení peněz |
| Způsob platby | Platební nástroj zákazníka, který se používá pro transakci, jako je karta, fakturace mobilních dopravců nebo PayPal |
| Země nebo oblast | Země nebo oblast, kde se transakce stala |
| Místní poskytovatel/prodejce | Místní poskytovatel/prodejce záznamu |
| Transakční měna | Měna transakce |
| Částka transakce | Množství transakce |
| DPH poukázané | Množství poplatků za daň (prodej, použití nebo DPH/GST) |
| Čisté příjmy | Množství transakce méně se propoukázané. |
| Poplatek za Store | Procento čistých příjmů uchovávaných Microsoftem jako poplatek za zpřístupnění aplikace nebo doplňku ve Storu |
| Výsledek aplikace | Čisté příjmy minus poplatek za Store |
| Odmítnuté daně | Množství srážky daně z příjmu (zahrnuté do **rezervovaného** souboru CSV) |
| Platba | Aplikace pokračuje bez jakýchkoli příslušných srážkových daní za příjem (částka uvedená v transakční měně). Nezahrnuto do **rezervovaného** souboru CSV. |
| Míra FX | Směnný kurz, který se používá k převodu transakční měny na platební měnu |
| Měna platby | Měna, ve které se platby provedly |
| Převedená platba | Částka platby převedená na platební měnu pomocí míry FX |
| Model daňové úhrady | Strana odpovědná za přebírání daní (prodej, použití nebo DPH/GST daně) |
| Datum a čas nároku | Datum a čas, kdy transakce pokračuje v nároku na výběr (UTC). Když je vytvořen výběr, zahrnuje transakci transakce s datem a časem nároku před datem vytvoření výběr (zahrnuto pouze do **rezervovaného** souboru CSV). |
| Poplatky | Zobrazuje rozpis všech podrobností o poplatcích, které jsou agregované ve sloupci částka transakce (zahrnuté jenom pro Azure Marketplace; nezahrnuté do **rezervovaného** souboru CSV). |
|||

## <a name="next-steps"></a>Další kroky

- [Rozhraní API pro výplaty partnerům](https://apidocs.microsoft.com/services/partnerpayouts)
- [Podrobnosti zásad plateb](payout-policy-details.md)
- Pro podporu fakturace kontaktujte komerční [podporu vydavatele](https://partner.microsoft.com/support/v2/?stage=1)na webu Marketplace.
