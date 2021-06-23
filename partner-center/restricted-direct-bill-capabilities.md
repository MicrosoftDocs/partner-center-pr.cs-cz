---
title: Omezené možnosti přímého vyúčtování
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Seznamte se Cloud Solution Provider (CSP) s přímým vyúčtováním od partnerů a zjistěte, jak se vyhnout omezení možností. Zjistěte, jestli jsou vaše možnosti omezené.
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e5bc33101809a805ba591be5a9b51d8dfff2397b
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551414"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>Omezené možnosti přímého vyúčtování a požadavky potřebné pro partnery CSP s přímým vyúčtováním

**Odpovídající role:** Globální správce

## <a name="overview"></a>Přehled

Partneři s přímým vyúčtováním musí [splňovat](direct-partner-new-requirements.md) nové požadavky, aby zůstali v Cloud Solution Provider programu csp (Direct Bill Partner). V opačném případě bude jejich přístup k funkcím s přímým vyúčtováním nakonec omezený a může už dál provádět konkrétní úlohy, například provádět nové nákupy zákazníkům.

> [!Note]
> Partneři s přímým vyúčtováním, kteří nesplňuje nové požadavky na program CSP s přímým vyúčtováním, bude Microsoft informovat o tom, že jejich možnosti přímého vyúčtování budou omezené. To platí pro všechny partnery s přímým vyúčtováním bez ohledu na to, jestli se rozhodli přejít z partnera s přímým vyúčtováním na nepřímé [prodejce,](transition-direct-to-indirect.md) nebo ne.  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>Jak říct, jestli jsou možnosti přímého vyúčtování omezené

Pokud chcete ověřit, jestli je přístup z tenanta partnera s přímým vyúčtováním k možnostem přímého vyúčtování omezený, postupujte podle těchto kroků.

1. Přihlaste se k [řídicímu panelu pro Partnerské centrum](https://partner.microsoft.com/dashboard).

2. Přejděte na **Nastavení účtu Právní**  >  **profil**.

3. V **části Informace o** programu vyhledejte Microsoft Cloud Solution Provider **stav**.

4. Pokud je ve stavu programu omezená **hodnota**, znamená to, že byl omezen přístup vašeho tenanta partnera s přímým vyúčtováním k funkcím přímého vyúčtování.

## <a name="affected-direct-bill-capabilities"></a>Ovlivněné možnosti přímého vyúčtování

Pokud jste omezili možnosti přímého vyúčtování, nemůžete už zákazníkům provádět nové nákupy v Partnerské centrum. Toto omezení zahrnuje:

- Předplatná Azure

- Předplatná založená na licencích

- Přidejte nové doplňky do stávajících předplatných založených na licencích.

- Jednorázové nákupy softwaru a rezervačních produktů (například softwarových předplatných, časově neomezeného softwaru a rezervovaných instancí virtuálních počítačů Azure)

Nemůžete také využít nabídku [sdílených služeb](shared-services.md) partnerů Azure v rámci programu CSP k nákupu nových předplatných Azure pro vlastní použití.

Stávající předplatná s přímým vyúčtováním nejsou ovlivněná. Zůstanou platné a budou automaticky nové. Microsoft vám bude dál účtovat fakturu, dokud je nezrušíte. Stávající předplatná můžete spravovat následujícími způsoby:

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

- Nemůžete vytvořit nového tenanta sandboxu. Každý tenant partnera s přímým vyúčtováním může vytvořit jednoho tenanta sandboxu pro integraci rozhraní API s přímým vyúčtováním. Pokud jste si ho ještě nevytá typ vytvořili, po omezení možností partnera s přímým vyúčtováním to už není možné.  

## <a name="next-steps"></a>Další kroky

- [Další informace o tom, jak se stát nepřímým prodejcem](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [Nové požadavky přímých partnerů CSP](direct-partner-new-requirements.md)
