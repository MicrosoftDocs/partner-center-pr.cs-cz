---
title: Vytváření zákaznických předplatných v partnerském centru
ms.topic: how-to
ms.date: 05/17/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si, jak prodávat předplatná vašim zákazníkům pro produkty publikované Microsoftem a také pro produkty SaaS publikované třetí stranou nezávislého výrobce softwaru.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 3269fa994d704c0a0dae067087bad8589a7ce031
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148190"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Vytváření, pozastavování nebo rušení zákaznických předplatných

**Platí pro**: partnerské Centrum | Partnerské centrum pro Microsoft Cloud pro státní správu USA

**Příslušné role**: Agent správce | Správce fakturace | Globální správce | Agent helpdesku | Agent prodeje

Až vytvoříte záznam o zákazníkovi v partnerském centru, můžete si ho prodávat do produktů v katalogu. To zahrnuje produkty publikované produkty Microsoft a software jako služba (SaaS), které publikovali nezávislí výrobci softwaru (ISV) třetích stran na [komerčním tržišti](https://azuremarketplace.microsoft.com/marketplace).

Některé nabídky jsou omezené na jedno předplatné na zákazníka. Pokud chcete zobrazit seznam nabídek, které jsou omezené, navštivte stránku ceny a nabídky partnerského centra.

>[!IMPORTANT]
> Jako partner v programu CSP si můžete koupit předplatné SaaS **založené na licencích** nebo **účtované podle objemu** od vydavatelů ISV v partnerském centru. To znamená, že si můžete koupit jakoukoli nabídku **založenou na licencích** nebo **měřený** SaaS. Vydavatel ISV vám k dispozici, včetně [exkluzivních nabídek](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) , ke kterým máte přístup. Pokud si chcete koupit nebo spravovat jiné komerční nabídky na webu Marketplace od nezávislého výrobce softwaru (jako jsou nabídky na základě využití zahrnující aplikace a kontejnery Azure), musíte přejít na [Azure Portal](https://portal.azure.com/).

## <a name="create-a-new-subscription"></a>Vytvoření nového předplatného

1. Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard).

2. V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.

3. Vyberte **přidat odběr**. Na kartě **online služby** se zobrazí všechny dostupné nabídky SaaS Marketplace.

4. Chcete-li zobrazit pouze určité typy předplatných, proveďte výběr v dostupných filtrech:
   - **Vydavatel**: vyberte **Microsoft** , pokud chcete zobrazit jenom nabídky od Microsoftu nebo **partnera** , aby viděli produkty z komerčního tržiště publikované prostřednictvím nezávislého výrobce softwaru.
   - **Typ fakturace**: Vyberte typ fakturace předplatného, který chcete použít: **licence** nebo **použití**. Informace, [které vám pomůžou](license-based-billing.md) s rozhodováním mezi měsíční a roční frekvencí fakturace, najdete v tématu Fakturace na základě licencí.
   - **Kategorie:** Zvolte **Enterprise**, **Small business** nebo **Trial**. Informace o zkušebních předplatných najdete v tématu [Nabídka zkušebních verzí produktů Microsoftu zákazníkům.](offer-your-customers-trials-of-microsoft-products.md)

5. Vyberte předplatná produktů, která chcete pro zákazníka zakoupit. Produkty, které se zobrazí, závisí na typu segmentu zákazníků (vzdělávání, státní správa atd.) a použitých filtrech. Některé nabídky zobrazené na Marketplace nemusí být vždy dostupné konkrétnímu zákazníkovi nebo konkrétnímu partnerovi CSP. Může to být proto, že:

   - Zákazník už má předplatné tohoto produktu a má povolené jenom jedno.

   - Předplatné zákazníka může být pozastavené (v tomto případě můžete předplatné znovu aktivovat a nekupovat nové).)

   - U nabídek SaaS od isv může být několik důvodů, proč není možné nabídku koupit: Tento isv nemusí podporovat fakturační zemi nebo oblast zákazníka. Je možné, že se isV rozhodl nabídku nezvolovat prostřednictvím programu CSP. nebo může isv made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners. Nabídku isv také není možné provádět prostřednictvím Partnerské centrum (například kontejnery nebo některé nabídky založené na využití).  

