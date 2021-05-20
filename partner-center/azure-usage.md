---
title: Nastavení velikosti virtuálního počítače Azure, která maximálně využívá rezervace
description: Zjistěte, jak velikost virtuálního počítače podle výpočetních potřeb vašich zákazníků při nákupu virtuálních Microsoft Azure za ně.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 14d488091227e30909b3d41af0684494a8b55de7
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149447"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Nastavení velikosti virtuálního počítače Microsoft Azure, která maximálně využívá rezervaci

**Odpovídající role:** Agent pro správu | Agent prodeje

Tento článek vysvětluje, jak velikost virtuálního počítače podle výpočetních potřeb vašich zákazníků při nákupu virtuálních Microsoft Azure za ně.
 
> [!NOTE]
> Tento článek se týká jenom partnerů v Cloud Solution Provider (CSP). Zákazníci, kteří používají jiné typy předplatných (například předplatná s platbami, jednotlivá předplatná, Smlouva se zákazníkem Microsoftu nebo předplatná smlouva Enterprise), by si místo toho měli přečíst tuto dokumentaci k [rezervacím Azure.](/azure/cost-management-billing/reservations)

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Určení velikosti virtuálního počítače pro rezervaci Azure zákazníka

Při Microsoft Azure rezervací jménem vašich zákazníků budete muset zvolit virtuální počítač s velikostí, která bude splňovat výpočetní potřeby zákazníka. Tyto informace najdete pomocí jedné z těchto metod:

- Rozhraní API využití Azure
- Azure Portal
- Azure PowerShell
- Rozhraní API Azure Resource Manager (ARM)

Pokyny pro použití každé z těchto metod jsou uvedené níže. Po zakoupení rezervace se sleva za rezervaci automaticky uplatňuje na virtuální počítače odpovídající atributům a množství rezervace. Rezervaci nemusíte přiřazovat k virtuálnímu počítače.

>[!NOTE]
>Slevy za rezervace se nevztahují na klasické ani propagační virtuální počítače.

>[!IMPORTANT]
>Pokud chcete správně identifikovat typ a velikost virtuálního počítače, který chcete koupit jménem zákazníka, musíte použít jednu z níže popsaných metod, protože typ řady virtuálních Partnerské centrum v souborech pro sesouhlasení.

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a>Získání informací o velikosti virtuálního počítače pomocí rozhraní API pro využití Azure

1. Pomocí hodnoty atributu ServiceType z additionalInfo v odpovědi rozhraní API identifikujte velikost virtuálního počítače, který chcete koupit.

2. Další informace najdete v [tématu Získání záznamů o využití Azure zákazníkem](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) v rozhraní PARTNERSKÉ CENTRUM [API.](/partner-center/develop/)

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a>Získání informací o velikosti virtuálního počítače pomocí portál Microsoft Azure

1. V Partnerské centrum přejděte na stránku **zákazníci.**

2. Najděte zákazníka, který chce koupit rezervace virtuálních počítačů Azure, a potom výběrem šipky dolů rozbalte informace o zákazníkovi. Výběrem **portál pro správu Microsoft Azure** otevřete záznam zákazníka v Azure Portal.

3. V nabídce portál vyberte **virtuální počítače** a potom vyberte virtuální počítač, pro který chcete zakoupit rezervaci.

4. Na stránce Podrobnosti o virtuálním počítači Najděte informace o velikosti a oblasti, jak je znázorněno níže, a tyto informace použijte k nákupu rezervace v partnerském centru.  

   :::image type="content" source="images/usage1.png" alt-text="Informace o velikosti a oblasti na stránce podrobností":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a>Získání informací o velikosti virtuálních počítačů pomocí Microsoft Azure PowerShell

K získání umístění a velikosti virtuálního počítače, pro který chcete zakoupit rezervaci, použijte informace na obrázku níže. 

:::image type="content" source="images/usage2.png" alt-text="Umístění a velikost virtuálního počítače":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a>Získání informací o velikosti virtuálních počítačů pomocí rozhraní API pro Azure Resource Manager (ARM)

1. Pomocí rozhraní API ARMClient nebo ARM volejte klienta ARM pro virtuální počítač, pro který chcete zakoupit rezervaci.

2. /Subscriptions/ <Subscription ID> /ResourceGroups/ <Resource group name> /providers/Microsoft.COMPUTE/virtualMachines/ <VM Instance Name> ? API-Version = 2017-12-01

3. Volání vrátí hodnoty pro **vmSize** a **Location**, jak je znázorněno níže.

    :::image type="content" source="images/usage3.png" alt-text="hodnota vmSize":::
    :::image type="content" source="images/usage4.png" alt-text="Hodnota umístění":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Ověření využití virtuálních počítačů Azure a slevy za rezervaci

