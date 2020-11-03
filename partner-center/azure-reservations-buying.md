---
title: Nákup Microsoft Azure rezervací pro zákazníky
description: Zjistěte, jak koupit nebo koupit rezervace Azure jménem zákazníků v partnerském centru. Také uvádí trhy, kde nejsou k dispozici rezervace Azure.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.date: 08/06/2020
ms.openlocfilehash: 22ee2b6b76662ae3c7f7a956dc42f4425c321309
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/14/2020
ms.locfileid: "92527686"
---
# <a name="buy-microsoft-azure-reservations-on-behalf-of-your-customers-in-partner-center"></a>Nákup Microsoft Azurech rezervací jménem vašich zákazníků v partnerském centru

**Platí pro**

- Partnerské centrum
- Microsoft Azure Portal
- Partneři v CSP

**Příslušné role**

- Agent správce
- Globální správce
- Agent helpdesku
- Agent prodeje
- Správce správy uživatelů
 
> [!NOTE]
> Tento článek se týká jenom partnerů v programu Cloud Solution Provider (CSP). [Tuto dokumentaci k rezervacím Azure](/azure/cost-management-billing/reservations)by si měli přečíst zákazníci, kteří používají jiné typy předplatných (například, platby na základě průběžných plateb, jednotlivce, smlouvy o zákaznících Microsoftu nebo předplatná smlouva Enterprise).

## <a name="before-you-begin"></a>Než začnete

