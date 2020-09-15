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
# <a name="access-denied-when-viewing-a-workflow"></a>Åtkomst nekad när du visar ett arbets flöde

SharePoint 2013-arbets flöden som försöker skicka ett e-postmeddelande till en SharePoint-grupp kan Miss lyckas med fel meddelandet "åtkomst nekad" om medlemskapet i SharePoint-gruppen inte är inställt på alla.
  
 **Så här löser du problemet:**
  
 1. Tillåt alla att se medlemmarna i SharePoint-gruppen.
  
 2. Ta bort SharePoint-gruppen från raden till eller kopia i e-postmeddelandet.
  
 3. Lägg uttryckligen till användarna i raden till eller kopia om Synlighets synligheten inte kan ändras för SharePoint-gruppen.
  
Mer information finns i [http-obehörig till/_vti_bin/client.svc/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  