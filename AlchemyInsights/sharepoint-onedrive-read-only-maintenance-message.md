---
title: Skrivskyddad för underhåll meddelande när du försöker använda SharePoint eller OneDrive
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620741"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="4247d-102">Skrivskyddad för underhåll meddelande när du försöker använda SharePoint eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="4247d-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="4247d-103">Användare får ett meddelande **Skrivskyddad för underhåll** vid försök att använda SharePoint- eller OneDrive för något av följande scenarier.</span><span class="sxs-lookup"><span data-stu-id="4247d-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="4247d-104">Planerade eller aktiva underhållsåtgärd.</span><span class="sxs-lookup"><span data-stu-id="4247d-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="4247d-105">Kontrollera dem genom att navigera till [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="4247d-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="4247d-106">En hög prioritet, aktiv tjänst tillbud som kan ske.</span><span class="sxs-lookup"><span data-stu-id="4247d-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="4247d-107">Kontrollera alla rekommendationerna/incidenter genom att navigera till [Tjänsten hälsa](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="4247d-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="4247d-108">En mindre smart automatisk återställningsscenario som kan bero på grund av oväntade händelser på servrar som kan pågå i minst 30 min eller så.</span><span class="sxs-lookup"><span data-stu-id="4247d-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="4247d-109">Det finns inga Message Center eller tjänsten hälsa bokförs för dessa mindre återställningar, men du bör vara tillbaka till normal mycket snart.</span><span class="sxs-lookup"><span data-stu-id="4247d-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="4247d-110">Vid mycket få tillfällen observerade vi att en av tre scenarier som anges ovan har varit orsaken, och tjänsten har återställts, men användare webbläsarens cacheminne har rensats.</span><span class="sxs-lookup"><span data-stu-id="4247d-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="4247d-111">Försök att rensa webbläsarens cacheminne innan navigera till webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="4247d-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="4247d-112">I webbläsaren Microsoft Edge, Välj **Inställningar**och välj **Sekretess och säkerhet**.</span><span class="sxs-lookup"><span data-stu-id="4247d-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="4247d-113">Markera under **Rensa bläddring**, **välja vad du vill ta bort**.</span><span class="sxs-lookup"><span data-stu-id="4247d-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="4247d-114">Välj **Cookies och sparade webbplats data**och välj **Radera**.</span><span class="sxs-lookup"><span data-stu-id="4247d-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="4247d-115">Stegen kan skilja sig när du använder andra webbläsare som Mozilla Firefox eller Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="4247d-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="4247d-116">Ett annat alternativ är att öppna din SharePoint-webbplats eller en OneDrive i ett nytt InPrivate-fönster.</span><span class="sxs-lookup"><span data-stu-id="4247d-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>