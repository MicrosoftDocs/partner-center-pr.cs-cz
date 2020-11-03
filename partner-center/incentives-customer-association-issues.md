---
title: Problémy s přidružováním zákazníků v programu Incentives
description: Naučte se řešit problémy, které se při práci s deklarovaným přidružením zákazníků na záznam (CPOR) tvrdí partner.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.date: 09/11/2020
ms.openlocfilehash: ab2c26cf097d6212375382cadd9ac5f4f80b5c2a
ms.sourcegitcommit: b91119c587d37b4ed36dda00c2b0b1946beb3012
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/17/2020
ms.locfileid: "92527252"
---
# <a name="issues-with-claimed-partner-of-record-cpor-customer-associations"></a>Problémy s deklarovaným partnerem pro zákazníky záznamů (CPOR)

**Platí pro:**

- Partnerské centrum

**Příslušné role:**

- Správce fakturace
- Globální správce
- Motivace správce

Následující obsah vám pomůže vyřešit problémy, které se můžou při práci se zákaznickými přidruženími.

## <a name="domain-tenant-mismatch"></a>Doména-tenant nesouhlasí

V toku deklarace identity přihlášeného partnera pro záznam (CPOR) se zobrazí výzva k zadání ID tenanta a subdomény zákazníka. Pokud se zobrazí chyba s oznámením, že se neshodují, obraťte se na zákazníka, abyste měli jistotu, že máte správné podrobnosti.

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a>Chyby předplatného v toku deklarací přidružení CPOR

V toku deklarací přidružení CPOR se může zobrazit výzva k zadání předplatného produktu, který se snažíte uplatnit prostřednictvím Business Applications (Dynamics 365). Vyžádáme si předplatné, protože dynamicky kontrolujeme, že produkt a odběr patří do tenanta, pro který se žádá. Kontrolujeme také, že předplatné je aktivní/ve stavu odkladu.

Pokud se zobrazí chyba, může to být z několika důvodů:

- Vybraný produkt neexistuje v tenantovi zákazníka.
- Zadané předplatné není pro Dynamics.
- Zadané předplatné je určené pro CSP.
- Zákazník ještě neaktivoval/nezřídil produkty pro toto předplatné.
- Předplatné se již nárokuje.
- Zadaný identifikátor není ID předplatného.

Pokud máte dotaz týkající se přesnosti vašeho předplatného, spolupracujte se svým zákazníkem a ujistěte se, že je předplatné správné a že používáte správné ID tenanta.

