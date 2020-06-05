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
ms.openlocfilehash: 5dab9fce935936898927afd55f8f6e9260249157
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582829"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="150af-102">Problem när du skapar en gruppansluten webbplats i SharePoint</span><span class="sxs-lookup"><span data-stu-id="150af-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="150af-103">Några vanliga problem uppstod när du skapar eller återskapar en gruppansluten plats.</span><span class="sxs-lookup"><span data-stu-id="150af-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="150af-104">Om du har tagit bort en grupp och dess anslutna webbplats och vill skapa en annan webbplats med samma WEBBADRESS måste du ta bort den tidigare webbplatsen permanent.</span><span class="sxs-lookup"><span data-stu-id="150af-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="150af-105">Ladda ner [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="150af-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="150af-106">Mer information om hur du kommer igång med Powershell finns i [Komma igång med SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="150af-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="150af-107">Ta bort webbplatsen från borttagna platser med hjälp av [cmdleten Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell.</span><span class="sxs-lookup"><span data-stu-id="150af-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="150af-108">Powershell krävs för att permanent ta bort gruppwebbplatser.</span><span class="sxs-lookup"><span data-stu-id="150af-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="150af-109">Om du skapar en gruppansluten webbplats och får en varning: Det finns redan en **annan grupp med samma alias**kontrollerar du de befintliga grupperna från Administrationscentret för Microsoft [365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="150af-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="150af-110">Lös problemet genom att ta bort den befintliga gruppen om den inte längre behövs eller skapa platsen med ett annat alias tilldelat.</span><span class="sxs-lookup"><span data-stu-id="150af-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="150af-111">Det finns olika sätt att skapa och använda moderna grupper med SharePoint.</span><span class="sxs-lookup"><span data-stu-id="150af-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="150af-112">Du kan ansluta befintliga webbplatser till en Microsoft 365-grupp.</span><span class="sxs-lookup"><span data-stu-id="150af-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="150af-113">Mer information finns i [Ansluta en Microsoft 365-grupp med SharePoint-användargränssnittet](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="150af-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="150af-114">Om du vill skapa en ansluten microsoft 365-gruppwebbplats måste du skapa en [gruppwebbplats](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="150af-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