6. Pro každé předplatné, které chcete přidat, zadejte počet licencí (v případě potřeby) a vyberte **Přidat do košíku.**

7. Až přidávání předplatných dokončíte, vyberte **Zkontrolovat** a zkontrolovat objednávku.

8. Jakmile si prošete objednávky a jste připravení si tato předplatná koupit, vyberte **Koupit.**

9. Po zakoupení předplatného pro zákazníka dojde k těmto akcím:

    - Předplatné můžete zkontrolovat nebo upravit výběrem názvu předplatného na stránce **Předplatná** tohoto zákazníka. Tady můžete vybrat případné další licence, změnit jejich počet nebo předplatné pozastavit.

    **Pro předplatná ISV SaaS (založená na licencích a na základě měření):**
    - Zobrazí se odkaz na web vydavatele ISV. Tento odkaz by vám měl pomáhat s dokončením nastavení nasazení nebo účtu u předplatného zákazníka.
      
    >[!NOTE]
    > Ani vy ani váš zákazník neobdrží e-mail s pokyny k dokončení nastavení/zřizování pro tento typ předplatného ISV.)

    - Pokud vaše předplatné předchází 30denní bezplatnou zkušební verzi, použije se k automatickému vyzkoušení bezplatné zkušební období. Jako partner v programu CSP se nemůžete vzdát bezplatné zkušební doby pro nabídky, které zakoupíte pro zákazníky. Po skončení bezplatné zkušební doby se předplatné spustí a předplatné se převede na placený stav. Předplatné se pak automaticky obnoví podle stejného plánu.
   
## <a name="update-subscriptions-with-add-ons"></a>Aktualizace předplatných o doplňky 

K nákupu doplňku musí zákazník nejdřív mít aktivní základní předplatné.  Doplňky není možné kupovat prostřednictvím katalogu.

1. Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.

2. V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.

3. Vyberte předplatné, které chcete spravovat.

4. Pod oddílem **stav** je seznam dostupných doplňků pro předplatné.  

5. Aktualizujte množství licencí pro každý požadovaný doplněk. Pak změny **odešlete**.

Možnost zakoupit doplňky prostřednictvím partnerského centra je dostupná jenom pro přímé faktury a nepřímé poskytovatele.
Na základě základních požadavků a regionální dostupnosti se zobrazují jenom opravňující doplňky. Další informace o cenách a nabídkách najdete v tématu matice nabídky prodejce cloudu. Pozastavením základního předplatného se pozastaví také všechny přidružené doplňky.

Počáteční datum doplňků odpovídá základnímu předplatnému a poplatky se u první faktury účtují poměrně a následně se účtují na základě počátečního a koncového data účtování poplatků. Další informace najdete v tématu [fakturace na základě licencí](license-based-billing.md).


## <a name="suspend-or-cancel-a-subscription"></a>Pozastavení nebo zrušení předplatného

Partneři můžou předplatné pozastavit nebo zrušit, pokud ho požaduje zákazník nebo v případě nedoplatku nebo podvodu.

### <a name="suspend-a-subscription"></a>Pozastavení předplatného

Když změníte stav předplatného na **pozastaveno**, uživatelé se nebudou moct přihlašovat ani získat přístup ke službám.

