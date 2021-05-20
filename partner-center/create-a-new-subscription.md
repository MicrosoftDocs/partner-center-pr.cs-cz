---
title: Vytváření zákaznických předplatných v Partnerské centrum
ms.topic: how-to
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Zjistěte, jak zákazníkům prodávat předplatná pro produkty publikované Microsoftem i produkty SaaS publikované výrobcem softwaru třetích stran.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 9052954c81ef55a2bfa06778ace651c9d0f9b26f
ms.sourcegitcommit: e0444145d7720df948b9d02ae2469206db48dba5
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110201404"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Vytváření, pozastavování nebo rušení zákaznických předplatných

**Platí pro**: Partnerské centrum | Partnerské centrum pro Microsoft Cloud for US Government

**Odpovídající role:** Agent pro správu | Správce fakturace | Globální správce | Agent helpdesku | Agent prodeje

Po vytvoření záznamu zákazníka v katalogu Partnerské centrum můžete prodávat předplatná produktů v katalogu. To zahrnuje produkty publikované společností Microsoft a produkty SaaS (software jako služba), které publikovali nezávislí dodavatelé softwaru (ISV) třetích stran na [komerčním marketplace.](https://azuremarketplace.microsoft.com/marketplace)

Některé nabídky jsou omezené na jedno předplatné na zákazníka. Pokud chcete zobrazit seznam nabídek, které jsou omezené, přejděte na Partnerské centrum Ceny a nabídky.

>[!IMPORTANT]
> Jako partner v programu CSP můžete  zakoupit předplatná **SaaS** založená na licencích nebo na základě měření od vydavatelů ISV v rámci Partnerské centrum. To znamená, že si můžete zakoupit jakoukoli **nabídku** **SaaS** založenou na [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) licencích nebo na základě měření, kterou vám vydavatel ISV nabízí, včetně výhradních nabídek, ke kterým máte přístup. Pokud chcete nakupovat nebo spravovat jiné nabídky na komerčním marketplace od isv (například nabídky založené na využití zahrnující aplikace Azure, kontejnery nebo virtuální počítače), musíte přejít na [web Azure Portal](https://portal.azure.com/).

>[!NOTE]
>Všechna data a časy v Partnerské centrum jsou uvedeny v časovém standardu UTC (Universal Time Coordinated). To se může lišit až o 24 hodin od místního času.

## <a name="create-a-new-subscription"></a>Vytvoření nového předplatného

1. Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard).

2. V Partnerské centrum vyberte **Zákazníci** a pak v seznamu zvolte zákazníka.

3. Vyberte **Přidat předplatné.** Na **kartě Online služby** se zobrazí všechny dostupné nabídky SaaS na Marketplace.

4. Pokud chcete zobrazit pouze určité typy předplatných, proveďte výběr v dostupných filtrech:
   - **Vydavatel**: vyberte **Microsoft** , pokud chcete zobrazit jenom nabídky od Microsoftu nebo **partnera** , aby viděli produkty z komerčního tržiště publikované prostřednictvím nezávislého výrobce softwaru.
   - **Typ fakturace**: Vyberte typ fakturace předplatného, který chcete použít: **licence** nebo **použití**. Informace, které vám pomůžou při rozhodování mezi měsíční a roční frekvencí fakturace, najdete v tématu [fakturace na základě licencí](license-based-billing.md) .
   - **Kategorie**: vyberte **podnik**, **malý podnik** nebo **zkušební verzi**. Informace o zkušebních předplatných najdete v tématu [Nabídka vašich zákazníků s zkušebními produkty Microsoftu](offer-your-customers-trials-of-microsoft-products.md).

5. Vyberte předplatné produktů, které chcete pro zákazníka koupit. Produkty, které vidíte, závisí na typu segmentu zákazníka (vzdělávání, státní správa atd.) a na použitých filtrech. Některé nabídky zobrazené na webu Marketplace nemusí být vždy dostupné konkrétnímu zákazníkovi nebo konkrétnímu partnerovi CSP. To může být způsobeno tím, že:

   - Zákazník už má k tomuto produktu předplatné a je povolený jenom jeden.

   - Předplatné zákazníka může být pozastavené (v takovém případě můžete předplatné znovu aktivovat, ale nekoupit nové).

   - V případě nabídek ISV SaaS může být nabídka k dispozici z několika důvodů k zakoupení: ISV nemusí podporovat fakturační zemi nebo oblast zákazníka; nezávislý výrobce softwaru se možná rozhodl, že nabídku zpřístupní prostřednictvím programu CSP. nebo nezávislý výrobce softwaru mohl vytvořit nabídku [výhradně](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) pro určité partnery CSP. Nabídku ISV nelze také využít v partnerském centru (například v kontejnerech nebo v některých nabídkách založených na používání).  

6. U každého předplatného, které chcete přidat, zadejte počet licencí (v případě potřeby) a vyberte **Přidat do košíku**.

7. Až skončíte s přidáváním předplatných, vyberte **zkontrolovat** a zkontrolovat vaši objednávku.

8. Po kontrole objednávek a jejich přípravě na nákup můžete vybrat **koupit**.

9. Po zakoupení předplatného pro zákazníka dojde k následujícímu:

    - Předplatné můžete zkontrolovat nebo upravit výběrem názvu předplatného na stránce **Předplatná** tohoto zákazníka. Tady můžete vybrat případné licence doplňků, změnit jejich počet nebo předplatné pozastavit.

    **Pro předplatná ISV SaaS (založená na licencích a na základě měření):**
    - Zobrazí se odkaz na web vydavatele ISV. Tento odkaz by vám měl pomoct dokončit nasazení nebo nastavení účtu předplatného zákazníka.
      
    >[!NOTE]
    > Ani vy ani váš zákazník neobdržíte e-mail s pokyny k dokončení nastavení nebo zřízení účtu pro tento typ předplatného ISV.)

    - Pokud se vaše předplatné dodává s 30denní bezplatnou zkušební verzí, automaticky se použije bezplatné zkušební období. Jako partner v programu CSP se nemůžete u nabídek, které si koupíte pro zákazníky, uchýlíte bezplatné zkušební období. Po uplynutí bezplatné zkušební doby začne období předplatného a předplatné se převede na placený stav. Předplatné se pak automaticky prodlužuje podle stejného plánu.
   
