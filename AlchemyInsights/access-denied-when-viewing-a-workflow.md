---
title: Åtkomst nekad när ett arbetsflöde visas
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/18/2019
ms.locfileid: "36747766"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="118e3-102">Åtkomst nekad när ett arbetsflöde visas</span><span class="sxs-lookup"><span data-stu-id="118e3-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="118e3-103">SharePoint 2013 arbetsflöden som försöker skicka ett e-postmeddelande till en SharePoint-grupp kan misslyckas med felmeddelandet "åtkomst nekad" om medlemskap i SharePoint-gruppen inte är inställd på alla.</span><span class="sxs-lookup"><span data-stu-id="118e3-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="118e3-104">**Gör så här om du vill lösa problemet:**</span><span class="sxs-lookup"><span data-stu-id="118e3-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="118e3-105">Tillåt alla att se medlemmarna i SharePoint-gruppen.</span><span class="sxs-lookup"><span data-stu-id="118e3-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="118e3-106">Ta bort SharePoint-gruppen från raden till eller kopia av e-postmeddelandet.</span><span class="sxs-lookup"><span data-stu-id="118e3-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="118e3-107">Lägg uttryckligen till användarna till raden till eller kopia om medlemskapets synlighet inte kan ändras för SharePoint-gruppen.</span><span class="sxs-lookup"><span data-stu-id="118e3-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="118e3-108">För att se mer information hänvisas till [http obehörig till/_vti_bin/client.svc/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="118e3-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  