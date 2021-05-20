---
title: Výpisy plateb
description: Přečtěte si o výpisech a souhrnech plateb a o tom, jak zobrazit a exportovat platební údaje z Microsoft Partnerské centrum
ms.subservice: partnercenter-marketplace-publisher
ms.service: marketplace
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 3/22/2021
ms.openlocfilehash: 4e9ab721fe356dbcdff7316a5ed5b52c81f2d4eb
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152592"
---
# <a name="payout-statements"></a>Výpisy plateb

**Odpovídající role:** Správce účtu | Globální správce

Výpis **platby představuje** přehled vašich výplat z nabídek prodaných prostřednictvím komerčního marketplace. Zobrazuje historii transakcí vašich příjmů, odhadne vaši další platbu a zobrazuje trendy plateb. Můžete si také stáhnout historii transakcí a výpisy plateb. Tento článek vysvětluje, jak získat přístup k výpisu platby a různým stránkám výplaty a souborům ke stažení, které máte Partnerské centrum.

>[!NOTE]
>Zobrazí se pouze data pro ID MPN a programy, ke které jste přidruženi. Pokud chcete zobrazit další data, pracujte s oprávněními u správce účtu. 

## <a name="roles-and-permissions"></a>Role a oprávnění

Pokud chcete získat přístup k výpisu platby, musíte mít přiřazenou roli Vlastník **účtu** nebo **Přispěvatel finančních** prostředků.

| Sestavy/stránky | Vlastník účtu | Manažer | Vývojář | Přispěvatel pro firmy | Přispěvatel financí | Marketingu |
| --- | --- | --- | --- | --- | --- | --- |
| Sestava pořízení (včetně dat v reálném čase) | Může zobrazit | Může zobrazit | Bez přístupu | Bez přístupu | Může zobrazit | Bez přístupu |
| Sestava zpětné vazby / odpovědi | Může zobrazit a odeslat zpětnou vazbu. | Může zobrazit a odeslat zpětnou vazbu. | Může zobrazit a odeslat názor. | Bez přístupu | Bez přístupu | Může zobrazit a odeslat názor. |
| Sestava stavu (včetně dat téměř v reálném čase) | Může zobrazit | Může zobrazit | Může zobrazit | Může zobrazit | Bez přístupu | Bez přístupu |
| Sestava využití | Může zobrazit | Může zobrazit | Může zobrazit | Může zobrazit | Bez přístupu | Bez přístupu |
| Účet pro výběr | Může aktualizovat | Bez přístupu | Bez přístupu | Bez přístupu | Může aktualizovat | Bez přístupu |
| Daňový profil | Může aktualizovat | Bez přístupu | Bez přístupu | Bez přístupu | Může aktualizovat | Bez přístupu |
| Přehled plateb | Může zobrazit | Bez přístupu | Bez přístupu | Bez přístupu | Může zobrazit | Bez přístupu |
|

## <a name="access-your-payout-statement"></a>Přístup k příkazu výběr

