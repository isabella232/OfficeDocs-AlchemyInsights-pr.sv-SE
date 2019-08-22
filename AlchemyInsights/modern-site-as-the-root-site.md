---
title: Modern webbplats som rotwebbplatsen
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2f75f1e60af06da47fe846e84bbb370dd60084e9
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543871"
---
# <a name="modern-site-as-root-site"></a>Modern webbplats som rotplats

Vi har börjat introduktionen en ny funktion som gör att du kan byta klassiska webbplats rotplatsen med en modern webbplats. Använd [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) för att byta en plats till en annan site under arkivering den ursprungliga webbplatsen. Tillgängligt för både gruppwebbplats (inte ansluten till en grupp) och kommunikation. 

>[!Important]
> Ta inte bort klassiska rot-webbplats om du vill skapa en webbplats för modern kommunikation. Detta stöds inte av Microsoft. Ta bort rotwebbplatsen blir alla SharePoint-webbplatser i organisationen inte tillgänglig för alla användare förrän du återställer en webbplats eller skapa en ny webbplats med samma URL. Vi ska kommunicera denna funktion via message center. Du kan förvänta dig funktionen att vara aktiverad i din hyresgäst inom kort.

## <a name="known-issues-with-swapping-sites"></a>Kända problem med att byta platser
- Målplatsen kan returnera ett ”hittades inte” fel (HTTP 404) under en kort tid.
- Innehållet måste vara crawlas igen om du vill uppdatera sökindexet. Det finns inga manuella steg krävs här, detta görs automatiskt.
- Allt beroende på ”statisk” länkar (till exempel filsynkronisering och OneNote-filer) måste korrigeras manuellt.
- Project Server-platser kan behöva valideras för att säkerställa att de är fortfarande kopplade på rätt sätt. 
