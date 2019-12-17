---
title: Åtkomst nekad när ett arbetsflöde visas
ms.author: pebaum
author: pebaum
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 1cfda8e08ada05858a28f2bede8c31261f9de351
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050543"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="489c9-102">Åtkomst nekad när ett arbetsflöde visas</span><span class="sxs-lookup"><span data-stu-id="489c9-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="489c9-103">SharePoint 2013 arbetsflöden som försöker skicka ett e-postmeddelande till en SharePoint-grupp kan misslyckas med felmeddelandet "åtkomst nekad" om medlemskap i SharePoint-gruppen inte är inställd på alla.</span><span class="sxs-lookup"><span data-stu-id="489c9-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="489c9-104">**Gör så här om du vill lösa problemet:**</span><span class="sxs-lookup"><span data-stu-id="489c9-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="489c9-105">Tillåt alla att se medlemmarna i SharePoint-gruppen.</span><span class="sxs-lookup"><span data-stu-id="489c9-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="489c9-106">Ta bort SharePoint-gruppen från raden till eller kopia av e-postmeddelandet.</span><span class="sxs-lookup"><span data-stu-id="489c9-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="489c9-107">Lägg uttryckligen till användarna till raden till eller kopia om medlemskapets synlighet inte kan ändras för SharePoint-gruppen.</span><span class="sxs-lookup"><span data-stu-id="489c9-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="489c9-108">För att se mer information hänvisas till [http obehörig till/_vti_bin/client.svc/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="489c9-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  