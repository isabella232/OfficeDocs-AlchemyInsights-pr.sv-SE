---
title: Skapa en SharePoint-webbplats
ms.author: pebaum
author: todmccoy
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: e1e71ae9401448ed18058f6307302dcbaf773649
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770873"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="a6aa4-102">Skapa en SharePoint-webbplats</span><span class="sxs-lookup"><span data-stu-id="a6aa4-102">Create a SharePoint site</span></span>

<span data-ttu-id="a6aa4-103">Skapa eller hantera webbplatser från [aktiva webbplatser](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) i SharePoint-administrationscenter.</span><span class="sxs-lookup"><span data-stu-id="a6aa4-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="a6aa4-104">Mer information finns i [Hantera webbplatser i det nya Administrationscentret](https://docs.microsoft.com/sharepoint/manage-site-creation)för SharePoint .</span><span class="sxs-lookup"><span data-stu-id="a6aa4-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="a6aa4-105">Tips:</span><span class="sxs-lookup"><span data-stu-id="a6aa4-105">Tips:</span></span>

- <span data-ttu-id="a6aa4-106">Du **kan inte** skapa en webbplats med samma URL för en befintlig webbplats.</span><span class="sxs-lookup"><span data-stu-id="a6aa4-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="a6aa4-107">Om du har tagit bort en webbplats och vill använda URL:en igen, är det möjligt att den borttagna webbplatsen fortfarande finns under [Borttagna webbplatser](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="a6aa4-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="a6aa4-108">Webbplatsen måste tas bort permanent för att återanvända URL:en.</span><span class="sxs-lookup"><span data-stu-id="a6aa4-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="a6aa4-109">Information om hur du tar bort en webbplats med Powershell finns i exempel på [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet.</span><span class="sxs-lookup"><span data-stu-id="a6aa4-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="a6aa4-110">Vissa användare kanske inte kan skapa en webbplats.</span><span class="sxs-lookup"><span data-stu-id="a6aa4-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="a6aa4-111">[Mer information finns i Hantera webbplatsskapande i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="a6aa4-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="a6aa4-112">Det är möjligt att webbplatsen verkar fast på **att skapa** längre än väntat.</span><span class="sxs-lookup"><span data-stu-id="a6aa4-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="a6aa4-113">Om mer än 24 timmar har gått sedan du först såg detta problem, vänligen logga en supportbiljett.</span><span class="sxs-lookup"><span data-stu-id="a6aa4-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="a6aa4-114">I många fall arbetar vi redan på en lösning.</span><span class="sxs-lookup"><span data-stu-id="a6aa4-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="a6aa4-115">Vänligen ge oss minst 24 timmar att slutföra en lösning.</span><span class="sxs-lookup"><span data-stu-id="a6aa4-115">Please give us at least 24 hours to complete a solution.</span></span>
