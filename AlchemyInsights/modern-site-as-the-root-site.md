---
title: Modern webbplats som rotwebbplats
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: a0f48dc79b51168c9cc045078ad8fc7d668343c7
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327620"
---
# <a name="modern-site-as-root-site"></a>Modern webbplats som rotwebbplats

Vi har börjat distribuera en ny funktion som gör att du kan byta ut den klassiska webbplatsens [rotwebbplats mot en modern webbplats.](https://docs.microsoft.com/sharepoint/modern-root-site) Använd [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) för att växla plats för en webbplats med en annan webbplats medan den ursprungliga webbplatsen arkiveras. Tillgängligt för både gruppwebbplats (inte ansluten till en grupp) och kommunikationswebbplats.

**Viktigt:** Ta inte bort din klassiska rotwebbplats för att skapa en modern kommunikationswebbplats. Detta stöds inte av Microsoft. Om du tar bort rotwebbplatsen blir alla SharePoint i organisationen otillgängliga för alla användare, tills du återställer webbplatsen eller skapar en ny webbplats med samma URL. Vi meddelar den här funktionen via meddelandecentret. Du kan förvänta dig att funktionen aktiveras i klientorganisationen inom kort.

## <a name="known-issues-with-swapping-sites"></a>Kända problem med webbplatsbyte
- Målwebbplatsen kan returnera ett "hittades inte" (HTTP 404)-fel under en kort tidsperiod.
- Innehållet måste omsökas för att uppdatera sökindexet. Det krävs inget manuellt steg här, det görs automatiskt.
- Allt som är beroende av "statiska" länkar (till exempel filsynkronisering OneNote filer) behöver korrigeras manuellt.
- Project Serverwebbplatser kan behöva verifieras för att säkerställa att de fortfarande är korrekt associerade. 