## <a name="update-subscriptions-with-add-ons"></a>Aktualizace předplatných o doplňky 

Pokud si zákazník chcete koupit doplněk, musí nejprve mít aktivní základní předplatné.  Doplňky není možné kupovat prostřednictvím katalogu.

1. Přihlaste se k Partnerské centrum [řídicího panelu.](https://partner.microsoft.com/dashboard)

2. V Partnerské centrum vyberte **Zákazníci** a pak v seznamu zvolte zákazníka.

3. Zvolte předplatné, které chcete spravovat.

4. Pod **částí Stav** je seznam dostupných doplňků pro předplatné.  

5. Aktualizujte počet licencí pro každý požadovaný doplněk. Pak změny **odešlete**.

Možnost nákupu doplňků prostřednictvím služby Partnerské centrum k dispozici pouze pro přímé vyúčtování a nepřímé poskytovatele.
V závislosti na základních požadavcích a regionální dostupnosti se zobrazí pouze oprávněné doplňky. Další informace o cenách a nabídkách najdete v matici nabídek cloudových prodejců. Pozastavením základního předplatného se pozastaví také všechny přidružené doplňky.

Počáteční datum doplňků odpovídá základnímu předplatnému a poplatky se u první faktury účtují poměrně a následně se účtují na základě počátečního a koncového data účtování poplatků. Další informace najdete v tématu [Fakturace na základě licencí.](license-based-billing.md)


## <a name="suspend-or-cancel-a-subscription"></a>Pozastavení nebo zrušení předplatného

Partneři můžou předplatné pozastavit nebo zrušit, pokud ho požaduje zákazník nebo v případě nedoplatku nebo podvodu.

### <a name="suspend-a-subscription"></a>Pozastavení předplatného

Když změníte stav předplatného na **pozastaveno**, uživatelé se nebudou moct přihlašovat ani získat přístup ke službám.

1. Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.

2. V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.

3. Vyberte předplatné, které chcete spravovat.

4. V části **Stav** zvolte **Pozastaveno**. Pak změny **odešlete**.

5. Všechna data budou odstraněna, pokud předplatné nebude znovu aktivováno během 90 dnů nebo 90 dnů plus počet dní mezi časem otevření účtu a prvním fakturačním obdobím (maximum 120 dní).

Když pozastavíte předplatné, datum zobrazené pod tlačítkem **pozastavit** indikuje, kdy by předplatné automaticky vyprší, pokud ho znovu neaktivujete. 

>[!NOTE]
>Předplatné CSP neobsahují dobu platnosti (způsobující předplatná na webu), během které služby stále fungují, ale předplatné negeneruje žádné fakturační poplatky. Odběry CSP jsou aktivní nebo pozastavené (nebo zcela odstraněny).

### <a name="cancel-a-subscription"></a>Zrušení předplatného

Předplatné SaaS na základě licencí můžete zrušit od třetích stran vydavatelů ISV v rámci [obchodního tržiště](csp-commercial-marketplace-overview.md)partnerského centra. Pokud zrušíte v rámci období zrušení, obdržíte plnou refundaci.

U nezávislých výrobců softwaru nabízíme fakturaci za měsíc:

- Pokud po umístění objednávky zrušíte méně než 24 hodin, obdržíte na další faktuře celý kredit.

- Pokud zrušíte pozdější dobu než 24 hodin od okamžiku, kdy jste objednávku nastavili, zrušení se naplánuje při obnovení.

Pro nabídky účtované ročně:

- Pokud po umístění objednávky zrušíte méně než 14 dní, obdržíte na další faktuře celý kredit.

- Pokud zrušíte akci později než 14 dní po umístění objednávky, zrušení se naplánuje při obnovení.

Po uplynutí těchto období se už nebude zobrazovat možnost zrušit předplatné.

> [!NOTE]
> Služby isv třetích stran založené na využití a na základě měření (které například používají virtuální počítače nebo kontejnery) nemají nárok na vrácení. Služby založené na využití je možné zrušit jako metodu zrušení. Vzhledem k tomu, že se poplatky účtují po použití, nemají tyto služby nárok na refundaci.

Pokud chcete zrušit předplatné SaaS založené na licencích od vydavatele ISV, postupujte následovně:

1. Přihlaste se k Partnerské centrum [řídicího panelu.](https://partner.microsoft.com/dashboard)

2. V Partnerské centrum vyberte **Zákazníci** a pak v seznamu zvolte zákazníka.

3. Vyhledejte předplatné, které chcete zrušit.

4. Ve **sloupci Stav** vyberte **Zrušit.** Pak změny **odešlete**.

5. Pokud se zobrazí dialogové okno, vyplňte všechny relevantní podrobnosti a pak vyberte **Odeslat.**

6. Zrušení potvrdíte výběrem **možnosti Ano, zrušit**.

> [!NOTE]
> Můžete se také rozhodnout zrušit předplatné Azure Marketplace pomocí rozhraní API. Pokud to chcete udělat, podívejte [se na Azure Marketplace předplatného.](/partner-center/develop/cancel-an-azure-marketplace-subscription)

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>Zvolte, jestli se má předplatné komerčního marketplace automaticky obnovit.

Ve výchozím nastavení jsou aktivní předplatná nastavená tak, aby se při vypršení jejich časového limitu automaticky prodlužovala jejich platnost. U [předplatných produktů komerčního marketplace](csp-commercial-marketplace-overview.md)můžete volitelně zvolit, že se předplatné automaticky neobnoví.

Pokud chcete zabránit automatickému prodlužování platnosti aktivního předplatného komerčního marketplace:

1. Přihlaste se k Partnerské centrum [řídicího panelu.](https://partner.microsoft.com/dashboard)

2. V Partnerské centrum vyberte **Zákazníci** a pak v seznamu zvolte zákazníka.

3. Vyberte **Předplatná**. Zobrazí se seznam všech předplatných založených na licencích, která jste pro zákazníka zakoupili.

4. Ve **sloupci Předplatné** vyberte předplatné, které chcete upravit.

5. Na stránce s podrobnostmi o předplatném vyhledejte **část Stav** a zrušte zaškrtnutí políčka **Automatické prodloužení platnosti.**

6. Vyberte **Odeslat**.

## <a name="next-steps"></a>Další kroky

- [Nákup produktů komerčního marketplace pro vaše zákazníky](csp-commercial-marketplace-purchase.md)

- [Správa produktů z komerčního tržiště pro vaše zákazníky](csp-commercial-marketplace-manage.md)

- [Přehled komerčního marketplace](csp-commercial-marketplace-overview.md)