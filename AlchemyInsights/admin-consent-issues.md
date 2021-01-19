---
title: Problem med administratörs medgivande
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901513"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="5a990-102">Problem med administratörs medgivande</span><span class="sxs-lookup"><span data-stu-id="5a990-102">Admin consent issues</span></span>

1. <span data-ttu-id="5a990-103">Aktivera [arbets flödet för administratörer](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) för att tillåta användare att begära administratörs godkännande direkt från medgivande skärmen.</span><span class="sxs-lookup"><span data-stu-id="5a990-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="5a990-104">Om du eller dina programs användare ser oväntade fel under medgivande processen läser du den här artikeln för fel söknings steg: [oväntat fel vid medgivande till ett program](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="5a990-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="5a990-105">Läs mer om [Administratörs medgivande på Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), hur [medgivande meddelandet](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) fungerar och hur du [utvärderar en begäran om klient medgivande](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span><span class="sxs-lookup"><span data-stu-id="5a990-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="5a990-106">Program som integreras med Microsoft Identity Platform följer en Authorization-modell som gör att användare och administratörer kan styra hur data nås.</span><span class="sxs-lookup"><span data-stu-id="5a990-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="5a990-107">Implementeringen av auktoriserings modellen har uppdaterats på slut punkten för Microsoft Identity Platform och ändrar hur en app måste samverka med Microsofts identitets plattform.</span><span class="sxs-lookup"><span data-stu-id="5a990-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="5a990-108">Se [behörigheter och medgivande i slut punkten för Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) för en översikt över den här verifierings modellen, inklusive omfattningar, behörigheter och medgivande.</span><span class="sxs-lookup"><span data-stu-id="5a990-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>