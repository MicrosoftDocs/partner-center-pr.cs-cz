---
title: Oznámení z března 2021
description: Z března 2021 oznámení pro partnerské Centrum Microsoftu, včetně nových možností, propagačních akcí, nabídek, trhů nebo změn stávajících nabídek.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: b503e928b1491d5c2c70ac52460080f9e1ba91b8
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150110"
---
# <a name="march-2021-announcements"></a>Oznámení z března 2021

Tato stránka poskytuje oznámení pro partnerské Centrum Microsoftu na březen 2021.

## <a name="readiness-changes-to-the-cloud-solution-provider-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="18"></a>Připravenost: změny v rozhraní API pro ověřování adres zákazníka v červnu v provozu poskytovatele Cloud Solution Provider (CSP) možnost testování je teď dostupná.

### <a name="categories"></a>Kategorie

- Datum: 2021-03-30
- Připravenost

### <a name="summary"></a>Souhrn

Abychom svým partnerům a zákazníkům usnadnili provoz na základě důvěry, budeme zvát partnery, aby otestovali změny v rozhraní API pro ověřování adres pro všechny země po celém světě.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Poskytovatelé služeb CSP Direct účtují a nepřímá zprostředkovatelé, kteří vytvářejí nové nebo aktualizují podrobnosti o adresách zákazníků.

### <a name="details"></a>Podrobnosti

Microsoft běží na důvěryhodnosti. Pro účely transakce zákaznických předplatných v programu CSP jsme zajistili poskytování kompatibilní, bezpečné a zabezpečené metody ověřování adres zákazníků. Od 31. března 2021 jsme představili změny v rozhraní API pro ověřování adres, které pozvaní partneři k testování ještě před tím, než budou v provozu změny v červnu 2021.

Změny mají vliv pouze na ověřování adres API. Vytváření zákazníků a aktualizace rozhraní API fakturačních profilů nejsou ovlivněny.

Odpověď vrátí jednu z následujících stavových zpráv:

| Status     | Popis |    Počet vrácených navrhovaných adres |
|-------|---------------|-------------------|
|Ověřené pro přepravce | Adresa je ověřena a může být expedována. | Jednoduché |
|Ověřují | Adresa je ověřena. | Jednoduché |
|Požadovaná interakce | Navrhovaná adresa se výrazně změnila a vyžaduje potvrzení uživatele. | Jednoduché |
|Částečná ulice | Ulice v adrese je částečná a potřebuje další informace. | Více – maximálně tři |
|Částečně místní | Dané prostory (číslo budovy, číslo sady a další) jsou částečné a potřebují další informace. | Více – maximálně tři |
|Několik | Adresa obsahuje několik polí, která jsou částečná (potenciálně zahrnují i částečná ulice a částečná místně). | Více – maximálně tři |
|Žádná | Adresa je nesprávná. | Žádná |
|Není ověřeno. | Adresu nebylo možné odeslat prostřednictvím procesu ověřování. | Žádná |

Poštovní kódy v USA vrátí další 4 číslice + spojovník – například 12345-6789.

Jakmile je adresa odeslána k ověření prostřednictvím rozhraní API pro ověření adresy, vrátí se následující schéma odpovědi:

```csharp

// <summary>
/// Object represents the address validation response.
/// </summary>

public class AddressValidationResponse
{
   /// <summary>
   /// Gets or sets the original address
   /// </summary>
   /// <value>
   /// Original Address
   /// </value>
   public Address OriginalAddress { get; set; }

   /// <summary>
   /// Gets or sets the suggested addresses
   /// </summary>
   /// <value>
   /// Suggested Addresses
   /// </value>
   public List<Address> SuggestedAddresses { get; set; }

   /// <summary>
   /// Gets or sets the validation status
   /// </summary>
   /// <value>
   /// Status
   /// </value>
   public string Status { get; set; }

   /// <summary>
   /// Gets or sets the validation message
   /// </summary>
   /// <value>
   /// Validation Message
   /// </value>
   public string ValidationMessage { get; set; }
   ```

Podívejte se na tuto ukázkovou odpověď. Všimněte si, že pro USA vrátí odpověď další čtyřmístné přípony pro řádek PSČ, pokud zadáte jenom pět číslic PSČ.

```csharp

"suggested_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Microsoft Way",
              "postal_Code": "98052-8300"
},
"original_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Micro Way",
              "postal_Code": "98052"
},
"status":  "InteractionRequired",
"validation_message": "Address field invalid for property: ‘Street’"
}
```

### <a name="next-steps"></a>Další kroky

- Podělte se o SVÉ ID tenanta sandboxu s odborníkem na předmět (Ali Protoki), který se zahrne do testovacího letu, abyste se mohli začít připravovat na aktualizaci.

- Pokud používáte řešení dodavatele ovládacích panelů (CPV), obraťte se na svého dodavatele CPV.

### <a name="questions"></a>Máte otázky?

Pokud potřebujete podporu pro vaše operace s Microsoftem, oslovte svou partnerskou podporu ve skupině Yammeru.

### <a name="change-log"></a>Protokol změn:

- 31. března 2020: původní publikace

- 30. dubna 2021: aktualizace pro ukázkovou odpověď a podrobnosti o PSČ

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a>Nové prostředí v centru pro správu Exchange (EAC)

### <a name="categories"></a>Kategorie

- Datum: 2021-03-29
- Možnosti

### <a name="summary"></a>Souhrn

Od 27. dubna 2021 se v centru pro správu Exchange (EAC) zavádí nové prostředí, které bude zlepšit každodenní efektivitu pro uživatele.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Delegovaní správci přistupující k Exchangi prostřednictvím partnerského centra

### <a name="details"></a>Podrobnosti

Od 27. dubna 2021 budou partneři, kteří se přecházejí na Exchange prostřednictvím partnerského centra, přesměrováni na nový EAC.

