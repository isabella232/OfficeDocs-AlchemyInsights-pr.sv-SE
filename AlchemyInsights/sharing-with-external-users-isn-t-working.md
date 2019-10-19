---
title: Delning med externa användare fungerar inte
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36502249"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="628aa-102">Åtgärda problem med att dela SharePoint-innehåll med externa användare</span><span class="sxs-lookup"><span data-stu-id="628aa-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="628aa-103">Kontrollera att extern delning är aktiverat för din organisation:</span><span class="sxs-lookup"><span data-stu-id="628aa-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="628aa-104">Gå till [sidan tjänster &amp; -tillägg i Microsoft 365 administratörscenter](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)och klicka på **platser**.</span><span class="sxs-lookup"><span data-stu-id="628aa-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="628aa-105">Kontrollera att inställningen är på.</span><span class="sxs-lookup"><span data-stu-id="628aa-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="628aa-106">Om "endast befintliga externa användare" är markerad, kontrollera att den externa användaren finns med i Microsoft 365 administratörscenter.</span><span class="sxs-lookup"><span data-stu-id="628aa-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="628aa-107">Kontrollera att extern delning är aktiverad för webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="628aa-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="628aa-108">För en klassisk webbplatssamling:</span><span class="sxs-lookup"><span data-stu-id="628aa-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="628aa-109">Klicka på **platser**i det vänstra fönstret i det nya administrationscentret för SharePoint.</span><span class="sxs-lookup"><span data-stu-id="628aa-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="628aa-110">Markera webbplatsen eller platserna och klicka på **delning**i menyfliksområdet.</span><span class="sxs-lookup"><span data-stu-id="628aa-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="628aa-111">För en gruppwebbplats som tillhör en Office 365-grupp eller en kommunikations plats:</span><span class="sxs-lookup"><span data-stu-id="628aa-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="628aa-112">De här nya webbplats typerna har samma delningsinställning som din organisationsomfattande inställning, såvida inte inställningen för hela organisationen tillåter delning av filer med länkar som inte kräver inloggning.</span><span class="sxs-lookup"><span data-stu-id="628aa-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="628aa-113">I det här fallet tillåter webbplatserna delning med nya och befintliga externa användare som loggar in.</span><span class="sxs-lookup"><span data-stu-id="628aa-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="628aa-114">Om du vill ändra inställningen för specifika webbplatser använder du det nya SharePoint Admin Center eller PowerShell.</span><span class="sxs-lookup"><span data-stu-id="628aa-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="628aa-115">[Läs mer](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="628aa-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="628aa-116">Den externa delningsinställningen för en webbplats kan vara mer restriktiv än inställningen för hela organisationen, men inte mer tillåtande än inställningen för hela organisationen.</span><span class="sxs-lookup"><span data-stu-id="628aa-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

