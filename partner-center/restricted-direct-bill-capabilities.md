---
title: Omezené přímé možnosti fakturace
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Přečtěte si o požadavcích na partnery pro poskytovatele CSP a o tom, jak zamezit omezením možností. Zjistěte, jestli jsou vaše schopnosti omezené.
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b3b1f3e1593f7e35bd3b9ed6c56ea28683bff95a
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855484"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>Omezené možnosti přímého vyúčtování a požadavky, které jsou potřeba pro partnery poskytovatele CSP Direct

**Příslušné role**: globální správce

## <a name="overview"></a>Přehled

Partneři s přímým účtováním musí splňovat nové [požadavky](direct-partner-new-requirements.md) , aby zůstali v programu pro partnery CSP Direct. V opačném případě budou mít přístup k přímým funkcím vyúčtování omezené a můžou už provádět konkrétní úkoly, jako je třeba nové nákupy pro zákazníky.

> [!Note]
> Poskytovatelé přímých faktur, kteří nesplňují nové požadavky na partnerský program pro zprostředkovatele CSP Direct, budou od Microsoftu informováni, když budou jejich přímé možnosti vyúčtování omezené. To platí pro všechny přímé partnery pro vyúčtování, ať už se jedná o [Přechod z přímé faktury na nepřímý prodejce](transition-direct-to-indirect.md) , nebo ne.  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>Jak zjistit, jestli jsou možnosti přímých faktur omezené

Chcete-li potvrdit, zda byl omezen přístup z partnerského klienta přímé fakturace na možnost přímé vyúčtování, postupujte podle těchto kroků.

1. Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard).

2. Přejít na **Nastavení účtu**  ->  **právní profil**.

3. V části **informace o programu** vyhledejte **Microsoft Cloud stav poskytovatele řešení**.

4. Pokud má stav programu hodnotu **omezeno**, znamená to, že váš partner s přímým poštovním partnerem má přístup k přímým možnostem fakturace.

## <a name="affected-direct-bill-capabilities"></a>Ovlivněné možnosti přímého vyúčtování

Pokud jsou možnosti přímých faktur omezené, nebudete už moct zákazníkům v partnerském centru vytvářet nové nákupy. Toto omezení zahrnuje:

- Předplatná Azure

- Odběry na základě licencí

- Přidejte nové doplňky do stávajících předplatných založených na licencích.

- Vytvořte jednorázové nákupy softwaru a rezervací produktů (například odběry softwaru, trvalého softwaru a instance rezervovaných virtuálních počítačů Azure).

Nemůžete také využít nabídku [sdílených služeb](shared-services.md) partnerů Azure v rámci programu CSP k nákupu nových předplatných Azure pro vlastní použití.

Stávající předplatná s přímým vyúčtováním nejsou ovlivněná. Zůstanou platné a automaticky se obnovují. Microsoft vám bude dál účtovat fakturu, dokud je nezrušíte. Stávající předplatná můžete spravovat následujícími způsoby:

- Pozastavení stávajících předplatných

- Úprava počtu licencí u stávajících předplatných založených na licencích

- Upravte počet licencí stávajících doplňků k předplatnému. 

    >[!Note]
    >K existujícím předplatným nemůžete přidávat nové doplňky, protože se s nimi zachází jako s novým nákupem.

- Nasaďte nové prostředky Azure a spravujte stávající prostředky Azure v rámci stávajících předplatných Azure. To zahrnuje prostředky, které jsou k dispozici prostřednictvím Azure Marketplace a Visual Studio předplatných.

Kromě nových nákupů nemůžete získat přístup k následujícím funkcím přímého vyúčtování v Partnerské centrum:

- Nemůžete vytvářet nové tenanty zákazníků. Možnost **Vytvořit zákazníka** na stránce **Zákazníci** v Partnerské centrum nebude dostupná.

- Nemůžete vygenerovat pozvánku pro zákazníka, který žádá o vztah přímého prodejce. Možnost **Požádat o vztah prodejce** na **stránce** Zákazníci v Partnerské centrum nebude dostupná.

    >[!NOTE]
    >Pokud jste v rámci přechodu z partnera s přímým vyúčtováním na nepřímého prodejce už zaregistrovali tenanta partnera s přímým vyúčtováním jako nepřímý prodejce, můžete místo toho vygenerovat pozvánku pro zákazníka, který žádá o vztah nepřímého prodejce.

- Nemůžete vytvořit nového tenanta sandboxu. Každý tenant partnera s přímým vyúčtováním může vytvořit jednoho tenanta sandboxu pro integraci rozhraní API s přímým vyúčtováním. Pokud jste si ho ještě nevytá vytvořili, po omezení možností partnera s přímým vyúčtováním to nebude možné.  

## <a name="next-steps"></a>Další kroky

- [Další informace o tom, jak se stát nepřímým prodejcem](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [Nové požadavky poskytovatele CSP Direct partner](direct-partner-new-requirements.md)
