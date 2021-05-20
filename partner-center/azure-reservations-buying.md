---
title: Nákup Microsoft Azure rezervací pro zákazníky
description: Zjistěte, jak zakoupit nebo zakoupit rezervace Azure jménem vašich zákazníků v Partnerské centrum. Uvádí také trhy, kde nejsou k dispozici rezervace Azure.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.date: 08/06/2020
ms.openlocfilehash: cd8a78edab25b94e678aafd61ca96e61a625fb07
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149532"
---
# <a name="buy-microsoft-azure-reservations-on-behalf-of-your-customers-in-partner-center"></a>Nákup Microsoft Azure rezervací jménem vašich zákazníků v Partnerské centrum

**Odpovídající role:** Agent pro správu | Globální správce | Agent helpdesku | Sales agent | Správce správy uživatelů

Tento článek vysvětluje, jak zakoupit nebo koupit rezervace Azure jménem vašich zákazníků v Partnerské centrum. Identifikuje také trhy, kde jsou nedostupné rezervace Azure.
 
> [!NOTE]
> Tento článek se týká jenom partnerů v Cloud Solution Provider (CSP). Zákazníci, kteří používají jiné typy předplatných (například předplatná s platbami, jednotlivá předplatná, Smlouva se zákazníkem Microsoftu nebo předplatná smlouva Enterprise), by si místo toho měli přečíst tuto dokumentaci k [rezervacím Azure.](/azure/cost-management-billing/reservations)

## <a name="before-you-begin"></a>Než začnete

