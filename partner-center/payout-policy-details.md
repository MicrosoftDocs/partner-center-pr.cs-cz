---
title: Podrobnosti o plánech a zásadách pro výběr – Azure Marketplace
description: Přečtěte si o podrobnostech týkajících se obchodních zásad na webu Marketplace, včetně plánů a recoupment.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 11/06/2020
ms.openlocfilehash: cbd849001d128db1912a9bb61ef4c5217a5932ce
ms.sourcegitcommit: 7e32544cf91f932cbeb053c9de506ba9ee773fe2
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 11/20/2020
ms.locfileid: "94947660"
---
# <a name="payout-schedules-and-policy-details"></a>Podrobnosti o plánech a zásadách pro výběr

Tento článek popisuje proces výběrového plánu od společnosti Microsoft, plán výběrů, kde najít stav druhu a postup pro zákazníka, který není vyplácen.

## <a name="payment-schedules"></a>Platební plány

V následujících částech jsou popsány naše výběry pro **smlouva Enterprise** a transakce **platební karty nebo faktury** .

### <a name="enterprise-agreement-transactions"></a>Transakce smlouva Enterprise

Když zákazník koupí produkt z Microsoft AppSource nebo Azure Marketplace pomocí svých stávajících smlouva Enterprise Microsoftu pro transakce, budeme vydávat výběry v dalším cyklu zadávání 30 dnů po fakturaci od zákazníka. Transakce, ve kterých zákazník používá platební kartu, má před výběrem 30denní dobu v týdnu.