Toto nové prostředí je teď k dispozici ve verzi Preview a správci můžou aktivovat toto prostředí výběrem přepínače v pravém horním rohu v klasickém poli EAC. Můžou také přejít k novému poli EAC tím, že vyberou banner "vyzkoušet ho Now", který se zobrazí na všech stránkách.

Mezi výhody nového pole EAC patří:

- Přidání přehledů, sestav a mechanismů výstrah pro řízení toku pošty – problémy související s. 

- Individuální řídicí panely pro zvýšení produktivity.

K usnadnění navigace v novém prostředí jsou k dispozici videa v části **školení & příručka** na novém prostředí EAC. Tyto informace vám poskytnou přehled o tom, jak můžete nový portál nejlépe využít.

>[!NOTE]
>V rámci této změny nebudou klasické prostředí EAC zastaralé. Před implementací jakékoli změny se bude předem informovat.

### <a name="next-steps"></a>Další kroky

- Projděte si [materiály k tomuto tématu](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), kde můžete zobrazit snímky obrazovky nového prostředí.

- Tyto informace sdílejte s příslušnými zúčastněnými stranami ve vaší organizaci. 

### <a name="questions"></a>Máte otázky?

Jakékoli otázky týkající se těchto změn najdete v příslušných komunitách Yammeru.

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a>Microsoft Operations: Představujeme kalendář uvedení produktu na trh

### <a name="categories"></a>Kategorie

- Datum: 25. 3. 2021
- Nabídky | Moderní pracoviště

### <a name="summary"></a>Souhrn

V reakci na zpětnou vazbu od partnerů provozní operace Microsoftu zjednoduší komunikaci pro uvedení produktů na trh.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Cloud Solution Provider (CSP)

### <a name="details"></a>Podrobnosti

Microsoft se zavazuje, že bude partnerská prostředí neustále vylepšovat. Obdrželi jsme od vás zpětnou vazbu, že od Microsoftu dostáváte příliš mnoho komunikací, včetně duplicitních oznámení o uvedení produktu na trh.

V reakci na vaši zpětnou vazbu Microsoft zjednodušil prostředí připravenosti pro uvedení produktů na trh pro nové i stávající nabídky.

Nyní vám poskytujeme jedno měsíční zobrazení uvedení produktů na trh, které je publikováno v galerii zdrojů informací o připravenosti provozu. Toto zobrazení [měsíčního kalendáře spuštění produktu](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) nahradí komunikaci o spuštění jednotlivých produktů v galerii zdrojů provozní připravenosti a v Partnerské centrum oznámení.

