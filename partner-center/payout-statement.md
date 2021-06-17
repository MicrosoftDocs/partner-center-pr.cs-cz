---
title: Výpisy plateb
description: Přečtěte si o výpisech a souhrnech plateb a o tom, jak zobrazit a exportovat platební údaje z Microsoft Partnerské centrum
ms.subservice: partnercenter-marketplace-publisher
ms.service: marketplace
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 3/22/2021
ms.openlocfilehash: dc0c720544f4a8a3c95e5b91ec656e65dbce7c80
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276106"
---
# <a name="payout-statements"></a>Výpisy plateb

**Odpovídající role:** Správce účtu | Globální správce

Výpis **platby představuje** přehled vašich výplat z nabídek prodaných prostřednictvím komerčního marketplace. Zobrazuje historii transakcí vašich příjmů, odhadne vaši další platbu a zobrazuje trendy plateb. Můžete si také stáhnout historii transakcí a výpisy plateb. Tento článek vysvětluje, jak získat přístup k výpisu platby a různým stránkám výplat a souborům ke stažení, které máte Partnerské centrum.

>[!NOTE]
>Zobrazí se pouze data pro ID MPN a programy, ke které jste přidruženi. Pokud chcete zobrazit další data, pracujte s oprávněními u správce účtu. 

## <a name="roles-and-permissions"></a>Role a oprávnění

Pokud chcete získat přístup k výpisu platby, musíte mít přiřazenou roli Vlastník **účtu** nebo **Přispěvatel finančních** prostředků.

| Sestavy/stránky | Vlastník účtu | Manažer | Vývojář | Přispěvatel pro firmy | Přispěvatel financí | Marketingu |
| --- | --- | --- | --- | --- | --- | --- |
| Sestava pořízení (včetně dat v reálném čase) | Může zobrazit | Může zobrazit | Bez přístupu | Bez přístupu | Může zobrazit | Bez přístupu |
| Sestava zpětné vazby / odpovědi | Může zobrazit a odeslat zpětnou vazbu. | Může zobrazit a odeslat zpětnou vazbu. | Může zobrazit a odeslat zpětnou vazbu. | Bez přístupu | Bez přístupu | Může zobrazit a odeslat zpětnou vazbu. |
| Sestava stavu (včetně dat v reálném čase) | Může zobrazit | Může zobrazit | Může zobrazit | Může zobrazit | Bez přístupu | Bez přístupu |
| Sestava využití | Může zobrazit | Může zobrazit | Může zobrazit | Může zobrazit | Bez přístupu | Bez přístupu |
| Platební účet | Může aktualizovat | Bez přístupu | Bez přístupu | Bez přístupu | Může aktualizovat | Bez přístupu |
| Daňový profil | Může aktualizovat | Bez přístupu | Bez přístupu | Bez přístupu | Může aktualizovat | Bez přístupu |
| Přehled plateb | Může zobrazit | Bez přístupu | Bez přístupu | Bez přístupu | Může zobrazit | Bez přístupu |
|

## <a name="access-your-payout-statement"></a>Přístup k výpisu platby

