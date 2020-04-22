---
title: Modern plats som rotplats
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713809"
---
# <a name="modern-site-as-root-site"></a>Modern plats som rotplats

Vi har börjat rulla ut en ny funktion som gör att du kan [byta din klassiska webbplats rotplats med en modern webbplats](https://docs.microsoft.com/sharepoint/modern-root-site). Använd [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) för att byta plats på en plats med en annan plats medan du arkiverar den ursprungliga platsen. Tillgänglig för både gruppwebbplats (inte ansluten till en grupp) och kommunikationswebbplats.

>[!Important]
> Ta inte bort din klassiska rotplats för att skapa en modern kommunikationswebbplats. Detta stöds inte av Microsoft. Om du tar bort rotwebbplatsen blir alla SharePoint-webbplatser i organisationen otillgängliga för alla användare, tills du återställer webbplatsen eller skapar en ny webbplats med samma URL. Vi kommer att kommunicera den här funktionen via meddelandecentret. Du bör förvänta dig att funktionen ska aktiveras i din klient inom kort.

## <a name="known-issues-with-swapping-sites"></a>Kända problem med att byta webbplatser
- Målplatsen kan returnera ett HTTP 404-fel (inte hittats" (HTTP 404) under en kort tidsperiod.
- Innehållet måste testas igen för att uppdatera sökindexet. Det finns inget manuellt steg som krävs här, detta kommer att göras automatiskt.
- Allt som är beroende av "statiska" länkar (till exempel Filsynkronisering och OneNote-filer) måste korrigeras manuellt.
- Project Server-platser kan behöva valideras för att säkerställa att de fortfarande är korrekt associerade. 
