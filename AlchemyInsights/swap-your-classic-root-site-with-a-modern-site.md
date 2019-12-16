---
title: Byt ut din klassiska rotwebbplats mot en modern sajt
ms.author: pebaum
author: pebaum
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: fe1f0f662c49de2bd0b5b997697c98309cb7983f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042945"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Byt ut din klassiska rotwebbplats mot en modern sajt

Om din miljö har ställts in före april 2019, kan du ändra din rotwebbplats till en modern webbplats med hjälp av Microsoft PowerShell:

- Om du har en annan webbplats som du vill använda som rotwebbplats kan du ersätta [(byta) rotwebbplatsen](https://docs.microsoft.com/sharepoint/modern-root-site) med den. 
    - Använd [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) för att byta plats på en plats med en annan plats medan du arkiverar den ursprungliga platsen. Tillgänglig för både gruppwebbplats (inte ansluten till en grupp) och kommunikations plats. 

- Ytterligare funktioner kommer att introduceras snart som gör att du kan fortsätta att använda innehållet på webbplatsen, men konvertera den befintliga platsen till en kommunikations plats. 
>[!Important]
>Dessa funktioner kommer att rullas ut gradvis. Fortsätt att kontrollera Office 365 Message Center för uppdateringar. 

## <a name="known-issues-with-swapping-sites"></a>Kända problem med att byta webbplatser

- Målwebbplatsen kan returnera felet "hittades inte" (HTTP 404) under en kort tidsperiod.
- Innehållet kommer att behöva återupprepas för att uppdatera sökindexet. Det finns ingen manuell steg krävs-detta kommer att ske automatiskt.
- Allt som är beroende av "statiska" länkar (till exempel filsynkronisering och OneNote-filer) måste korrigeras manuellt.
- Om källplatsen var en nyhetswebbplats för organisationen uppdaterar du URL: en.Få en lista över alla organisationens nyhetssidor.
- Project Server-platser kan behöva verifieras för att säkerställa att de fortfarande är korrekt associerade.





