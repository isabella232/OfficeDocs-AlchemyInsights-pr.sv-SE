---
title: Delning med externa användare fungerar inte
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691593"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="9e92b-102">Åtgärda problem med att dela SharePoint-innehåll med externa användare</span><span class="sxs-lookup"><span data-stu-id="9e92b-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="9e92b-103">Kontrol lera att extern delning är aktiverat för organisationen:</span><span class="sxs-lookup"><span data-stu-id="9e92b-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="9e92b-104">Gå till [sidan tjänster &amp; -tillägg i administrations centret för Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)och klicka på **webbplatser**.</span><span class="sxs-lookup"><span data-stu-id="9e92b-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="9e92b-105">Kontrol lera att inställningen är på.</span><span class="sxs-lookup"><span data-stu-id="9e92b-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="9e92b-106">Om "endast befintliga externa användare" är markerat kontrollerar du att den externa användaren finns med i Microsoft 365 Admin Center.</span><span class="sxs-lookup"><span data-stu-id="9e92b-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="9e92b-107">Kontrol lera att extern delning är aktiverat för webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="9e92b-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="9e92b-108">För en klassisk webbplats samling:</span><span class="sxs-lookup"><span data-stu-id="9e92b-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="9e92b-109">Klicka på **webbplatser**i det nya administrations centret för SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9e92b-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="9e92b-110">Välj webbplatsen eller platserna och klicka på **delning**i menyfliksområdet.</span><span class="sxs-lookup"><span data-stu-id="9e92b-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="9e92b-111">För en grupp webbplats som tillhör en Microsoft 365-grupp eller en kommunikations webbplats:</span><span class="sxs-lookup"><span data-stu-id="9e92b-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="9e92b-112">Dessa nya webbplats typer har samma delnings inställningar som inställning för hela organisationen, såvida inte inställningen för hela organisationen tillåter att filer delas med länkar som inte kräver inloggning.</span><span class="sxs-lookup"><span data-stu-id="9e92b-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="9e92b-113">I det här fallet kan webbplatserna dela med nya och befintliga externa användare som loggar in.</span><span class="sxs-lookup"><span data-stu-id="9e92b-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="9e92b-114">Om du vill ändra inställningen för vissa webbplatser kan du använda det nya administrations centret för SharePoint eller PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9e92b-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="9e92b-115">[Mer information](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="9e92b-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="9e92b-116">Inställningen för extern delning för en webbplats kan vara mer restriktiv än inställningen för hela organisationen, men inte fler tillåtna än inställningen för hela organisationen.</span><span class="sxs-lookup"><span data-stu-id="9e92b-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

