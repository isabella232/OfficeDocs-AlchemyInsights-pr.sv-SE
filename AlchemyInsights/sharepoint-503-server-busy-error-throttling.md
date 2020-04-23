---
title: Begränsning av SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 50b2c29db1fd294abe6c9e60f067156109de392b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742227"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="c695b-102">Begränsning av SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="c695b-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="c695b-103">**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="c695b-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="c695b-104">**503-servern är upptagen fel**</span><span class="sxs-lookup"><span data-stu-id="c695b-104">**503 server is busy error**</span></span>

<span data-ttu-id="c695b-105">Användare kan få ett 503-server är upptaget när de försöker navigera till SharePoint- eller OneDrive-webbplatser.</span><span class="sxs-lookup"><span data-stu-id="c695b-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="c695b-106">Det här felet kan orsakas av begränsning i SharePoint-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="c695b-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="c695b-107">SharePoint Online använder begränsning för att bibehålla optimala prestanda och tillförlitlighet i SharePoint Online-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="c695b-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="c695b-108">Begränsningen begränsar antalet användaråtgärder och samtidiga anrop (med skript eller kod) för att förhindra att resurserna utnyttjas för mycket.</span><span class="sxs-lookup"><span data-stu-id="c695b-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="c695b-109">Mer information om begränsning finns i [Undvik att bli begränsad eller blockerad i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="c695b-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="c695b-110">Om du tror att det här felet inte har något samband med begränsningen kan du kontrollera om det finns aktivt underhåll på din klient genom att navigera till [meddelandecentret](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="c695b-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="c695b-111">Se slutligen till att du besöker sidan [Service Health](https://portal.office.com/adminportal/home#/servicehealth) för att kontrollera eventuella råd/incidenter som kan inträffa.</span><span class="sxs-lookup"><span data-stu-id="c695b-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

