---
title: Skapa en SharePoint-webbplats
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806957"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="ac25c-102">Skapa en SharePoint-webbplats</span><span class="sxs-lookup"><span data-stu-id="ac25c-102">Create a SharePoint site</span></span>

<span data-ttu-id="ac25c-103">Skapa eller hantera webbplatser från [aktiva webbplatser](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) i administrations centret för SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ac25c-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="ac25c-104">Mer information finns i [Hantera webbplatser i det nya administrations centret för SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="ac25c-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="ac25c-105">Bland</span><span class="sxs-lookup"><span data-stu-id="ac25c-105">Tips:</span></span>

- <span data-ttu-id="ac25c-106">Du **kan inte** skapa en webbplats med samma URL för en befintlig webbplats.</span><span class="sxs-lookup"><span data-stu-id="ac25c-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="ac25c-107">Om du har tagit bort en webbplats och vill återanvända URL-adressen är det möjligt att den borttagna webbplatsen fortfarande finns under [borttagna webbplatser](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="ac25c-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="ac25c-108">Webbplatsen måste tas bort permanent för att du ska kunna använda den igen.</span><span class="sxs-lookup"><span data-stu-id="ac25c-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="ac25c-109">Information om hur du tar bort en webbplats med PowerShell finns i exemplet [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet.</span><span class="sxs-lookup"><span data-stu-id="ac25c-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="ac25c-110">Vissa användare kanske inte kan skapa en webbplats.</span><span class="sxs-lookup"><span data-stu-id="ac25c-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="ac25c-111">[Se Hantera webbplats skapande i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="ac25c-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="ac25c-112">Det är möjligt att webbplatsen ser snygg ut när den **skapas** längre än förväntat.</span><span class="sxs-lookup"><span data-stu-id="ac25c-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="ac25c-113">Om det inte finns mer än 24 timmar sedan du först såg det här problemet, logga in ett support ärende.</span><span class="sxs-lookup"><span data-stu-id="ac25c-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="ac25c-114">I många fall jobbar vi redan med en lösning.</span><span class="sxs-lookup"><span data-stu-id="ac25c-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="ac25c-115">Ange minst 24 timmar för att slutföra en lösning.</span><span class="sxs-lookup"><span data-stu-id="ac25c-115">Please give us at least 24 hours to complete a solution.</span></span>
