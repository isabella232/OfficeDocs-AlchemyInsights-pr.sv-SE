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
ms.openlocfilehash: c7881c0c7331e0aa74fcc439f52157bb75a56160
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559859"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="0e5ba-102">SharePoint Online-begränsning</span><span class="sxs-lookup"><span data-stu-id="0e5ba-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="0e5ba-103">Användare kan få ett 503-servern är upptagen fel när du försöker gå till SharePoint-eller OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0e5ba-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="0e5ba-104">Det här felet kan orsakas av begränsning i SharePoint-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="0e5ba-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="0e5ba-105">SharePoint Online använder begränsning för att bibehålla optimal prestanda och tillförlitlighet i SharePoint Online-tjänsten.</span><span class="sxs-lookup"><span data-stu-id="0e5ba-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="0e5ba-106">Begränsning begränsningar anrop antal användaråtgärder eller samtidiga (genom skript eller kod) för att förhindra felaktig användning av resurser.</span><span class="sxs-lookup"><span data-stu-id="0e5ba-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="0e5ba-107">Om du hämta begränsats 99% av tiden är det på grund av anpassad kod.</span><span class="sxs-lookup"><span data-stu-id="0e5ba-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="0e5ba-108">Mer information om processbegränsning finns [Undvik komma begränsats eller blockeras i SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="0e5ba-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="0e5ba-109">Om du tror att det här felet är beroende av begränsning kan du kontrollera om det finns aktiva Underhåll uppstår på din hyresgäst genom att navigera till [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="0e5ba-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="0e5ba-110">Slutligen se till att du besöker sidan [Service hälsa](https://portal.office.com/adminportal/home#/servicehealth) för alla rekommendationerna/olyckor som kan ske.</span><span class="sxs-lookup"><span data-stu-id="0e5ba-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