Po zakoupení rezervované instance virtuálního počítače Azure jménem zákazníka se sleva za platbu za místo na virtuálním počítači automaticky aplikuje na virtuální počítače, které odpovídají atributům a množství rezervací zákazníka.

Pomocí jedné z následujících metod si můžete ověřit využití rezervace zákazníka a zjistit, na které virtuální počítače se vztahují slevy na rezervace:

- Azure Portal
- Rozhraní API využití Azure

Pokyny k používání každé z těchto metod jsou uvedeny níže.

>[!NOTE]
>Jenom rozhraní API využití Azure ukazuje, na který virtuální počítač se sleva aplikuje.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Ověření využití rezervací zákazníka v portál Microsoft Azure

1. V Partnerské centrum přejděte na stránku **zákazníci.**

2. Vyhledejte zákazníka, jehož slevu za rezervaci a využití chcete ověřit, a pak výběrem šipky dolů rozbalte informace o zákazníkovi. Výběrem **Portál pro správu Microsoft Azure** otevřete záznam zákazníka v Azure Portal.
3. V **nabídce portálu** vyberte Rezervace a pak vyberte rezervaci, u které chcete zkontrolovat využití.
4. Na stránce **Přehled** zkontrolujte graf využití rezervace, který ukazuje, jak velká část rezervace se použila na virtuální počítače.

    >[!NOTE]
    >Data o využití mohou být zpožděna až o 8 hodin.

    a. Pokud je využití rezervace 100 %, zákazník dostává všechny možné úspory, které může nákup rezervace poskytnout.
    b. Pokud je využití rezervace 0 %, sleva se na žádný virtuální počítač nevyučuje.
    c. Pokud je využití rezervace mezi 1 a 99 %, existují nevyužité výhody.

5. Pokud se chcete této situaci vyhnout, před nákupem určete správnou velikost virtuálního počítače pro podporu výpočetních potřeb zákazníka.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Ověření využití rezervací zákazníka pomocí rozhraní API využití Azure

>[!NOTE]
>Pouze rozhraní API využití Azure ukazuje, na který virtuální počítač se sleva uplatňuje.  

Pomocí rozhraní API pro využití Azure můžete získat data o využití rezervací, abyste ověřili, že zákazník dostává slevu za rezervaci, a zjistit, na které virtuální počítače (virtuální počítače) se sleva uplatňuje. Porovnejte příklad A s příkladem B a podívejte se, jak ověřit využití rezervací zákazníka.

:::image type="content" source="images/usage5.png" alt-text="Příklady využití rezervací":::

- ReservationId identifikuje rezervaci Azure, která se použila k použití slevy na virtuální počítač.
- consumptionMeter je MeterId pro virtuální počítač, na který se uplatňuje sleva za rezervaci.
- ReservationMeter zobrazuje náklady 0 USD od použití slevy za rezervaci.

Další informace najdete v [tématu Získání záznamů o využití Azure zákazníkem](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) v rozhraní PARTNERSKÉ CENTRUM [API.](/partner-center/develop/)

>[!IMPORTANT]
>Náklady na software, jako je Microsoft Windows Server, se v současné době nezahrnou do ceny rezervace virtuálního počítače a v záznamu objednávky a na faktuře se zobrazí jako samostatné řádkové položky. Pokud má ale zákazník Zvýhodněné hybridní využití Azure, náklady na software se neuplatní. Další informace najdete v tématu [Náklady na software Windows, které nejsou součástí rezervovaných instancí](/azure/billing/billing-reserved-instance-windows-software-costs).  

## <a name="next-steps"></a>Další kroky

|**Informace o**   |**Přečtěte si:**    |
|:-----------------------------|:-----------------|
|Přehled rezervací Azure v CSP  | [Prodej Microsoft Azure rezervovaných instancí virtuálních počítače](azure-reservations.md)
|Nákup rezervací Azure pro zákazníky v Partnerské centrum   | [Nákup rezervací Azure](azure-reservations-buying.md)
|Správa rezervací Azure v Partnerské centrum | [Správa rezervací Azure v Partnerské centrum](azure-reservations-manage.md)
|Nákup rezervací Azure v Azure Portal | [Předplatná virtuálních počítačů s Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) v nápovědě Azure |
|Správa rezervací Azure v Azure Portal   | [Správa rezervovaných instancí virtuálních počítače v](/azure/billing/billing-manage-reserved-vm-instance) nápovědě Azure  |
|Nákup rezervací Azure pomocí rozhraní PARTNERSKÉ CENTRUM API | [Informace Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) najdete v dokumentaci Partnerské centrum pro vývojáře.   |
|Dáváte zákazníkům oprávnění k nákupu vlastních rezervací Azure z předplatného, které jste pro ně zakoupili. | [Udělit zákazníkům oprávnění k nákupu vlastních rezervací Azure](give-customers-permission.md)   |