---
title: Vytváření zákaznických předplatných v partnerském centru
ms.topic: how-to
ms.date: 07/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Naučte se prodávat předplatné vašich zákazníků k produktům publikovaným společností Microsoft a produktům SaaS zveřejněným nezávislým výrobcům softwaru.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 8c3cfc2a6576029a8fdfb902a7b3889b4ea6c628
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/22/2020
ms.locfileid: "92527583"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Vytváření, pozastavování nebo rušení zákaznických předplatných

**Platí pro**

- Partnerské centrum
- Partnerské centrum pro Microsoft Cloud pro státní správu USA
- Partneři CSP

**Příslušné role**

- Agent správce
- Správce fakturace
- Globální správce
- Agent helpdesku
- Agent prodeje

Až vytvoříte záznam o zákazníkovi v partnerském centru, můžete si ho prodávat do produktů v katalogu. To zahrnuje produkty publikované společností Microsoft i produkty SaaS (software jako služba), které publikovali nezávislí výrobci softwaru (ISV) třetích stran na [komerčním tržišti](https://azuremarketplace.microsoft.com/marketplace).

Některé nabídky jsou omezené na jedno předplatné na zákazníka. Pokud chcete zobrazit seznam nabídek, které jsou omezené, navštivte stránku ceny a nabídky partnerského centra.

> [!IMPORTANT]
> Jako partner v programu CSP můžete zakoupit jenom SaaS odběry **založené na licencích** od vydavatelů ISV v partnerském centru. To znamená, že si můžete koupit jakoukoli nabídku SaaS **založenou na licencích** , kterou vám vydavatel ISV zpřístupnila, včetně [exkluzivních nabídek](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) , ke kterým máte přístup. Pokud si chcete koupit nebo spravovat jiné komerční nabídky na webu Marketplace od nezávislého výrobce softwaru (jako jsou nabídky na základě **využití** , měřené nebo spotřebované na základě spotřeby zahrnující aplikace, kontejnery nebo virtuální počítače Azure), musíte přejít na [portál pro správu Azure](https://portal.azure.com/). Další informace najdete v tématu [Nákup produktů z komerčního tržiště](csp-commercial-marketplace-purchase.md).

## <a name="create-a-new-subscription"></a>Vytvoření nového předplatného

1. Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard).

2. V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.

3. Vyberte **přidat odběr** . Na kartě **online služby** se zobrazí všechny dostupné nabídky SaaS Marketplace.

4. Chcete-li zobrazit pouze určité typy předplatných, proveďte výběr v dostupných filtrech:
   - **Vydavatel** : vyberte **Microsoft** , pokud chcete zobrazit jenom nabídky od Microsoftu nebo **partnera** , aby viděli produkty z komerčního tržiště publikované prostřednictvím nezávislého výrobce softwaru.
   - **Typ fakturace** : Vyberte typ fakturace předplatného, který chcete použít: **licence** nebo **použití** . Informace, které vám pomůžou při rozhodování mezi měsíční a roční frekvencí fakturace, najdete v tématu [fakturace na základě licencí](license-based-billing.md) .
   - **Kategorie** : vyberte **podnik** , **malý podnik** nebo **zkušební verzi** . Informace o zkušebních předplatných najdete v tématu [Nabídka vašich zákazníků s zkušebními produkty Microsoftu](offer-your-customers-trials-of-microsoft-products.md).

5. Vyberte předplatné produktů, které chcete pro zákazníka koupit. Produkty, které vidíte, závisí na typu segmentu zákazníka (vzdělávání, státní správa atd.) a na použitých filtrech. Některé nabídky zobrazené na webu Marketplace nemusí být vždy dostupné konkrétnímu zákazníkovi nebo konkrétnímu partnerovi CSP. To může být způsobeno tím, že:

   - Zákazník už má k tomuto produktu předplatné a je povolený jenom jeden.

   - Předplatné zákazníka může být pozastavené (v takovém případě můžete předplatné znovu aktivovat, ale nekoupit nové).

   - V případě nabídek ISV SaaS může být nabídka k dispozici z několika důvodů k zakoupení: ISV nemusí podporovat fakturační zemi nebo oblast zákazníka; nezávislý výrobce softwaru se možná rozhodl, že nabídku zpřístupní prostřednictvím programu CSP. nebo nezávislý výrobce softwaru mohl vytvořit nabídku [výhradně](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) pro určité partnery CSP. Nabídku ISV nelze také využít v partnerském centru (například v kontejnerech nebo v některých nabídkách založených na používání).  

6. U každého předplatného, které chcete přidat, zadejte počet licencí (v případě potřeby) a vyberte **Přidat do košíku** .

7. Až skončíte s přidáváním předplatných, vyberte **zkontrolovat** a zkontrolovat vaši objednávku.

8. Po kontrole objednávek a jejich přípravě na nákup můžete vybrat **koupit** .

9. Po zakoupení předplatného pro zákazníka dojde k následujícímu:

    - Předplatné můžete zkontrolovat nebo upravit výběrem názvu předplatného ze stránky **předplatné** daného zákazníka. Tady můžete vybrat licence pro doplňky, pokud jsou k dispozici, změnit množství licencí nebo pozastavit předplatné.

    **Pro předplatná ISV SaaS (založená na licencích):**
    - Zobrazí se odkaz na web vydavatele ISV. Tento odkaz by vám měl pomáhat s dokončením nastavení nasazení nebo účtu u předplatného zákazníka.
      
    >[!NOTE]
    > Ani vy ani váš zákazník neobdrží e-mail s pokyny k dokončení nastavení/zřizování pro tento typ předplatného ISV.)

    - Pokud vaše předplatné předchází 30denní bezplatnou zkušební verzi, použije se k automatickému vyzkoušení bezplatné zkušební období. Jako partner v programu CSP se nemůžete vzdát bezplatné zkušební doby pro nabídky, které zakoupíte pro zákazníky. Po skončení bezplatné zkušební doby se předplatné spustí a předplatné se převede na placený stav. Předplatné se pak automaticky obnoví podle stejného plánu.
   
