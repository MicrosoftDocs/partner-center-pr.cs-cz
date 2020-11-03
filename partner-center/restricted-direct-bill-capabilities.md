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
ms.openlocfilehash: 7ee6f4fdb537752cccbceb68716ed22bb8c5fb3a
ms.sourcegitcommit: b4771fd0781d95551e65baa481a572291c729d7d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 10/28/2020
ms.locfileid: "92795762"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>Omezené možnosti přímého vyúčtování a požadavky, které jsou potřeba pro partnery poskytovatele CSP Direct  

## <a name="overview"></a>Přehled

Partneři s přímým účtováním musí splňovat nové [požadavky](direct-partner-new-requirements.md) , aby zůstali v programu pro partnery CSP Direct. V opačném případě budou mít přístup k přímým funkcím vyúčtování omezené a můžou už provádět konkrétní úkoly, jako je třeba nové nákupy pro zákazníky.

> [!Note]
> Poskytovatelé přímých faktur, kteří nesplňují nové požadavky na partnerský program pro zprostředkovatele CSP Direct, budou od Microsoftu informováni, když budou jejich přímé možnosti vyúčtování omezené. To platí pro všechny přímé partnery pro vyúčtování, ať už se jedná o [Přechod z přímé faktury na nepřímý prodejce](transition-direct-to-indirect.md) , nebo ne.  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>Jak zjistit, jestli jsou možnosti přímých faktur omezené

Chcete-li potvrdit, zda byl omezen přístup z partnerského klienta přímé fakturace na možnost přímé vyúčtování, postupujte podle těchto kroků.

1. Přihlaste se k [řídicímu panelu partnerského centra](https://partner.microsoft.com/dashboard).

2. Přejít na partnerský profil **nastavení partnera**  ->  **Partner Profile** .

3. V části **informace o programu** vyhledejte **Microsoft Cloud stav poskytovatele řešení** .

4. Pokud má stav programu hodnotu **omezeno** , znamená to, že váš partner s přímým poštovním partnerem má přístup k přímým možnostem fakturace.

## <a name="affected-direct-bill-capabilities"></a>Ovlivněné možnosti přímého vyúčtování

Pokud jsou možnosti přímých faktur omezené, nebudete už moct zákazníkům v partnerském centru vytvářet nové nákupy. Toto omezení zahrnuje:

- Předplatná Azure

- Odběry na základě licencí

- Přidejte nové doplňky do stávajících předplatných založených na licencích.

- Vytvořte jednorázové nákupy softwaru a rezervací produktů (například odběry softwaru, trvalého softwaru a instance rezervovaných virtuálních počítačů Azure).

V rámci programu CSP nemůžete použít [nabídku Azure partner Shared Services](shared-services.md) k nákupu nových předplatných Azure pro vlastní použití.

Existujícím předplatným přímých fakturování nejsou ovlivněny. Zůstávají platné a jsou automaticky obnovovány. Společnost Microsoft bude nadále účtována přímo, dokud nebudou zrušeny. Stávající odběry můžete spravovat následujícími způsoby:

- Pozastavit existující předplatná

- Upravit počet licencí stávajících předplatných založených na licencích

- Upravte počet licencí existujících doplňků v předplatném. 
 
    >[!Note] 
    >Do stávajících předplatných nemůžete přidávat nové doplňky, protože se považují za nové nákupy.

- Nasaďte nové prostředky Azure a spravujte stávající prostředky Azure v rámci stávajících předplatných Azure. To zahrnuje prostředky, které jsou k dispozici prostřednictvím předplatných Azure Marketplace a Visual Studio.

Kromě nových nákupů nemůžete získat přístup k následujícím možnostem přímého vyúčtování v partnerském centru:

- Nemůžete vytvářet nové klienty zákazníka. Možnost **vytvořit zákazníka** na stránce **zákazníci** v partnerském centru nebude k dispozici.

- Nemůžete vygenerovat pozvánku pro zákazníka žádajícího o přímý vztah prodejce. Možnost **požadavek na vztah prodejce** na stránce **zákazníci** v partnerském centru nebude k dispozici.

    >[!NOTE]
    >V rámci přechodu z přímého poštovního partnera na nepřímý prodejce, pokud jste už zaregistrovali svého tenanta partnera pro fakturaci jako nepřímý prodejce, můžete místo toho vygenerovat pozvánku pro zákazníka žádajícího o nepřímý vztah prodejců.

- Nemůžete vytvořit nového tenanta izolovaného prostoru (sandbox). Každý partnerský partner pro přímé faktury může vytvořit jednoho tenanta izolovaného prostoru (sandbox) pro účely přímé integrace služby API. Pokud jste ho ještě nevytvořili, nemusíte to udělat, až budete mít k možnost směrování na straně serveru.  

## <a name="next-steps"></a>Další kroky

- [Další informace o tom, jak se stát nepřímým prodejcem](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [Nové požadavky poskytovatele CSP Direct partner](direct-partner-new-requirements.md)