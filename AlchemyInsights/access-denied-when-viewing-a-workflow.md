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
# <a name="access-denied-when-viewing-a-workflow"></a>Åtkomst nekad när du visar ett arbetsflöde

SharePoint 2013-arbetsflöden som försöker skicka ett e-postmeddelande till en SharePoint-grupp kan misslyckas med felmeddelandet "Åtkomst nekad" om medlemskapet i SharePoint-gruppen inte är inställt på Alla.
  
 **Lös problemet genom att göra så här:**
  
 1. Tillåt alla att se medlemmarna i SharePoint-gruppen.
  
 2. Ta bort SharePoint-gruppen från raden Till eller KOPIA i e-postmeddelandet.
  
 3. Lägg uttryckligen till användarna på raden Till eller KOPIA om medlemskapssynligheten inte kan ändras för SharePoint-gruppen.
  
Mer information finns i [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  