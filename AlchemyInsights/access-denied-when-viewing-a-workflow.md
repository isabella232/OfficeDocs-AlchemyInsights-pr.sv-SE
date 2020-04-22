---
title: Åtkomst nekad när du visar ett arbetsflöde
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687348"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="99ed9-102">Åtkomst nekad när du visar ett arbetsflöde</span><span class="sxs-lookup"><span data-stu-id="99ed9-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="99ed9-103">SharePoint 2013-arbetsflöden som försöker skicka ett e-postmeddelande till en SharePoint-grupp kan misslyckas med felmeddelandet "Åtkomst nekad" om medlemskapet i SharePoint-gruppen inte är inställt på Alla.</span><span class="sxs-lookup"><span data-stu-id="99ed9-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="99ed9-104">**Lös problemet genom att göra så här:**</span><span class="sxs-lookup"><span data-stu-id="99ed9-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="99ed9-105">Tillåt alla att se medlemmarna i SharePoint-gruppen.</span><span class="sxs-lookup"><span data-stu-id="99ed9-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="99ed9-106">Ta bort SharePoint-gruppen från raden Till eller KOPIA i e-postmeddelandet.</span><span class="sxs-lookup"><span data-stu-id="99ed9-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="99ed9-107">Lägg uttryckligen till användarna på raden Till eller KOPIA om medlemskapssynligheten inte kan ändras för SharePoint-gruppen.</span><span class="sxs-lookup"><span data-stu-id="99ed9-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="99ed9-108">Mer information finns i [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="99ed9-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  