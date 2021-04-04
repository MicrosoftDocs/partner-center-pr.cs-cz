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
ms.openlocfilehash: 5b8c5f52207a7b9a49d07885a36b61486be45497
ms.sourcegitcommit: 60bbb8f4056120264b769f94431f84d86984c2e9
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/03/2021
ms.locfileid: "106280866"
---
# <a name="march-2021-announcements"></a>Oznámení z března 2021

Tato stránka poskytuje oznámení pro partnerské Centrum Microsoftu na březen 2021.

________________
## <a name="updated-csp-customer-address-validation-api-now-available-for-testing"></a><a name="18"></a>Aktualizované rozhraní API pro ověřování zákaznických adres poskytovatele CSP je nyní k dispozici pro testování

### <a name="categories"></a>Kategorie

- Datum: 2021-03-31
- Možnosti

### <a name="summary"></a>Souhrn

V rámci našeho závazku pomáhat partnerům a zákazníkům, kteří provozují své podnikání na základě důvěry, budeme zvát partneři po celém světě, aby otestovali změny v rozhraní ValidateAddress API.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Všichni partneři poskytovatele CSP Direct účtují a nepřímá poskytovatelé, kteří vytvářejí nové nebo aktualizují podrobnosti stávajících adres zákazníka

### <a name="details"></a>Podrobnosti

Microsoft běží na důvěryhodnosti. Zavázali jsme se poskytovat kompatibilní, bezpečnou a zabezpečenou metodu odesílání ověření zákaznické adresy pro účely transakcí předplatných zákazníků v programu CSP. V dnešní době 31. března 2021 jsme zavedli změny rozhraní ValidateAddress API, které bychom Vás pozvali k testování, před tím, než budete moct začít pracovat se změnami v červnu 2021. 

Všimněte si, že tyto změny mají vliv pouze na rozhraní ValidateAddress API. Rozhraní API CreateCustomer a UpdateBillingProfile nejsou ovlivněná.

Odpověď vrátí jednu z následujících stavových zpráv:

| Status | Popis | Počet vrácených navrhovaných adres |
|----------|-------------|-------------------|
| VerifiedShippable | Adresa je ověřena a může být expedována. | Jednoduché |
| Ověřují | Adresa je ověřena. | Jednoduché |
| InteractionRequired | Navrhované adresy byly významně změněny a potřebuje potvrzení uživatele. | Jednoduché |
| StreetPartial | Daná ulice v adrese je částečně a potřebuje další informace. | Více – maximálně tři|
| PremisesPartial | Daný prostor (stavební číslo, číslo sady atd.) je částečný a potřebuje další informace. | Více – maximálně tři |
| Několik | Adresa obsahuje několik polí, která jsou v této adrese částečně (případně také včetně StreetPartial a PremisesPartial). | Více – maximálně tři |
| Žádné | Adresa je nesprávná. | Žádné |
| NotValidated | Adresu nelze odeslat prostřednictvím procesu ověřování.  | Žádné |

Po odeslání adresy, která se má ověřit prostřednictvím rozhraní ValidateAddress API, se vrátí následující schéma odpovědi:

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

Podívejte se na tuto ukázkovou odpověď. Všimněte si, že pro nás odpověď vrátí další příponu se čtyřmi číslicemi, pokud pro PSČ zadáte jenom pět číslic.