Ke kalendáři pro spuštění tohoto [produktu se můžete také přihlásit z](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) komunitní [kolekce,](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) [zobrazení kalendáře](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated)a [bulletinů CSP.](https://partner.microsoft.com/resources/collection/csp-monthly-update#/) Jakmile každý měsíc publikujete kalendář spuštění produktu, upozorníme vás oznámením v galerii prostředků provozní připravenosti.

Informace týkající se nových a stávajících nabídek najdete i v protokolech změn ceníku a ceníku a také v blogech o produktech, průvodcích licencování a marketingových stránkách produktů.

Tato změna se bude vztahovat na starty následujících produktů:

- Místní Dynamics
- Microsoft 365
- Microsoft Dynamics 365
- Windows
- Server  
- nástroje
- Teams a Telco

Budeme pokračovat v odesílání konkrétních oznámení o uvedení produktů, která vyžadují podrobnosti o připravenosti provozu.

### <a name="next-steps"></a>Další kroky

Prohlédněte si materiály k tomuto tématu a podělte se o tyto informace s příslušnými účastníky ve vaší organizaci.

### <a name="questions"></a>Máte otázky?

Pokud máte další dotazy k těmto nabídekm, podívejte se na příslušné komunity Yammeru.

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a>Změny požadavků na onboarding zákazníků CSP

### <a name="categories"></a>Kategorie

- Datum: 25. 3. 2021
- Možnosti

### <a name="summary"></a>Souhrn

V rámci našeho závazku pomáhat partnerům a zákazníkům s provozem firmy na základě důvěry si vyžádáme další informace o zákaznících s účinností od 25. března 2021.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Cloud Solution Provider (CSP) s přímým vyúčtováním a nepřímými poskytovateli, kteří mají nové nebo stávající zákazníky v zemích uvedených v další části.

### <a name="details"></a>Podrobnosti

Microsoft běží na vztahu důvěryhodnosti. Zavázali jsme se poskytovat vyhovující, bezpečnou a zabezpečenou metodu ověřování zákazníků pro transakce zákaznických předplatných v programu CSP. 25. března 2021 představíme vylepšení rozhraní Partnerské centrum API Partnerské centrum uživatelského rozhraní, která ovlivní partnery, kteří splňují obě následující kritéria:

1. Partner má vztah přímé fakturace s Microsoftem (to znamená, že partner je partner s přímým vyúčtováním nebo nepřímý poskytovatel).

2. Partner spolupracuje s novými nebo stávajícími zákazníky v následujících zemích:

    - Thajsko
    - Vietnam
    - Turecko
    - Polsko
    - Jižní Afrika
    - Indie
    - Brazílie
    - Irák
    - Myanmar
    - Jižní Súdán
    - Saúdská Arábie
    - Spojené arabské emiráty
    - Venezuela

Partneři, kteří splňují tato kritéria, budou muset při onboardování nových zákazníků nebo  úpravě stávajících podrobností o zákaznících odeslat **ID** registrace společnosti zákazníka (označované také jako **INN** organizace zákazníka) a telefonní číslo. Tito partneři můžou volitelně zadat také **druhé jméno** zákazníka.

Upozorňujeme, že když přidáte ID registrace společnosti, měli byste použít své DIČ, a ne osobní ID zákazníka.

Partneři, kteří podniká s novými nebo stávajícími zákazníky v následujících zemích, jsou už v listopadu 2020 onboardované s předchozím vydáním.

- Arménie
- Ázerbájdžán
- Bělorusko
- Maďarsko
- Kazachstán
- Kyrgyzstán
- Moldavsko
- Rusko
- Tádžikistán
- Ukrajina
- Uzbekistán

Partneři se zákazníky ve zbytku světa budou mít možnost 25. března 2021 zadat  jako volitelné podrobnosti **ID** registrace **společnosti,** telefonní číslo a prostřední jméno pro zákazníky.

### <a name="next-steps"></a>Další kroky

- Podrobnější pokyny najdete v technické dokumentaci [](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) a nejčastějších dotazech ve vyhrazené kolekci partnerů.

- Připravte se na začlenění změn pomocí rozhraní PARTNERSKÉ CENTRUM API a webového uživatelského prostředí. Rozhraní API nebo sdk budou k dispozici pro testování.

- Při onboardingu nových zákazníků nebo úpravě stávajících podrobností o zákaznících nezapomeňte odeslat další data.

- Pokud používáte řešení dodavatele ovládacích panelů (CPV), obraťte se na svého dodavatele CPV.

### <a name="questions"></a>Máte otázky?

Pokud máte nějaké dotazy související s právním identifikátorem (nazývaným také "INN" nebo "TIN"). Microsoft nemůže poskytnout pokyny k daňovým záležitostem.

Pokud ve svých operacích s Microsoftem potřebujete podporu, [otevřete žádost o služby.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a>Opravy provedené k 1. březnu 2021 – ceník časově neomezeného softwaru

### <a name="categories"></a>Kategorie

- Datum: 23. 3. 2021
- Nabídky/trhy

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Nepřímí poskytovatelé a partneři s přímým vyúčtováním, kteří v programu Cloud Solution Provider software 

### <a name="details"></a>Podrobnosti

Ceník pro časově neomezené software zveřejněný 1. března 2021 zahrnoval trhy, které tam neměly být. 17. března 2021 se ceník časově neomezeného softwaru aktualizoval opravami. Tyto opravy se vztahují pouze na:

- ID produktu: DF77X4D43RKT 
- Název produktu: Windows 10 Home na Upgrade Pro pro Microsoft 365 Business
- Trh odebrání nebo nepodporovaný trh: AE, AF, AL, AM, AO, BA, BB, BD, PO, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, NC, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KW, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG , NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW

Tyto změny se vztahují pouze na výše uvedený produkt. Ostatní produkty nemají žádné opravy. 

### <a name="next-steps-and-resources"></a>Další kroky a zdroje informací

- Partneři, kteří provádí transakce s časově trvalým softwarem, by si měli stáhnout nejnovější ceník časově neomezeného softwaru.
- Popisné [mapování dvousmenné](/azure/marketplace/commercial-marketplace-co-sell-countries) zkratky na země najdete v kódech zemí v jednotlivých oblastech.
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> Vydání sady SDK na .NET Standard (v1.17.0)

### <a name="categories"></a>Kategorie

- Datum: 23. 3. 2021

- Možnosti
 
### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Partneři s přímým vyúčtováním a nepřímí poskytovatelé účastnící se programu CSP, kteří používají Partnerské centrum .NET SDK.

### <a name="details"></a>Podrobnosti

Od 23. března 2020 mohou partneři začít stahovat verzi [sady MicrosoftPartnerCenter.NETSDK (Galerie NuGet | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)a aktualizované ukázky SDK pro Partnerské centrum [GitHubu.](https://github.com/Microsoft/Partner-Center-DotNet-Samples) Tato verze zahrnuje aktualizace následujících metod:

#### <a name="audit-updated-new-operation-types"></a>Audit aktualizován: Nové typy operací

Přidali [jsme nové typy operací,](/partner-center/develop/auditing-resources) které vám poví, kdy zákazník DAP schválil a ukončil.

- DapAdminRelationshipApproved

- DapAdminRelationshipTerminated

#### <a name="audit-updated-new-resource-and-operation-types"></a>Audit aktualizován: Nové typy prostředků a operací

Přidání nových [typů prostředků a operací](/partner-center/develop/auditing-resources) pro podporu scénáře role adresáře zákazníka

- Nový typ prostředku CustomerDirectoryRole

- Typy operací AddUserMember a RemoveUserMember

#### <a name="sdk-updates-to-customer-accounts"></a>Aktualizace sady SDK pro zákaznické účty

- Podpora pro GET /customers/{id_tenanta_zákazníka}/directSignedMicrosoftCustomerAgreementStatus

- GET /customers/{id-tenanta zákazníka}/kvalifikace

- POST /customers/{customer_id}/qualifications?code={validationCode}

#### <a name="additional-changes"></a>Další změny

Následující změny jsou zavedené v rámci nového obchodování a jsou v současné době dostupné pouze na základě pozvánek partnerům, kteří jsou součástí prostředí M365/D365 New Commerce technical preview. Partneři, kteří nejsou součástí nového obchodního technical preview by si neměli všimnout dopadu a měli by být zpětně kompatibilní.

- Změny katalogu:

  - ZÍSKAT/Products/{Product-ID}/skus/{SKU-ID}

- Nákup a správa:
  - ZÍSKAT/customers/{customerId}/subscriptions
  - ZÍSKAT/customers/{customerId}/subscriptions/{subscriptionId}
  - /Customers/{customerId}/subscriptions/{subscriptionId} opravy
  - ZÍSKAT/customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities
  - ZÍSKAT/customers/{customerId}/subscriptions/{subscriptionId}/transitions
  - PŘÍSPĚVEK/customers/{customerId}/subscriptions/{subscriptionId}/transitions

### <a name="next-steps"></a>Další kroky

- Stáhněte si nejnovější verzi [MicrosoftPartnerCenter. NETSDK (galerie NuGet | Microsoft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)
- Stažení a kontrola [ukázek GitHubu](https://github.com/Microsoft/Partner-Center-DotNet-Samples)

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a>Nabídka CSP pro komerční web Marketplace a FY21 CSP pro opravňující nabídky

### <a name="categories"></a>Kategorie

- Datum: 2021-03-18
- Možnosti

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Neposkytovatelé nepřímých zprostředkovatelů a přímých partnerů v programu Cloud Solution Provider 

### <a name="details"></a>Podrobnosti

Nepřímá poskytovatelé a přímá Partnerská partneři v programu Cloud Solution Provider můžou prodávat nabídky třetích stran a získat motivaci slev pro každou způsobilou nabídku třetí strany, která je v partnerském centru nebo Azure Portal. Motivace bude ve formě rabatu na účtovaných prodejích pro příslušné nabídky a bude **k dispozici do 30. června 2021**.  

Pokračujte v učení o této nabídce komerčního webu Web Marketplace níže a kontaktujte své zákazníky ještě dnes a Identifikujte správné nabídky, které umožní jejich pokračující úspěšnost a digitální transformaci.

Spolupracujeme s nezávislými výrobci softwaru (ISV) za účelem uvedení nejnovějších řešení IaaS a SaaS na trh pro zákazníky Microsoftu. Vydavatelé ISV mají možnost povolit prodej svých nabídek prostřednictvím kanálu Microsoft Partner. Naše nabídky s nárokem na pobídky spadají do dvou kategorií:

- Vyberte Nabídky SaaS a IaaS třetích stran s incentivizovaným stavem spoluprodávku IP Azure. 

- Aplikace SaaS integrované s Teams nebo alespoň dvě Microsoft 365, jako jsou PowerPoint, Word, Excel, Outlook nebo SharePoint.

### <a name="next-steps-and-resources"></a>Další kroky a zdroje informací

- Přečtěte si o [příjmech pobídek pro partnery za](https://partner.microsoft.com/membership/partner-incentives) prodej oprávněných aplikací z marketplace, které jsou způsobilými pro pobídky. Nové nabídky se přidávají každý měsíc.  
- [Cloud Solution Provider prostředků pobídek pro partnery s přímým vyúčtováním](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [Cloud Solution Provider prostředků pobídek nepřímých poskytovatelů](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- Další informace [o prodeji](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) aplikací komerčního marketplace najdete v této prezentaci. Další zdroje informací najdete [tady.](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/) 
- Prozkoumejte katalog komerčního marketplace v [Partnerské centrum](../csp-commercial-marketplace-discover.md) [nebo Azure Portal](https://ms.portal.azure.com/#home)
- Integrace [aplikací do](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) firemního marketplace pomocí rozhraní API
- Oslovte isv, se kterou máte zájem podnikat.
- Nepřímí poskytovatelé se musí integrovat s využitím rozhraní API a vést prodejce, na kterých aplikacích se má prodávat.

### <a name="questions"></a>Máte otázky?  

V tomto [článku najdete](../csp-commercial-marketplace-overview.md) přehled komerčního marketplace v Partnerské centrum.

Pokud potřebujete další pomoc, můžete žádost o podporu vytvořit v Partnerské centrum. Další informace najdete na adrese [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a>Power BI Premium nabídky pojmenování a aktualizace předpokladů

### <a name="categories"></a>Kategorie

- Datum: 18. 3. 2021
- Možnosti

### <a name="summary"></a>Souhrn

Finální ceník pro 1. dubna 2021 se aktualizuje, aby byl srozumitelný pro pojmenování a/nebo požadované informace pro Power BI Premium na uživatele.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Přímý a nepřímý partneři poskytovatele Cloud Solution Provider (CSP)

### <a name="details"></a>Podrobnosti

Konečný Ceník od 1. dubna 2021 se aktualizuje, aby se zvýšila přesnost na pojmenování a informace o požadavcích pro Power BI Premium pro jednotlivé uživatele.

Až do doby, kdy se aktualizuje Poslední ceník, použijte informace v této části, abyste zajistili, že se správně objednal správný produkt.

Následující podrobnosti obsahují informace o ovlivněné SKU a požadovaných položkách.

| Zobrazované jméno nabídky na 1. březnu Preview ceníku |  Aktualizovaný zobrazovaný název nabídky na 1. dubnu – konečný Ceník| ID nabídky |
| ------ | ----------- | ----------- |
| Power BI Premium Add-On na uživatele (ceny neziskových zaměstnanců)  |  Power BI Premium pro uživatele Add-On **(Office)** (ceny neziskových zaměstnanců)   | 31c03289-47ab-4ab0-8df1-03742c127ac6   |

Aby si zákazníci mohli koupit tuto nabídku, musí mít některý z následujících požadavků:

| Zobrazované jméno nabídky | ID nabídky |
| ------ | ----------- |
| Microsoft 365 E5 (ceny neziskových zaměstnanců)  |  31bedf01-9e57-4ece-a53a-d3656a563931   |
|   Microsoft 365 E5 bez audio Conferencing (ceny neziskových zaměstnanců)|  b456810a-c414-4e07-98fc-ef74e8175a09|
|   Office 365 E5 (ceny neziskových zaměstnanců)| ce139fe5-8bd5-47ed-a5be-07c286f8b9e    |
|   Zkušební verze Office 365 E5 (ceny neziskových zaměstnanců)|  2f192efe-608a-4c9c-9d19-2b0b70b0962e|
|   Office 365 E5 bez audiokonference (ceny pro neziskové pracovníky)|  c3897426-9f49-4eaf-9b4d-7d9a1c72aef7|

Následující Power BI Premium má požadavek na nákup:

| Zobrazovaný název nabídky | ID nabídky |
| ------ | ----------- |
|   Power BI Premium na uživatele Add-On (ceny pro neziskové pracovníky)|  ef0b895b-681b-4026-a5b1-dda182a57d40 |

Zákazníci musí mít tento požadavek na nákup této nabídky:

| Zobrazovaný název nabídky | ID nabídky |
| ------ |----------|
| Power BI Pro (ceny pro neziskové pracovníky)  |   cabdfc93-5786-4224-bfd3-35d58f833b35 |

### <a name="next-steps"></a>Další kroky

Prohlédněte si materiály k tomuto tématu a podělte se o tyto informace s příslušnými účastníky ve vaší organizaci.  

### <a name="questions"></a>Máte otázky?

Pokud máte jakékoli dotazy k těmto nabídekm, podívejte se na příslušné komunity Yammeru. 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> Březnové aktualizace cen pro Microsoft 365 F3

### <a name="categories"></a>Kategorie

- Datum: 16. 3. 2021
- Nabídky/trhy

### <a name="summary"></a>Souhrn

Nesprávná cena z března 2021 byla opravena pro Microsoft 365 F3 British Pound (GBP) a Euro (EUR).

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Partneři, Microsoft 365 od 1. března 2021 do 17. března 2021 prostřednictvím programu Cloud Solution Provider (CSP) F3 v GB nebo EUR.

### <a name="details"></a>Podrobnosti

Microsoft vyřešil nesprávné ceny pro Microsoft 365 F3. Nesprávné ceny byly pro GB/s a EUR a pouze pro nabídky zakoupené od 1. března do 17. března 2021. Ovlivněné nabídky a měny jsou uvedené níže. 

| Název nabídky | Měna | ID nabídky | ID materiálu |
| ------ |----------- |----------- |----------- |
| Microsoft 365 F3 (dobročinný) | GBP | 57b722c2-c435-4bfb-9bc8-80509213a13a | AAD-11626 |
| Microsoft 365 F3 (komerční) | EUR| 3451a3b0-8cda-44a7-bad7-c30be81c4aaa | AAA-89898 |
 
Licence na březen a duben Preview – základní ceníky byly aktualizovány 16. března 17:00 tichomořského času (běžný čas).

### <a name="next-steps"></a>Další kroky

- Partneři by si měli stáhnout aktuální ceníky založené na licencích, a to v březnu i v dubnu Preview. Tyto ceny se v případě potřeby opraví.  
- Společnost Microsoft bude kontaktovat dotčené partnery v nadcházejících týdnech prostřednictvím e-mailu, aby jim informovala o dalších krocích souvisejících s opravou ovlivněných transakcí.

### <a name="questions"></a>Máte otázky?

Jakékoli další otázky vám poskytne příslušné komunity zprostředkovatele CSP pro Yammer.

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> Aktualizace názvu právní společnosti prostřednictvím partnerského centra

### <a name="categories"></a>Kategorie

- Datum: 2021-03-16
- Škálování & škály při zvyšování produktivity

### <a name="summary"></a>Souhrn

Od března 2021 se partneři Microsoft Partner Network (MPN) a poskytovatelé Cloud Solution Provider (CSP) můžou prostřednictvím partnerského centra aktualizovat svůj zákonný název společnosti.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Partneři programu MPN a neposkytovatelé nepřímých poskytovatelů CSP (neplatí pro partnery s přímým účtováním CSP)

### <a name="details"></a>Podrobnosti

Od března 2021 partneři programu MPN a nepřímý prodej CSP můžou aktualizovat svůj právní název společnosti prostřednictvím partnerského centra v souladu se svým vlastním způsobem. S touto novou funkcí už partneři nebudou muset odeslat lístek podpory pro partnerský partner, aby aktualizovali jeho název společnosti. Tím se při provádění těchto aktivit uloží značná doba pro partnery. 

Další informace najdete v tématu [Aktualizace vašeho zákonného obchodního profilu.](../update-your-partner-profile.md#update-your-legal-business-profile)

>[!NOTE]
>Zajistěte, aby název společnosti ve vašem oficiálním obchodním profilu bez pravopisných chyb a zkratek a přesně odpovídal oficiálním záznamům o firemní registraci. Další informace o aktualizaci profilu organizace najdete v tématu [Ověření profilu organizace.](../update-your-partner-profile.md#update-your-legal-business-profile)

### <a name="next-steps"></a>Další kroky

Sdílejte tyto informace v rámci vaší organizace, aby příslušný tým mohl zkontrolovat a aktualizovat své procesy.

### <a name="questions"></a>Máte otázky?

Další dotazy najdete v příslušných komunitách CSP Yammer.

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> Aktualizace na vývoj Cloud Solution Provider (CSP) a Open License změn programu

### <a name="categories"></a>Kategorie

- Datum: 15. 3. 2021
- Možnosti

### <a name="summary"></a>Souhrn

Do programu CSP (Cloud Solution Provider)a ke změnám programu Open Licensing přicházejí nové časově neomezené nabídky komerčního a veřejného sektoru.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Komerční distributory a spravované prodejce prodá Open License programu a také všichni partneři CSP, kteří provádí transakce s časově trvalým softwarem.

### <a name="details"></a>Podrobnosti

V září 2020 [Microsoft](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) oznámil sérii kroků na naší cestě digitální transformace k rozšíření příležitostí partnerům v programu CSP, včetně dostupnosti místního softwaru pro partnery. Díky těmto změnám rozšiřují své podnikání partneři a rozšiřují svůj dosah využitím softwarových licencí v PROGRAMU CSP a umožňují jim dosáhnout úspěchu v dnešním světě, který je prvním cloudem. Umožňují také zákazníkům přejít do cloudu a poskytují partnerům flexibilitu potřebnou pro hybridní cloudová prostředí zákazníků.

V pokračování této digitální transformace oznamujeme následující změny:

- 1. července 2021: Do ceníku pro program Open License se nepřidá žádné nové skladové položky, produkty ani propagační akce.

- 7. července 2021: Do ceníku časově neomezeného softwaru CSP přibyjí dvě komerční [](./2020-december.md#9)nabídky, Get Genuine Windows a Visual Studio Professional a nabídky veřejného sektoru (státní správa, vzdělávání a nezisková organizace – viz oznámení).  Ceník najdete v části software [nabídky prodej > price & nabízí](https://partnercenter.microsoft.com/pcv/sales) stránku v partnerském centru a bude se v tomto datu znovu publikovat.

Úplné podrobnosti týkající se vývoje programu CSP a Open License programových změn naleznete v **následujících krocích** níže.

### <a name="next-steps"></a>Další kroky:

- Vývoj programu CSP: Projděte si [Trvalá softwarová řešení v materiálech připravenosti programu Cloud Solution Provider](https://partner.microsoft.com/resources/collection/software-in-csp#/) . Pomocí této [mapy připravenosti](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) můžete rychle najít správné informace pro vaši roli.

- Změny Open License programu: Přečtěte si materiály pro [vývoj programu CSP a Open License program změny](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) připravenosti. Pomocí této [mapy připravenosti](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) můžete rychle najít správné informace pro vaši roli.

### <a name="questions"></a>Dotazy

Jakékoli další otázky vám poskytne příslušné komunity zprostředkovatele CSP pro Yammer.

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a>Aktualizace na předchozí oznámení: posouzení Premium, doplněk ke Správci dodržování předpisů

### <a name="categories"></a>Kategorie

- Datum: 2021-03-15
- Podpora růstu vaší firmy

### <a name="summary"></a>Souhrn

Nabídky zkušební verze by neměly být uvedené na ceníku a budou se odeberou.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Transakce partnerů prostřednictvím poskytovatele Cloud Solution Provider

### <a name="details"></a>Podrobnosti

Ceník by neměl být zahrnut do ceníku. Ty se odeberou z ceníku 1. května 2021.

Původní oznámení [najdete tady](./2021-february.md#4).

### <a name="additional-resources"></a>Další zdroje informací

- [Microsoft 365 zabezpečení E5 a dodržování předpisů](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [Sestavování a Správa hodnocení v nástroji Microsoft dodržování předpisů – Microsoft 365 dodržování předpisů](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a>Další kroky

Projděte si materiály k tomuto tématu a sdílejte tyto informace s příslušnými zúčastněnými stranami ve vaší organizaci.

### <a name="questions"></a>Máte otázky?

Otázky týkající se těchto nabídek najdete v příslušných komunitách Yammeru.

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> Migrace řešení od jednoho komerčního partnera (OCP) přejít na trh (GTM) do komerčního tržiště Microsoftu

### <a name="categories"></a>Kategorie

- Datum: 12. 3. 2021
- Možnosti

### <a name="summary"></a>Souhrn

Od 29. března 2021 se u vás začnou vyskytnout omezené možnosti nabídky OCP (One Commercial Partner) na trh (GTM). Doporučujeme vám migrovat řešení na komerční marketplace v Partnerské centrum.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Organizace se spoluprodá s řešeními v OCP GTM

### <a name="details"></a>Podrobnosti

V prosinci 2020 jsme zahájili cestu od nástroje Microsoft OCP GTM k komerčnímu marketplace Microsoftu v Partnerské centrum. Tento přechod rozšiřuje možnosti komerčního marketplace, kde můžete předvést řešení milionům zákazníků, obousměrně sdílet příležitosti s ostatními prodejci Microsoftu a partnery a společně prodávat inovativní řešení.

Další milník v přechodu se bude odehrát 29. března 2021. V tomto případě začnete mít omezené možnosti OCP GTM a některá pole se stanou jen pro čtení. Pokud se v současné době spoluprodáte s řešeními v OCP GTM, doporučujeme vám migrovat svá řešení na komerční marketplace, abyste využili výhod jeho funkcí a zjednodušili prostředí pro publikování. 

Přechodem na komerční marketplace Partnerské centrum primárním cílem prostředí pro publikování spoluprodávání. Tady můžete pokračovat v růstu firmy propojením vašich řešení s našimi sdílenými zákazníky prostřednictvím stejných kanálů a prostředí v produktech, které používáme pro produkty Microsoftu. [Přečtěte si další informace o komerčním marketplace.](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/)

### <a name="next-steps"></a>Další kroky

- Pokud jste řešení ještě neposouvali, postupujte [](/azure/marketplace/co-sell-solution-migration) podle pokynů uvedených v průvodci přechodem nebo si prohlédněte podrobný videokumerii, ve které můžete dokončit všechny aktivity migrace a začít publikovat vaše řešení na komerčním marketplace. [](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4)

- V případě dotazů týkajících se omezeného prostředí funkcí v OCP GTM si v nejčastějších dotazech ke komerčnímu marketplace Microsoftu prohlédněte požadavky na [spolutržby k publikování.](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf) (Viz část Omezené možnosti OCP GTM od 29. března 2021.)

### <a name="questions"></a>Máte otázky?

Pokud máte nějaké dotazy nebo potřebujete další informace, obraťte se na [podporu](https://partner.microsoft.com/support/?stage=1) .

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a>Rozšiřování nového prostředí pro obchod v programu Cloud Solution Provider (CSP) pro Azure na Rusko

### <a name="categories"></a>Kategorie

- Datum: 2021-03-10
- Možnosti

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Všichni partneři v Rusku procházejí v rámci programu Cloud Solution Provider (CSP).

### <a name="details"></a>Podrobnosti

Od března 10 2021 jsme s radostí oznamujeme dostupnost **nového prostředí pro obchodování v CSP pro Azure v Rusku**. Toto prostředí zjednodušuje a vylepšuje způsob, jakým zákazníci kupují a využívají služby Azure. Poskytne také partnerům v programu CSP konzistentní pohled na ceny Azure napříč prodejními pohyby, ceny za USD pro globální konzistenci, zarovnání data fakturace a přístup k Azure Cost Management.

### <a name="next-steps"></a>Další kroky

K dispozici je několik prostředků, které představují nové prostředí Azure Commerce a poskytují další informace. Nejnovější Nejčastější dotazy, balíčky, video a další informace najdete v [galerii prostředků aktualizace programu CSP](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a>Licenční klíč softwaru partnerského centra a stažení

### <a name="categories"></a>Kategorie

- Datum: 2021-03-04
- Možnosti

### <a name="summary"></a>Souhrn

Funkce pro stažení softwaru partnerského centra a plnění licenčního klíče se znovu nainstalovala.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Všichni partneři poskytovatele Cloud Solution Provider (CSP) postupující trvalé a serverové objednávky softwaru prostřednictvím partnerského centra

### <a name="details"></a>Podrobnosti

V reakci na zpětnou vazbu od partnerů aktualizujeme možnost plnění partnerského centra a získáte software a licenční klíče pro trvalé objednávky softwaru a předplatného serveru. Před odstraněním 19. ledna 2021 se obnoví do předchozího stavu. (Viz [oznámení](2020-september.md#17).)

Všimněte si, že licenční klíče softwaru a odkazy ke stažení jsou cenné a vysoce vyhledané – po prostředcích duševního vlastnictví. Pokud dojde k úniku, můžou se rychle vyčerpat z jejich aktivačních limitů a způsobit negativní činnost zákazníků a partnerů.

### <a name="next-steps"></a>Další kroky

Pokyny k použití a důležité pokyny k distribuci softwarových klíčů najdete v následujících zdrojích informací:

- [Prodej místního softwaru prostřednictvím programu CSP](../csp-on-premise-software.md)
- [Partnerské centrum průvodce novým komerčním provozem](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (viz **oddíl Pokyny k distribuci softwarových** klíčů).)

### <a name="questions"></a>Máte otázky?

Pokud máte k tomuto oznámení nějaké další dotazy, zkontrolujte příslušné komunity Yammeru.

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a>Migrace dohod z programu Partner Sales Connect (PSC) do Partnerské centrum

### <a name="categories"></a>Kategorie

- Datum: 4. 3. 2021
- Možnosti

### <a name="summary"></a>Souhrn

Partner Sales Connect (PSC) se od 31. března 2021 přesune na přístup jen pro čtení, takže doporučujeme začít s migrací vašich dohod z PSC do Partnerské centrum.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Partneři s obchody v PSC

### <a name="details"></a>Podrobnosti

V rámci našeho sdíleného závazku k růstu je spoluprodání s **Microsoftem** cestou, jak můžete být **zjištěni,** poskytovat své odborné znalosti a rozšiřovat nároky zákazníků na pozitivní výsledky zákazníků. Díky průměrné dohody, která je **3,5krát** rychlejší než obvykle, vám správa zkušeností se spoluprodávami v Partnerské centrum umožňuje prodávat napříč kanály přímých zákazníků, partnerů a prodejců Microsoftu a spravovat celý kanál referenčních doporučení na jednom místě.

Od **31. března 2021** se **PSC** přesune na přístup jen pro čtení, takže doporučujeme začít s přechodem na Partnerské centrum a přistupovat k těmto vylepšením funkcí:  

- **Přesnější směrování** dohod, které sdílíte s Microsoftem, správnému prodejci na základě typu pomoci, kterou potřebujete.
- **Počáteční ověření** způsobilosti dohody pro řešení s nárokem na pobídky a splnění kritérií programu ISV Connect, které zjednodušuje proces schvalování a ověření konečného důkazu o provedení.
- **Bezproblémové uživatelské prostředí** pro správu všech příležitostí ke spoluprodeji a kvalifikovaných prodejních zájemců na jednom místě.

Nedávno jsme také přidali nové funkce v Partnerské centrum, které vám pomohou s vaším přesunem:

- [Hromadné operace pro příležitosti ke spoluprodání](../bulk-operations.md)
- [Funkce deal migration](../psc-to-pc.md) (Dohody o migraci) (viz **část Migrace dohody o PSC).)**

Díky prostředí spoluprodeje v Partnerské centrum budou mít prodejní týmy více času na to, aby se soustředil na rozvoj potenciálních zákazníků a příležitostí, uzavírání dohod a vytváření dlouhotrajících vztahů se zákazníky.

### <a name="next-steps"></a>Další kroky

Pomocí průvodce Partnerské centrum [převodem](../psc-to-pc.md) najdete postup migrace dohod z PSC do Partnerské centrum.

### <a name="questions"></a>Máte otázky?

Pokud máte další dotazy, kontaktujte [podporu](https://partner.microsoft.com/support/?stage=1).

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a>Nové produkty a nabídky Microsoft Dynamics 365 dostupné 1. dubna 2021

### <a name="categories"></a>Kategorie

- Datum: 4. 3. 2021
- Možnosti

### <a name="summary"></a>Souhrn

1. dubna 2021 bude Microsoft zahajovat několik nových produktů a nabídek pro program Cloud Solution Provider (CSP).

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Všichni partneři, kteří provádí transakce prostřednictvím Cloud Solution Provider (CSP)

### <a name="details"></a>Podrobnosti

1. dubna 2021 bude Microsoft spouštět následující nové produkty a nabídky:

- Power BI Premium na uživatele
- Geografické a segmentační rozšíření USL Customer Voice a Marketing

**Power BI Premium na uživatele**

Microsoft představí první nabídky pro uživatele Power BI Premium uživatele. Power BI Premium se momentálně prodává pouze v konstruktoru kapacity. Power BI Premium na uživatele poskytuje přístup k podnikovým business intelligence (BI) a analytickým možnostem. Její flexibilní individuální licencování je k řešení pro malé a střední firmy.

Další informace [o Power BI najdete v podrobnostech](/power-platform-release-plan/2020wave2/power-bi/planned-features) o této verzi.


**Podrobnosti o nabídce**

Všimněte si, že název nabídky se mírně liší od verze Preview ceníku.

| Název nabídky | ID nabídky |
| ------ |----------- |
| Power BI Premium na uživatele | 9c810018-9356-4903-95ab-eeb956289290 | 
| Power BI Premium na uživatele pro vyučujícího | 3affc44f-f372-4ad5-8657-aadd9574fce0 | 
| Power BI Premium na uživatele pro studenty | 657eea87-d0b0-4c89-8c8e-9b04395bd940 | 
| Power BI Premium na uživatele (ceny neziskových zaměstnanců) | 7a0a856c-059f-45dd-9d26-ae27992e706a | 
| Power BI Premium pro uživatele Add-On | 244ff87e-5925-44a0-bf31-cea189719b58 | 
| Power BI Premium Add-On na uživatele pro vyučující | 5da849bd-b8f7-4340-b4f4-3a9eaeb8987e | 
| Power BI Premium Add-On na uživatele pro studenty | cf62d70d-5af5-422a-bda8-97936402ac8e | 
| Power BI Premium Add-On na uživatele (ceny neziskových zaměstnanců) | 31c03289-47ab-4ab0-8df1-03742c127ac6 | 

**USL a rozšiřování geografických a segmentů zákazníků**

Jako při spuštění z prosince 2020 se přidávají nabídky hlasu a marketingu pro zákazníky Dynamics 365 za účelem přidání nových zemí a dalších neziskových a vzdělávacích SKU.

| Název nabídky | ID nabídky |
| ------ |----------- |
| Dynamics 365 Customer Voice USL (ceny neziskových zaměstnanců) | 7a8642a5-481e-4906-a642-b56dbeeb62a0 |
| Dynamics 365 Customer Voice USL pro vyučujícího | 85162d70-9676-4cf6-a4bc-a0d6672f2657 |

Další informace o těchto nabídek najdete na následujících stránkách:

- [Domovská stránka Dynamics 365 Customer Service Voice](https://dynamics.microsoft.com/customer-voice/overview/)
- [Domovská stránka Dynamics 365 Marketing](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a>Další kroky

Prohlédněte si materiály k tomuto tématu a podělte se o tyto informace s příslušnými účastníky ve vaší organizaci.  

### <a name="questions"></a>Máte otázky?

Pokud máte jakékoli dotazy k těmto nabídekm, podívejte se na příslušné komunity Yammeru. 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> Microsoft Univerzální tisk nyní k dispozici v některých sadech

### <a name="categories"></a>Kategorie

- Datum: 3. 3. 2021
- Možnosti

### <a name="summary"></a>Souhrn

Microsoft Univerzální tisk bude k dispozici pro transakce v rámci Microsoft 365 sad a jako samostatný doplněk od 1. března 2021.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Všichni partneři, kteří provádí transakce prostřednictvím Cloud Solution Provider (CSP)

### <a name="details"></a>Podrobnosti

[Univerzální tisk](https://aka.ms/universalprint) je Microsoft 365 tisková služba, která eliminuje potřebu místních tiskových serverů a umožňuje zařízením s Windows tisknout na tiskárny zaregistrované v Azure. Bude k dispozici pro transakce od 1. března 2021.

Pracovní pracovníci těží z tisku bez ovladačů, zjednodušeného zjišťování tiskáren založeného na poloze a intuitivního prostředí tisku bez křivek učení. Zařízení připojená k Azure Active Directory (Azure AD) používají k zabezpečenému tisku stávající přihlašovací údaje Azure AD. Správci spravují tisk pomocí Azure Portal a můžou snadno připojit tiskárny s nativní podporou pro Univerzální tisk. Univerzální tisk můžete nasadit s nekompatibilní tiskárnou pomocí Konektor pro Univerzální tisk softwaru.

Univerzální tisk startu se znovu doplní do Windows E3, A3, E5 a A5 a Microsoft 365 BP, F3, E3, A3, E5 a A5.  

**Podrobnosti o nabídce**

Všimněte si, že název nabídky se mírně liší od verze Preview ceníku.

| Název nabídky | ID nabídky | ID materiálu |
| ------ |----------- |----------- |  
| Doplněk objemu univerzálního tisku (úlohy 500) – Microsoft 365  | cb131356-45ee-4ae2-8537-873b706c8e75     | 9BI-00004   |
| Doplněk objemu univerzálního tisku (úlohy 500) pro vyučující – Microsoft 365   | 477bee81-9872-43d6-91d3-c72390bfcf49   | 9BK-00004   |
| Doplněk objemu univerzálního tisku (úlohy 500) – Windows    | d3ddc493-5741-4e0d-a02d-07edbb0bb72e   | 9BI-00002   |
| Doplněk objemu univerzálního tisku (úlohy 500) pro vyučujícího – Windows   |  d0862f05-80f5-4fd4-8432-fe72dd893cc7  | 9BK-00002   |

### <a name="next-steps"></a>Další kroky

Seznamte se s ceníkem a s [přehledem univerzálního tisku](/universal-print/fundamentals/universal-print-whatis). Tyto informace Sdílejte se všemi odpovídajícími kontakty ve vaší organizaci.

### <a name="questions"></a>Máte otázky?

Jakékoli otázky týkající se těchto nabídek najdete v příslušných komunitách Yammeru.