Než zakoupíte rezervace Azure jménem svých zákazníků, projděte si níže uvedené důležité informace. (Chcete, aby si zákazníci mohli koupit vlastní rezervace Azure z předchozího předplatného Azure, které jste pro ně zakoupili? Viz [Udělit zákazníkům oprávnění k nákupu vlastních rezervací Azure.)](give-customers-permission.md#give-customers-permission-to-buy-their-own-azure-reservations)

- Pokud a když zákazník podepíše novou Smlouva se zákazníkem Microsoftu (viz Potvrzení přijetí smlouvy zákazníkem Smlouva se zákazníkem Microsoftu [),](confirm-customer-agreement.md)musíte zakoupit rezervace Azure v rámci plánu Azure. Další informace najdete v nákupu [plánu Azure.](purchase-azure-plan.md)

- Před nákupem rezervací jejich jménem už zákazníci musí mít aktivní předplatné Azure.
  
- Náklady na softwarové předplatné, jako SQL Database nebo software SUSE Linux, nejsou zahrnuté v cenách rezervací Azure.

- Komerční ceny Microsoftu pro vás nezahrnují daně, pokud vaše poloha není Brazílie. Pokud se nacházíte v Brazílii, komerční cena pro vás zahrnuje příslušné daně.

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
> | Ázerbájdžán       | Guyana     | Saint Pierre a Miquelon   |
> | Benin     | Haiti       | Svatý Vincenc a Grenadiny     |
> | Bhútán     | Heardův ostrov a McDonaldovy ostrovy       | Samoa     |
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
> | Komory     | Marshallovy ostrovy     | Špicberky     |
> | Kongo     | Martinik     | Svazijsko     |
> | Konžská demokratická republika     | Mauritánie     | Timor Leste   |
> | Cookovy ostrovy     | Mayotte     | Togo   |
> | Džibutsko     | Mikronésie     | Tokelau   |
> | Dominika     | Montserrat     | Tonga   |
> | Rovníková Guinea     | Mosambik     | Ostrovy Turks a Caicos   |
> | Eritrea     | Myanmar     | Tuvalu   |
> | Falklandské ostrovy     | Nauru     | Odlehlé ostrovy USA   |
> | Francouzská Guyana     | Nová Kaledonie     | Vanuatu   |
> | Francouzská Polynésie     | Niger     | Vatikán   |
> | Francouzská jižní území     | Niue     | Wallis a Futuna   |
> | Gabon     | Norfolk     | Jemen   |
> | Gambie     | Severní Mariany     |    |
> | Gibraltar     | Palau       |    |

## <a name="purchase-azure-reservations"></a>Nákup rezervací Azure

Podle následujících kroků můžete koupit Microsoft Azure rezervace jménem vašich zákazníků v partnerském centru. (Chcete, aby zákazníci mohli koupit své vlastní rezervace Azure z předchozího předplatného Azure, které pro ně jste si zakoupili? Viz [udělení oprávnění zákazníkům k nákupu vlastních rezervací Azure](give-customers-permission.md).)

1. V nabídce partnerské Centrum vyberte **zákazníci** .  

2. Na stránce **Vaši** zákazníci vyhledejte zákazníka, který chce zakoupit rezervace Azure, a pak výběrem šipky dolů rozbalte řádek zákazníka.  

3. Vyberte **Přidat produkty a** pak vyberte **Azure**. 

    a. Ze seznamu Segment zvolte segment **trhu** zákazníka.

    b. V **seznamu Typ** produktu **zvolte** Rezervace.

    c. V seznamu Typ rezervace zvolte typ rezervace, který zákazník **chce.**

4. Rezervace Azure musí být přidružené k aktivnímu předplatnému Azure. V seznamu Předplatné zákazníka zvolte předplatné zákazníka, ke které chcete **přidat rezervace** Azure. 

   >[!IMPORTANT]
   >Pokud zákazník ještě nemá aktivní předplatné Azure, vyberte **Azure** a přidejte ho teď. 

5. Pomocí filtrů vyhledejte rezervace Azure na virtuálních počítačích, které splňují požadavky vašich zákazníků.  

6. Jakmile najdete rezervace, které chcete koupit, zadejte počet rezervovaných instancí, které zákazník bude potřebovat, do pole **Quantity** a pak vyberte Add to cart (Přidat do **košíku).**  

7. Opakujte kroky 5 a 6, dokud nepřidáte všechny potřebné položky do objednávky. Vyberte **Zkontrolovat a** ověřte správnost objednávky.  

8. Na **stránce Kontrola objednávek** můžete: 

    - Ověřte nebo změňte množství rezervovaných instancí.

    - Vyberte rozsah rezervace. Rozsah rezervace může pokrývat jedno nebo více předplatných (sdílený rozsah). Pokud rozsah rezervace vymešete na jedno předplatné, sleva za rezervaci se použije pouze na toto předplatné. Pokud vyberete sdílené, sleva za rezervaci se použije u všech předplatných v kontextu fakturace zákazníka. 

      >[!NOTE] 
      >Pokud se rozhodnete omezit rozsah rezervace na jedno předplatné Azure, možná budete muset navýšit kvótu virtuálních procesorů předplatného. Pokud chcete zvýšit kvótu virtuálních procesorů předplatného, budete muset vytvořit žádost o podporu v Azure Portal. Pokud chcete vytvořit žádost, postupujte podle pokynů [v tomto tématu](/azure/azure-supportability/resource-manager-core-quotas-request) . 

      >[!NOTE]   
      >Pokud je zákazník v rámci plánu Azure, **obor**  bude nastaven na **Shared**. 

    - Pokud jste partnerem poskytovatele, vyberte prodejce, kterého chcete k produktu přidružit.
    
    - Pokud vaše rezervace Azure podporuje plán fakturace, můžete z rozevírací nabídky vybrat možnost fakturační frekvence jako měsíčně. 
    - Pokud vaše rezervace Azure nepodporuje plán fakturace, vaše četnost fakturace se nastaví jako jednorázové fakturace. 

9. Pokud chcete objednávku koupit, vyberte **koupit** . Podrobnosti o vaší objednávce, včetně čísla objednávky, se zobrazí na stránce **potvrzení** . Výběrem možnosti **Hotovo** přejdete na stránku **Historie objednávky** . 

10. Pokud chcete spravovat rezervaci zákazníka v Azure Portal, najděte zákazníka na stránce vaši **zákazníci** a pak výběrem šipky dolů rozbalte řádek zákazníka. Výběrem **portál pro správu Microsoft Azure** otevřete záznam zákazníka v Azure Portal.

## <a name="next-steps"></a>Další kroky

|**Pro informace o**   |**Přečtěte si:**    |
|:-----------------------------|:-----------------|
|Přehled rezervací Azure v CSP  | [Prodej rezervovaných instancí Microsoft Azure](azure-reservations.md) |
|Správa rezervací Azure v partnerském centru | [Správa rezervací Azure v partnerském centru](azure-reservations-manage.md)
|Určení správné velikosti virtuálního počítače a ověření využití virtuálního počítače zákazník   |[Změna velikosti virtuálního počítače pro maximální využití rezervace Azure](azure-usage.md)   |
|Nákup rezervací Azure pomocí rozhraní API partnerského centra | [Koupit Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) v dokumentaci pro vývojáře partnerského centra   |
|Udělení oprávnění zákazníkům k nákupu vlastních rezervací Azure  | [Udělit zákazníkům oprávnění k nákupu vlastních rezervací Azure](give-customers-permission.md)  |