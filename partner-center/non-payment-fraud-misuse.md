---
title: Správa neplacení, podvodů nebo zneužití
description: Přečtěte si o různých rizicích spojených s online transakcemi a osvědčených postupech pro správu a zmírnění těchto rizik v Partnerské centrum.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: c3b7db95bbbd039f8328ddd2785579bb533197cc
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686292"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>Řešení nezaplacení, podvodu nebo zneužití v Partnerském centru

**Platí pro**

- Partnerské centrum pro Microsoft Cloud for US Government

**Odpovídající role**

- Globální správce
- Správce správy uživatelů
- Agent pro správu
- Správce fakturace

Finančně zodpovídáte za podvodné nákupy ze strany zákazníků nebo zákazníků za nezaplacení zakoupených služeb. Proto důrazně *doporučujeme, abyste zasadili řízení* rizik před podvody a jejich odhalování.

Pokud se chcete vyhnout podvodným aktivitám nebo zneužití nebo je řešit, je důležité porozumět potenciálním rizikům a vyvinout zásady a postupy, které by snížily riziko ohrožení.

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a>Vynucování zásad přijatelného použití od Microsoftu

Pokud Microsoft zjistí aktivitu partnera nebo zákazníka a potvrdí nebo se domnívá, že porušuje zásady přijatelného použití, podnikáme kroky pro vynucení. Zákazník může být okamžitě pozastavený. Microsoft vás upozorní na akce vynucení nebo aktualizuje na vaše žádosti.

## <a name="abuse-of-service-risks"></a>Zneužití rizik služeb

**Zneužití rizik služeb** znamená zákazníky, kteří používají cloudové služby v rozporu se zásadou přijatelného použití společnosti Microsoft.

### <a name="examples-of-abuse-of-service"></a>Příklady zneužití služby

Mezi příklady těchto porušení zásad přijatelného použití společnosti Microsoft patří:

- Spam
- Hacking
- Distribuované útoky na odepření služeb (DDoS)
- Bitcoin mining
- Distribuce malwaru
- Další prodej kradených předplatných

## <a name="theft-of-service-risks"></a>Krádež rizik služeb

**Krádež rizik spojených s službami** znamená zákazníky, kteří nemají žádný úmysl platit za spotřebované služby. Tato krádež může zahrnovat použití odcizených platebních nástrojů, poskytování falešných fakturačních informací nebo výchozí hodnoty na nevyřízených zůstatcích.

### <a name="examples-of-service-theft"></a>Příklady krádeže služby

Příklady těchto rizik online transakcí můžou zahrnovat:

- Transakce, které se nevyskytují v osobě ("platební karta není přítomna")
- Nereprezentované identity
- Služby zřízené a používané před přijetím počáteční platby
- Nově vznikající trhy a/nebo vysoce rizikové oblasti pro online podvod
- Automatizace vytváření účtů a nákupy pomocí špatných aktérů

## <a name="managing-online-risk"></a>Správa rizik online

Následující doporučení vám pomohou při vývoji zásad a postupů pro snížení rizika online transakcí v životním cyklu vašich vztahů se zákazníky.

### <a name="onboarding-new-customers"></a>Připojování nových zákazníků

Návrhy na snížení rizik online při připojování nových zákazníků zahrnují:

- Navažte osobní vztahy se zákazníky, pokud je to možné (například kontaktujte zákazníky na telefonu).
- Ověřte přihlašovací údaje a pozadí pro zákazníky prostřednictvím lepších metod (například používání úřadů pro kredity nebo obchodní komerční sestavy).
- Během registrace použijte vícefaktorové ověřování (například ověření SMS), abyste minimalizovali vystavení automatickému vytváření a nákupu účtů.
- Spravujte a sledujte identity pomocí služeb (třeba služeb Digital identity).
- Vyhodnoťte finanční sílu zákazníka prostřednictvím přísných systémů pro detekci podvodných platebních karet.
- Vytvořte zásadu jasných kolekcí. Podrobnosti o procesu kolekcí a o tom, kdy bude mít nezaplacení vliv na přístup k předplatným. (Můžete zakázat přístup nebo [pozastavit předplatná](create-a-new-subscription.md#suspend-a-subscription) zákazníka pro nezaplacení.)

### <a name="managing-customer-accounts"></a>Správa zákaznických účtů

Mezi návrhy pro správu zákaznických účtů po nákupu patří:

- Implementujte proces pro rychlé přijímání, reagování na oznámení Microsoftu, reagování na ně a jejich reagování.
- Spolupracujte se zákazníky, abyste porozuměli firemním potřebám využívání cloudu při nastavení vhodných prahových hodnot monitorování. (Můžete například nastavit měsíční [rozpočet útraty Azure](set-an-azure-spending-budget-for-your-customers.md) v Partnerské centrum. Toto porozumění vám umožní monitorovat využití zákazníků v průběhu měsíce a být informováni, když se zákazníci blíží jejich rozpočtu.)
- Pravidelně [monitorujte protokoly aktivit zákazníků,](activity-logs.md) abyste podvody včas odhalovat.
- Rychlá akce při zjištění podezřelých aktivit
- Vyhněte se poskytování úplného přístupu pro správu k předplatným bez první implementace kontrol omezení rizik.

### <a name="managing-customer-billing"></a>Správa fakturace zákazníků

Mezi návrhy pro správu fakturace zákazníků po nákupu patří:

- Vyžádejte si zálohy před počátečními transakcemi a fakturací.
- Nepřijímá vysoce rizikové platební nástroje (například předplacené karty nebo karty uložené hodnoty).
- Monitorujte platby zákazníků a stárnoucí účty v rámci závazků. Agresivně vynucovat standardizované procesy dunningu pro pozdní platby nebo nezaplacení.

Podrobnější strategie pro zmírnění online rizik najdete v průvodci [řízením rizik online transakcí.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)
