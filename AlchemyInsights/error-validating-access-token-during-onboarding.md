---
title: Ett fel uppstod vid validering av åtkomsttokenfel vid skrivbords analys vid ombordstigning
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741286"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="62974-102">"Det uppstod ett fel vid validering av åtkomsttoken" fel vid registrering av skrivbords analys</span><span class="sxs-lookup"><span data-stu-id="62974-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="62974-103">Det här felet observeras normalt när autentiseringstoken upphör att gälla.</span><span class="sxs-lookup"><span data-stu-id="62974-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="62974-104">Vanligtvis uppdatera sidan uppdaterar token.</span><span class="sxs-lookup"><span data-stu-id="62974-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="62974-105">Det här problemet kan dock kvarstå om det finns några principer för villkorlig åtkomst tillämpas på kontot som används för att ombord Desktop Analytics.</span><span class="sxs-lookup"><span data-stu-id="62974-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="62974-106">Du kan granska den Azure AD loggar in loggar i Azure-portalen för att se om det finns några Inloggningsfel för det konto som används för Desktop Analytics onboarding.</span><span class="sxs-lookup"><span data-stu-id="62974-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="62974-107">Mer information om villkorlig åtkomst finns i [Planera distributionen av villkorlig åtkomst](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="62974-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>