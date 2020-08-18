---
title: Skapa en SharePoint-webbplats
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: ba682f3c2b2600031f6856621691b1e0fba64113
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786583"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="bdb57-102">Skapa en SharePoint-webbplats</span><span class="sxs-lookup"><span data-stu-id="bdb57-102">Create a SharePoint site</span></span>

<span data-ttu-id="bdb57-103">Skapa eller hantera webbplatser från [aktiva webbplatser](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) i administrations centret för SharePoint.</span><span class="sxs-lookup"><span data-stu-id="bdb57-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="bdb57-104">Mer information finns i [Hantera webbplatser i det nya administrations centret för SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="bdb57-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="bdb57-105">Bland</span><span class="sxs-lookup"><span data-stu-id="bdb57-105">Tips:</span></span>

- <span data-ttu-id="bdb57-106">Du **kan inte** skapa en webbplats med samma URL för en befintlig webbplats.</span><span class="sxs-lookup"><span data-stu-id="bdb57-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="bdb57-107">Om du har tagit bort en webbplats och vill återanvända URL-adressen är det möjligt att den borttagna webbplatsen fortfarande finns under [borttagna webbplatser](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="bdb57-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="bdb57-108">Webbplatsen måste tas bort permanent för att du ska kunna använda den igen.</span><span class="sxs-lookup"><span data-stu-id="bdb57-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="bdb57-109">Information om hur du tar bort en webbplats med PowerShell finns i exemplet [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet.</span><span class="sxs-lookup"><span data-stu-id="bdb57-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="bdb57-110">Vissa användare kanske inte kan skapa en webbplats.</span><span class="sxs-lookup"><span data-stu-id="bdb57-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="bdb57-111">[Se Hantera webbplats skapande i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="bdb57-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="bdb57-112">Det är möjligt att webbplatsen ser snygg ut när den **skapas** längre än förväntat.</span><span class="sxs-lookup"><span data-stu-id="bdb57-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="bdb57-113">Om det inte finns mer än 24 timmar sedan du först såg det här problemet, logga in ett support ärende.</span><span class="sxs-lookup"><span data-stu-id="bdb57-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="bdb57-114">I många fall jobbar vi redan med en lösning.</span><span class="sxs-lookup"><span data-stu-id="bdb57-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="bdb57-115">Ange minst 24 timmar för att slutföra en lösning.</span><span class="sxs-lookup"><span data-stu-id="bdb57-115">Please give us at least 24 hours to complete a solution.</span></span>
