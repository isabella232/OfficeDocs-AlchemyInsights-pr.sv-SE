---
title: Skapa en SharePoint-webbplats
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: ac894195d847dfc009bc0b57647e1a474361f1c1
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769609"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="c219f-102">Skapa en SharePoint-webbplats</span><span class="sxs-lookup"><span data-stu-id="c219f-102">Create a SharePoint site</span></span>

<span data-ttu-id="c219f-103">Du kan se följande information om hur du skapar SharePoint-webbplatser:</span><span class="sxs-lookup"><span data-stu-id="c219f-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="c219f-104">[Hantera platser i det nya SharePoint-administratörscenter](https://docs.microsoft.com/sharepoint/manage-site-creation): Lär dig mer om alternativ för att skapa webbplatser, inklusive hur du skapar en klassisk webbplats eller en Teams-webbplats som inte innehåller en Office 365-grupp.</span><span class="sxs-lookup"><span data-stu-id="c219f-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="c219f-105">[Skapa en gruppwebbplats i SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Lär dig hur du skapar en gruppwebbplats.</span><span class="sxs-lookup"><span data-stu-id="c219f-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="c219f-106">[Skapa en kommunikations plats i SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Lär dig hur du skapar en kommunikations plats.</span><span class="sxs-lookup"><span data-stu-id="c219f-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="c219f-107">[Hantera platser i det nya SharePoint-administratörscenter](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Lär dig hur du skapar en klassisk webbplats eller en gruppwebbplats som inte innehåller en Office 365-grupp.</span><span class="sxs-lookup"><span data-stu-id="c219f-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
<span data-ttu-id="c219f-108">**Tips:**</span><span class="sxs-lookup"><span data-stu-id="c219f-108">**Tips:**</span></span>
- <span data-ttu-id="c219f-109">Du kan inte skapa en webbplats med samma URL för en befintlig plats.</span><span class="sxs-lookup"><span data-stu-id="c219f-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="c219f-110">Om du har tagit bort en webbplats och vill återanvända URL-adressen är det möjligt att den borttagna webbplatsen fortfarande finns under **borttagna webbplatser**.</span><span class="sxs-lookup"><span data-stu-id="c219f-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="c219f-111">Om du vill hantera borttagna webbplatser se, [ta bort en webbplats](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="c219f-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="c219f-112">Om du vill ta bort en webbplats med PowerShell helt, se [ta bort SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet exempel.</span><span class="sxs-lookup"><span data-stu-id="c219f-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="c219f-113">Vissa användare kanske inte kan skapa en webbplats.</span><span class="sxs-lookup"><span data-stu-id="c219f-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="c219f-114">Se [Hantera webbplats skapas i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="c219f-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="c219f-115">Det är möjligt att webbplatsen visas fast på **att skapa** längre än förväntat.</span><span class="sxs-lookup"><span data-stu-id="c219f-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="c219f-116">Om mer än 24 timmar har gått sedan du först såg detta problem, vänligen logga ett supportärende.</span><span class="sxs-lookup"><span data-stu-id="c219f-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="c219f-117">I många fall arbetar vi redan på en lösning.</span><span class="sxs-lookup"><span data-stu-id="c219f-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="c219f-118">Vänligen ge oss minst 24 timmar för att slutföra en lösning.</span><span class="sxs-lookup"><span data-stu-id="c219f-118">Please give us at least 24 hours to complete a solution.</span></span>
- <span data-ttu-id="c219f-119">Om du behöver skapa en ny gruppwebbplats som inte innehåller en Office 365-grupp,</span><span class="sxs-lookup"><span data-stu-id="c219f-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