## <a name="update-subscriptions-with-add-ons"></a>Aktualizace předplatných o doplňky 

Aby si zákazník mohl koupit doplněk, musí nejprve mít aktivní základní předplatné.  Doplňky není možné kupovat prostřednictvím katalogu.

1. Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.

2. V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.

3. Vyberte předplatné, které chcete spravovat.

4. Pod oddílem **stav** je seznam dostupných doplňků pro předplatné.  

5. Aktualizujte množství licencí pro každý požadovaný doplněk. Pak změny **odešlete** .

Možnost zakoupit doplňky prostřednictvím partnerského centra je dostupná jenom pro přímé faktury a nepřímé poskytovatele.
Na základě základních požadavků a regionální dostupnosti se zobrazují jenom opravňující doplňky. Další informace o cenách a nabídkách najdete v tabulce nabídek pro prodejce cloudových řešení.  Pozastavením základního předplatného se pozastaví také všechny přidružené doplňky.

Počáteční datum doplňků odpovídá základnímu předplatnému a poplatky se u první faktury účtují poměrně a následně se účtují na základě počátečního a koncového data účtování poplatků. Další informace najdete v tématu [fakturace na základě licencí](license-based-billing.md).


## <a name="suspend-or-cancel-a-subscription"></a>Pozastavení nebo zrušení předplatného

Partneři můžou předplatné pozastavit nebo zrušit, pokud ho požaduje zákazník nebo v případě nedoplatku nebo podvodu.

### <a name="suspend-a-subscription"></a>Pozastavení předplatného

Když změníte stav předplatného na **pozastaveno** , uživatelé se nebudou moct přihlašovat ani získat přístup ke službám.

1. Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.

2. V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.

3. Vyberte předplatné, které chcete spravovat.

4. V části **Stav** zvolte **Pozastaveno** . Pak změny **odešlete** .

