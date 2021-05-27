---
title: Plány a procesy výplat
description: Seznamte se s platbami a transakcemi, jako jsou plány plateb a procesy opětovného Azure Marketplace a dalších transakcí.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 05/25/2021
ms.openlocfilehash: bcecd4c31d80a4130331c652491e7951af180c67
ms.sourcegitcommit: f1255fb65eac6ee2e0ff0cb95cc16a02dc57fc1a
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/27/2021
ms.locfileid: "110582411"
---
# <a name="payout-schedules-and-processes"></a>Plány a procesy výplat

**Odpovídající role:** Správce účtu | Globální správce

Tento článek popisuje platební kalendář Microsoftu, kde najít stav výplaty a proces nezaplacení ze zákazníka.

## <a name="payment-schedules"></a>Plány plateb

Následující části popisují proces výplat za transakce **smlouva Enterprise** Smlouva se zákazníkem Microsoftu **nebo CSP.**

### <a name="transactions-when-customer-has-an-enterprise-agreement"></a>Transakce, když má zákazník smlouva Enterprise

Když zákazník zakoupí produkt od Microsoft AppSource nebo Azure Marketplace pomocí stávající služby Microsoft smlouva Enterprise pro transakce, vydáme výplaty v dalším cyklu výplaty po 30denní faktuře od zákazníka. Transakce, u kterých zákazník používá platební kartu, mají před výplatou 30denní období platnosti.

