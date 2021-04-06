---
title: Správa neplacení, podvodů nebo zneužití
description: Přečtěte si o různých rizicích souvisejících s online transakcemi a s osvědčenými postupy pro správu a zmírnění těchto rizik v partnerském centru.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: 9b3beef70052ad204327dd53c4aa9f477056bbcb
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441859"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>Řešení nezaplacení, podvodu nebo zneužití v Partnerském centru

Platí pro:

- Partnerské centrum pro Microsoft Cloud for US Government

**Příslušné role**

- Globální správce
- Správce správy uživatelů
- Agent správce
- Správce fakturace

Máte finančně odpovědnost za podvodné nákupy zákazníků a/nebo zákazníky, kteří si zakoupili koupené služby. Proto *důrazně doporučujeme, abyste provedli řízení prevence podvodů a detekci rizik*.

Aby nedocházelo k podvodné aktivitě nebo zneužití adres, je důležité pochopit potenciální rizika a vyvíjet zásady a postupy, které mohou snížit vaši expozici.

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a>Vynucování zásad přijatelného použití Microsoftu

Pokud společnost Microsoft zjistí, že se partner nebo aktivita zákazníka domnívá nebo podezření porušuje přijatelné zásady použití, budeme postupovat podle kroků pro vynucení. Zákazník může být okamžitě pozastaven. Budete upozorněni na akce vynucení nebo aktualizovány na základě vašich požadavků od Microsoftu.

## <a name="abuse-of-service-risks"></a>Zneužití rizik služeb

**Zneužití rizik služeb** znamená, že zákazníci, kteří používají cloudové služby, jsou v rozporu s podmínkami přijatelného používání společnosti Microsoft.

### <a name="examples-of-abuse-of-service"></a>Příklady zneužití služby

Příklady těchto porušení zásad přijatelného používání společnosti Microsoft můžou zahrnovat:

- Spamem
- Kusů
- Distribuované útoky s cílem odepření služeb (DDoS)
- Bitcoin dolování
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
- Vytvořte zásadu zrušení kolekce. Podrobné informace o procesu sběru a o přístupu k předplatným budou ovlivněny neplatbou. (Můžete zakázat přístup nebo [pozastavit předplatná zákazníka](create-a-new-subscription.md#suspend-a-subscription) pro neplatbu.)

### <a name="managing-customer-accounts"></a>Správa zákaznických účtů

Návrhy správy zákaznických účtů po nákupu zahrnují:

- Implementací procesu můžete rychle přijímat, kontrolovat, reagovat na oznámení Microsoftu a reagovat na ně.
- Spolupracujte se zákazníky, abyste porozuměli obchodním potřebám využití cloudu a nastavení vhodné prahové hodnoty monitorování. (Můžete například [nastavit měsíční rozpočet Azure útraty](set-an-azure-spending-budget-for-your-customers.md) v partnerském centru. Díky tomuto porozumění můžete sledovat využití zákazníků v průběhu měsíce a informovat se o tom, že se zákazníci blíží jejich rozpočtu.)
- Pravidelně monitorujte [protokoly aktivit zákazníků](activity-logs.md) , abyste mohli včas detekovat podvod.
- Provede rychlou akci při zjištění podezřelých aktivit.
- Vyhněte se tomu, aby zákazníci měli úplný přístup správce k předplatným bez prvotní implementace řízení zmírnění rizik.

### <a name="managing-customer-billing"></a>Správa fakturace zákazníků

Návrhy pro správu fakturace zákazníků na základě nákupu zahrnují:

- Před počátečními transakcemi a fakturací si vyžádejte platby.
- Nepřijímejte vysoce rizikové platební nástroje (například předem placené karty nebo karty uložených hodnot).
- Sledovat platby zákazníků a účty pro vztahy se stárnutím Agresivní vymáhání standardizovaných upomínky procesů pro pozdní platby nebo nedoplatk.

Podrobnější strategie pro zmírnění rizika online najdete v tématu [Průvodce správou rizik online transakcí.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)