```csharp
// IAggregatePartner partnerOperations;
// string customerId;
// s{
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

- Sdílejte své ID tenanta izolovaného prostoru s naším odborníkem na danou problematiku (MSP), Ali pískově, který se má zahrnout do testovacího letu, abyste mohli začít připravovat aktualizaci.

- Pokud používáte řešení v rámci ovládacího panelu (CPV), obraťte se na CPV.

### <a name="questions"></a>Máte otázky?

Pokud máte nějaké dotazy nebo potřebujete podporu pro vaše operace s Microsoftem, obraťte se na svého partnera, který podporuje Yammer.

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
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a>Operace s Microsoftem: Úvod do kalendářního spuštění produktu

### <a name="categories"></a>Kategorie

- Datum: 2021-03-25
- Nabídky | Moderní pracoviště

### <a name="summary"></a>Souhrn

V reakci na zpětnou vazbu od partnerů budou operace společnosti Microsoft zjednodušovat komunikaci při spuštění produktu.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Partneři poskytovatele Cloud Solution Provider (CSP)

### <a name="details"></a>Podrobnosti

Společnost Microsoft se zavazuje nepřetržitě zdokonalit partnerské prostředí. Máme vám zpětnou vazbu od vás, že od Microsoftu jste obdrželi příliš mnoho komunikací, včetně duplicitních oznámení o spuštění produktu.

V reakci na vaši zpětnou vazbu společnost Microsoft zjednodušila možnosti připravenosti na spuštění produktů pro nové a stávající nabídky.

Teď vám nabízíme měsíční pohled na spuštění produktu, který je publikovaný v galerii prostředků připravenosti na operace. Tento měsíční [Náhled spuštění produktu](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) nahradí konkrétní komunikaci na spuštění produktu v galerii prostředků připravenosti na operace a v oznámeních partnerského centra.

K tomuto [kalendáři](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) můžete také přistupovat z [kolekcí komunit](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [zobrazení kalendáře](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated)a [bulletinů CSP](https://partner.microsoft.com/resources/collection/csp-monthly-update#/). Když publikujete kalendář pro spuštění produktu měsíčně s oznámením v galerii prostředků připravenosti na provoz, pošleme vám oznámení.

Informace týkající se nové a stávající nabídky najdete pořád v protokolech pro náhled ceníku a v protokolech změn ceníku a také v blogu k produktům, licenčních průvodcích a na stránkách pro marketing produktů.

Tato změna se bude vztahovat na spuštění následujících produktů:

- Místní aplikace Dynamics
- Microsoft 365
- Microsoft Dynamics 365
- Windows
- Server  
- nástroje
- Týmy a výpovědi

Budeme dál posílat konkrétní oznámení ke spuštění produktu, které vyžaduje podrobnosti o připravenosti na operace.

### <a name="next-steps"></a>Další kroky

Projděte si materiály k tomuto tématu a sdílejte tyto informace s příslušnými zúčastněnými stranami ve vaší organizaci.

### <a name="questions"></a>Máte otázky?

Další otázky týkající se těchto nabídek najdete v příslušných komunitách Yammeru.

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a>Změny požadavků na registraci zprostředkovatele CSP pro zákazníky

### <a name="categories"></a>Kategorie

- Datum: 2021-03-25
- Možnosti

### <a name="summary"></a>Souhrn

V rámci našeho závazku pomáhat partnerům a zákazníkům, kteří provozují své podnikání na základě důvěry, budeme požadovat další informace o zákaznících, účinnost 25. března 2021.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Partneři poskytovatele Cloud Solution Provider (CSP) a nepřímá poskytovatelé, kteří mají nové nebo existující zákazníky v zemích uvedených v další části

### <a name="details"></a>Podrobnosti

Microsoft běží na důvěryhodnosti. Zavázali jsme se poskytovat vyhovující, bezpečné a zabezpečené metody ověřování zákazníků pro transakce předplatných zákazníka v programu CSP. 25. března 2021 budeme zavádět vylepšení rozhraní API partnerského centra a uživatelského rozhraní, které bude mít vliv na partnery, kteří splňují obě následující kritéria:

1. Partner má přímý fakturační vztah s Microsoftem (to znamená, že partner je buď přímým partnerem, nebo nepřímým poskytovatelem).

2. Partner pracuje s novými nebo stávajícími zákazníky v těchto zemích:

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

Partneři, kteří splňují kritéria, budou muset odeslat **registrační ID společnosti** zákazníka (označované také jako **DIČ organizace** zákazníka) a **telefonní číslo** , když připojí nové zákazníky nebo změní stávající podrobnosti o zákaznících. Tito partneři můžou volitelně zadat také **druhé jméno** zákazníka.

Všimněte si, že při přidání registračního ID vaší společnosti byste měli použít své obchodní daňové ID, nikoli osobní ID zákazníka.

Partneři, kteří pracují s novými nebo stávajícími zákazníky v následujících zemích, už jsou připojení k předchozí verzi v listopadu 2020.

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

Partneři se zákazníky ve zbývající části světa budou mít možnost 25. března 2021 pro zadání **ID registrace společnosti**, **telefonního čísla** a **středního jména** pro zákazníky jako volitelné podrobnosti.

### <a name="next-steps"></a>Další kroky

- Podrobnější pokyny najdete v technické dokumentaci a nejčastější dotazy v [kolekci vyhrazených partnerů](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) .

- Připravte se na začlenění změn pomocí rozhraní API partnerského centra a uživatelského prostředí pro web. Pro testování bude k dispozici rozhraní API/sady SDK.

- Nezapomeňte odeslat další data při připojování nových zákazníků nebo úpravách stávajících informací o zákaznících.

- Pokud používáte řešení v rámci ovládacího panelu (CPV), obraťte se na CPV.

### <a name="questions"></a>Máte otázky?

Pokud máte dotazy související s platným identifikátorem (označovaným také jako DIČ nebo DIČ), kontaktujte daňového poradce nebo místní finanční kancelář. Microsoft nemůže poskytnout pokyny k daňovým aspektům.

Pokud potřebujete podporu v rámci svých operací s Microsoftem, [otevřete žádost o služby](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a>Opravy provedené 1. března 2021, což je trvalá Ceníková cena softwaru

### <a name="categories"></a>Kategorie

- Datum: 2021-03-23
- Nabídky/trhy

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Nepřímá poskytovatelé a Přímí partneři poskytující transakční transakce s probíhajícím softwarem v programu Cloud Solution Provider 

### <a name="details"></a>Podrobnosti

Ceník pro trvale zpracovaný software zveřejněný 1. března 2021 zahrnoval trhy, které by se tam nemusely nastavovat. Ceník trvalého softwaru byl aktualizován 17. března 2021 se opravami. Tyto opravy byly platné pouze pro:

- ID produktu: DF77X4D43RKT 
- Název produktu: upgrade Windows 10 Home na verzi pro pro Microsoft 365 Business
- Odebrané nebo nepodporované trhy: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, ČERNOBÍLé, by, BZ, CI, CL, CM, CO, CR, SH, DO, DZ, ES, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, SWEETIQ, JM, JO, KE, KG, KN, KW, KY, KZ, CR, LK, LY, MA, MC, MD, já, MN, M0, , NI,, NP, OM, PA, PE, PH, PK, PR, PY, QA, R, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, G, UY, UZ, VE, VN, BE, ZM, ZW

Tyto změny se vztahují pouze na výše uvedený produkt. Jiné produkty neobsahovaly žádné opravy. 

### <a name="next-steps-and-resources"></a>Další kroky a zdroje informací

- Partneři, kteří pracují s nezpracovaným softwarem, by si měli stáhnout nejnovější Ceník softwaru s trvalou cenou.
- V části [kódy zemí v oblasti](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) najdete popisné mapování obou zkratek na země.
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> Vydání sady SDK na .NET Standard (v 1.17.0)

### <a name="categories"></a>Kategorie

- Datum: 2021-03-23

- Možnosti
 
### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Přímé partnery a nepřímá poskytovatelé, kteří se účastní programu CSP, kteří používají sadu SDK pro partnerských Center.

### <a name="details"></a>Podrobnosti

Od března 23 2020 můžou partneři začít stahovat verzi [MicrosoftPartnerCenter. NETSDK (galerie NuGet | Microsoft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)spolu s aktualizovanými [ukázkami](https://github.com/Microsoft/Partner-Center-DotNet-Samples)služby Public partner Center SDK GitHub. Tato verze zahrnuje aktualizace následujících metod:

#### <a name="audit-updated-new-operation-types"></a>Audit byl aktualizován: nové typy operací

Přidání nových [typů operací](https://docs.microsoft.com/partner-center/develop/auditing-resources) pro znalost, kdy zákazník schválil a ukončil DAP.

- DapAdminRelationshipApproved

- DapAdminRelationshipTerminated

#### <a name="audit-updated-new-resource-and-operation-types"></a>Audit byl aktualizován: nové typy prostředků a operací

Přidali jsme nové [typy prostředků a operací](https://docs.microsoft.com/partner-center/develop/auditing-resources) pro podporu scénáře role adresáře zákazníka.

- Nový typ prostředku "CustomerDirectoryRole"

- Typy operací "AddUserMember" a "RemoveUserMember"

#### <a name="sdk-updates-to-customer-accounts"></a>Aktualizace sady SDK u zákaznických účtů

- Podpora pro GET/customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus

- ZÍSKAT/Customers/{Customer-tenant-ID}/Qualifications

- POST/Customers/{customer_id}/Qualifications? Code = {validationCode}

#### <a name="additional-changes"></a>Další změny

V rámci nového obchodu byly zavedeny následující změny, které jsou aktuálně k dispozici pouze partnerům, kteří jsou součástí M365/D365 New Commerce Experience Technical Preview. Partneři, kteří nejsou součástí nové verze nástroje Commerce Technical Preview, by neměli poznamenat dopady a měly by být zpětně kompatibilní.

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

Spolupracujeme s nezávislými výrobci softwaru (ISV) za účelem uvedení nejnovějších řešení IaaS a SaaS na trh pro zákazníky Microsoftu. Vydavatelé ISV mají možnost povolit prodej svých nabídek prostřednictvím kanálu Microsoft Partner. Naše pobídkové nabídky spadají do dvou kategorií:

- Vyberte SaaS a IaaS nabídky třetích stran pomocí Azure IP spoluprodejního stavu motivovaní. 

- SaaS aplikace integrované s týmy nebo aspoň dvě Microsoft 365 kancelářské aplikace, jako je PowerPoint, Word, Excel, Outlook nebo SharePoint.

### <a name="next-steps-and-resources"></a>Další kroky a zdroje informací

- Přečtěte si, jak získat [pobídky partnerských](https://partner.microsoft.com/membership/partner-incentives) webů pro prodej oprávněných aplikací na webu Marketplace. Nové nabídky se přidávají měsíčně.  
- [Prostředky pro definanční partnery poskytovatele Cloud Solution Provider Direct](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [Prostředky pro motivaci nepřímých poskytovatelů Cloud Solution Provider](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- Přečtěte si tuto [prezentaci](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) , kde najdete další informace o prodeji komerčních aplikací z webu Marketplace. Další materiály najdete [tady](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/). 
- Prozkoumejte katalog komerčního tržiště v [partnerském centru](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) nebo [Azure Portal](https://ms.portal.azure.com/#home)
- Použití [rozhraní API](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) k integraci aplikací do Marketplace vaší společnosti
- Přihlaste se k nezávislým výrobcům softwaru, se kterým se zajímá vaše podnikání
- Neposkytovatelé nepřímých zprostředkovatelů potřebují integrovat pomocí rozhraní API a prodejců s postupy, na kterých se aplikace prodávají.

### <a name="questions"></a>Máte otázky?  

V [tomto článku](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) najdete přehled komerčního tržiště v partnerském centru.

Pokud potřebujete další pomoc, můžete vytvořit žádost o podporu v partnerském centru. Další informace najdete na adrese [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a>Power BI Premium nabídky pro pojmenování a požadované aktualizace

### <a name="categories"></a>Kategorie

- Datum: 2021-03-18
- Možnosti

### <a name="summary"></a>Souhrn

Konečný Ceník od 1. dubna 2021 se aktualizuje, aby se zvýšila přesnost na pojmenování a informace o požadavcích pro Power BI Premium pro jednotlivé uživatele.

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
|   Office 365 E5 bez audio Conferencing (ceny za neziskové zaměstnance)|  c3897426-9f49-4eaf-9b4d-7d9a1c72aef7|

Pro nákup je nutné mít následující nabídku Power BI Premium:

| Zobrazované jméno nabídky | ID nabídky |
| ------ | ----------- |
|   Power BI Premium Add-On na uživatele (ceny neziskových zaměstnanců)|  ef0b895b-681B-4026-a5b1-dda182a57d40 |

Aby si zákazníci mohli koupit tuto nabídku, musí mít tyto předpoklady:

| Zobrazované jméno nabídky | ID nabídky |
| ------ |----------|
| Power BI Pro (ceny neziskových zaměstnanců)  |   cabdfc93-5786-4224-bfd3-35d58f833b35 |

### <a name="next-steps"></a>Další kroky

Projděte si materiály k tomuto tématu a sdílejte tyto informace s příslušnými zúčastněnými stranami ve vaší organizaci.  

### <a name="questions"></a>Máte otázky?

Jakékoli otázky týkající se těchto nabídek najdete v příslušných komunitách Yammeru. 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> Aktualizace ceny pro Microsoft 365 F3 v březnu

### <a name="categories"></a>Kategorie

- Datum: 2021-03-16
- Nabídky/trhy

### <a name="summary"></a>Souhrn

Nesprávná cena z března 2021 byla opravena pro Microsoft 365 F3, British (GBP) a eura (EUR).

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Partneři kupují Microsoft 365 F3 v GBP nebo EUR v rozmezí od 1. března 2021 v rámci programu Cloud Solution Provider (CSP).

### <a name="details"></a>Podrobnosti

Společnost Microsoft vyřešila nesprávné ceny za Microsoft 365 F3. Nesprávné ceny jsou pro GBP a EUR a jenom pro nabídky zakoupené v rozmezí od 1. března 2021. Ovlivněné nabídky a měny jsou uvedeny níže. 

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

Další informace najdete v tématu [aktualizace svého obchodního profilu](../update-your-partner-profile.md#update-your-legal-business-profile).

>[!NOTE]
>Ujistěte se, že název společnosti ve vašem oficiálním obchodním profilu není bez pravopisných chyb a zkratek a přesně odpovídá vašim oficiálním registračním záznamům společnosti. Další informace o aktualizaci profilu vaší organizace najdete v tématu [ověření profilu vaší organizace](../update-your-partner-profile.md#update-your-legal-business-profile).

### <a name="next-steps"></a>Další kroky

Tyto informace můžete sdílet v rámci organizace, aby mohl příslušný tým zkontrolovat a aktualizovat své procesy.

### <a name="questions"></a>Máte otázky?

Jakékoli další otázky vám poskytne příslušné komunity zprostředkovatele CSP pro Yammer.

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> Aktualizace pro vývoj programu Cloud Solution Provider (CSP) a Open License změny programu

### <a name="categories"></a>Kategorie

- Datum: 2021-03-15
- Možnosti

### <a name="summary"></a>Souhrn

Nový komerční a veřejný sektor trvalé nabídky softwaru přicházejí do programu Cloud Solution Provider (CSP) spolu se změnami v programu Open Licensing.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Komerční distributoři a spravováni prodejci se prodávají prostřednictvím Open License programu a také všichni partneři CSP s podporou trvalého softwaru.

### <a name="details"></a>Podrobnosti

V září 2020 společnost Microsoft [oznámila](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) řadu kroků v naší cestě k digitální transformaci, aby bylo možné rozšiřovat příležitosti pro partnery v programu CSP, včetně dostupnosti místního softwaru pro partnery. Tyto změny umožňují partnerům rozšiřovat svou firmu a rozšířit jejich dosah tím, že využívají licence na software v cloudu, a jejich umístění pro úspěch v dnešním cloudovém světě. Umožňují také přechody zákazníků do cloudu a poskytují partnerům potřebnou flexibilitu pro hybridní cloudová prostředí zákazníka.

V návaznosti na tuto digitální transformaci oznamujeme následující změny:

- 1. července 2021: do ceníku Open License programu nebudou přidány žádné nové SKU, produkty ani propagační akce.

- 7. července 2021: dvě komerční nabídky, Získejte originální Windows a Visual Studio Professional a nabídky veřejného sektoru (státní, vzdělávací a neziskové – viz [oznámení](./2020-december.md#9)) se přidají do ceníku trvalého softwaru CSP.  Ceník najdete v části software [nabídky prodej > price & nabízí](https://partnercenter.microsoft.com/pcv/sales) stránku v partnerském centru a bude se v tomto datu znovu publikovat.

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

- Datum: 2021-03-12
- Možnosti

### <a name="summary"></a>Souhrn

Od 29. března 2021 zahájíte práci s omezeným počtem funkcí GTM (komerční partner), které se vztahují k uvedení na trh (OCP). Doporučujeme migrovat vaše řešení na komerční tržiště v partnerském centru.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Organizace, které společně prodávají s řešeními v OCP GTM

### <a name="details"></a>Podrobnosti

V prosinci 2020 jsme začali cestu od nástroje Microsoft OCP GTM k komerčnímu tržišti Microsoftu v partnerském centru. Tento přechod rozšiřuje možnosti komerčního tržiště, kde můžete předprezentovat vaše řešení miliony zákazníků, obousměrně sdílet příležitosti s ostatními prodejci Microsoftu a partnerů a společně prodávat inovativní řešení.

Další milník v přechodu bude uskutečněn 29. března 2021. To je, když začnete používat omezené možnosti OCP GTM, přičemž některá pole se stanou jen pro čtení. Pokud v současné době spolupracujete s řešeními v OCP GTM, doporučujeme vám migrovat vaše řešení na komerční tržiště, abyste mohli využívat své možnosti a zjednodušili své možnosti publikování. 

Přechod na komerční tržiště poskytuje partnerskému centru primární cíl pro spoluprodejní prostředí pro publikování. Je to místo, kde můžete dál rozšiřovat své podnikání propojením vašich řešení s našimi sdílenými zákazníky přes stejné kanály a prostředí v produktu, které používáme pro produkty Microsoftu. [Přečtěte si další informace o komerčním tržišti](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).

### <a name="next-steps"></a>Další kroky

- Pokud jste vaše řešení ještě nepřesunuli, postupujte podle pokynů v [Průvodci přechodem](/azure/marketplace/co-sell-solution-migration) nebo si prohlédněte [podrobné výukové video](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) , které vám umožní dokončit všechny migrační aktivity a zahájit publikování vašich řešení na komerčním webu Marketplace.

- Otázky týkající se omezeného prostředí funkcí v systému OCP GTM najdete v tématu [Nejčastější dotazy k požadavkům pro publikování na komerčním webu Microsoft Marketplace](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf). (Další informace najdete v části "OCP GTM – omezené možnosti od 29. března 2021.")

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

Pokyny k používání a důležité pokyny k distribuci softwarového klíče najdete v následujících zdrojích informací:

- [Prodej místního softwaru prostřednictvím programu CSP](../csp-on-premise-software.md)
- [Průvodce vytvořením nové obchodní příručky pro partnerský](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) software (viz část **pokyny k distribuci softwarových klíčů** )

### <a name="questions"></a>Máte otázky?

Pokud máte další dotazy k tomuto oznámení, Projděte si příslušné komunity Yammeru.

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a>Migrace vašich obchodů z partnera Sales Connect (PSC) do partnerského centra

### <a name="categories"></a>Kategorie

- Datum: 2021-03-04
- Možnosti

### <a name="summary"></a>Souhrn

Partner Sales Connect (PSC) se přesune k přístupu jen pro čtení od 31. března 2021, proto doporučujeme začít migrovat vaše obchody z PSC do partnerského centra.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Partneři s obchody v PBV

### <a name="details"></a>Podrobnosti

V rámci našeho sdíleného závazku na růst se dá **společně prodávat pomocí Microsoftu** cesta, která se má **zjistit, zajistit vaše odbornost a rozšířit nároky zákazníků** na pozitivní výsledky zákazníků. Díky průměrnému obchodování, který je **3,5 časů rychleji** než normální, vám Správa možností společného prodeje v partnerském centru umožní prodávat přes přímé kanály zákazníka, partnera a prodejce Microsoftu a spravovat celý kanál odkazů na jednom místě.

**PBV** se přesune k **přístupu jen pro čtení** od **31. března 2021**, proto doporučujeme začít přesun do partnerského centra a získat přístup k těmto vylepšením schopností: 

- Přesnější **Směrování** všech obchodů, které sdílíte s Microsoftem, s dopravou prodávající na základě typu pomoci, kterou potřebujete.
- **Ověření nároku** na zajištění opravňujícího řešení pro pobídku a pro splnění kritérií programu ISV Connect, které zjednodušují proces schvalování a konečné ověření platnosti (PoE).
- **Bezproblémové uživatelské prostředí** pro správu všech příležitostí společného prodeje a potenciálních zákazníků na jednom místě.

V partnerském centru jsme také nedávno přidali nové funkce, které vám pomůžou při přesunu:

- [Hromadné operace pro společný prodej příležitostí](../bulk-operations.md)
- [Funkce migrace koupě](../psc-to-pc.md) (viz část věnované **migraci PSC** .)

S využitím možností společného prodeje v partnerském centru budou mít prodejní týmy víc času na zaměření na Nurturing potenciálních zákazníků a příležitostí, uzavírání obchodů a vytváření trvalých vztahů se zákazníky.

### <a name="next-steps"></a>Další kroky

Pomocí [Průvodce přechodem](../psc-to-pc.md) k partnerským centrům vás seznámíte s postupem migrace vašich obchodů z PSC do partnerského centra.

### <a name="questions"></a>Máte otázky?

Pokud chcete mít další otázky, obraťte se na [podporu](https://partner.microsoft.com/support/?stage=1).

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a>Nové produkty a nabídky společnosti Microsoft Dynamics 365, které jsou k dispozici od 1. dubna 2021

### <a name="categories"></a>Kategorie

- Datum: 2021-03-04
- Možnosti

### <a name="summary"></a>Souhrn

Od 1. dubna 2021 bude Microsoft spouštět několik nových produktů a nabídek pro program poskytovatele Cloud Solution Provider (CSP).

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Všechny partnery, kteří se docházejí prostřednictvím programu Cloud Solution Provider (CSP)

### <a name="details"></a>Podrobnosti

Od 1. dubna 2021 bude Microsoft spouštět následující nové produkty a nabídky:

- Power BI Premium na uživatele
- USL a rozšiřování geografických a segmentů zákazníků

**Power BI Premium na uživatele**

Microsoft bude zavádět první nabídky Power BI Premium pro jednotlivé uživatele. Power BI Premium se aktuálně prodává pouze v konstrukci kapacity. Power BI Premium pro jednotlivé uživatele poskytuje přístup k funkcím Enterprise business intelligence (BI) a Analytics. Flexibilní organizace pro licencování jednotlivých stanic na malé a střední firmy.

Další informace o této nabídce najdete v [podrobnostech o verzi Power BI](/power-platform-release-plan/2020wave2/power-bi/planned-features) .


**Podrobnosti nabídky**

Všimněte si, že název nabídky se mírně liší od ceníku ve verzi Preview.

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

Další informace o těchto nabídkách najdete na následujících stránkách:

- [Domovská stránka hlasu pro zákaznickou službu Dynamics 365](https://dynamics.microsoft.com/customer-voice/overview/)
- [Domovská stránka marketingu Dynamics 365](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a>Další kroky

Projděte si materiály k tomuto tématu a sdílejte tyto informace s příslušnými zúčastněnými stranami ve vaší organizaci.  

### <a name="questions"></a>Máte otázky?

Jakékoli otázky týkající se těchto nabídek najdete v příslušných komunitách Yammeru. 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> Univerzální tisk společnosti Microsoft je nyní k dispozici v některých sadách.

### <a name="categories"></a>Kategorie

- Datum: 2021-03-33
- Možnosti

### <a name="summary"></a>Souhrn

Univerzální tisk společnosti Microsoft bude k dispozici pro transakce v rámci vybraných Microsoft 365ch sad a jako samostatný doplněk od 1. března 2021.

### <a name="impacted-audience"></a>Ovlivněná cílová skupina

Všechny partnery, kteří se docházejí prostřednictvím programu Cloud Solution Provider (CSP)

### <a name="details"></a>Podrobnosti

[Univerzální tisk](https://aka.ms/universalprint) je Microsoft 365 tisková služba, která odstraňuje potřebu místních tiskových serverů a umožňuje zařízením s Windows tisk na tiskárnách registrovaných v Azure. Bude k dispozici pro Transact od 1. března 2021.

Pracovní procesy využívají tisk bez ovladačů, zjednodušené zjišťování tiskáren založené na poloze a intuitivní možnosti tisku bez výukové křivky. Zařízení, která jsou připojená k Azure Active Directory (Azure AD), používají k bezpečnému tisku existující přihlašovací údaje Azure AD. Správci spravují tisk pomocí Azure Portal a můžou snadno připojit tiskárny s nativní podporou univerzálního tisku. Univerzální tisk se dá nasadit s nekompatibilními tiskárnami pomocí softwaru univerzálního tiskového konektoru.

Univerzální tisk bude při spuštění vyplněn ve Windows E3, a3, E5 a A5 a Microsoft 365 BP, F3, E3, a3, E5 a a5.  

**Podrobnosti nabídky**

Všimněte si, že název nabídky se mírně liší od ceníku ve verzi Preview.

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
