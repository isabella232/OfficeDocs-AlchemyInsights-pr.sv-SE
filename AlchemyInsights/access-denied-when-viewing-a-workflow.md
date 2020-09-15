---
title: Åtkomst nekad när du visar ett arbets flöde
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688820"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="ef75e-102">Åtkomst nekad när du visar ett arbets flöde</span><span class="sxs-lookup"><span data-stu-id="ef75e-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="ef75e-103">SharePoint 2013-arbets flöden som försöker skicka ett e-postmeddelande till en SharePoint-grupp kan Miss lyckas med fel meddelandet "åtkomst nekad" om medlemskapet i SharePoint-gruppen inte är inställt på alla.</span><span class="sxs-lookup"><span data-stu-id="ef75e-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="ef75e-104">**Så här löser du problemet:**</span><span class="sxs-lookup"><span data-stu-id="ef75e-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="ef75e-105">Tillåt alla att se medlemmarna i SharePoint-gruppen.</span><span class="sxs-lookup"><span data-stu-id="ef75e-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="ef75e-106">Ta bort SharePoint-gruppen från raden till eller kopia i e-postmeddelandet.</span><span class="sxs-lookup"><span data-stu-id="ef75e-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="ef75e-107">Lägg uttryckligen till användarna i raden till eller kopia om Synlighets synligheten inte kan ändras för SharePoint-gruppen.</span><span class="sxs-lookup"><span data-stu-id="ef75e-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="ef75e-108">Mer information finns i [http-obehörig till/_vti_bin/client.svc/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="ef75e-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  