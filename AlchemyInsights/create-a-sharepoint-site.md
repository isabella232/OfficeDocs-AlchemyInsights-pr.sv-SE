---
title: Skapa en SharePoint-webbplats
ms.author: efrene
author: efrene
ms.date: 1/16/2019
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
ms.openlocfilehash: 96780bd2f4182c1385406ec2a31cd62745137985
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36515825"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="190af-102">Skapa en SharePoint-webbplats</span><span class="sxs-lookup"><span data-stu-id="190af-102">Create a SharePoint site</span></span>

<span data-ttu-id="190af-103">Du kan se följande information om skapande av SharePoint-webbplats:</span><span class="sxs-lookup"><span data-stu-id="190af-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="190af-104">[Hantera platser i nya SharePoint administratörscenter](https://docs.microsoft.com/sharepoint/manage-site-creation): Lär dig mer om webbplatsen Skapandealternativ, inklusive hur du skapar en klassisk eller en Team-webbplats som inte innehåller en Office 365-grupp.</span><span class="sxs-lookup"><span data-stu-id="190af-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="190af-105">[Skapa en gruppwebbplats i SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Lär dig hur du skapar en gruppwebbplats.</span><span class="sxs-lookup"><span data-stu-id="190af-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="190af-106">[Skapa en webbplats för kommunikation i SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Lär dig hur du skapar en webbplats för kommunikation.</span><span class="sxs-lookup"><span data-stu-id="190af-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="190af-107">[Hantera platser i nya SharePoint administratörscenter](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Lär dig hur du skapar en klassisk eller en gruppwebbplats som inte innehåller en Office 365-grupp.</span><span class="sxs-lookup"><span data-stu-id="190af-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> [! Tips]
> - <span data-ttu-id="190af-109">Du kan inte skapa en webbplats med samma URL-Adressen till en befintlig webbplats.</span><span class="sxs-lookup"><span data-stu-id="190af-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="190af-110">Om du ta bort en webbplats och önskar att återanvända URL kan webbplatsen borttagen kvarstår under **borttagna platser**.</span><span class="sxs-lookup"><span data-stu-id="190af-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="190af-111">Ta bort platser finns i [Ta bort en webbplats](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)att hantera.</span><span class="sxs-lookup"><span data-stu-id="190af-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="190af-112">Om du vill ta bort en webbplats med Powershell, se [Ta bort SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) -cmdlet exempel.</span><span class="sxs-lookup"><span data-stu-id="190af-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="190af-113">Vissa användare kanske inte kan skapa en webbplats.</span><span class="sxs-lookup"><span data-stu-id="190af-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="190af-114">Se [Hantera webbplats skapas i SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="190af-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="190af-115">Det är möjligt att webbplatsen visas fast vid **Skapa** längre tid än förväntat.</span><span class="sxs-lookup"><span data-stu-id="190af-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="190af-116">Om mer än 24 timmar har gått sedan du först såg problemet, logga en biljett stöd.</span><span class="sxs-lookup"><span data-stu-id="190af-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="190af-117">I många fall kan arbetar vi redan på en lösning.</span><span class="sxs-lookup"><span data-stu-id="190af-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="190af-118">Ge oss minst 24 timmar att slutföra en lösning.</span><span class="sxs-lookup"><span data-stu-id="190af-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="190af-119">Om du behöver skapa en ny gruppwebbplats som inte innehåller en Office 365-grupp</span><span class="sxs-lookup"><span data-stu-id="190af-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