Před nákupem rezervací Azure za vaše zákazníky si přečtěte důležité informace níže. (Chcete, aby zákazníci mohli koupit své vlastní rezervace Azure z předchozího předplatného Azure, které pro ně jste si zakoupili? Viz [udělení oprávnění zákazníkům k nákupu vlastních rezervací Azure](give-customers-permission.md#give-customers-permission-to-buy-their-own-azure-reservations).)

- Pokud a když zákazník podepíše nové smlouvy o zákaznících Microsoftu (viz [potvrzení přijetí smlouvy na zákazníky od zákazníka](confirm-customer-agreement.md)), musíte si koupit Azure rezervací v rámci plánu Azure. Další informace najdete v článku o [nákupu plánu Azure](purchase-azure-plan.md).

- Před nákupem rezervací jménem zákazníků už musí mít aktivní předplatné Azure.
  
- Náklady na předplatné softwaru, jako je SQL Database nebo software SUSE Linux, nejsou zahrnuté v cenách za rezervované služby Azure.

- Komerční ceny Microsoftu nezahrnují daně, pokud vaše poloha není Brazílie. Pokud je vaše poloha Brazílie, zahrnuje komerční cena za vás příslušné daně.

- Prodejní a helpdeskní agenti potřebují explicitní přístup k předplatnému Azure, aby je mohli koupit nebo spravovat v Azure Portal a žádosti o podporu souborů, včetně výměn a refundací jménem zákazníka.  

- Pokud jste nepřímý poskytovatel a koupíte rezervace Azure prostřednictvím Azure Portal, partner záznamu (nepřímý prodejce) se dědí z předplatného služby Azure CSP, které jste vybrali.

- Partner záznamu pro rezervace Azure nejde změnit po nákupu. Stávající rezervaci můžete zrušit a koupit ji nového s novým partnerem záznamu.

- Pokud chce zákazník přenést předplatné Azure z Direct nebo EA na CSP, nebudou se rezervace přenášet.

## <a name="azure-reservations-unavailable-markets"></a>Nedostupné trhy Azure rezervací

> [!IMPORTANT]
> **Rezervace Azure nejsou k** dispozici na následujících trzích:  
>  
> **Nedostupné trhy (v abecedním pořadí)**
>
> |A až GI   | Gr až PAL  | PAP na Z |
> |--------------------------------|-----------------------------------|------------------------------------------|
> | Ostrovy Aland     | Grónsko     | Papua-Nová Guinea     |
> | Americká Samoa     | Grenada     | Pitcairnovy ostrovy     |
> | Andorra     | Guadeloupe     | Réunion     |
> | Anguilla     | Guam     | Saba   |
> | Antarktida     | Guernsey     | Svatý Bartoloměj   |
> | Antigua a Barbuda       | Guinea     | Svatá Lucie   |
> | Aruba       | Guinea-Bissau     | Svatý Martin (Francie)   |
> | Ázerbájdžán       | Guyana     | Saint-Pierre a Miquelon   |
> | Benin     | Haiti       | Svatý Vincenc a Grenadiny     |
> | Bhútán     | Heardův ostrov a MacDonaldovy ostrovy       | Samoa     |
> | Bonaire     | Ostrov Man     | San Marino     |
> | Bouvetův ostrov     | Jan Mayen     | Svatý Tomáš a Princův ostrov   |
> | Britské indickooceánské území       | Jersey     | Seychely   |
> | Britské Panenské ostrovy     | Kiribati       | Sierra Leone   |
> | Burkina Faso     | Kosovo     | Svatý Eustach     |
> | Burundi     | Laos     | Svatý Martin (Nizozemsko)     |
> | Kambodža     | Lesotho     | Šalamounovy ostrovy     |
> | Středoafrická republika     | Libérie     | Somálsko     |
> | Čad     | Madagaskar     | Jižní Georgie a Jižní Sandwichovy ostrovy     |
> | Čína     | Malawi     | Jižní Súdán     |
> | Vánoční ostrov     | Maledivy     | Svatá Helena, Ascension a Tristan da Cunha     |
> | Kokosové ostrovy     | Mali     | Surinam     |
> | Komory     | Marshallovy ostrovy     | Svalbard     |
> | Kongo     | Martinik     | Svazijsko     |
> | Konžská demokratická republika     | Mauritánie     | Timor Leste   |
> | Cookovy ostrovy     | Mayotte     | Togo   |
> | Džibutsko     | Mikronésie     | Tokelau   |
> | Dominika     | Montserrat     | Tonga   |
> | Rovníková Guinea     | Mosambik     | Ostrovy Turks a Caicos   |
> | Eritrea     | Myanmar     | Tuvalu   |
> | Falklandské ostrovy     | Nauru     | Menší odlehlé ostrovy USA   |
> | Francouzská Guyana     | Nová Kaledonie     | Vanuatu   |
> | Francouzská Polynésie     | Niger     | Vatikán   |
> | Francouzská jižní území     | Niue     | Wallis a Futuna   |
> | Gabon     | Norfolk     | Jemen   |
> | Gambie     | Severní Mariany     |    |
> | Gibraltar     | Palau       |    |

## <a name="purchase-azure-reservations"></a>Nákup rezervací Azure

Podle následujících kroků můžete koupit Microsoft Azure rezervace jménem vašich zákazníků v partnerském centru. (Chcete, aby zákazníci mohli koupit své vlastní rezervace Azure z předchozího předplatného Azure, které pro ně jste si zakoupili? Viz [udělení oprávnění zákazníkům k nákupu vlastních rezervací Azure](give-customers-permission.md).)

1. V nabídce partnerské Centrum vyberte **zákazníci** .  

2. Na stránce vaši **zákazníci** vyhledejte zákazníka, který chce koupit rezervace Azure, a potom výběrem šipky dolů rozbalte řádek zákazníka.  

3. Vyberte **Přidat produkty** a potom vyberte **Azure** . 

    a. Vyberte segment trhu zákazníka ze seznamu **segmentů** .

    b. V seznamu **typ** produktu vyberte možnost **rezervace** .

    c. Vyberte typ rezervace, kterou zákazník požaduje ze seznamu **typ rezervací** .

4. Rezervace Azure musí být přidružené k aktivnímu předplatnému Azure. Vyberte předplatné zákazníka, ze kterého chcete přidat rezervace Azure, ze seznamu **předplatných zákazníků** . 

   >[!IMPORTANT]
   >Pokud zákazník ještě nemá aktivní předplatné Azure, vyberte **Azure** a přidejte ho hned teď. 

5. Pomocí filtrů můžete najít rezervace Azure na virtuálních počítačích, které splňují požadavky vašich zákazníků.  

6. Po vyhledání rezervací, které chcete koupit, zadejte počet rezervovaných instancí, které zákazník bude potřebovat **, a pak** vyberte **Přidat do košíku** .  

7. Opakujte kroky 5 a 6, dokud nepřidáte všechny potřebné položky do objednávky. Vyberte **zkontrolovat** a ověřte, jestli je vaše objednávka správná.  

8. Na stránce **Kontrola objednávek** můžete: 

    - Ověřte nebo změňte množství rezervovaných instancí.

    - Vyberte obor rezervace. Rozsah rezervace může zahrnovat jedno nebo víc předplatných (sdílený rozsah). Pokud zadáte obor rezervace na jedno předplatné, použije se sleva rezervace jenom pro toto předplatné. Pokud vyberete Shared, použije se sleva rezervace pro všechna předplatná v rámci fakturačního kontextu zákazníka. 

      >[!NOTE] 
      >Pokud se rozhodnete omezit rozsah rezervace na jedno předplatné Azure, možná budete muset zvýšit kvótu vCPU předplatného. Pokud chcete zvýšit kvótu vCPU předplatného, budete muset vytvořit žádost o podporu v Azure Portal. Pokud chcete vytvořit žádost, postupujte podle pokynů [v tomto tématu](/azure/azure-supportability/resource-manager-core-quotas-request) . 

      >[!NOTE]   
      >Pokud je zákazník v rámci plánu Azure, **obor**  bude nastaven na **Shared** . 

    - Pokud jste partnerem poskytovatele, vyberte prodejce, kterého chcete k produktu přidružit.
    
    - Pokud vaše rezervace Azure podporuje plán fakturace, můžete z rozevírací nabídky vybrat možnost fakturační frekvence jako měsíčně. 
    - Pokud vaše rezervace Azure nepodporuje plán fakturace, vaše četnost fakturace se nastaví jako jednorázové fakturace. 

9. Pokud chcete objednávku koupit, vyberte **koupit** . Podrobnosti o vaší objednávce, včetně čísla objednávky, se zobrazí na stránce **potvrzení** . Výběrem možnosti **Hotovo** přejdete na stránku **Historie objednávky** . 

10. Pokud chcete spravovat rezervaci zákazníka v Azure Portal, najděte zákazníka na stránce vaši **zákazníci** a pak výběrem šipky dolů rozbalte řádek zákazníka. Výběrem **portál pro správu Microsoft Azure** otevřete záznam zákazníka v Azure Portal.

## <a name="azure-reservations-resources"></a>Prostředky rezervací Azure
|**Pro informace o**   |**Přečtěte si:**    |
|:-----------------------------|:-----------------|
|Přehled rezervací Azure v CSP  | [Prodej rezervovaných instancí Microsoft Azure](azure-reservations.md) |
|Správa rezervací Azure v partnerském centru | [Správa rezervací Azure v partnerském centru](azure-reservations-manage.md)
|Určení správné velikosti virtuálního počítače a ověření využití virtuálního počítače zákazník   |[Změna velikosti virtuálního počítače pro maximální využití rezervace Azure](azure-usage.md)   |
|Nákup rezervací Azure pomocí rozhraní API partnerského centra | [Koupit Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) v dokumentaci pro vývojáře partnerského centra   |
|Udělení oprávnění zákazníkům k nákupu vlastních rezervací Azure  | [Poskytněte zákazníkům oprávnění k nákupu svých rezervací Azure.](give-customers-permission.md)  |