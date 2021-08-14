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
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932115"
---
# <a name="api-permissions-and-consent"></a>API-behörigheter och medgivande

Program som integreras med Microsofts identitetsplattform följer en auktoriseringsmodell som ger användare och administratörer kontroll över hur data kan nås. Implementeringen av auktoriseringsmodellen har uppdaterats på Microsofts identitetsplattform slutpunkt. Det ändrar hur en app måste interagera med Microsofts identitetsplattform. [Behörigheter och medgivande i Microsofts identitetsplattform omfattar](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) de grundläggande begreppen i den här auktoriseringsmodellen, inklusive omfattningar, behörigheter och medgivande.

Med [Azure Active Directory (Azure AD) medgivanderam](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) gör det enkelt att utveckla webbprogram med flera klientgrupper och inbyggda klientprogram. Med de här programmen kan du logga in med användarkonton från en Azure AD-klientorganisation som skiljer sig från den där programmet är registrerat. De kan också behöva åtkomst till webb-API:er som Microsoft Graph API (för åtkomst till Azure AD, Intune och tjänster i Microsoft 365) och andra MICROSOFT-TJÄNSTER-API:er, utöver dina egna webb-API:er.

