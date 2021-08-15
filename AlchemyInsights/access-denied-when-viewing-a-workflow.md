---
title: Access denied when viewing a Workflow
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955219"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Access denied when viewing a Workflow

SharePoint 2013-arbetsflöden som försöker skicka ett e-postmeddelande till en SharePoint-grupp kan misslyckas och felmeddelandet "Åtkomst nekad" visas om medlemskapet i SharePoint-gruppen inte är inställt på Alla.
  
 **Lös problemet genom att göra följande:**
  
 1. Tillåta att alla ser medlemmar i SharePoint grupp.
  
 2. Ta SharePoint gruppen från raden Till eller kopia i e-postmeddelandet.
  
 3. Lägg uttryckligen till användare på raden Till eller Kopia om medlemskapssynligheten inte kan ändras SharePoint grupp.
  
Mer information finns på HTTP Obehörig åtkomst till [/_vti_bin/client.svc/sp.utilities.utility.SendEmail.](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)
  