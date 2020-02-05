---
title: Lägga till en grupp på en SharePoint-webbplats
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770369"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="29ed7-102">Problem när du skapar en gruppansluten webbplats i SharePoint</span><span class="sxs-lookup"><span data-stu-id="29ed7-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="29ed7-103">Några vanliga problem uppstod när du skapar eller återskapar en gruppansluten plats.</span><span class="sxs-lookup"><span data-stu-id="29ed7-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="29ed7-104">Om du har tagit bort en grupp och dess anslutna webbplats och vill skapa en annan webbplats med samma URL måste du ta bort den tidigare webbplatsen permanent.</span><span class="sxs-lookup"><span data-stu-id="29ed7-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="29ed7-105">Hämta [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="29ed7-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="29ed7-106">Mer information om hur du kommer igång med Powershell finns i [Komma igång med SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="29ed7-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="29ed7-107">Ta bort webbplatsen från borttagna webbplatser med hjälp av den [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span><span class="sxs-lookup"><span data-stu-id="29ed7-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="29ed7-108">Powershell krävs för att permanent ta bort gruppplatser.</span><span class="sxs-lookup"><span data-stu-id="29ed7-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="29ed7-109">Om du skapar en gruppansluten webbplats och får en varning: **Det finns redan en annan grupp med samma alias**kontrollerar du de befintliga grupperna från Office [365 från Administrationscenter](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="29ed7-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="29ed7-110">LÃ¶s problemet genom att ta bort den befintliga gruppen om den inte lÃ¤ngre behövs eller skapar webbplatsen med ett annat alias tilldelat.</span><span class="sxs-lookup"><span data-stu-id="29ed7-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="29ed7-111">Det finns olika sätt att skapa och använda moderna grupper med SharePoint.</span><span class="sxs-lookup"><span data-stu-id="29ed7-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="29ed7-112">Du kan ansluta befintliga webbplatser till en Office 365-grupp.</span><span class="sxs-lookup"><span data-stu-id="29ed7-112">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="29ed7-113">Mer information finns i [Ansluta en Office 365-grupp med hjälp av SharePoint-användargränssnittet](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="29ed7-113">For more info, see [Connect an Office 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="29ed7-114">Om du vill skapa en Office 365-gruppansluten webbplats måste du skapa en [gruppwebbplats](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="29ed7-114">To create an Office 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
