---
title: Dela med externa användare fungerar inte
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36502249"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="38c88-102">Åtgärda problem med SharePoint-innehåll med externa användare</span><span class="sxs-lookup"><span data-stu-id="38c88-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="38c88-103">Kontrollera extern delning har aktiverats för organisationen:</span><span class="sxs-lookup"><span data-stu-id="38c88-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="38c88-104">Gå till den [tjänster &amp; tillägg sidan i Microsoft 365 administratörscenter](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), och på **platser**.</span><span class="sxs-lookup"><span data-stu-id="38c88-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="38c88-105">Kontrollera att inställningen är ”on”.</span><span class="sxs-lookup"><span data-stu-id="38c88-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="38c88-106">Om ”endast befintliga externa användare” är markerad, kontrollera att den externa användaren finns med i Microsoft 365 administratörscenter.</span><span class="sxs-lookup"><span data-stu-id="38c88-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="38c88-107">Kontrollera att externa dela den aktiverad för webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="38c88-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="38c88-108">För en klassisk webbplatssamling:</span><span class="sxs-lookup"><span data-stu-id="38c88-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="38c88-109">Klicka på **webbplatser**i nya SharePoint administratörscenter, i den vänstra rutan.</span><span class="sxs-lookup"><span data-stu-id="38c88-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="38c88-110">Markera den eller de platser och klicka på **Dela**på menyfliken.</span><span class="sxs-lookup"><span data-stu-id="38c88-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="38c88-111">För en gruppwebbplats som hör till en grupp i Office 365, eller en webbplats för kommunikation:</span><span class="sxs-lookup"><span data-stu-id="38c88-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="38c88-112">Dessa nya typer av webbplatsen har samma delning inställning som inställning för hela organisationen om inställningen hela organisationen kan dela filer med hjälp av länkar som inte kräver inloggning.</span><span class="sxs-lookup"><span data-stu-id="38c88-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="38c88-113">I det här fallet att webbplatser delar med nya och befintliga externa användare som loggar in.</span><span class="sxs-lookup"><span data-stu-id="38c88-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="38c88-114">Använd nya SharePoint administratörscenter eller PowerShell om du vill ändra inställningen för specifika platser.</span><span class="sxs-lookup"><span data-stu-id="38c88-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="38c88-115">[Läs mer](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="38c88-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="38c88-116">Inställningen för extern delning för en webbplats kan vara mer restriktiva än inställningarna hela organisationen, men inte mer tillåtna än inställningen för hela organisationen.</span><span class="sxs-lookup"><span data-stu-id="38c88-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

