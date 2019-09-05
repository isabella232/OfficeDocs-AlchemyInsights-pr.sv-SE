---
title: Begränsning av SharePoint Online
ms.author: pebaum
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: d9e1400697b1e6435fea78703d2ecadc6733a57f
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751906"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="a99b0-102">Begränsning av SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="a99b0-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="a99b0-103">Användare kan få en 503 Server är upptagen fel när du försöker navigera till SharePoint eller OneDrive webbplatser.</span><span class="sxs-lookup"><span data-stu-id="a99b0-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="a99b0-104">Det här felet kan orsakas av begränsning i SharePoint-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="a99b0-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="a99b0-105">SharePoint Online använder begränsning för att bibehålla optimala prestanda och tillförlitlighet för SharePoint Online-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="a99b0-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="a99b0-106">Begränsning begränsar antalet användaråtgärder eller samtidiga anrop (med skript eller kod) för att förhindra överanvändning av resurser.</span><span class="sxs-lookup"><span data-stu-id="a99b0-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="a99b0-107">Om du inte blir begränsad, 99% av tiden är det på grund av anpassad kod.</span><span class="sxs-lookup"><span data-stu-id="a99b0-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="a99b0-108">Mer information om begränsning se, [undvika att få begränsas eller blockeras i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="a99b0-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="a99b0-109">Om du tror att det här felet inte är relaterat till begränsning, kan du kontrollera om det finns aktivt underhåll som inträffar på din klient genom att navigera till [meddelandecentret](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="a99b0-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="a99b0-110">Slutligen, se till att du besöker sidan för [tjänstens hälsa](https://portal.office.com/adminportal/home#/servicehealth) för att kontrollera eventuella bulletiner/incidenter som kan inträffa.</span><span class="sxs-lookup"><span data-stu-id="a99b0-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

