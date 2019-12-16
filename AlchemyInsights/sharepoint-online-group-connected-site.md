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
ms.openlocfilehash: 14ad9dd094902c85eaf0398c76003cea20ad4c0a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051119"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="fac45-102">Problem när du skapar eller grupperar anslutna platser i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="fac45-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="fac45-103">Det finns ett par vanliga problem som uppstår när du skapar eller återskapar en grupp ansluten webbplats.</span><span class="sxs-lookup"><span data-stu-id="fac45-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="fac45-104">Om du har raderat en grupp och dess anslutna webbplats och vill skapa en annan webbplats med samma webbadress måste du ta bort den tidigare webbplatsen permanent.</span><span class="sxs-lookup"><span data-stu-id="fac45-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="fac45-105">Hämta [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="fac45-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="fac45-106">Mer information om att komma igång med PowerShell finns i [komma igång med SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="fac45-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="fac45-107">Ta bort webbplatsen från borttagna webbplatser med hjälp av [denTa bort SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell-cmdlet.</span><span class="sxs-lookup"><span data-stu-id="fac45-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="fac45-108">Om du skapar en grupp ansluten webbplats och får en varning en annan grupp med samma alias redan finns, kontrollera befintliga grupper från [Office 365 från administratörs Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="fac45-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="fac45-109">Lös problemet genom att ta bort den befintliga gruppen om den inte längre behövs eller skapa webbplatsen med ett annat alias tilldelat.</span><span class="sxs-lookup"><span data-stu-id="fac45-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="fac45-110">Det finns olika sätt att skapa och använda moderna grupper med SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fac45-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="fac45-111">Du kan ansluta befintliga webbplatser till en Office 365-grupp.</span><span class="sxs-lookup"><span data-stu-id="fac45-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="fac45-112">Mer information finns [i ansluta en Office 365-grupp med hjälp av SharePoint-användaren ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="fac45-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="fac45-113">Om du vill skapa en Office 365-grupp ansluten webbplats måste du skapa en gruppwebbplats.</span><span class="sxs-lookup"><span data-stu-id="fac45-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="fac45-114">Mer information finns [i skapa en gruppwebbplats i SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="fac45-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

