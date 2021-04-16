---
title: Ett fel uppstod vid validering av åtkomsttoken under skrivbordsanalys på boarding
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813706"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="5b4c2-102">Felet "Ett fel uppstod vid validering av åtkomsttoken" under registrering av Skrivbordsanalys</span><span class="sxs-lookup"><span data-stu-id="5b4c2-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="5b4c2-103">Det här felet observeras normalt när autentiseringstoken upphör att gälla.</span><span class="sxs-lookup"><span data-stu-id="5b4c2-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="5b4c2-104">Vanligtvis uppdateras token när sidan uppdateras.</span><span class="sxs-lookup"><span data-stu-id="5b4c2-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="5b4c2-105">Men det här problemet kan kvarstå om det finns några villkorsstyrda åtkomstprinciper som tillämpas på det konto som används för skrivbordsanalys.</span><span class="sxs-lookup"><span data-stu-id="5b4c2-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="5b4c2-106">Du kan granska Azure AD-inloggningsloggarna i Azure Portal för att se om det uppstår något inloggningsfel för det konto som används för registrering av Skrivbordsanalys.</span><span class="sxs-lookup"><span data-stu-id="5b4c2-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="5b4c2-107">Mer information om villkorsstyrd åtkomst finns i [Planera villkorsstyrd åtkomstdistribution.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)</span><span class="sxs-lookup"><span data-stu-id="5b4c2-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>