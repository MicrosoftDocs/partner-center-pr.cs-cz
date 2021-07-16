---
title: Požadavky pro programové získání přístupu k analytickým datům
description: Požadavky pro programové získání přístupu k analytickým datům
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d4c39025aa3804435dd4d2359b93cd4a2e13ccc4
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: cs-CZ
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376385"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a>Požadavky pro programové získání přístupu k analytickým datům

**Příslušné role:** Globální správce | Správce MPN

Předtím, než budete moci programově získat přístup k datům o partner Insights Analytics, je nutné splnit následující požadavky.

## <a name="mpn-program-enrollment"></a>Registrace programu MPN

Chcete-li získat přístup k datům služby partner Insights Analytics programově, je nutné se zaregistrovat v programu MPN a mít účet partnerského centra. Další informace o postupu najdete [v tématu Vytvoření účtu MPN v partnerském centru](mpn-create-a-partner-center-account.md) .

## <a name="create-azure-active-directory-aad-application"></a>vytvořit aplikaci Azure Active Directory (AAD)

přihlašovací údaje pro běžné uživatele nelze použít pro programový přístup k datům partnerů Přehledy Analytics. pro přístup k rozhraním api pro přístup k programování se musí vytvořit aplikace Azure Active Directory (AAD) společně s tajným klíčem (přístup uživatelů a aplikací). Informace o tom, jak vytvořit aplikaci AAD a tajný klíč, najdete v tématu [rychlý Start: registrace aplikace pomocí Microsoft Identity Platform.](/azure/active-directory/develop/quickstart-register-app)   Pro přístup k rozhraní Microsoft Partner API se vyžaduje oprávnění. Další informace o tom, jak přidat oprávnění, najdete v tématu [ověřování rozhraní API pro partnery – partner](/partner/develop/api-authentication#application-and-user-access)

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a>Přiřazení role ERV (Executive Report Viewer) uživateli

Chcete-li získat přístup k datům pro analýzu partnerského Insights prostřednictvím kódu programu, měli byste mít manažera sestavy (ERV). informace o tom, jak přiřadit roli ERV uživateli, najdete v tématu [partnerským centrem Přehledy přístupu na základě role – partnerské centrum](insights-roles.md) .

## <a name="generate-an-aad-token"></a>Vygenerovat token AAD

Je potřeba vygenerovat token AAD pomocí ID aplikace (klienta), tajného klíče klienta, vašeho uživatelského ID a hesla.   [Tady najdete](insights-programmatic-first-api-call.md#token-generation) postup pro vygenerování tokenu AAD.

> [!Note]
> Token je platný po dobu jedné hodiny.

## <a name="next-steps"></a>Další kroky
[Programové přístupové paradigma](insights-programmatic-access-paradigm.md)