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
ms.openlocfilehash: 8f1c087911e6dd7e58182c99e2b97b7a6b2246d8
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152167"
---
# <a name="issues-with-claimed-partner-of-record-cpor-customer-associations"></a>Problémy s deklarovaným partnerem pro zákazníky záznamů (CPOR)

**Příslušné role**: správce fakturace | Globální správce | Motivace správce

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

Při deklaracích identity pro předplatné se zobrazí chyba, pokud předplatné ještě není zřízené. K dispozici je několik kroků, které zákazník potřebuje k tomu, aby předplatné mohlo být dostupné pro platformu CPOR, aby ji bylo možné vybrat a zpřístupnit. Pokud se vám při pokusu o deklaraci předplatného zobrazí chyba, obraťte se na zákazníka a ujistěte se, že je zřízené a že předplatné, o které se pokoušíte, je správné. Pokud jste tuto trasu už probrali, kontaktujte [podporu](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="which-activity-do-i-choose"></a>Kterou aktivitu mám zvolit?

Platforma CPOR pro nárokování umožňuje žádosti o přidružení CPOR související s Business Applications a Microsoft 365 oblastmi řešení. Aktivity, které se vztahují na jednotlivé oblasti řešení, jsou uvedené níže. Na základě popisů vyberte správnou aktivitu, abyste se vyhnuli budoucímu opětovnému získání. Nárok na nesprávnou aktivitu může mít za následek vynechání způsobilosti a příjmů v rámci pobídek.


| Oblast řešení | Aktivita | Platí pro |
| ------ | ----------- | ----------- |
| Obchodní aplikace      | Předprodej   | Tuto možnost vyberte, pokud jste ovlivnili nákup způsobilého produktu a chcete požádat o pobídky před prodejem. Tato možnost je platná jenom v případě, že zákazník tyto produkty zakoupil prostřednictvím multilicenční smlouvy nebo programu Web-Direct. |
|    |  Využití  | Tuto možnost vyberte, pokud chcete řídit jejich přijetí a využití oprávněné úlohy a chcete požádat o pobídky využití. Tato možnost je platná jenom v případě, že zákazník tyto produkty zakoupil prostřednictvím multilicenční smlouvy nebo programu Web-Direct. |
|    | Revenue association   | Tuto možnost vyberte, pokud jste ovlivnili výběr vhodného produktu jako obchodního vlivového. Tato možnost se používá pouze pro přidružení výnosů, nikoli pro platby v rámci pobídek. Tato možnost je platná jenom v případě, že zákazník tyto produkty zakoupil prostřednictvím multilicenční smlouvy nebo programu Web-Direct.   |
| Microsoft 365   | Využití   | Tuto možnost vyberte, pokud chcete řídit jejich přijetí a využití oprávněné úlohy a chcete požádat o pobídky využití. |

## <a name="which-mpn-do-i-choose"></a>Které MPN zvolím?

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

4. Vaše deklarace identity přidružení CPOR bude i nadále přezkoumána během pěti pracovních dnů, i když jeho stav může zůstat _pod kontrolou_ po delší dobu. K tomuto scénáři může dojít, když Microsoft spolupracuje s partnerem aktuálně vlastnícím produkt nebo úlohu. V takovém případě budete upozorněni v části komentáře vaší žádosti. 

>[!IMPORTANT]
>Pokud k ověření důkazu o provedení přidružení CPOR potřebujeme další informace, budeme vás kontaktovat v části Komentáře k žádosti o přidružení CPOR.

## <a name="next-steps"></a>Další kroky

- [Začínáme s pobídkami](incentives-get-started-intro.md)
