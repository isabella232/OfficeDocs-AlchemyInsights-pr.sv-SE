---
title: API-behörigheter och medgivande
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974995"
---
# <a name="api-permissions-and-consent"></a>API-behörigheter och medgivande

Program som integreras med Microsoft Identity Platform följer en Authorization-modell som gör att användare och administratörer kan styra hur data nås. Implementeringen av auktoriserings modellen har uppdaterats på slut punkten för Microsoft Identity Platform. Det ändrar hur en app måste interagera med Microsofts identitets plattform. [Behörigheter och medgivande i Microsoft Identity Platform-slutpunkten](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) täcker de grundläggande begreppen i den här verifierings modellen, inklusive omfattningar, behörigheter och medgivande.

Med [godkännande ramverket för Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) blir det enkelt att utveckla klient program för flera innehavare. Dessa program tillåter inloggning av användar konton från en Azure AD-klient organisation som skiljer sig från den där programmet är registrerat. De kan även behöva komma åt webb-API: er, till exempel Microsoft Graph API (för åtkomst till Azure AD, Intune och tjänster i Microsoft 365) och andra Microsoft-tjänsters API: er, utöver dina egna API: er för Internet.

