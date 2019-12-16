---
title: Skrivskyddad för underhåll meddelande när du försöker använda SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051299"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="06738-102">Skrivskyddad för underhåll meddelande när du försöker använda SharePoint eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="06738-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="06738-103">Användare kan få en **skrivskyddad för underhåll** meddelande när du försöker använda SharePoint eller OneDrive för något av följande scenarier.</span><span class="sxs-lookup"><span data-stu-id="06738-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="06738-104">En planerad eller aktiv underhållsaktivitet.</span><span class="sxs-lookup"><span data-stu-id="06738-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="06738-105">Sök efter dem genom att navigera till [meddelandecentret](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="06738-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="06738-106">En hög prioritet, aktiv tjänst incident som kan inträffa.</span><span class="sxs-lookup"><span data-stu-id="06738-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="06738-107">Kontrollera om det finns några bulletiner/incidenter genom att navigera till [tjänstens hälsa](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="06738-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="06738-108">En mindre Auto-Healing återhämtning scenario som kan hända på grund av oväntade händelser på servrarna som kan pågå i mindre än 30 min eller så.</span><span class="sxs-lookup"><span data-stu-id="06738-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="06738-109">Det finns inga meddelanden Center eller Tjänsthälsa inlägg för dessa mindre återvinningar men du bör vara tillbaka till det normala mycket snart.</span><span class="sxs-lookup"><span data-stu-id="06738-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="06738-110">Vid mycket få tillfällen konstaterade vi att en av de tre scenarierna som anges ovan har varit orsaken, och tjänsten har återställts, men användarnas webbläsarens cacheminne inte har klarats upp.</span><span class="sxs-lookup"><span data-stu-id="06738-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="06738-111">Försök att rensa webbläsarens cacheminne innan du navigerar till webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="06738-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="06738-112">Välj **Inställningar**i webbläsaren Microsoft Edge och välj sedan **Sekretess och säkerhet**.</span><span class="sxs-lookup"><span data-stu-id="06738-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="06738-113">Under **Rensa bläddring**väljer du **Välj vad du vill rensa**.</span><span class="sxs-lookup"><span data-stu-id="06738-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="06738-114">Välj **cookies och sparade webbplatsdata**och välj **Rensa**.</span><span class="sxs-lookup"><span data-stu-id="06738-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="06738-115">Dessa steg kan skilja sig åt när du använder andra webbläsare som Mozilla Firefox eller Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="06738-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="06738-116">Ett annat alternativ är att öppna SharePoint-webbplatsen eller OneDrive i ett nytt InPrivate-fönster.</span><span class="sxs-lookup"><span data-stu-id="06738-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>