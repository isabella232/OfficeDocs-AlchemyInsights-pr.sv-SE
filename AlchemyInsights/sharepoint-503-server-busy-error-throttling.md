---
title: SharePoint Online-begränsning
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: b157ce22962ac1616d6e9b3a5475edaec7fed9f7
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761276"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="47b1c-102">SharePoint Online-begränsning</span><span class="sxs-lookup"><span data-stu-id="47b1c-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="47b1c-103">Användare kan få ett 503-servern är upptagen fel när du försöker gå till SharePoint-eller OneDrive.</span><span class="sxs-lookup"><span data-stu-id="47b1c-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="47b1c-104">Det här felet kan orsakas av begränsning i SharePoint-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="47b1c-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="47b1c-105">SharePoint Online använder begränsning för att bibehålla optimal prestanda och tillförlitlighet i SharePoint Online-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="47b1c-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="47b1c-106">Begränsning begränsningar anrop antal användaråtgärder eller samtidiga (genom skript eller kod) för att förhindra felaktig användning av resurser.</span><span class="sxs-lookup"><span data-stu-id="47b1c-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="47b1c-107">Om du hämta begränsats 99% av tiden är det på grund av anpassad kod.</span><span class="sxs-lookup"><span data-stu-id="47b1c-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="47b1c-108">Mer information om processbegränsning finns [Undvik komma begränsats eller blockeras i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="47b1c-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="47b1c-109">Om du tror att det här felet är beroende av begränsning kan du kontrollera om det finns aktiva Underhåll uppstår på din hyresgäst genom att navigera till [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="47b1c-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="47b1c-110">Slutligen se till att du besöker sidan [Service hälsa](https://portal.office.com/adminportal/home#/servicehealth) för alla rekommendationerna/olyckor som kan ske.</span><span class="sxs-lookup"><span data-stu-id="47b1c-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

