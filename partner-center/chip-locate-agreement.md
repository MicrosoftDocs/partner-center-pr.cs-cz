---
title: Najít počet klientů a úroveň poplatků
ms.topic: how-to
ms.date: 02/18/2021
description: Naučte se používat platformu pro motivaci kanálů (čip) k vyhledání informací o počtu klientů a úrovních poplatků za smlouvu.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 64dbbbae0087275fa8d0c5fd4f364079623efe63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148988"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>Vyhledání počtu klientů a úrovně poplatků pro smlouvu

**Příslušné role**: primární kontakt nebo správce programu

Můžete se přihlásit k [Explore.MS](https://www.explore.ms/) a zkontrolovat smlouvu nebo stáhnout soubor s podrobnostmi o smlouvě pro počet klientů a úroveň poplatku.

## <a name="to-locate-the-information"></a>Vyhledání informací

### <a name="method-1--explorems"></a>Metoda 1 – Explore.ms

1. Otevřete [Explore.MS](https://www.explore.ms/) v Internet Exploreru. 

>[!Note]
>Tuto funkci nelze provést v Google Chrome nebo Microsoft Edge.

2. Přihlaste se pomocí svého pracovního nebo školního účtu nebo Live ID.  

3. V poli **sestavy** vyberte možnost **smlouvy**.

4. Na výsledné stránce zadejte číslo smlouvy do **vyhledávacího** pole a pak vyberte **sloupce vybrat/objednat**.

5. V automaticky otevíraném okně vyberte v seznamu Dostupné sloupce možnost **Smlouva o počtu klientů** a pak vyberte šipku vpravo a přidejte sloupec. Vyberte **OK**.

6. Vyberte **Hledat.**

7. Na výsledné obrazovce posuňte výsledky a vyhledejte sloupec **počet klientů smlouvy** . 

8. Pomocí počtu klientů určete úroveň poplatku podle níže uvedené tabulky sazeb.  

| Úroveň poplatku | Počet klientů |
| ------ | :-----------: |
|  A | 0 – 2 399    |
|  B | 2 400 – 5 999    |
|  C | 6 000 – 14 999    |
|  D | 15 000 +   |

>[!NOTE]
>Úrovně podnikového pobídky vycházejí z počtu počítačů nebo uživatelů (podle toho, co je vyšší) v rámci registrace komerčního a veřejného sektoru (PS). V případě registrací, které nemají přiřazenou fyzickou plochu nebo počet uživatelů, používá společnost Microsoft počet klientů na základě počtu klientů nebo počtu uživatelů v doprovodném programu EA. <br><br>Pokud neexistuje žádný doprovodný EA, úroveň poplatku vychází z cenové úrovně registrace. Cenová úroveň obchodu se dá zobrazit také na [www.Explore.MS](https://www.explore.ms/). <br><br>Pokud existuje více fondů a/nebo cenových úrovní na stávajícím EA/EAS, Microsoft bude platit pobídky na nejvyšší přiřazené úrovni cen/fondu, přičemž úroveň A má nejvyšší úroveň a úroveň D.

#### <a name="pool-and-pricing-levels"></a>Fond a cenové úrovně

Po vyhledání čísla smlouvy v explore.ms pomocí výše uvedeného postupu vyberte číslo smlouvy. Tím přejdete na stránku s podrobnostmi o smlouvě, na které se zobrazí souhrn a **nabídky** **smluv** . Část nabídky obsahuje cenové úrovně.

## <a name="method-2---chip"></a>Metoda 2 – čip

1. Přihlaste se ke čipu a vyberte LSP pobídek.

2. Na stránce **Souhrn platby partnera** vyberte měsíc vykazování, který chcete zobrazit, a potom v rozevíracím seznamu **exportovat do aplikace Excel** vyberte možnost **Podrobnosti o výpočtech** :

:::image type="content" source="images/chip/chiplocate.png" alt-text="Vyhledat podrobnosti o programu":::

3. Export se spustí a můžete ho buď otevřít, nebo Uložit nebo Uložit jako do cílového umístění.

4. Když je sestava otevřená, přejděte vlevo dolů na kartu **DetailReport-Flatfile** :

:::image type="content" source="images/chip/flatfile.png" alt-text="Stažení plochého souboru":::

Nyní můžete vyhledat číslo smlouvy, které hledáte ve sloupci J. a získáte přiřazený počet klientů ve sloupci R, označený Agreement_DesktopCount. Úroveň poplatku pro tuto smlouvu můžete také potvrdit ve sloupci AI s popiskem úrovně.

## <a name="next-steps"></a>Další kroky

- [Řešení problémů s přístupem k čipu](chip-access-trouble.md)
