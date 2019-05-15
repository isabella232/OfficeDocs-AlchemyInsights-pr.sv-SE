---
title: Modern webbplats som rotwebbplatsen
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057783"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="8c540-102">Modern webbplats som rotplats</span><span class="sxs-lookup"><span data-stu-id="8c540-102">Modern site as root site</span></span>

<span data-ttu-id="8c540-103">[Målet Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) -kunder kan nu modern kommunikations webbplats erfarenhet på klassiska rotwebbplatsen för sina SharePoint-innehavare.</span><span class="sxs-lookup"><span data-stu-id="8c540-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) customers can now enable the modern communication site experience at the classic root site of their SharePoint tenant.</span></span>

<span data-ttu-id="8c540-104">Den här funktionen kan aktiveras genom att köra en enkel PowerShell-cmdlet.</span><span class="sxs-lookup"><span data-stu-id="8c540-104">This feature can be activated by running a simple PowerShell cmdlet.</span></span> <span data-ttu-id="8c540-105">I PowerShell-kommandon att utföra har rotplatsen en ny hemsida för kommunikation webbplats.</span><span class="sxs-lookup"><span data-stu-id="8c540-105">On the successful execution of the PowerShell command(s), the root site will have a new communication site home page.</span></span> <span data-ttu-id="8c540-106">Information om krav för PowerShell-cmdlet och funktionen finns i artikeln [Aktivera SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="8c540-106">Details about the PowerShell cmdlet and feature requirements are available in the article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span></span> 

<span data-ttu-id="8c540-107">Vi kommer gradvis rullande detta, av som standard till riktade Release kunder i tidiga maj 2019 och rulle ut blir tillgänglig över hela världen i slutet av juni 2019.</span><span class="sxs-lookup"><span data-stu-id="8c540-107">We'll be gradually rolling this out, off by default, to Targeted Release customers in early May 2019, and the roll out will be available worldwide by the end of June 2019.</span></span> <span data-ttu-id="8c540-108">Fortsätta att referera till [Meddelandecenter](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) för andra nya funktioner med Modern.</span><span class="sxs-lookup"><span data-stu-id="8c540-108">Continue to refer to the [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for other new features with Modern.</span></span> 

<span data-ttu-id="8c540-109">**Viktigt**: ta inte bort klassiska rot-webbplats om du vill skapa en webbplats för modern kommunikation.</span><span class="sxs-lookup"><span data-stu-id="8c540-109">**Important**: Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="8c540-110">Detta stöds inte av Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8c540-110">This is not supported by Microsoft.</span></span> <span data-ttu-id="8c540-111">Ta bort rotwebbplatsen blir alla SharePoint-webbplatser i organisationen inte tillgänglig för alla användare förrän du återställer en webbplats eller skapa en ny webbplats med samma URL.</span><span class="sxs-lookup"><span data-stu-id="8c540-111">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> 
 
 