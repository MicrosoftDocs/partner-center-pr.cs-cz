---
title: Registrace obchodů
ms.topic: article
ms.date: 06/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Když zaregistrujete obchod, který jste vyhráli v partnerském centru, pomůže vám to společnosti Microsoft v budoucnu s dalšími příležitostmi.
author: rajap-ms
ms.author: rajap
ms.localizationpriority: medium
ms.openlocfilehash: eaa9bb6f8e57033669ef584e7c52c0d050a532e0
ms.sourcegitcommit: 8235c89e789cdb5115fc1c19151fa8e97c743fe5
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/30/2021
ms.locfileid: "113080655"
---
# <a name="register-deals-youve-won-in-partner-center"></a>Zaregistrujte obchody, které jste vyhráli v partnerském centru

**Příslušné role**: Správce odkazů

Obchody, které jste vyhráli v partnerském centru, můžete zaregistrovat poskytnutím dalších informací o smlouvě. Tyto informace nám pomáhají zajistit další příležitosti v budoucnu.

Existují dvě cesty, které vedou k registraci koupě:

- V části **příležitosti společného prodeje** jste vytvořili novou práci a vaše koupě splňuje kritéria pro registraci obchodu.
- Chcete ohlásit uzavřenou práci nezávislého výrobce softwaru, která nebyla společně prodávana s Microsoftem.

## <a name="register-a-deal-originating-from-a-co-sell-opportunity"></a>Registrace obchodu pocházejícího z příležitosti společného prodeje

Pokud chcete zaregistrovat obchod pocházející z příležitosti společného prodeje, musí vaše koupě splňovat následující požadavky na způsobilost:

- Typ kouposti je buď společný prodej, nebo byl vyveden partner (Pokud jste se rozhodli, že chcete, aby si tuto práci mohli zobrazit i prodejci Microsoftu).
- V obchodu se nachází alespoň jedno řešení s nárokem na motivaci. Řešení je vhodné, pokud obsahuje alespoň jednu z následujících značek:
  - Azure IP – společný prodej
  - Business Applications Premium
  - Business Applications Standard
- Stav obchodu je "výhra".
- Pokud je typ kouposti spoluprodejní, společnost Microsoft musí buď přijmout pozvánku, nebo ji označit jako získanou. Stav společnosti Microsoft si můžete prohlédnout na kartě společnosti Microsoft pod podrobnostmi o vaší koupi.

Pokud jste splnili požadavky na způsobilost, budete automaticky vyzváni k registraci vašeho obchodu s tlačítkem **zaregistrovat nyní** , které se zobrazuje na řádku průběh práce:

:::image type="content" source="images/register-deals.png" alt-text="Snímek obrazovky znázorňující indikátor průběhu obchodu":::

> [!NOTE]
> Pokud se položka **registrace koupě** nezobrazuje na indikátoru průběhu obchodování pro vaši práci, nesplňuje obchod všechny požadavky na registraci koupek.

Po kliknutí na **zaregistrovat** se budete přesměrováni na stránku registrace koupě a zobrazí se výzva k vyplnění formuláře, který obsahuje předem vyplněné informace pro zákazníka a řešení. Vyplňte formulář podle pokynů níže a klikněte na **zaregistrovat**.

Po registraci se v závislosti na řešení vytvoří jeden nebo dva záznamy o registraci koupek.

- Pokud má vaše řešení nárok na nezávislé výrobce softwaru, vytvoří se záznam registrace prodejce ISV Connect. Tento záznam registrace koupě bude použit k fakturaci.
- Pokud má vaše řešení nárok na spoluprodejní pobídky, vytvoří se záznam o registraci služby IP v rámci společného prodeje. Tento záznam o registraci obchodu bude přezkoumán a schválen nebo odmítnut týmem pro kontrolu obchodu.

## <a name="report-a-closed-isv-connect-deal"></a>Vykázat uzavřenou práci nezávislého výrobce softwaru.

Pokud chcete ohlásit uzavřenou práci s nezávislým dodavatelem softwaru, přejděte na kartu **registrace** do práce a klikněte na **+ Sestava uzavřený ISV Connect**. Vyplňte požadovaná pole a klikněte na **zaregistrovat**. Tento záznam registrace koupě bude použit k fakturaci.

## <a name="fill-out-the-deal-registration-form"></a>Vyplnění formuláře registrace koupě

