---
title: SharePoint Online-begränsning
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 21d0f8d0118d92562b425921742513157563b5fb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773865"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="951af-102">SharePoint Online-begränsning</span><span class="sxs-lookup"><span data-stu-id="951af-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="951af-103">**Viktigt**: under denna extraordinära tid vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänsterna har hög tillgänglighet. Mer information finns i [temporära funktionsjusteringar för SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="951af-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="951af-104">**503-felet är upptaget**</span><span class="sxs-lookup"><span data-stu-id="951af-104">**503 server is busy error**</span></span>

<span data-ttu-id="951af-105">Användare kan få en 503-server att vara upptagen när du försöker navigera till SharePoint-eller OneDrive-webbplatser.</span><span class="sxs-lookup"><span data-stu-id="951af-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="951af-106">Det här felet kan orsakas av begränsning i SharePoint-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="951af-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="951af-107">SharePoint Online använder begränsning för att bibehålla optimala prestanda och tillförlitlighet i SharePoint Online-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="951af-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="951af-108">Begränsningen begränsar antalet användaråtgärder och samtidiga anrop (med skript eller kod) för att förhindra att resurserna utnyttjas för mycket.</span><span class="sxs-lookup"><span data-stu-id="951af-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="951af-109">Mer information om begränsning finns i [undvika begränsning eller blockering i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="951af-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="951af-110">Om du tror att det här felet inte är relaterat till begränsning kan du kontrol lera om det finns ett aktivt underhåll för klient organisationen genom att gå till [meddelande Center](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="951af-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="951af-111">Se till att du går till sidan [tjänstens hälsa](https://portal.office.com/adminportal/home#/servicehealth) för att kontrol lera eventuella rådgivare/tillbud som kan uppstå.</span><span class="sxs-lookup"><span data-stu-id="951af-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