5. Všechna data budou odstraněna, pokud předplatné nebude znovu aktivováno během 90 dnů nebo 90 dnů plus počet dní mezi časem otevření účtu a prvním fakturačním obdobím (maximum 120 dní).

Když pozastavíte předplatné, datum zobrazené pod tlačítkem **pozastavit** indikuje, kdy by předplatné automaticky vyprší, pokud ho znovu neaktivujete. 

### <a name="cancel-a-subscription"></a>Zrušení předplatného

Máte možnost zrušit si předplatné SaaS založené na licencích od třetích stran vydavatelů ISV v rámci [obchodního tržiště](csp-commercial-marketplace-overview.md)partnerského centra. Pokud zrušíte v rámci období zrušení, obdržíte plnou refundaci.

U nezávislých výrobců softwaru nabízíme fakturaci za měsíc:

- Pokud po umístění objednávky zrušíte méně než 24 hodin, obdržíte na další faktuře celý kredit.

- Pokud zrušíte pozdější dobu než 24 hodin od okamžiku, kdy jste objednávku nastavili, zrušení se naplánuje při obnovení.

Pro nabídky účtované ročně:

- Pokud po umístění objednávky zrušíte méně než 14 dní, obdržíte na další faktuře celý kredit.

- Pokud zrušíte akci později než 14 dní po umístění objednávky, zrušení se naplánuje při obnovení.

Po uplynutí těchto období se už nebude zobrazovat možnost zrušit předplatné.

> [!NOTE]
> Služby nezávislé na používání a měřené od jiných výrobců ISV (například virtuální počítače nebo kontejnery) nejsou způsobilé k návratu. Služby založené na využití se dají zrušit jako metoda zrušení. Vzhledem k tomu, že se poplatky účtují po použití, tyto služby nemají nárok na refundaci.

Pokud chcete zrušit předplatné SaaS založené na licencích od vydavatele ISV, postupujte následovně:

1. Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.

2. V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.

3. Vyhledejte předplatné, které chcete zrušit.

4. Ve sloupci **stav** vyberte **Zrušit** . Pak změny **odešlete** .

5. Pokud se zobrazí dialogové okno, vyplňte příslušné podrobnosti a pak vyberte **Odeslat** .

6. Zrušení potvrďte tak, že vyberete **Ano, zrušit** .

> [!NOTE]
> Můžete také zvolit zrušení předplatného Azure Marketplace pomocí rozhraní API. Pokud to chcete udělat, přečtěte si téma [zrušení předplatného Azure Marketplace](/partner-center/develop/cancel-an-azure-marketplace-subscription).

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>Vyberte, jestli se má automaticky obnovit předplatné z komerčního tržiště.

Ve výchozím nastavení jsou aktivní předplatná nastavená tak, aby se při vypršení jejich časového limitu automaticky prodlužovala jejich platnost. Pro [odběry komerčních produktů na webu Marketplace](csp-commercial-marketplace-overview.md)můžete volitelně zvolit automatické obnovení předplatného.

Pokud chcete zastavit aktivní předplatné komerčního tržiště z automatického obnovování:

1. Přihlaste se na [řídicí panel](https://partner.microsoft.com/dashboard)partnerského centra.

2. V nabídce partnerské Centrum vyberte **zákazníci** a pak ze seznamu vyberte zákazníka.

3. Vyberte **Předplatná** . Obsahuje seznam všech předplatných založených na licencích, které jste zakoupili pro zákazníka.

4. Ve sloupci **předplatné** vyberte předplatné, které chcete upravit.

5. Na stránce Podrobnosti předplatného vyhledejte část **stav** a zrušte kontrolu **automatického obnovení** .

6. Vyberte **Odeslat** .

## <a name="next-steps"></a>Další kroky

- [Nákup produktů z komerčního tržiště pro vaše zákazníky](csp-commercial-marketplace-purchase.md)

- [Správa produktů z komerčního tržiště pro vaše zákazníky](csp-commercial-marketplace-manage.md)

- [Přehled komerčního tržiště](csp-commercial-marketplace-overview.md)