> [!NOTE]
> Můžete filtrovat obchody podle názvu zákazníka, stavu a typu rozdat. Provedete to tak, že kliknete na tlačítko **Filtr** v horní části stránky registrace do obchodu.

Bez ohledu na to, jestli jste se přihlásili k registraci ze společného prodeje, nebo když hlásíte uzavřenou koupi ISV Connect, která nebyla společně prodávana s Microsoftem, budete vyzváni, abyste do formuláře pro registraci koupě vyplnili tato pole.

- **Podrobnosti o zákazníkovi**: zadejte **název společnosti** pro zákazníka a vyberte svou **zemi/oblast**. Pak zadejte své **město** a **kraj**.
- **Řešení**: vyberte řešení, které se bude používat pro obchod. Pokud nevidíte správné řešení v seznamu, obraťte se na podporu.
- **Typ kontraktu**: Určete, jestli je tato koupě **novou** smlouvou nebo **obnovením** předchozí smlouvy.
- **Celková hodnota kontraktu**: celková očekávaná hodnota pro zapojení. Tato hodnota by měla zahrnovat všechny poplatky za software a služby, ale ne hardwarové náklady. Nezapomeňte vybrat příslušnou měnu.
- **Hodnota řešení**: celková hodnota cloudového řešení, které se bude používat pro obchod. Nezapomeňte zahrnout všechny náklady spojené s poplatky za software a údržbu, ale Nezahrnovat nenávratové položky, poplatky za vlastní nastavení nebo přímo přidružené licenční poplatky za CSP placené Microsoftem.
- **Bude řešení nasazeno v Azure? Pokud ne, zvolte jiný**: vyberte **Azure** nebo **jiné**.
- **Bude se spotřeba řešení spouštět v partnerském tenantovi nebo tenantovi zákazníka?**: vyberte **tenanta zákazníka** nebo **partnerský tenant**.
- **Počáteční datum smlouvy**: datum zahájení smlouvy. Pro obchody s průběžnými platbami (PAYG) použijte datum první faktury. V rámci návrhu se v partnerském centru neumožní zadat počáteční datum, které je dřívější než datum podpisu smlouvy. To může mít vliv na některé obchody, jako jsou například nasazení protokolu IP, která začínají před datem podpisu. Aby bylo možné tyto obchody úspěšně zadat, při odesílání použijte **Datum podpisu smlouvy pro pole** datum a čas zahájení. (Kontrakt by měl explicitně stanovit dobu trvání obchodu, aby bylo možné ACV správně vypočítat.)
- **Datum ukončení smlouvy**: Pokud bude smlouva ukončena na konkrétní datum, vyberte **má datum ukončení** a zadejte datum. Pokud kontrakt nemá konkrétní datum ukončení, vyberte možnost **trvalá**. V případě obchodů s průběžnými platbami (PAYG) použijte datum poslední nebo poslední faktury.
- **Datum podpisu smlouvy**: datum, kdy byl poslední kontrakt podepsán vaší organizací a zákazníkem. Pro obchody s průběžnými platbami (PAYG) použijte datum první faktury.
- **Kontakt na registraci**: **křestní jméno**, **příjmení**, **telefonní číslo** a **e-mail** pro osobu ve vaší organizaci, které můžeme kontaktovat, pokud potřebujeme další podrobnosti o jakékoli z informací, které tady poskytneme.

Po dokončení všech sekcí stránky klikněte na **zaregistrovat**.

- Pokud se jedná o koupi nezávislého výrobce softwaru, zjistíte, že stav obchodu je "odesláno, dokončeno". Pro tento záznam registrace koupě není vyžadována žádná další akce. Tento záznam bude použit k fakturaci.
- Pokud je obchod obchodem s IP adresami, můžete si všimnout, že stav obchodu je "odesláno". Tým recenze obchodu pro Microsoft spolupracuje s informacemi, které jste zadali na tomto záznamu registrace koupě. V případě potřeby si tým pro kontrolu vyžádá další akci, nebo přímo schválí nebo odmítne obchod.
- Pokud zaregistrujete obchod pocházející z příležitosti společného prodeje a vidíte, že byly vytvořeny dva záznamy registrace koupě, znamená to, že řešení na základě vaší práce je vhodné pro nezávislé výrobce softwaru (ISV) i pro souběžný prodej. Záznam ISV Connect bude použit k fakturaci. Záznam o společném prodeji protokolu IP bude přezkoumán týmem pro ověření koupě.