Pokud tato trasa problém nevyřeší, obraťte se na [podporu](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="when-subscriptions-will-be-available-to-claim"></a>Když budou předplatná k dispozici pro nárok

Při deklaracích identity pro předplatné se zobrazí chyba, pokud předplatné ještě není zřízené. K dispozici je několik kroků, které zákazník potřebuje k tomu, aby předplatné mohlo být dostupné pro platformu CPOR, aby ji bylo možné vybrat a zpřístupnit. Pokud při pokusu o vyzkoušení předplatného dojde k chybě, obraťte se na zákazníka, aby se zajistilo, že je zřízené a že předplatné, které vyžádáte, je správné. Pokud jste tuto trasu již provedli, obraťte se na [podporu](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="which-activity-do-i-choose"></a>Jakou aktivitu mám zvolit?

Platforma pro nárokování na CPOR umožňuje deklarace CPOR přidružení souvisejících s oblastmi řešení Business Applications a Microsoft 365. Aktivity, které platí pro jednotlivé oblasti řešení, jsou uvedené níže. Vyberte správnou aktivitu na základě popisů, abyste se vyhnuli nutnosti v budoucnu znovu vymáhat. Nárokování s nesprávnou aktivitou může mít za následek zmeškaný zisk a finanční zisky.


| Oblast řešení | Aktivita | Platí pro |
| ------ | ----------- | ----------- |
| Obchodní aplikace      | Předprodejní   | Tuto možnost vyberte, pokud si nejste ovlivnili nákup opravňujícího produktu a chcete ho použít pro pobídky předběžného prodeje. Tato možnost se vztahuje jenom v případě, že zákazník tyto produkty koupil prostřednictvím multilicenční smlouvy nebo na webu. |
|    |  Využití  | Tuto možnost vyberte, pokud chcete, aby jejich přijetí a použití způsobilých úloh bylo vhodné a aby se dalo použít k motivaci využití. Tato možnost se vztahuje jenom v případě, že zákazník tyto produkty koupil prostřednictvím multilicenční smlouvy nebo na webu. |
|    | Přiřazení výnosů   | Tuto možnost vyberte, pokud jste ovlivnili výběr oprávněného produktu jako jeho vliv na firmu. Tato možnost je určena pouze pro sdružení příjmů, nikoli pro pobídkové platby. Tato možnost se vztahuje jenom v případě, že zákazník tyto produkty koupil prostřednictvím multilicenční smlouvy nebo na webu.   |
| Microsoft 365   | Využití   | Tuto možnost vyberte, pokud chcete, aby jejich přijetí a použití způsobilých úloh bylo vhodné a aby se dalo použít k motivaci využití. |

## <a name="which-mpn-do-i-choose"></a>Který MPN si vyberu?

V toku deklarace identity přidružení CPOR se zobrazí výzva k výběru MPN společnosti, který by se měl přidružit k práci, kterou na koncovém zákazníkovi připravujete. Vaše společnost může mít spoustu MPNs, z nichž některé můžou být zaregistrované v rámci motivačních programů, a další související s typem partnera, jako je FRP FastTrack. Tok deklarace identity CPOR identifikuje, které MPNs jsou zaregistrované v programu pro podnět, ale neupozorní vás, pokud se jedná o konkrétní partnerský typ MPN. Je důležité si vybrat správný MPN, abyste se vyhnuli nutnosti v budoucnu znovu vymáhat. Nárokování na nesprávný MPN může mít za následek zmeškaný zisk a finanční zisky.

Pokud si nejste jisti, který MPN chcete použít, obraťte se na svého globálního správce.

Pokud MPN, který chcete použít, není zaregistrované, můžete ho spravovat na [kartě Přehled pobídek](https://partner.microsoft.com/dashboard/incentives/enrollment/summary) (vyžaduje se přihlášení).

## <a name="choosing-a-product-vs-entering-a-subscription"></a>Výběr produktu a zadání předplatného

Když je produkt Dynamics deklarovaný a schválený, partner může zobrazit ID předplatného v samotné deklaraci CPOR přidružení. V případě, že je toto předplatné požadováno, je aktivní nebo ve stavu odkladu, ale může nastat čas, kdy předplatné skončí, a nové odběry bude nutné uplatnit v samostatné deklaraci CPOR přidružení.

## <a name="competing-claims"></a>Konkurenční deklarace

Pokud vytváříte deklaraci CPOR přidružení pro zákazníka a jejich produkty, které jsou už přidružené k jinému partnerovi, vaše deklarace prochází arbitráží:

1. Po vytvoření nového přidružení zákazníka Microsoft ověří podrobnosti o přidružení a zkontroluje správnost zadaného důkazu o provedení.

2. Pokud vy a jiný partner vyžádáte stejného zákazníka a produkt nebo zatížení, Microsoft zkontroluje dokumentaci k vykonání všech partnerů, aby určil, který partner se má schválit.

3. Od obou partnerů můžou být požadovány další informace, které by mohly způsobit zpoždění při zpracování žádosti o přidružení.

4. Vaše deklarace identity přidružení CPOR bude i nadále přezkoumána během pěti pracovních dnů, i když jeho stav může zůstat _pod kontrolou_ po delší dobu. K tomuto scénáři může dojít, když Microsoft spolupracuje s partnerem aktuálně vlastnícím produkt nebo úlohu. V případě, že se jedná o případ, budete upozorněni v části komentáře vaší deklarace. 

>[!IMPORTANT]
>Pokud budeme potřebovat další informace k ověření CPOR provádění (PoE), budeme vás kontaktovat v části komentáře deklarace identity CPOR.

## <a name="next-steps"></a>Další kroky

- [Začínáme s motivací](incentives-get-started-intro.md)
