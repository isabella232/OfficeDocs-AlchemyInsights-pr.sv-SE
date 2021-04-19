---
title: Adressering av Inloggningsfel i Teams AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822005"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="f9b81-102">Adressering av Inloggningsfel i Teams AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="f9b81-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="f9b81-103">När du loggar in i Microsoft Teams kan du få felmeddelandet: Tyvärr, men vi har problem med att logga in dig i **AADSTS9000411: Begäran är inte korrekt formaterad. Parametern "login_hint" dupliceras.**</span><span class="sxs-lookup"><span data-stu-id="f9b81-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="f9b81-104">Åtgärda problemet genom att se till att dina Microsoft Teams-klienter är uppdaterade.</span><span class="sxs-lookup"><span data-stu-id="f9b81-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="f9b81-105">Mer information om hur du uppdaterar din klient finns [i Uppdatera Microsoft Teams.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)</span><span class="sxs-lookup"><span data-stu-id="f9b81-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="f9b81-106">Om du av någon anledning inte kan uppdatera klienten rensas de flesta cachelagrade data när du loggar ut från klienten.</span><span class="sxs-lookup"><span data-stu-id="f9b81-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="f9b81-107">Avsluta Teams om du fortfarande har problem efter inloggning/inloggning och rensa klientcachen genom att göra följande:</span><span class="sxs-lookup"><span data-stu-id="f9b81-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="f9b81-108">Stäng Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f9b81-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="f9b81-109">Gå till: %appdata%\microsoft\teams och ta bort alla filer.</span><span class="sxs-lookup"><span data-stu-id="f9b81-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="f9b81-110">Öppna Microsoft Teams igen.</span><span class="sxs-lookup"><span data-stu-id="f9b81-110">Reopen Microsoft Teams.</span></span>
