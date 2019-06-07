---
title: Lägga till en grupp till en SharePoint-webbplats
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758748"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a><span data-ttu-id="82890-102">Skapa grupp ansluten plats i SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="82890-102">Create group connected site in SharePoint Online</span></span>

<span data-ttu-id="82890-103">Det finns några vanliga problem som kan uppstå när Skapa eller återskapa en grupp ansluten plats.</span><span class="sxs-lookup"><span data-stu-id="82890-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="82890-104">Om du har tagit bort en grupp och dess anslutna platsen och vill skapa en annan webbplats med samma URL, måste du ta bort den tidigare webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="82890-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="82890-105">Hämta [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="82890-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="82890-106">Mer information om att komma igång med powershell finns i [komma igång med SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="82890-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="82890-107">Ta bort webbplatsen från bort platser med hjälp av powershell-cmdlet för [Ta bort SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="82890-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="82890-108">Om du skapar en grupp ansluten plats och en varning redan finns en annan grupp med samma alias, kontrollera befintliga grupper från [Office 365 Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="82890-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="82890-109">Kopplad till problemet, ta bort den befintliga gruppen om den inte längre behövs eller skapa webbplatsen med ett annat alias.</span><span class="sxs-lookup"><span data-stu-id="82890-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="82890-110">Det finns olika sätt att skapa och använda moderna grupper med SharePoint.</span><span class="sxs-lookup"><span data-stu-id="82890-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="82890-111">Du kan ansluta befintliga webbplatser till en Office 365-grupp.</span><span class="sxs-lookup"><span data-stu-id="82890-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="82890-112">Mer information finns i [ansluta en Office 365-grupp med hjälp av ineterface för SharePoint-användare](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="82890-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="82890-113">Om du vill skapa en Office 365-grupp ansluten plats måste du skapa en gruppwebbplats.</span><span class="sxs-lookup"><span data-stu-id="82890-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="82890-114">Mer information finns i [Skapa en gruppwebbplats i SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="82890-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

