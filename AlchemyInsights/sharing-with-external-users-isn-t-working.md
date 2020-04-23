---
title: Delning med externa användare fungerar inte
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 285535d6144825f0935bf72579a483260c2f2bd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767267"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="765ff-102">Åtgärda problem med att dela SharePoint-innehåll med externa användare</span><span class="sxs-lookup"><span data-stu-id="765ff-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="765ff-103">Kontrollera att extern delning är aktiverat för din organisation:</span><span class="sxs-lookup"><span data-stu-id="765ff-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="765ff-104">Gå till [ &amp; sidan Tjänster-tillägg i administrationscentret för Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)och klicka på **Webbplatser**.</span><span class="sxs-lookup"><span data-stu-id="765ff-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="765ff-105">Kontrollera att inställningen är aktiverad.</span><span class="sxs-lookup"><span data-stu-id="765ff-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="765ff-106">Om "Endast befintliga externa användare" är markerat kontrollerar du att den externa användaren finns med i Microsoft 365-administrationscentret.</span><span class="sxs-lookup"><span data-stu-id="765ff-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="765ff-107">Kontrollera att extern delning är aktiverat för webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="765ff-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="765ff-108">För en klassisk webbplatssamling:</span><span class="sxs-lookup"><span data-stu-id="765ff-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="765ff-109">Klicka på **webbplatser**i det nya administrationscentret för SharePoint i det nya administrationscentret för SharePoint.</span><span class="sxs-lookup"><span data-stu-id="765ff-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="765ff-110">Markera webbplatsen eller webbplatserna och klicka på **Dela**i menyfliksområdet .</span><span class="sxs-lookup"><span data-stu-id="765ff-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="765ff-111">För en gruppwebbplats som tillhör en Office 365-grupp eller en kommunikationswebbplats:</span><span class="sxs-lookup"><span data-stu-id="765ff-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="765ff-112">Dessa nya webbplatstyper har samma delningsinställning som din organisationsomfattande inställning, såvida inte inställningen för hela organisationen tillåter delning av filer med hjälp av länkar som inte kräver inloggning.</span><span class="sxs-lookup"><span data-stu-id="765ff-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="765ff-113">I det här fallet tillåter webbplatserna delning med nya och befintliga externa användare som loggar in.</span><span class="sxs-lookup"><span data-stu-id="765ff-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="765ff-114">Om du vill ändra inställningen för specifika webbplatser använder du det nya Administrationscentret för SharePoint eller PowerShell.</span><span class="sxs-lookup"><span data-stu-id="765ff-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="765ff-115">[Mer information](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="765ff-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="765ff-116">Inställningen för extern delning för en webbplats kan vara mer restriktiv än din organisationsomfattande inställning, men inte mer tillåtande än den organisationsomfattande inställningen.</span><span class="sxs-lookup"><span data-stu-id="765ff-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

