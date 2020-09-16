---
title: Lägga till en grupp på en SharePoint-webbplats
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771226"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="5e6c1-102">Problem med att skapa en gruppansluten webbplats i SharePoint</span><span class="sxs-lookup"><span data-stu-id="5e6c1-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="5e6c1-103">Några vanliga problem inträffade när du skapade eller återskapade en grupp webbplats.</span><span class="sxs-lookup"><span data-stu-id="5e6c1-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="5e6c1-104">Om du har tagit bort en grupp och dess anslutna webbplats och vill skapa en ny webbplats med samma URL måste du ta bort den föregående webbplatsen permanent.</span><span class="sxs-lookup"><span data-stu-id="5e6c1-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="5e6c1-105">Ladda ned [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="5e6c1-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="5e6c1-106">Mer information om hur du kommer igång med PowerShell finns i [komma igång med SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="5e6c1-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="5e6c1-107">Ta bort webbplatsen från borttagna webbplatser med PowerShell-cmdleten [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="5e6c1-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="5e6c1-108">PowerShell krävs för att permanent ta bort grupp webbplatser.</span><span class="sxs-lookup"><span data-stu-id="5e6c1-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="5e6c1-109">Om du skapar en sammankopplad webbplats och får ett varnings meddelande: **en annan grupp med samma alias finns**i [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="5e6c1-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="5e6c1-110">Lös problemet genom att ta bort den befintliga gruppen om den inte längre behövs eller skapa webbplatsen med ett annat tilldelat alias.</span><span class="sxs-lookup"><span data-stu-id="5e6c1-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="5e6c1-111">Det finns olika sätt att skapa och använda moderna grupper med SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5e6c1-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="5e6c1-112">Du kan ansluta befintliga webbplatser till en Microsoft 365-grupp.</span><span class="sxs-lookup"><span data-stu-id="5e6c1-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="5e6c1-113">Mer information finns i [ansluta en Microsoft 365-grupp med användar gränssnittet i SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="5e6c1-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="5e6c1-114">Om du vill skapa en Microsoft 365-gruppansluten webbplats måste du skapa en [grupp webbplats](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="5e6c1-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