Platba často nastane dříve, než Microsoft od zákazníka shromáždí platbu. V [části Proces nezaplacení zákazníka](#process-for-customer-non-payment) níže najdete informace o akcích, které můžeme v případě, že zákazník neprovede platbu Microsoftu, ale my už vydali platbu.

| Událost | Description | Vytváření sestav viditelnosti | Časování* |
| --- | --- | --- | --- |
| Využití nebo měsíc transakce | Zákazník používá nebo kupuje službu. | [Řídicí panel Využití](/azure/marketplace/partner-center-portal/usage-dashboard) [nebo](/azure/marketplace/partner-center-portal/orders-dashboard) Objednávka | **1. měsíc** |
| Microsoft vypočítá fakturační částku. | Určení celkového využití, celkových transakcí | [Řídicí panel Využití](/azure/marketplace/partner-center-portal/usage-dashboard) [nebo](/azure/marketplace/partner-center-portal/orders-dashboard) Objednávka | **2. měsíc** |
| Vyslaný výběr | Určení poplatků za platební instituce a jejich výběr | Označení jako nezpracované v historii transakce v [příkazu výběr](payout-statement.md) | **Měsíc 3 (1. týden)** |
| Připravit výběr | Tržby se připravují na měsíční platby. | Označeno jako nadcházející v historii transakce v [příkazu výběr](payout-statement.md) | **Měsíc 3 (1. týden)** |
| **Vysílaný výběr** | **Platba se posílá vydavateli.** | **Označeno jako odesláno v historii transakce a v části platby [příkazu výběr](payout-statement.md)** | **Měsíc 3 (ne později než 15.)** |
| Faktura placená zákazníkem | Microsoft shromažďuje platbu od zákazníka. | Beze změny | **Měsíc 4 až 12** |
|

\* Datum vyvýběru je v Tichomoří (běžný čas) (PST).

:::image type="content" source="images/payouts/timeline-enterprise.png" alt-text="Časová osa plateb pro zákazníky se smlouvou Enterprise":::

### <a name="transactions-when-customer-has-a-microsoft-customer-agreement-or-csp"></a>Transakce, pokud má zákazník smlouvu nebo CSP Microsoftu pro zákazníky.

Všechny nákupy pomocí platební karty nebo faktury za měsíc mají za úkol, aby bylo zajištěno shromažďování finančních prostředků od zákazníka.

| Událost | Description | Viditelnost sestav | Časování* |
| --- | --- | --- | --- |
| Využití nebo měsíc transakce | Zákazník používá nebo kupuje službu. | [Řídicí panel Využití](/azure/marketplace/partner-center-portal/usage-dashboard) [nebo](/azure/marketplace/partner-center-portal/orders-dashboard) Objednávka | **1. měsíc** |
| Faktura zaplacená zákazníkem | Určení celkového využití, celkové hodnoty transakce a faktury za platbu zákazníkem | [Řídicí panel Využití](/azure/marketplace/partner-center-portal/usage-dashboard) [nebo](/azure/marketplace/partner-center-portal/orders-dashboard) Objednávka | **2. měsíc** |
| Výplata zveřejněná | Určení příjmů z poplatků a výplat pro agenturu | Označení v historii transakcí jako nezpracované v [výpisu platby](payout-statement.md) | **2. měsíc** |
| 30denní období držení | Zajištění shromažďování prostředků, možných vratek a žádostí o refundaci | Označení v historii transakcí jako nezpracované v [výpisu platby](payout-statement.md) | **3. měsíc** |
| Příprava výplaty | Příjmy jsou připravené na měsíční platbu. | Označení jako Nadcházející v historii transakcí ve [výpisu platby](payout-statement.md) | **Měsíc 4 (1 týden)** |
| **Vysílaný výběr** | **Platba se posílá vydavateli.** | **Označeno jako odesláno v historii transakce a v části platby [příkazu výběr](payout-statement.md)** | **Měsíc 4 (ne později než 15.)** |
|

\* Datum vyvýběru je v Tichomoří (běžný čas) (PST).

:::image type="content" source="images/payouts/timeline-credit-card-invoice.png" alt-text="Časová osa plateb za platební kartu a zákazníky faktur":::

## <a name="process-for-customer-non-payment"></a>Postup pro zákazníka bez platby

Ve výjimečných případech Microsoft nedokáže shromažďovat platby od zákazníků po nákupy komerčních webů na webu Marketplace. Když se zákazníkovi nepodaří platit Microsoft podle svého plánu fakturace, zahájíme proces sběru. Tento proces trvá přibližně čtyři měsíce a vyžaduje trvalou komunikaci od Microsoftu. Pokud platba na konci tohoto procesu neobdrží, Microsoft zapisuje fondy jako neshromážditelné.

V rámci procesu vyzkoušení, který je zde kloubem, společnost Microsoft již mohla zaplatila fondy vydavatelům (vy), které jsou nakonec neshromažďovány. Proto máme proces pro sjednocení těchto částek.

Společnost Microsoft bude recoup všechny již placené výběry pomocí jedné z následujících metod: (1) Společnost Microsoft může odečíst neplacené částky z budoucích výběrů; Například pokud je $1 000 ve vydaných vzorcích považován za neshromažďující a zapisování, vaše budoucí výběry budou zadrženy až do obnovení $1 000 nebo (2) Společnost Microsoft může požádat o refundaci nebo vydavatelům faktur pro jakékoli neshromážděné částky.

Následující plán je příkladem:

| Událost | Přibližné datum * | Viditelnost partnerů |
| --- | --- | --- |
| Příklad data pro výběr | 10/15/2020 | Označí se jako **Odeslané** v historii transakcí a v části Platby na řídicím panelu plateb. |
| <font color="red">Pokud zákazník nezaplatíte Microsoftu</font> | 12/2/2020 – 12/5/2020 | Žádná změna, stejně jako výše |
| Zákazník obdrží e-mail s první pozdní platbou | 12/6/2020 | Žádná |
| Zákazník dostává pravidelné e-maily s rostoucí naléhavostí | 12/7/2020 – 1/31/2021 | Žádná |
| Vydavatel je informován o pravděpodobném odepisování. | 1/7/2021 | - |
| Zákazník obdrží oznámení o ukončení | 2/1/2021 | Žádná |
| Proces shromažďování končí / prostředky se odepisuje | 2/15/2021 | E-mailové oznámení zaslané vydavateli, že prostředky byly zapsány. |
| Odečítá se platba | 1\. 3. 2021 | Vydavatel uvidí zápornou transakci v Partnerské centrum výpisu platby. |
| Platba se odsoudí | 3/15/2021 | Budoucí výplaty se zobrazí ve výpisu Partnerské centrum platbách. Vydavatel neobdrží platbu, dokud zůstatek nebude záporný.  |
|||

\* Datum vyvýběru je v Tichomoří (běžný čas) (PST).

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Počet dní, po které se mají platby oslovit k účtu typu výběr

Na 15. den tohoto měsíce obvykle posíláme jakékoli platby splatné v daném měsíci, ale u platby k vašemu účtu může trvat jinou dobu. Počet dní závisí na způsobu platby, který používáme pro váš účet, jak je popsáno níže.

> [!NOTE]
> Níže uvedené dny jsou přibližné. Vaše platba může trvat déle nebo méně času, než se dostanou k vašemu účtu.

| Způsob platby     | Počet dní, po které se má přejít k účtu typu výběr     |
|--------------------|--------------------------------------------|
| Paypal             | 1 pracovní den                             |
| ACH/SEPA           | 2-3 pracovních dnů                          |
| Přenos po drátě      | 7-10 pracovních dnů                         |
|

## <a name="next-steps"></a>Další kroky

- [Podrobné informace o daních](tax-details-marketplace.md)