1. Přihlaste se k řídicímu [Partnerské centrum.](https://partner.microsoft.com/dashboard)

2. V Partnerské centrum vyberte **Zákazníci** a pak v seznamu zvolte zákazníka.

3. Zvolte předplatné, které chcete spravovat.

4. V části **Stav** zvolte **Pozastaveno**. Pak změny **odešlete**.

5. Všechna data se odstraní, pokud se předplatné znovu neaktivuje do 90 dnů nebo 90 dnů plus počet dní mezi časem otevření účtu a prvním fakturačním obdobím (maximálně 120 dnů).

Když předplatné pozastavíte, datum, které se zobrazí pod tlačítkem **Pozastaveno,** značí, kdy automaticky vyprší platnost předplatného, pokud ho znovu neaktivujete. 

>[!NOTE]
>Předplatná CSP nemají prošlé období (stejně jako předplatná s přímým přístupem na web), během kterého služby stále fungují, ale předplatné negeneruje žádné poplatky za fakturaci. Předplatná CSP jsou aktivní nebo pozastavená (nebo úplně odstraněná).

### <a name="cancel-a-subscription"></a>Zrušení předplatného

Předplatná SaaS založená na licencích můžete zrušit od vydavatelů ISV třetích stran v rámci Partnerské centrum [komerčního marketplace.](csp-commercial-marketplace-overview.md) Pokud zrušíte v rámci období zrušení, obdržíte úplnou refundaci.

Nabídky isv fakturované měsíčně:

- Pokud zrušíte méně než 24 hodin od vystavení objednávky, obdržíte úplný kredit na další faktuře.

- Pokud ji zrušíte později než 24 hodin po vystavení objednávky, bude zrušení naplánováno na prodloužení.

Pro nabídky fakturované ročně:

- Pokud zrušíte méně než 14 dnů od vystavení objednávky, obdržíte úplný kredit na další faktuře.

- Pokud objednávku zrušíte později než 14 dnů od vystavení objednávky, bude zrušení naplánováno na prodloužení.

Po uplynutí těchto období se už možnost zrušení předplatného nebude zobrazit.

> [!NOTE]
> Služby isv třetích stran založené na využití a na základě měření (které například používají virtuální počítače nebo kontejnery) nemají nárok na vrácení. Služby založené na využití je možné zrušit jako metodu zrušení. Vzhledem k tomu, že se poplatky účtují po použití, nemají tyto služby nárok na refundaci.

Pokud chcete zrušit předplatné SaaS založené na licencích od vydavatele ISV, postupujte následovně:

1. Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.

2. V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.

3. Vyhledejte předplatné, které chcete zrušit.

4. Ve sloupci **stav** vyberte **Zrušit**. Pak změny **odešlete**.

5. Pokud se zobrazí dialogové okno, vyplňte příslušné podrobnosti a pak vyberte **Odeslat**.

6. Zrušení potvrďte tak, že vyberete **Ano, zrušit**.

> [!NOTE]
> Můžete také zvolit zrušení předplatného Azure Marketplace pomocí rozhraní API. Pokud to chcete udělat, přečtěte si téma [zrušení předplatného Azure Marketplace](/partner-center/develop/cancel-an-azure-marketplace-subscription).

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>Vyberte, jestli se má automaticky obnovit předplatné z komerčního tržiště.

Ve výchozím nastavení jsou aktivní předplatná nastavená tak, aby se při vypršení jejich časového limitu automaticky prodlužovala jejich platnost. Pro [odběry komerčních produktů na webu Marketplace](csp-commercial-marketplace-overview.md)můžete volitelně zvolit automatické obnovení předplatného.

Pokud chcete zastavit aktivní předplatné komerčního tržiště z automatického obnovování:

1. Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.

2. V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.

3. Vyberte **Předplatná**. Obsahuje seznam všech předplatných založených na licencích, které jste zakoupili pro zákazníka.

4. Ve sloupci **předplatné** vyberte předplatné, které chcete upravit.

5. Na stránce Podrobnosti předplatného vyhledejte část **stav** a zrušte kontrolu **automatického obnovení** .

6. Vyberte **Odeslat**.

## <a name="next-steps"></a>Další kroky

- [Nákup produktů z komerčního tržiště pro vaše zákazníky](csp-commercial-marketplace-purchase.md)

- [Správa produktů z komerčního tržiště pro vaše zákazníky](csp-commercial-marketplace-manage.md)

- [Přehled komerčního marketplace](csp-commercial-marketplace-overview.md)