---
title: Kalenderhändelser saknas eller uppdateras inte
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10932"
- "9001435"
ms.openlocfilehash: b114411d6285a68a41bbcbf64151c212ee2cf661
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51837589"
---
# <a name="calendar-events-missing-or-not-updating"></a><span data-ttu-id="9e570-102">Kalenderhändelser saknas eller uppdateras inte</span><span class="sxs-lookup"><span data-stu-id="9e570-102">Calendar Events missing or not updating</span></span>

<span data-ttu-id="9e570-103">Om kalenderobjekt saknas eller inte uppdateras börjar du med att titta på antalet objekt i kalendermappens egenskaper i Outlook:</span><span class="sxs-lookup"><span data-stu-id="9e570-103">If calendar items are missing or not updating, start by looking at the item count in your Calendar folder properties in Outlook:</span></span> 

1. <span data-ttu-id="9e570-104">Högerklicka på den aktuella **användarens kalendermapp** och välj sedan **Egenskaper**.</span><span class="sxs-lookup"><span data-stu-id="9e570-104">Right-click on the affected user **Calendar** folder, and then select **Properties**.</span></span>

1. <span data-ttu-id="9e570-105">Välj **fliken Synkronisering.**</span><span class="sxs-lookup"><span data-stu-id="9e570-105">Select the **Synchronization** tab.</span></span>

<span data-ttu-id="9e570-106">Om objektantalet inte är samma mellan servermappen och offlinemappen:</span><span class="sxs-lookup"><span data-stu-id="9e570-106">If the item count is not the same between the Server folder and the Offline Folder:</span></span>

1.  <span data-ttu-id="9e570-107">Markera **mappen** Kalender.</span><span class="sxs-lookup"><span data-stu-id="9e570-107">Highlight the **Calendar** folder.</span></span>

1.  <span data-ttu-id="9e570-108">Gå till fliken / **Skicka/ta** emot och välj sedan **Uppdatera mapp**.</span><span class="sxs-lookup"><span data-stu-id="9e570-108">Go to the **Send**/**Receive** tab, and then select **Update Folder**.</span></span>

<span data-ttu-id="9e570-109">Om kalendern fortfarande inte uppdateras eller om händelser saknas hämtar du verktyget Calendar Checking Tool för Outlook från [Microsoft Download Center.](https://www.microsoft.com/download/details.aspx?id=28786)</span><span class="sxs-lookup"><span data-stu-id="9e570-109">If your calendar is still not updating or events are missing, download the Calendar Checking Tool for Outlook from the [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=28786).</span></span> <span data-ttu-id="9e570-110">Avgör om det finns fler än 5 000 objekt i kalendermappen eftersom det kan orsaka symptom som kalendermöten som inte har uppdaterats eller mötesfel.</span><span class="sxs-lookup"><span data-stu-id="9e570-110">Determine if there are more than 5000 items in the calendar folder as this can cause symptoms such as calendar meetings not updated or meeting errors.</span></span> 

<span data-ttu-id="9e570-111">Mer information finns i Prestandaproblem i Outlook när det finns för många objekt eller mappar i [en cachelagrad .ost- eller .pst-fil.](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders)</span><span class="sxs-lookup"><span data-stu-id="9e570-111">For more information, see [Outlook performance issues when there are too many items or folders in a cached mode .ost or .pst file](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).</span></span>