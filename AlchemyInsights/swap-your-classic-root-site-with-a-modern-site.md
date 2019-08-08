---
title: Byt plats på webbplatsen klassisk rot med en Modern webbplats
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "2579"
- "9000687"
ms.openlocfilehash: dad7d7a52222dc09aea532714a93ca89c0d9ae19
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/07/2019
ms.locfileid: "36246089"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Byt plats på webbplatsen klassisk rot med en Modern webbplats

Om din miljö har registrerat före April 2019 ändra du webbplatsens rot till en modern webbplats med hjälp av Microsoft PowerShell:

- Om du har en annan plats som du vill använda som din rotwebbplats kan ersätta du webbplats (swap) roten med den. 
    - Använd [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) för att byta en plats till en annan site under arkivering den ursprungliga webbplatsen. Tillgängligt för både gruppwebbplats (inte ansluten till en grupp) och kommunikation. 

- Ytterligare funktioner kommer att införas snart som gör att du kan fortsätta använda innehållet på webbplatsen, men konvertera den befintliga webbplatsen till en webbplats för kommunikation. 
>[!Important]
>Dessa funktioner ska slås gradvis. Fortsätta att kontrollera Office 365 Message Center för uppdateringar. 

## <a name="known-issues-with-swapping-sites"></a>Kända problem med att byta platser

- Målplatsen kan returnera ett ”hittades inte” fel (HTTP 404) under en kort tid.
- Innehållet måste vara crawlas igen om du vill uppdatera sökindexet. Det finns inga manuella steg krävs - detta görs automatiskt.
- Allt beroende på ”statisk” länkar (till exempel filsynkronisering och OneNote-filer) måste korrigeras manuellt.
- Om källwebbplatsen var en organisatorisk nyhetswebbplats, uppdatera URL: en.Visa en lista över alla webbplatser med nyheter om organisationen.
- Project Server-platser kan behöva valideras för att säkerställa att de är fortfarande kopplade på rätt sätt.





