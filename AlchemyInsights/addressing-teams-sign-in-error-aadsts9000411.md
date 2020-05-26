---
title: Åtgärda inloggningsfel för team AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/20/2020
ms.locfileid: "44358368"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="b0afd-102">Åtgärda inloggningsfel för team AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="b0afd-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="b0afd-103">När du loggar in på Microsoft Teams kan felet visas: **Tyvärr, men vi har problem med att logga in dig i AADSTS9000411: Begäran är inte korrekt formaterad. Parametern "login_hint" dupliceras.**</span><span class="sxs-lookup"><span data-stu-id="b0afd-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="b0afd-104">Om du vill lösa problemet bör du se till att dina Microsoft Teams-klienter är uppdaterade.</span><span class="sxs-lookup"><span data-stu-id="b0afd-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="b0afd-105">Mer information om hur du uppdaterar klienten finns i [Uppdatera Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="b0afd-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="b0afd-106">Om du inte kan uppdatera klienten av någon anledning rensas de flesta cachelagrade data genom att logga ut klienten.</span><span class="sxs-lookup"><span data-stu-id="b0afd-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="b0afd-107">Men om du fortfarande har problem efter utloggning/inloggning avslutar du Teams och rensar klientcachen genom att göra följande:</span><span class="sxs-lookup"><span data-stu-id="b0afd-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="b0afd-108">Stäng Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="b0afd-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="b0afd-109">Gå till: %appdata%\microsoft\teams och ta bort alla filer.</span><span class="sxs-lookup"><span data-stu-id="b0afd-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="b0afd-110">Öppna Microsoft Teams igen.</span><span class="sxs-lookup"><span data-stu-id="b0afd-110">Reopen Microsoft Teams.</span></span>
