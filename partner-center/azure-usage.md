---
title: Nastavení velikosti virtuálního počítače Azure, která maximálně využívá rezervace
description: Naučte se, jak velikost virtuálního počítače (VM) nastavit na výpočetní požadavky vašich zákazníků při nákupu Microsoft Azure rezervacích.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: e6c4e3e7a68de720f586754703308a447d7d30c1
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 09/22/2020
ms.locfileid: "92527338"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Nastavení velikosti virtuálního počítače Microsoft Azure, která maximálně využívá rezervaci

**Platí pro**

- Partnerské centrum
- portál Azure
- Partneři v programu CSP
 
> [!NOTE]
> Tento článek se týká jenom partnerů v programu Cloud Solution Provider (CSP). [Tuto dokumentaci k rezervacím Azure](/azure/cost-management-billing/reservations)by si měli přečíst zákazníci, kteří používají jiné typy předplatných (například, platby na základě průběžných plateb, jednotlivce, smlouvy o zákaznících Microsoftu nebo předplatná smlouva Enterprise).

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Určení velikosti virtuálního počítače pro rezervaci Azure zákazníka

Při nákupu Microsoft Azure rezervacích jménem vašich zákazníků budete muset vybrat velikost virtuálního počítače, aby splňovala výpočetní požadavky zákazníka. Tyto informace můžete najít pomocí jedné z těchto metod:

- Rozhraní API využití Azure
- Azure Portal
- Azure PowerShell
- Rozhraní API pro Azure Resource Manager (ARM)

Pokyny k používání každé z těchto metod jsou uvedeny níže. Po zakoupení rezervované slevy se sleva pro rezervaci automaticky použije na virtuální počítače, které odpovídají atributům a množstvím rezervace. Nemusíte přiřazovat rezervaci k virtuálnímu počítači.

>[!NOTE]
>Slevy za rezervace se nevztahují na klasické nebo propagační virtuální počítače.

>[!IMPORTANT]
>Pokud chcete správně identifikovat typ a velikost virtuálního počítače, který se má koupit jménem zákazníka, musíte použít jednu z níže popsaných metod, protože typ řady virtuálních počítačů se v souborech pro odsouhlasení partnerského centra nezobrazuje správně.

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a>Získání informací o velikosti virtuálních počítačů pomocí rozhraní API využití Azure

1. Použijte hodnotu pro atribut ServiceType z additionalInfo v odpovědi rozhraní API k identifikaci velikosti virtuálního počítače, který se má koupit.

2. Další informace najdete v tématu [získání záznamů o využití zákazníka pro Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) v [PARTNERSKÉM centru rozhraní API](/partner-center/develop/).

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a>Získání informací o velikosti virtuálních počítačů pomocí portál Microsoft Azure

1. V partnerském centru přejdete na stránku **Customers** .

2. Najděte zákazníka, který chce koupit rezervace virtuálních počítačů Azure, a potom výběrem šipky dolů rozbalte informace o zákazníkovi. Výběrem **portál pro správu Microsoft Azure** otevřete záznam zákazníka v Azure Portal.

3. V nabídce portál vyberte **virtuální počítače** a potom vyberte virtuální počítač, pro který chcete zakoupit rezervaci.

4. Na stránce Podrobnosti o virtuálním počítači Najděte informace o velikosti a oblasti, jak je znázorněno níže, a tyto informace použijte k nákupu rezervace v partnerském centru.  

   :::image type="content" source="images/usage1.png" alt-text="Informace o velikosti a oblasti na stránce podrobností":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a>Získání informací o velikosti virtuálních počítačů pomocí Microsoft Azure PowerShell

K získání umístění a velikosti virtuálního počítače, pro který chcete zakoupit rezervaci, použijte informace na obrázku níže. 

:::image type="content" source="images/usage2.png" alt-text="Informace o velikosti a oblasti na stránce podrobností":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a>Získání informací o velikosti virtuálních počítačů pomocí rozhraní API pro Azure Resource Manager (ARM)

1. Pomocí rozhraní API ARMClient nebo ARM volejte klienta ARM pro virtuální počítač, pro který chcete zakoupit rezervaci.

2. /Subscriptions/ <Subscription ID> /ResourceGroups/ <Resource group name> /providers/Microsoft.COMPUTE/virtualMachines/ <VM Instance Name> ? API-Version = 2017-12-01

3. Volání vrátí hodnoty pro **vmSize** a **Location** , jak je znázorněno níže.

    :::image type="content" source="images/usage3.png" alt-text="Informace o velikosti a oblasti na stránce podrobností":::
    :::image type="content" source="images/usage4.png" alt-text="Informace o velikosti a oblasti na stránce podrobností":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Ověření využití virtuálních počítačů Azure a slevy za rezervaci