Přihlaste se [Partnerské centrum](https://partner.microsoft.com/dashboard/home) a výběrem ikony výplaty v pravém horním rohu obrazovky získejte přístup k těmto různým souhrnům:

- Historie transakcí
- Platby
- Exportovat data

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Znázorňuje ikonu Výplata v pravém horním rohu portálu Partnerské centrum Portal.":::

K přímému připojení a získání transakčních a platebních údajů o platbě můžete použít také rozhraní [PARTNER Payout API.](https://apidocs.microsoft.com/services/partnerpayouts)


## <a name="transaction-history"></a>Historie transakcí

Na **stránce Historie transakcí** se zobrazuje souhrn vašich příjmů, odhadovaná příští platba a trend příjmů a plateb za posledních 36 měsíců. Podrobnosti o transakcích si také můžete stáhnout z této části.<br><br>Tato sestava zobrazuje všechny příjmy vhodné k výplatě, včetně dosud neposlaných plateb. Příjmy jsou způsobilé k výplatě, když isV dokončí všechny bankovní a daňové údaje v Partnerské centrum, získá >50 USD, účet ISV je aktivní a zákazníkovi se fakturuje (za transakce EA) nebo byla přijata platba (za transakce mimo EA).

:::image type="content" source="images/payouts/transaction-overview.png" alt-text="Přehled transakcí":::

- **Příjmy odeslané v tomto roce** – celkové příjmy a rozpis příjmů, které byly zaplaceny a budou zaplaceny v nadcházejícím měsíci.
- **Odhadovaný měsíc platby** – celkové příjmy očekávané v nadcházejících měsících.
- **Výnosy a trend plateb** – měsíční příjmy a částky plateb za posledních 36 měsíců.
- **Download** – stáhne podrobnosti o transakcích .csv nebo .tsv.

Pomocí výběru rozsahu dat v pravém horním rohu stránky vyfiltrujte výstup stránky tak, aby se zobrazí posledních 3, 6, 12 nebo 36 měsíců. Nebo vyberte vlastní rozsah dat až 36 měsíců. Výchozí rozsah dat je 12 měsíců. Můžete také filtrovat podle ID registrace, programu, ID platby, typu příjmu, využití a stavu. Data jsou k dispozici pro aktuální fiskální rok (1. července až 30. června) a předchozí dva fiskální roky.

:::image type="content" source="images/payouts/search-filter.png" alt-text="Vyhledávací filtr v pravém horním rohu stránky.":::

Pokud chcete zobrazit další podrobnosti o výdělku, vyberte šipku dolů na pravé straně stránky. Tím se zobrazí využití, výše výnosů, produkt a zákazník. Pokud z nějakého důvodu některá z těchto dat nejsou k dispozici, ale potřebujete k ní přístup, obraťte se na podporu. Pokud je příjmem výsledek úpravy, a ne transakce, pole Product (Produkt) a Customer (Zákazník) se nezobrazí.

### <a name="transaction-history-summary"></a>Souhrn historie transakcí

V tomto zobrazení se zobrazují podrobnosti o příjmech, včetně původu výdělku z dat výdělku prodaného produktu, stavu a odhadovaného měsíce platby.

:::image type="content" source="images/payouts/transaction-history.png" alt-text="Historie transakcí.":::

- **Datum** vydělání – datum nákupu
- **Typ příjmových** ingem – typ příjmových ingem, jako je prodej, rebace nebo spolupráce.
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

Všimněte si, že vaše platba se vydává v předpokládaném měsíci, pokud jsou splněné prahové hodnoty a podmínky pro nárok na platbu v programu. Tato pravidla zahrnují, ale nejsou omezená na seznam níže:

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
| exchangeRateDate | Datum směnného kurzu použitého k výpočtu hodnoty EarningAmount USD | Vše |
| ID externalReferenceId | Jedinečný identifikátor programu | Programy s přímými platbami (pobídky a marketplace) |
| externalReferenceIdLabel | Popisek jedinečného identifikátoru | Programy s přímými platbami (pobídky a marketplace) |
| instantRebateAmount |  |  |
| invoiceDate (datum faktury) |  |  |
| invoiceNumber | Číslo faktury (platí jenom pro podniky) | Incentives a marketplace – jenom některé programy |
| lastPaymentCurrency | Poslední měna platby (pole bude prázdné, pokud nebyla zaplacena žádná předchozí platba) |  |
| Páčku | Označuje obchodní pravidlo pro příjmy. | Vše |
| LicensingProgramName | Název licenčního programu |  |
| ID položky řádku | Jednotlivý řádek na faktuře zákazníka |  |
| localProviderSeller | Místní poskytovatel/prodejce záznamu |  |
| Měsíc splatnosti | Odhadovaný měsíc platby | Vše |
| OrderId | Vztahuje se k faktuře zákazníka  | Tržiště |
| parentProductId | Jedinečný identifikátor nadřazeného produktu. Pokud pro transakci neexistuje nadřazený produkt, pak ID nadřazeného produktu = ID produktu. | Tržiště |
| parentProductName | Název nadřazeného produktu. Pokud pro transakci neexistuje nadřazený produkt, pak název nadřazeného produktu = název produktu. | Tržiště |
| participantId (ID účastníka) | Primární identita partnera, který v programu získá příjmy | Vše |
| participantIdType | Většinou ID programu pro programy pobídek a IF prodejce pro marketplace | Vše |
| participantName | Název partnera poskytujícího příjmy | Vše |
| partnerCountryCode | Umístění/země/oblast partnera poskytujícího příjmy | Vše |
| partNumber | Bude vždy prázdné. | Některé programy pobídek a marketplace |
| paymentId (ID platby) | Jedinečný identifikátor pro korelaci všech transakcí v sestavě transakcí s konkrétní platbou v sestavě plateb | Vše |
| stav platby | Stav platby | Vše |
| popis stavu platby | Popis stavu platby | Vše |
| productId | Jedinečný identifikátor produktu | Tržiště |
| Productname | Název produktu propojený s transakcí | Vše |
| productType | Typ produktu, například Aplikace, Doplněk nebo Hra | Tržiště |
| Programový kód | Řetězec pro mapování s názvem programu |  |
| programName | Název programu incentive/store | Vše |
| purchaseOrderCoverageEndDate | Bude vždy prázdné. | Program pobídek – CRI |
| purchaseOrderCoverageStartDate | Bude vždy prázdné. | Program pobídek – CRI |
| purchaseOrderType | Bude vždy prázdné. | Program pobídek – CRI |
| purchaseTypeCode | Bude vždy prázdné. | Program pobídek – CRI |
| quantity | Liší se v závislosti na programu. Označuje fakturované množství pro transakční programy. | Vše |
| reasonCode (kód důvodu) |  |  |
| resellerCountry |  |  |
| resellerId (ID prodejce) | Identifikátor prodejce | Incentives – jenom některé programy |
| resellerName | Jméno prodejce |  |
| ID SKU | ID SKU definované během publikování. Nabídka může mít mnoho skladové náklady, ale SKU je možné sdružovat pouze s jednou nabídkou. Incentives – jenom některé programy |  |
| storeFee | Množství uchovávané Microsoftem jako poplatek za zpřístupnění aplikace nebo doplňku ve Storu | Tržiště |
| subscriptionEndDate | Koncové datum předplatného | Incentives – jenom některé programy |
| subscriptionId | Identifikátor předplatného přidružený k zákazníkovi | Incentives – jenom některé programy |
| subscriptionStartDate | Počáteční datum předplatného | Incentives – jenom některé programy |
| taxCity |  |  |
| taxCountry |  |  |
| taxRemitModel | Strana zodpovědná za daně (tržby, využití nebo DANĚ Z DPH/daně GST) | Tržiště |
| taxRemitted (Vynecháno daně) | Částka zaplacené daně (tržby, využití nebo daně z DPH/GST) | Tržiště |
| taxState | Stav zákazníka |  |
| taxZipCode | PSČ zákazníka |  |
| tpan (tpan) | Označuje síť reklam třetích stran. | marketplaces Pouze ads |
| transactionAmount (částka transakce) | Částka transakce v původní měně transakce, na základě které se generují příjmy | Vše |
| transactionAmount TRANSACTION | Částka transakce v USD | Vše |
| transactionCountryCode | Kód země nebo oblasti, ve které došlo k transakci |  |
| transactionCurrency | Měna, ve které došlo k původní transakci zákazníka (není to měna umístění partnera) | Vše |
| transactionDate (datum transakce) | Datum transakce Užitečné pro programy, kde mnoho transakcí přispívá k jednomu výdělku | Vše |
| transactionExchangeRate | Datum směnného kurzu použité k zobrazení odpovídající částky transakce v USD | Vše |
| ID transakce | Jedinečný identifikátor transakce | Vše |
| transactionPaymentMethod | Platební nástroj zákazníka použitý pro transakci, jako je karta, fakturace mobilního dopravce nebo PayPal | Tržiště |
| Transactiontype | Typ transakce, jako je nákup, refundace, vrácení peněz nebo vratka | Tržiště |
| workload | Úloha | Incentives – jenom některé programy |
|

### <a name="transaction-adjustment-codes"></a>Kódy úpravy transakcí

Následující tabulka uvádí kódy důvodů pro úpravy a jejich popisy.

|**Kód důvodu**   |**Popis**   |
|------------------|:-------------------------------------|
| Dodržování předpisů pro ar | Úprava, která snižuje příjmy v případě, že partner nezaplatil faktury Microsoftu včas. |
| Převrácení spolupráce | Úprava, která převádí příjmy spolupráce na jiné období nebo převádí příjmy spolupráce na slevu. |
| Úprava operací | Úprava, která opravuje chyby výpočtů systému microsoftu. |
| Ops Adjustment Microsoft incorrect calc | Úprava, která opravuje přepočítání. |
| Úprava operací – Nesprávná registrace Microsoftu | Úprava přepočítání souvisejících s registrací |
| Mapování partnerů (předplatné) MCI/CSP | Úprava, která opravuje nesoulad předplatného. |
| Výjimka zásad | Úprava, která přepisuje pravidlo programu.  |
| Příjmy za předchozí období | Úprava příjmů mimo aktuální období příjmů |

## <a name="payments"></a>Platby

Na **stránce Platby** najdete podrobnosti o penězích, které jste u Microsoftu získali. Také ukazuje, kdy a kolik budete platit.

>[!Note]
> Pokud chcete mít nárok na výplatu, musí vaše výnosy dosáhnout [prahové hodnoty platby](payment-thresholds-methods-timeframes.md) 50 USD. Další informace najdete ve Smlouvě s [vydavatelem Microsoftu.](/legal/marketplace/msft-publisher-agreement)

:::image type="content" source="images/payouts/payments-overview.png" alt-text="Obrazovka s přehledem plateb":::

- **Total paid this year** – celková celková částka, kterou vám tento rok zaplatily v amerických dolarech, pro všechny vaše programy.
- **Příští odhadovaná platba** – jediná příští platba, která vám přijde (i když brzy nasází další) v amerických dolarech.
- **Poslední platba** – částka (v amerických dolarech), název programu a program vaší poslední platby.
- **Platba podle zdroje** – částka plateb (v amerických dolarech) na program za posledních 12 měsíců.

### <a name="payments-list"></a>Seznam plateb

Tabulka **Seznam plateb zobrazuje** placené a nevyřízené platby. Můžete si stáhnout daňové údaje o poplatek za služby ve formátu PDF a zobrazit podrobnosti o příjmech pro danou platbu.

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="Export historie transakcí.":::

- **Placené** – všechny úspěšně odeslané platby. V rozevírací nabídce vyberte rok a vyfiltrujte platby vydané v tomto roce.
- **Čeká** na vyřízení – nadcházející platby.
- **Daň za poplatek za služby (formulář PDF)** – k dispozici pro platby, na které se vztahuje daň za poplatek za služby. Daně z poplatků za služby jsou uvedené v **části Ostatní daně**.
- **Zobrazení** – přesměruje se na historii transakcí se seznamem příjmů, které jsou součástí platby.

Informace o tom, proč vám můžou chybět nebo neočekávané příjmy, najdete v tématu Běžné dotazy týkající se výplat [na komerčním marketplace.](payout-faq.md#why-are-my-earnings-missing)

### <a name="payment-status"></a>Stav platby

Následující tabulka vysvětluje různé stavy výdělku.

| Stav příjmů | Důvod | Vyžaduje se akce partnera? |
| --- | --- | --- |
| Nezpracované | Příjmy jsou způsobilé k platbě. Zůstává v tomto stavu po dobu chlazení, jak je definováno v průvodci programem pro program Pobídky. | No |
| Nadcházející | Před zpracováním platby vygenerovala platební objednávka nevyřízené interní kontroly. | No |
| Nevyřízená daňová faktura | Vaše daňové doklady jsou neúplné nebo neplatné. | Než budete moci zaplatit platbu, musíte si aktualizovat fakturu za dani. |
| Zamítnuto během revize | Platba se během revize zamítla. | Podrobnosti získáte od podpory Microsoftu. |
| Neúspěšný | Platba selhala kvůli systémové chybě Microsoftu. | Podrobnosti získáte od podpory Microsoftu. |
| Rozpracované | Platba probíhá. | No |
| Nesprávná platba | Platba probíhá. | No |
| Odesláno | Platba byla odeslána do vaší banky. | No |
| Přepracování | Při platbě došlo k systémové chybě Microsoftu a znovu se zpracuje. | No |
| Reversed | Vaše banka platbu převrácena a bude odeslána znovu v dalším platebním cyklu. | No |
| Daňová faktura se zamítla | Vaše daňová faktura se během revize zamítla. Všechny nevyřízené platby budou ve stavu hold až do dokončení revize daňové faktury. | Podrobnosti získáte od podpory Microsoftu. |
| Kontrola daňové faktury | Vaše daňové doklady se právě prochová. Po schválení daňové faktury se vaše platba uvolní. | No |
| Zamítnuto | Vaše banka platbu zamítla. | S podrobnostmi se obraťte na svou banku. |
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
| withheldTax | Částka srážkové daně v měně Pay To pro program/participantID |
| salesTax | Celková částka daně z prodeje v měně Pay To pro program/participantID (platí pouze pro programy pobídek) |
| serviceFeeTax | Celková částka službyFeeTax v měně Pay To pro program/participantID (platí pouze pro programy v obchodech a Azure Marketplace) |
| totalPayment | Celková platba v místní měně bez srážkové daně a včetně daně z prodeje (pokud je k dispozici) pro program/participantID |
| currencyCode | Kód měny Pay To |
| paymentMethod | Metoda použitá k platbě partnerovi, například elektronický bankovní převod, kreditní poznámka |
| id platby | Jedinečný identifikátor platby Toto číslo je obvykle viditelné v bankovním výpisu (platí pouze pro platby SAP). |
| stav platby | Stav platby |
| popis stavu platby | Popis stavu platby |
| datum platby | Datum odeslání platby od Microsoftu |
|

## <a name="export-data"></a>Exportovat data

Stránka **Export dat** se sama o sobě ne aktualizována. Možná budete muset stránku aktualizovat ručně, abyste viděli nejnovější data. Na těchto třech kartách můžete exportovat historii **transakcí,** **platby,** souhrn **transakcí** nebo **historický výpis**.

Váš filtr může vést k chybě **Nejsou k dispozici žádná** data. K tomu může dojít v případě, že jste nechali výchozí časové období vybrané na tři měsíce a pak jste vybrali ID platby z příjmů, které jsou mimo toto období. Pokud k tomu dojde, rozbalte časové období a zkuste to znovu.

Tady je ukázkový export plateb:

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="Export sestavy plateb.":::

### <a name="historical-statements"></a>Historické příkazy

Souhrn **Export dat** také poskytuje přístup k historickým výpisům.

> [!NOTE]
> Historický příkaz je snímek a není aktualizován. V případě [potřeby se](https://partner.microsoft.com/support/v2/?stage=1) obraťte na podporu a požádejte o nejnovější data.

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