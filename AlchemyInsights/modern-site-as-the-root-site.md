---
title: Modern sajt som root site
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2e2bb02b9dbaf7f8ede0b4c5ba8c8f29453309cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054720"
---
# <a name="modern-site-as-root-site"></a>Modern sajt som root site

Vi har börjat utbyggnaden en ny funktion som gör att du kan [byta din klassiska webbplats rotwebbplats med en modern webbplats](https://docs.microsoft.com/sharepoint/modern-root-site). Använd [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) för att byta plats på en plats med en annan plats medan du arkiverar den ursprungliga platsen. Tillgänglig för både gruppwebbplats (inte ansluten till en grupp) och kommunikations plats.

>[!Important]
> Ta inte bort din klassiska rotwebbplats för att skapa en modern kommunikations plats. Detta stöds inte av Microsoft. Om du tar bort rotwebbplatsen blir alla SharePoint-webbplatser i organisationen otillgängliga för alla användare, tills du återställer webbplatsen eller skapar en ny plats på samma webbadress. Vi kommunicerar den här funktionen via Message Center. Du bör förvänta dig att funktionen ska aktiveras i din klient inom kort.

## <a name="known-issues-with-swapping-sites"></a>Kända problem med att byta webbplatser
- Målwebbplatsen kan returnera felet "hittades inte" (HTTP 404) under en kort tidsperiod.
- Innehållet kommer att behöva återupprepas för att uppdatera sökindexet. Det finns inget manuellt steg som krävs här, detta kommer att ske automatiskt.
- Allt som är beroende av "statiska" länkar (till exempel filsynkronisering och OneNote-filer) måste korrigeras manuellt.
- Project Server-platser kan behöva verifieras för att säkerställa att de fortfarande är korrekt associerade. 