Po zakoupení rezervované instance virtuálního počítače Azure jménem zákazníka se sleva za platbu za místo na virtuálním počítači automaticky aplikuje na virtuální počítače, které odpovídají atributům a množství rezervací zákazníka.

Pomocí jedné z následujících metod si můžete ověřit využití rezervace zákazníka a zjistit, na které virtuální počítače se vztahují slevy na rezervace:

- Azure Portal
- Rozhraní API využití Azure

Pokyny k používání každé z těchto metod jsou uvedeny níže.

>[!NOTE]
>Jenom rozhraní API využití Azure ukazuje, na který virtuální počítač se sleva aplikuje.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Ověření využití rezervace zákazníka v portál Microsoft Azure

1. V partnerském centru přejdete na stránku **Customers** .

2. Vyhledejte zákazníka, jehož zlevněnou slevu a využití chcete ověřit, a potom výběrem šipky dolů rozbalte informace o zákazníkovi. Výběrem **portál pro správu Microsoft Azure** otevřete záznam zákazníka v Azure Portal.
3. V nabídce portálu vyberte možnost **rezervace** a pak vyberte rezervaci, pro kterou chcete zjistit využití.
4. Na stránce **Přehled** ověřte graf využití rezervace, který ukazuje, jak velká část rezervace byla aplikována na virtuální počítače.

    >[!NOTE]
    >Data o využití se můžou zpozdit až o 8 hodin.

    a. Pokud je využití rezervace 100%, zákazník získá veškerou možnou úsporu, kterou může koupit rezervace.
    b. Pokud je využití rezervace 0%, sleva se nepoužije na žádný virtuální počítač.
    c. Pokud je využití rezervace v rozmezí od 1 do 99%, nevyužité výhody.

5. Abyste se vyhnuli této situaci, před provedením nákupu určete správnou velikost virtuálního počítače pro podporu výpočetních potřeb zákazníků.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Ověření využití rezervace zákazníka pomocí rozhraní API využití Azure

>[!NOTE]
>Jenom rozhraní API využití Azure ukazuje, na který virtuální počítač se sleva aplikuje.  

Data o využití rezervace můžete získat pomocí rozhraní API využití Azure, abyste ověřili, že zákazník získává slevu za rezervaci, a zobrazí, na kterých virtuálních počítačích se sleva vztahuje. Porovnejte příklad A s příkladem B, abyste viděli, jak ověřit využití rezervace zákazníka.

:::image type="content" source="images/usage5.png" alt-text="Informace o velikosti a oblasti na stránce podrobností":::

- ReservationId identifikuje rezervaci Azure, která se použila k uplatnění slevy na virtuální počítač.
- consumptionMeter je MeterId pro virtuální počítač, na kterém je nastavená sleva rezervace.
- ReservationMeter ukazuje náklady $0 od použití slevy rezervace.

Další informace najdete v tématu [získání záznamů o využití zákazníka pro Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) v [PARTNERSKÉM centru rozhraní API](/partner-center/develop/).

>[!IMPORTANT]
>Náklady na software, jako je například Microsoft Windows Server, nejsou aktuálně zahrnuté v ceně rezervovaného virtuálního počítače a zobrazí se jako samostatné položky řádku v záznamu objednávky a na faktuře. Pokud ale má zákazník zvýhodněné hybridní využití Azure, náklady na software se nepoužijí. Další informace najdete v tématu [náklady na software systému Windows, které nejsou součástí rezervovaných instancí](/azure/billing/billing-reserved-instance-windows-software-costs).  

## <a name="azure-reservations-resources"></a>Prostředky rezervací Azure

|**Pro informace o**   |**Přečtěte si:**    |
|:-----------------------------|:-----------------|
|Přehled rezervací Azure v CSP  | [Prodej Microsoft Azure rezervovaných instancí virtuálních počítačů](azure-reservations.md)
|Nákup rezervací Azure pro vaše zákazníky v partnerském centru   | [Nákup rezervací Azure](azure-reservations-buying.md)
|Správa rezervací Azure v partnerském centru | [Správa rezervací Azure v partnerském centru](azure-reservations-manage.md)
|Nákup rezervací Azure v Azure Portal | [Platba za virtuální počítače s Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) v nápovědě k Azure |
|Správa rezervací Azure v Azure Portal   | [Správa rezervovaných instancí virtuálních počítačů](/azure/billing/billing-manage-reserved-vm-instance) v nápovědě k Azure  |
|Nákup rezervací Azure pomocí rozhraní API partnerského centra | [Koupit Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) v dokumentaci pro vývojáře partnerského centra   |
|Udělení oprávnění zákazníkům k nákupu svých rezervací Azure z předplatného, které pro ně jste nakoupili. | [Poskytněte zákazníkům oprávnění k nákupu svých rezervací Azure.](give-customers-permission.md)   |