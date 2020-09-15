---
title: Skriv skydd för underhålls meddelande när du försöker använda SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670850"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="25d4d-102">Skriv skydd för underhålls meddelande när du försöker använda SharePoint eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="25d4d-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="25d4d-103">Användare kan få ett **skrivskyddat för underhålls** meddelande när de försöker använda SharePoint eller OneDrive för något av följande scenarier.</span><span class="sxs-lookup"><span data-stu-id="25d4d-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="25d4d-104">En planerad eller aktiv underhålls aktivitet.</span><span class="sxs-lookup"><span data-stu-id="25d4d-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="25d4d-105">Leta efter dem genom att gå till [meddelande Center](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="25d4d-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="25d4d-106">Ett högprioriterat, aktivt tjänst problem som kan uppstå.</span><span class="sxs-lookup"><span data-stu-id="25d4d-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="25d4d-107">Sök efter eventuella rådgivare/incidenter genom att gå till [tjänstens hälsa](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="25d4d-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="25d4d-108">Ett mindre automatiskt återställnings scenario som kan förekomma på grund av eventuella oväntade händelser på de servrar som eventuellt har varit mindre än 30 minuter.</span><span class="sxs-lookup"><span data-stu-id="25d4d-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="25d4d-109">Det finns inga poster för meddelande Center eller tjänstens hälsa för dessa mindre återställningar, men du bör vara tillbaka till normalt.</span><span class="sxs-lookup"><span data-stu-id="25d4d-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="25d4d-110">Under de senaste inloggningarna observerade vi att ett av de tre ovanstående scenarierna var orsaken och att tjänsten har återställts men att användarens webbläsare inte har rensats.</span><span class="sxs-lookup"><span data-stu-id="25d4d-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="25d4d-111">Försök rensa webbläsarens cache innan du navigerar till webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="25d4d-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="25d4d-112">I webbläsaren Microsoft Edge väljer du **Inställningar**och sedan **Sekretess och säkerhet**.</span><span class="sxs-lookup"><span data-stu-id="25d4d-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="25d4d-113">Under **Rensa bläddring**väljer **du Välj vad du vill rensa**.</span><span class="sxs-lookup"><span data-stu-id="25d4d-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="25d4d-114">Välj **cookies och sparade webbplats data**och välj **Rensa**.</span><span class="sxs-lookup"><span data-stu-id="25d4d-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="25d4d-115">De här stegen kan skilja sig från andra webbläsare, till exempel Mozilla Firefox och Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="25d4d-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="25d4d-116">Ett annat alternativ är att öppna SharePoint-webbplatsen eller OneDrive i ett nytt InPrivate-fönster.</span><span class="sxs-lookup"><span data-stu-id="25d4d-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>