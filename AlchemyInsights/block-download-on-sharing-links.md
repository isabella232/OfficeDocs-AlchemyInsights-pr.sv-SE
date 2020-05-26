---
title: Blockera nedladdning på delningslänkar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 8cb53754125cedf4a3d0426d6c3bf70297eb3d74
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358512"
---
# <a name="block-download-on-sharing-links"></a><span data-ttu-id="0edcd-102">Blockera nedladdning på delningslänkar</span><span class="sxs-lookup"><span data-stu-id="0edcd-102">Block download on sharing links</span></span>

<span data-ttu-id="0edcd-103">**Hämtning av block** är tillgängligt för **endast visningslänkar** till Office-dokument.</span><span class="sxs-lookup"><span data-stu-id="0edcd-103">**Block download** is available for **view-only links** to Office documents.</span></span> <span data-ttu-id="0edcd-104">När du väljer det här alternativet visas inte alternativ för att hämta, skriva ut eller kopiera filen när du får åtkomst till filen via länken som du skapade.</span><span class="sxs-lookup"><span data-stu-id="0edcd-104">When you select this option, people who gain access to the file via the link you created will not see options to download, print, or copy the file.</span></span>

<span data-ttu-id="0edcd-105">Administratörer kan styra om inställningen "blockera hämtning" bara visas för Office-filer eller inte genom att ändra `BlockDownloadLinksFileType` inställningen i [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) eller [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell-cmdlets.</span><span class="sxs-lookup"><span data-stu-id="0edcd-105">Administrators can control whether the "block download" setting appears only for Office files or not by changing the `BlockDownloadLinksFileType` setting in the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) or [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell cmdlets.</span></span>
