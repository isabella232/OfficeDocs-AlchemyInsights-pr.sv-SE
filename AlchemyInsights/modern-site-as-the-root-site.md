---
title: Modern webbplats som rotplats
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
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666888"
---
# <a name="modern-site-as-root-site"></a>Modern webbplats som rotplats

Vi har börjat använda en ny funktion som gör att du kan [byta till en klassisk webbplats med en modern webbplats](https://docs.microsoft.com/sharepoint/modern-root-site). Använd [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) för att byta plats för en webbplats med en annan webbplats när du arkiverar den ursprungliga webbplatsen. Tillgängligt för både grupp webbplatsen (inte ansluten till en grupp) och kommunikations webbplats.

>[!Important]
> Ta inte bort den klassiska rot webbplatsen för att skapa en modern kommunikations webbplats. Det här stöds inte av Microsoft. Om du tar bort rot webbplatsen kommer alla SharePoint-webbplatser inte att vara tillgängliga för alla användare förrän du återställer webbplatsen eller skapar en ny webbplats på samma URL. Vi kommer att kommunicera denna funktion via meddelande Center. Du bör förvänta dig att funktionen är aktive rad i klient organisationen.

## <a name="known-issues-with-swapping-sites"></a>Kända problem med att byta plats
- Mål webbplatsen kan returnera fel meddelandet "inte hittas" (HTTP 404) under en kort tids period.
- Innehåll måste crawlas om för att uppdatera Sök indexet. Det finns inget manuell steg här, detta görs automatiskt.
- Allt som är beroende av "statiska" länkar (till exempel filsynkronisering och OneNote-filer) måste åtgärdas manuellt.
- Project Server-webbplatser måste kanske val IDE ras för att säkerställa att de är korrekt kopplade. 