Přihlaste se [Partnerské centrum](https://partner.microsoft.com/dashboard/home) a výběrem ikony výplaty v pravém horním rohu obrazovky získejte přístup k těmto různým souhrnům:

- Historie transakcí
- Platby
- Exportovat data

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Znázorňuje ikonu Výplata v pravém horním rohu portálu Partnerské centrum Portal":::

Rozhraní API pro výplatu [partnerů můžete](https://apidocs.microsoft.com/services/partnerpayouts) použít také k přímému připojení a získání platební transakce a platebních dat.


## <a name="transaction-history"></a>Historie transakcí

Na **stránce Historie transakcí** se zobrazuje souhrn vašich příjmů, odhadovaná příští platba a trend příjmů a plateb za posledních 36 měsíců. Podrobnosti o transakcích si také můžete stáhnout z této části.<br><br>Tato sestava zobrazuje všechny příjmy vhodné k výplatě, včetně dosud neposlaných plateb. Příjmy jsou způsobilé k výplatě, když isV dokončí všechny bankovní a daňové údaje v Partnerské centrum, získá >50 USD, účet ISV je aktivní a zákazníkovi se fakturuje (za transakce EA) nebo byla přijata platba (za transakce mimo EA).

:::image type="content" source="images/payouts/transaction-overview.png" alt-text="Přehled transakcí":::

- **Příjmy odeslané v tomto roce** – celkové příjmy a rozpis příjmů, které byly zaplaceny a budou zaplaceny v nadcházejícím měsíci.
- **Odhadovaný měsíc platby** – celkové příjmy očekávané v nadcházejících měsících.
- **Výnosy a trend plateb** – měsíční příjmy a částky plateb za posledních 36 měsíců.
- **Stáhnout** – stáhne podrobnosti o transakci ve formátu .csv nebo .tsv.

Pomocí výběru rozsahu dat v pravém horním rohu stránky vyfiltrujte výstup stránky tak, aby se zobrazí posledních 3, 6, 12 nebo 36 měsíců. Nebo vyberte vlastní rozsah dat až 36 měsíců. Výchozí rozsah dat je 12 měsíců. Můžete také filtrovat podle ID registrace, programu, ID platby, typu příjmu, využití a stavu. Data jsou k dispozici pro aktuální fiskální rok (1. července až 30. června) a předchozí dva fiskální roky.

:::image type="content" source="images/payouts/search-filter.png" alt-text="Vyhledávací filtr v pravém horním rohu stránky.":::

Chcete-li zobrazit další podrobnosti o objektu k dispozici, vyberte šipku dolů na pravé straně stránky. Tím se zobrazí páčka, objem výnosů, produkt a zákazník. Pokud z nějakého důvodu není k dispozici některá z těchto dat, ale potřebujete k ní přístup, obraťte se na podporu. Pokud je vznikne výsledek úpravy, a ne transakce, nezobrazí se pole produktu a zákazníka.

### <a name="transaction-history-summary"></a>Souhrn historie transakcí

V tomto zobrazení se zobrazují podrobnosti o převádění, včetně původu z produktů, které se prodávají z dat, stavu a odhadované platební měsíce.

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

Stránka Historie transakcí teď obsahuje tabulku s odhadovanou částkou plateb za několik příštích měsíců. Tyto informace můžete také zobrazit a stáhnout v části Historie transakcí a Souhrnná exporty sestavy. Tyto informace usnadňují odsouhlasení a odhady plateb.

Odhadovaný měsíc platby se počítá na základě pravidel konfigurace programu a časových os a zpracovává se v dalším/nadcházejícím platebním cyklu.

Odhadovaný měsíc platby je aktuálně k dispozici pro všechny typy příjmových položek s výjimkou spolupráce, která se zobrazí jako **Nepoužili jste**. U příjmů před 1. červencem 2020 se odhadovaný měsíc platby zobrazí jako **Není k dispozici**.

V následující tabulce je příklad odhadovaného měsíce platby.

| Month (Měsíc) | Částka |
| ------ | :-----------: |
|  Září 2020 |  7 273,99 USD   |
|  Říjen–2020 | 8 692,30 USD  |
|  Listopad 2020 | 107,89 USD  |

Odhadovaná částka se může lišit od skutečného množství z různých důvodů:

- Přepočítání příjmů: Pokud se příjmy přepočítájí, skutečná částka se bude lišit.
- Úpravy: Skutečná částka se liší v závislosti na úpravách, ke kterým došlo nebo byly odeslány.
- Změna pravidel: Změna pravidel může odrážet přepočítání skutečné zaplacené částky.
- Splatné: Pokud dojde k selhání platby, skutečná částka se může lišit.

Mějte na vědomí, že vaše platba se v rámci plánu uvolní pouze v případě, že jsou splněna prahová hodnota vašeho programu a pravidla způsobilosti pro platby. Mezi tato pravidla patří mimo jiné následující seznam:

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
| agreementStartDate | Počáteční datum smlouvy | Incentives – jenom některé programy |
| calculationDate (datum výpočtu) | Datum výpočtu výdělku v systému | Vše |
| ID deklarace identity | Jedinečný identifikátor deklarace identity | Incentives – jenom některé programy |
| customerCountry | Země/oblast zákazníka | Tržiště |
| customerEmail |  |  |
| customerName | Může být prázdné | Pouze programy pobídek (výjimka: OEM) a marketplace. V případě transakcí CSP se na marketplace zobrazí název CSP. |
| customerTenantId |  |  |
| distributorId (ID distributora) | Identifikátor distributora | Incentives – jenom některé programy |
| distributorName | Název distributora | Motivace – jenom některé programy |
| earningAmount | Peněžní částka v původní transakční měně | Vše |
| earningAmountInLastPaymentCurrency | Peněžní částka v poslední platební měně (pole bude prázdné, pokud se nezaplatily žádné předchozí platby) |  |
| earningAmountUSD | Množství využité v USD | Vše |
| earningDate | Datum přijetí | Vše |
| earningExchangeRate | Směnný kurz použitý k zobrazení odpovídajících částek v USD | Vše |
| earningId | Jedinečný identifikátor pro každý z nich | Vše |
| earningRate | Míra pobídek uplatňovaná na částku transakce pro vygenerování výnosu | Vše |
| earningType | Indikuje, že se jedná o poplatek, Rabat, co-op, prodej atd. | Vše |
| exchangeRateDate | Datum směnného kurzu použité k výpočtu EarningAmount USD | Vše |
| externalReferenceId | Jedinečný identifikátor programu | Programy s přímými platbami (pobídky a marketplace) |
| externalReferenceIdLabel | Popisek jedinečného identifikátoru | Programy s přímými platbami (pobídky a marketplace) |
| instantRebateAmount |  |  |
| datum faktury |  |  |
| invoiceNumber | Číslo faktury (platí jenom pro podniky) | Pobídky a marketplace – jenom některé programy |
| lastPaymentCurrency | Poslední měna platby (pole bude prázdné, pokud nebyla zaplacena žádná předchozí platba) |  |
| Páčku | Označuje obchodní pravidlo pro příjmy. | Vše |
| LicensingProgramName | Název licenčního programu |  |
| ID položky řádku | Jednotlivý řádek na faktuře zákazníka |  |
| localProviderSeller | Místní poskytovatel/prodejce záznamu |  |
| Měsíc splatnosti | Odhadovaný měsíc platby | Vše |
| OrderId | Má vztah k faktuře zákazníka.  | tržišť |
| parentProductId | Jedinečný identifikátor nadřazeného produktu Pokud pro transakci není k dispozici nadřazený produkt, pak ID nadřazeného produktu = ID produktu. | tržišť |
| parentProductName | Název nadřazeného produktu Pokud pro transakci není k dispozici nadřazený produkt, pak název nadřazeného produktu = název produktu. | tržišť |
| participantId | Primární identita partnera v rámci programu | Vše |
| participantIdType | Převážně ID programu pro pobídkové programy a prodejce, pokud se jedná o tržiště | Vše |
| účastník | Název partnerského partnera | Vše |
| partnerCountryCode | Umístění/země/oblast pro partnerský partner | Vše |
| partNumber | Bude vždy prázdné | Některé programy pobídek a marketplace |
| paymentId (ID platby) | Jedinečný identifikátor pro korelaci všech transakcí v sestavě transakcí s konkrétní platbou v sestavě plateb | Vše |
| stav platby | Stav platby | Vše |
| Popis stavu platby | Popis stavu platby | Vše |
| productId | Jedinečný identifikátor produktu | Tržiště |
| Productname | Název produktu propojený s transakcí | Vše |
| productType | Typ produktu, například Aplikace, Doplněk nebo Hra | Tržiště |
| Programový kód | Řetězec, který se má mapovat s názvem programu |  |
| programName | Název programu incentive/store | Vše |
| purchaseOrderCoverageEndDate | Bude vždy prázdné. | Program pobídek – CRI |
| purchaseOrderCoverageStartDate | Bude vždy prázdné | Pobídkový program – CRI |
| purchaseOrderType | Bude vždy prázdné | Pobídkový program – CRI |
| purchaseTypeCode | Bude vždy prázdné | Pobídkový program – CRI |
| quantity | Liší se v závislosti na programu. Indikuje fakturované množství transakčních programů. | Vše |
| reasonCode |  |  |
| resellerCountry |  |  |
| resellerId | Identifikátor prodejce | Motivace – jenom některé programy |
| proprodejce | Jméno prodejce |  |
| SkuId | ID skladové položky, jak je definováno během publikování. Nabídka může mít mnoho SKU, ale SKU může být přidruženo pouze k jedné nabídce. Motivace – jenom některé programy |  |
| storeFee | Množství uchovávané Microsoftem jako poplatek za zpřístupnění aplikace nebo doplňku ve Storu | Tržiště |
| subscriptionEndDate | Koncové datum předplatného | Incentives – jenom některé programy |
| subscriptionId | Identifikátor předplatného přidružený k zákazníkovi | Incentives – jenom některé programy |
| subscriptionStartDate | Počáteční datum předplatného | Incentives – jenom některé programy |
| taxCity |  |  |
| taxCountry |  |  |
| taxRemitModel | Strana zodpovědná za daně (tržby, využití nebo daně z DPH/daně GST) | Tržiště |
| taxRemitted (Vynecháno daně) | Částka zaplacené daně (tržby, využití nebo daně z DPH/GST) | Tržiště |
| taxState | Stav zákazníka |  |
| taxZipCode | Poštovní směrovací číslo zákazníka |  |
| tpan | Indikuje síť AD třetí strany. | jenom reklamy Marketplace |
| transactionAmount | Částka transakce v původní měně transakce na základě toho, které z nich se vygenerovaly | Vše |
| transactionAmountUSD | Částka transakce v USD | Vše |
| transactionCountryCode | Kód země/oblasti, ve kterém se transakce stala |  |
| transactionCurrency | Měna, ve které došlo k původní transakci zákazníka (nejedná se o měnu umístění partnera) | Vše |
| transactionDate | Datum transakce Užitečné pro programy, kde mnoho transakcí přispívá k jednomu z nich | Vše |
| transactionExchangeRate | Datum směnného kurzu použité k zobrazení odpovídající částky transakce v USD | Vše |
| transactionId | Jedinečný identifikátor transakce | Vše |
| transactionPaymentMethod | Platební nástroj zákazníka použitý k transakci, jako je karta, fakturace mobilního dopravce nebo PayPal | Tržiště |
| Transactiontype | Typ transakce, jako je nákup, refundace, vrácení peněz nebo vratka | Tržiště |
| workload | Úloha | Incentives – jenom některé programy |
|

### <a name="transaction-adjustment-codes"></a>Kódy úpravy transakcí

Následující tabulka uvádí kódy důvodů pro úpravy a jejich popisy.

|**Kód důvodu**   |**Popis**   |
|------------------|:-------------------------------------|
| Dodržování předpisů ar | Úprava, která snižuje příjmy v případě, že partner nezaplatil faktury Microsoftu včas. |
| Převrácení spolupráce | Úprava, která převádí příjmy spolupráce na jiné období nebo převádí příjmy spolupráce na slevu. |
| Úprava operací | Úprava, která opravuje chyby výpočtů systému microsoftu. |
| Ops Adjustment Microsoft incorrect calc | Úprava, která opravuje přepočítání. |
| Úprava operací – Nesprávná registrace Microsoftu | Úprava pro neodpovídající výpočty týkající se registrace. |
| Mapování partnerů (předplatné) MCI/CSP | Úprava, která opravuje chybné zarovnání předplatného. |
| Výjimka zásad | Úprava, která přepíše pravidlo programu.  |
| Tržby za předchozí období | Úprava příjmů mimo aktuální období zisků. |

## <a name="payments"></a>Platby

Stránka s **platbami** detailně popisuje peníze, které jste získali od Microsoftu. Zobrazuje také, kdy a kolik vám bude placeno.

>[!Note]
> Aby bylo možné výsledek vyhodnotit, vaše výtěžek musí dosáhnout [prahové hodnoty pro platbu](payment-thresholds-methods-timeframes.md) $50. Další informace najdete v tématu [smlouva Microsoft Publisher](/legal/marketplace/msft-publisher-agreement).

:::image type="content" source="images/payouts/payments-overview.png" alt-text="Obrazovka s přehledem plateb":::

- **Celkem za tento rok** – celková částka za tento rok, v amerických dolarech, pro všechny vaše programy.
- **Další odhadovaná platba** – jediná další platba, kterou jste udělali (i když už brzy přijdete), v amerických dolarech.
- **Poslední platba** – částka (v amerických dolarech), název programu a program vaší poslední platby.
- **Platba podle zdroje** – množství plateb (v amerických dolarech), za program za posledních 12 měsíců.

### <a name="payments-list"></a>Seznam plateb

Tabulka **Seznam plateb** zobrazuje placené a nedokončené platby. Informace o daních poplatků za službu si můžete stáhnout ve formátu PDF a zobrazit detaily o vzdávkách pro danou platbu.

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="Exportovat historii transakcí":::

- **Placené** – všechny úspěšně odeslané platby. V rozevírací nabídce vyberte rok a vyfiltrujte platby vydané v tomto roce.
- **Čeká** na vyřízení – nadcházející platby.
- **Daň za poplatek za služby (formulář PDF)** – k dispozici pro platby, na které se vztahuje daň za poplatek za služby. Daně z poplatků za služby se zobrazují v **části Ostatní daně.**
- **Zobrazení** – přesměruje se na historii transakcí se seznamem příjmů, které jsou součástí platby.

Informace o tom, proč vám můžou chybět nebo neočekávané příjmy, najdete v tématu Běžné dotazy týkající se výplat [na komerčním marketplace.](payout-faq.md#why-are-my-earnings-missing)

### <a name="payment-status"></a>Stav platby

Následující tabulka vysvětluje různé stavy výdělku.

| Stav příjmů | Důvod | Vyžaduje se akce partnera? |
| --- | --- | --- |
| Nezpracované | Příjmy jsou způsobilé k platbě. Zůstává v tomto stavu po dobu chlazení, jak je definováno v průvodci programem pro program Pobídky. | No |
| Nadcházející | Před zpracováním platby vygeneruje platební příkaz nevyřízené interní kontroly. | No |
| Nevyřízená daňová faktura | Vaše daňové doklady jsou neúplné nebo neplatné. | Než budete moci zaplatit platbu, musíte si aktualizovat fakturu za dani. |
| Zamítnuto během revize | Platba se během revize zamítla. | Podrobnosti získáte od podpory Microsoftu. |
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

 Následující tabulka vysvětluje jednotlivé sloupce v sestavě. Pokud chcete zobrazit další podrobnosti o platbách, vyberte **Stáhnout** v horní části stránky Platby.

| Název sloupce | Popis |
| --- | --- |
| participantID | Primární identita partnera, který v programu získá příjmy |
| participantIDType | Obvykle ID programu pro programy Incentives a ID prodejce pro programy Store |
| participantName | Název partnera poskytujícího příjmy |
| programName | Název programu Incentives/Store |
| Vydělal | Částka získaná v měně Zaplatit za tento program/ID účastníka |
| získané šoupáky | Částka získaná za ID programu nebo účastníka v USD |
| withheldTax | Částka srážkové daně v měně Zaplatit do pro program nebo ID účastníka |
| salesTax | Celková částka daně z prodeje v měně Zaplatit do pro program/participantID (platí pouze pro programy pobídek) |
| serviceFeeTax | Celková částka službyFeeTax v měně Pay To pro program/participantID (platí pouze pro programy v obchodech a Azure Marketplace) |
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

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="Export sestavy plateb.":::

### <a name="historical-statements"></a>Historické příkazy

Souhrn **Export dat** také poskytuje přístup k historickým výpisům.

> [!NOTE]
> Historický příkaz je snímek a není aktualizován. V případě [potřeby se](https://partner.microsoft.com/support/v2/?stage=1) obraťte na podporu a požádejte o nejnovější data.

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="Export historických výpisů.":::

- Historie transakcí před 1. červencem 2019 se zpracovává samostatně a používá různá pole z pozdějších sestav historie.
- Starší historie transakcí obsahuje sloupec s názvem Reserved (Rezervovaná), který odpovídá sloupci Příjmy v moderní historii s tím rozdílem, že se vyloučí všechny příjmy se stavem Odeslaná platba.
- Filtry jako 3M, 6M nebo 12M se nevztahují na oddíl Historické příkazy.

### <a name="historical-statement-downloads"></a>Stažení historických výpisů

Následující tabulka vysvětluje jednotlivé sloupce v historického příkazu.

| Název pole | Description |
| --- | --- |
| Zdroj výnosů | Zdroj výnosů na základě místa, kde k transakci došlo, například Microsoft Store, Windows Phone Store, Windows Store 8 nebo reklama |
| ID objednávky | Jedinečný identifikátor objednávky. Toto ID vám umožní identifikovat nákupní transakce s příslušnými nekupci transakcí, jako jsou refundace nebo vratky. Obě budou mít stejné ID objednávky. Pokud se pro jeden nákup použilo více způsobů platby, navíc vám to umožní propojit nákupní transakce. |
| ID transakce | Jedinečný identifikátor transakce. |
| Datum a čas transakce | Datum a čas, kdy k transakci došlo (UTC) |
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
| Transaction Amount | Částka transakce |
| Vrácení daně | Částka zaplacené daně (tržby, využití nebo daně z DPH/GST) |
| Čisté účtenky | Částka transakce menší než promilené daně |
| Store Fee | Procento čistých účtenek uchované Microsoftem jako poplatek za zpřístupnění aplikace nebo doplňku ve Storu |
| Pokračování v aplikaci | Čisté účtenky minus poplatek za obchod |
| Daně se vyhověla | Částka srážkové daně z příjmů (zahrnutá v **rezervovaném souboru** CSV) |
| Platba | Aplikace postupuje bez jakýchkoli příslušná srážky daně z příjmu (částka zobrazená v měně transakce). Není součástí **rezervovaného souboru** CSV. |
| FX Rate | Směnný kurz použitý k převodu měny transakce na měnu platby |
| Měna platby | Měna, ve které je provedena platba |
| Převedená platba | Částka platby převedená na měnu platby pomocí fx rate |
| Model daňové úhrady | Strana odpovědná za přebírání daní (prodej, použití nebo DPH/GST daně) |
| Datum a čas nároku | Datum a čas, kdy transakce pokračuje v nároku na výběr (UTC). Když je vytvořen výběr, zahrnuje transakci transakce s datem a časem nároku před datem vytvoření výběr (zahrnuto pouze do **rezervovaného** souboru CSV). |
| Poplatky | Zobrazuje rozpis všech podrobností o poplatcích, které jsou agregované ve sloupci částka transakce (zahrnuté jenom pro Azure Marketplace; nezahrnuté do **rezervovaného** souboru CSV). |
|||

## <a name="next-steps"></a>Další kroky

- [Rozhraní API pro výplaty partnerům](https://apidocs.microsoft.com/services/partnerpayouts)
- [Podrobnosti zásad plateb](payout-policy-details.md)
- Pro podporu fakturace kontaktujte komerční [podporu vydavatele](https://partner.microsoft.com/support/v2/?stage=1)na webu Marketplace.