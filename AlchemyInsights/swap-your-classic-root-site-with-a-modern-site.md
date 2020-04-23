---
title: Byt din klassiska rotplats med en modern webbplats
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741562"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Byt din klassiska rotplats med en modern webbplats

Om din miljö har konfigurerats före april 2019 kan du ändra rotplatsen till en modern webbplats med hjälp av Microsoft PowerShell:

- Om du har en annan plats som du vill använda som rotplats kan du ersätta [(byta) rotplatsen](https://docs.microsoft.com/sharepoint/modern-root-site) med den. 
    - Använd [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) för att byta plats på en plats med en annan plats medan du arkiverar den ursprungliga platsen. Tillgänglig för både gruppwebbplats (inte ansluten till en grupp) och kommunikationswebbplats. 

- Ytterligare funktioner kommer att införas snart som gör att du kan fortsätta använda innehållet på webbplatsen, men konvertera den befintliga platsen till en kommunikationswebbplats. 
>[!Important]
>Dessa funktioner kommer att rullas ut gradvis. Fortsätt att söka efter uppdateringar i Meddelandecenter. 

## <a name="known-issues-with-swapping-sites"></a>Kända problem med att byta webbplatser

- Målplatsen kan returnera ett HTTP 404-fel (inte hittats" (HTTP 404) under en kort tidsperiod.
- Innehållet måste testas igen för att uppdatera sökindexet. Det finns inget manuellt steg som krävs - detta kommer att göras automatiskt.
- Allt som är beroende av "statiska" länkar (till exempel Filsynkronisering och OneNote-filer) måste korrigeras manuellt.
- Om källwebbplatsen var en organisationsnyhetswebbplats uppdaterar du webbadressen.Få en lista över alla organisationsnyhetswebbplatser.
- Project Server-platser kan behöva valideras för att säkerställa att de fortfarande är korrekt associerade.
