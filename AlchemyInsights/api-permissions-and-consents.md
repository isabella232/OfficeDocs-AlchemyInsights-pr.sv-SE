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
# <a name="api-permissions-and-consent"></a><span data-ttu-id="ea395-102">API-behörigheter och medgivande</span><span class="sxs-lookup"><span data-stu-id="ea395-102">API permissions and consent</span></span>

<span data-ttu-id="ea395-103">Program som integreras med Microsoft Identity Platform följer en Authorization-modell som gör att användare och administratörer kan styra hur data nås.</span><span class="sxs-lookup"><span data-stu-id="ea395-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="ea395-104">Implementeringen av auktoriserings modellen har uppdaterats på slut punkten för Microsoft Identity Platform.</span><span class="sxs-lookup"><span data-stu-id="ea395-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="ea395-105">Det ändrar hur en app måste interagera med Microsofts identitets plattform.</span><span class="sxs-lookup"><span data-stu-id="ea395-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="ea395-106">[Behörigheter och medgivande i Microsoft Identity Platform-slutpunkten](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) täcker de grundläggande begreppen i den här verifierings modellen, inklusive omfattningar, behörigheter och medgivande.</span><span class="sxs-lookup"><span data-stu-id="ea395-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="ea395-107">Med [godkännande ramverket för Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) blir det enkelt att utveckla klient program för flera innehavare.</span><span class="sxs-lookup"><span data-stu-id="ea395-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="ea395-108">Dessa program tillåter inloggning av användar konton från en Azure AD-klient organisation som skiljer sig från den där programmet är registrerat.</span><span class="sxs-lookup"><span data-stu-id="ea395-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="ea395-109">De kan även behöva komma åt webb-API: er, till exempel Microsoft Graph API (för åtkomst till Azure AD, Intune och tjänster i Microsoft 365) och andra Microsoft-tjänsters API: er, utöver dina egna API: er för Internet.</span><span class="sxs-lookup"><span data-stu-id="ea395-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

