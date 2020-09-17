---
title: Det gick inte att verifiera åtkomst-Tokenbegäran under den station ära dator analysen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783569"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="ccafd-102">Felet "ett fel uppstod vid verifiering av åtkomst-token" under en dator analys</span><span class="sxs-lookup"><span data-stu-id="ccafd-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="ccafd-103">Det här felet uppstår normalt när autentiseringstoken upphör att gälla.</span><span class="sxs-lookup"><span data-stu-id="ccafd-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="ccafd-104">Om du uppdaterar sidan uppdateras emellertid token.</span><span class="sxs-lookup"><span data-stu-id="ccafd-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="ccafd-105">Det här problemet kan dock kvarstå om principer för villkorsstyrd åtkomst används för kontot som används för Station ära datorer.</span><span class="sxs-lookup"><span data-stu-id="ccafd-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="ccafd-106">Du kan granska Azure AD-inloggnings loggarna i Azure-portalen för att se om det finns inloggnings problem för det konto som används för automatisk dator analys.</span><span class="sxs-lookup"><span data-stu-id="ccafd-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="ccafd-107">Om du vill ha mer information om villkorlig åtkomst kan du gå till [Planera distribution av villkorlig åtkomst](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="ccafd-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>