K určitému typu často dojde předtím, než Microsoft shromáždí platbu od zákazníka. V tématu [postup pro zákazníky, kteří nejsou placeni](#process-for-customer-non-payment) níže pro akce, které provedeme, pokud se zákazníkovi nepodaří platit společnost Microsoft, ale už jsme vybrali výběr.

| Událost | Popis | Viditelnost sestav | Okamžiku |
| --- | --- | --- | --- |
| Využití nebo měsíc transakce | Zákazník používá nebo kupuje službu. | Řídicí panel [využití](/azure/marketplace/partner-center-portal/usage-dashboard) nebo [objednávky](/azure/marketplace/partner-center-portal/orders-dashboard) | **Měsíc 1** |
| Objednávka nákupu se vytvoří. | Určení celkového využití, transakcí celkem | Řídicí panel [využití](/azure/marketplace/partner-center-portal/usage-dashboard) nebo [objednávky](/azure/marketplace/partner-center-portal/orders-dashboard) | **Měsíc 2** |
| Vytvoří se vydaný výběr ISV. | Určení poplatků za platební instituce a jejich výběr | Označení jako nezpracované v historii transakce v [příkazu výběr](payout-statement.md) | **Měsíc 3 (1. týden)** |
| Připravit výběr | Tržby se připravují na měsíční platby. | Označeno jako nadcházející v historii transakce v [příkazu výběr](payout-statement.md) | **Měsíc 3 (1. týden)** |
| **Datum vyvýběru** | **Platba se posílá vydavateli.** | **Označeno jako odesláno v historii transakce a v části platby [příkazu výběr](payout-statement.md)** | **Měsíc 3 (ne později než 15.)** |
| Faktura placená zákazníkem | Microsoft shromažďuje platbu od zákazníka. | Beze změny | **Měsíc 4 až 12** |
|

\* Datum vyvýběru je v Tichomoří (běžný čas) (PST).

### <a name="customers-who-pay-using-credit-card-or-invoice"></a>Zákazníci, kteří platíte pomocí platební karty nebo faktury

Všechny nákupy pomocí platební karty nebo faktury za měsíc mají za úkol, aby bylo zajištěno shromažďování finančních prostředků od zákazníka.

| Událost | Popis | Viditelnost sestav | Okamžiku |
| --- | --- | --- | --- |
| Využití nebo měsíc transakce | Zákazník používá nebo kupuje službu. | Řídicí panel [využití](/azure/marketplace/partner-center-portal/usage-dashboard) nebo [objednávky](/azure/marketplace/partner-center-portal/orders-dashboard) | **Měsíc 1** |
| Faktura placená zákazníkem | Určení celkového využití, celkové hodnoty transakcí a faktury zákazníka | Řídicí panel [využití](/azure/marketplace/partner-center-portal/usage-dashboard) nebo [objednávky](/azure/marketplace/partner-center-portal/orders-dashboard) | **Měsíc 2** |
| Vytvoří se vydaný výběr ISV. | Určení poplatků za platební instituce a jejich výběr | Označení jako nezpracované v historii transakce v [příkazu výběr](payout-statement.md) | **Měsíc 2** |
| 30denní doba uchovávání | Zajištění shromažďování prostředků, možných vrácení peněz a žádostí o refundaci | Označení jako nezpracované v historii transakce v [příkazu výběr](payout-statement.md) | **Měsíc 3** |
| Připravit výběr | Tržby se připravují na měsíční platby. | Označeno jako nadcházející v historii transakce v [příkazu výběr](payout-statement.md) | **Měsíc 4 (1 týden)** |
| **Datum vyvýběru** | **Platba se posílá vydavateli.** | **Označeno jako odesláno v historii transakce a v části platby [příkazu výběr](payout-statement.md)** | **Měsíc 4 (ne později než 15.)** |
|

\* Datum vyvýběru je v Tichomoří (běžný čas) (PST).

## <a name="process-for-customer-non-payment"></a>Postup pro zákazníka bez platby

Ve výjimečných případech Microsoft nedokáže shromažďovat platby od zákazníků po nákupy komerčních webů na webu Marketplace. Když se zákazníkovi nepodaří platit Microsoft podle svého plánu fakturace, zahájíme proces sběru. Tento proces trvá přibližně čtyři měsíce a vyžaduje trvalou komunikaci od Microsoftu. Pokud platba není na konci tohoto procesu přijatá, Microsoft zapisuje fondy jako neshromážditelné.

V rámci procesu vyzkoušení, který je zde kloubem, společnost Microsoft již mohla zaplatila fondy vydavatelům (vy), které jsou nakonec neshromažďovány. Proto máme proces pro sjednocení těchto částek. Abyste se ujistili, že se vaše (už přijatá) platba mohla sjednotit, budete upozorněni, když se zákazník v procesu sběru a nákupy budou pravděpodobně odepsány.

Společnost Microsoft bude recoup všechny již placené výběry pomocí jedné z následujících metod: (1) Společnost Microsoft může odečíst neplacené částky z budoucích výběrů; Například pokud je $1 000 ve vydaných vzorcích považován za neshromažďující a zapisování, vaše budoucí výběry budou zadrženy až do obnovení $1 000 nebo (2) Společnost Microsoft může požádat o refundaci nebo vydavatelům faktur pro jakékoli neshromážděné částky.

Následuje příklad plánu:

| Událost | Přibližné datum * | Viditelnost partnerů |
| --- | --- | --- |
| Příklad data pro výběr | 10/15/2020 | Označeno jako **odeslané** v části Historie transakcí a platby na řídicím panelu Výběr |
| <font color="red">Pokud zákazník neplatí od Microsoftu</font> | 12/2/2020 – 12/5/2020 | Beze změny, stejné jako u výše |
| Zákazník obdrží první pozdní e-mail s platbami. | 12/6/2020 | Žádné |
| Zákazník obdrží běžné e-maily s rostoucí naléhavostí. | 12/7/2020 – 1/31/2021 | Žádné |
| Vydavatel je upozorněn na zápis, je nejspíš | 1/7/2021 | E-mailové oznámení odeslané vydavateli, že si zákazník ještě neposlal platby. Zahrnuje ID transakce a částku dolaru. |
| Zákazník obdrží oznámení o ukončení. | 2/1/2021 | Žádné |
| Ukončení procesu shromažďování/fondů jsou odepsány | 2/15/2021 | E-mailové oznámení odeslané vydavateli, že prostředky byly odepsány. Zahrnuje ID transakce a částku dolaru. |
| Výběr je odečtený. | 1\. 3. 2021 | Vydavatel uvidí v příkazu výběr v partnerském centru negativní transakci. |
| Výběr se zamítne. | 3/15/2021 | Budoucí výběry se zobrazí v příkazu pro výběr partnerského centra. Vydavatel neobdrží platbu, dokud zůstatek nebude záporný.  |
|||

\* Datum vyvýběru je v Tichomoří (běžný čas) (PST).

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Počet dní, po které se mají platby oslovit k účtu typu výběr

Na 15. den tohoto měsíce obvykle posíláme jakékoli platby splatné v daném měsíci, ale čas potřebný k tomu, aby platba dosáhla svého účtu, trvá ještě déle. Počet dní závisí na způsobu platby, který používáme pro váš účet, jak je popsáno níže.

> [!NOTE]
> Níže uvedené dny jsou přibližné. jakákoli platba může trvat déle nebo kratší dobu, než se dostanou k vašemu účtu.

| Způsob platby     | Počet dní, po které se má přejít k účtu typu výběr     |
|--------------------|--------------------------------------------|
| Paypal             | 1 pracovní den                             |
| ACH/SEPA           | 2-3 pracovních dnů                          |
| Přenos po drátě      | 7-10 pracovních dnů                         |
|

## <a name="next-steps"></a>Další kroky

- [Podrobné informace o daních](tax-details-marketplace.md)
