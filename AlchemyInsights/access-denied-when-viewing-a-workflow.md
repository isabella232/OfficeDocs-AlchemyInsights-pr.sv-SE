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
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36747766"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Åtkomst nekad när ett arbetsflöde visas

SharePoint 2013 arbetsflöden som försöker skicka ett e-postmeddelande till en SharePoint-grupp kan misslyckas med felmeddelandet "åtkomst nekad" om medlemskap i SharePoint-gruppen inte är inställd på alla.
  
 **Gör så här om du vill lösa problemet:**
  
 1. Tillåt alla att se medlemmarna i SharePoint-gruppen.
  
 2. Ta bort SharePoint-gruppen från raden till eller kopia av e-postmeddelandet.
  
 3. Lägg uttryckligen till användarna till raden till eller kopia om medlemskapets synlighet inte kan ändras för SharePoint-gruppen.
  
För att se mer information hänvisas till [http obehörig till/_vti_bin/client.svc/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  