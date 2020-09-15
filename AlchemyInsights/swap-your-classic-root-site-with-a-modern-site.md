---
title: Byta till en klassisk rotplats med en modern webbplats
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691197"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Byta till en klassisk rotplats med en modern webbplats

Om din miljö installerades före april 2019 kan du ändra din rotplats till en modern webbplats med hjälp av Microsoft PowerShell:

- Om du har en annan webbplats som du vill använda som rotplats kan du byta ut [(byta plats) på rot webbplatsen](https://docs.microsoft.com/sharepoint/modern-root-site) . 
    - Använd [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) för att byta plats för en webbplats med en annan webbplats när du arkiverar den ursprungliga webbplatsen. Tillgängligt för både grupp webbplatsen (inte ansluten till en grupp) och kommunikations webbplats. 

- Ytterligare funktioner infogas snart så att du kan fortsätta att använda innehållet på webbplatsen, men konvertera den befintliga webbplatsen till en kommunikations webbplats. 
>[!Important]
>Dessa funktioner utdelas gradvis. Fortsätt att kontrol lera meddelande Center efter uppdateringar. 

## <a name="known-issues-with-swapping-sites"></a>Kända problem med att byta plats

- Mål webbplatsen kan returnera fel meddelandet "inte hittas" (HTTP 404) under en kort tids period.
- Innehåll måste crawlas om för att uppdatera Sök indexet. Ingen manuell åtgärd krävs – detta görs automatiskt.
- Allt som är beroende av "statiska" länkar (till exempel filsynkronisering och OneNote-filer) måste åtgärdas manuellt.
- Om käll webbplatsen var en webbplats för organisatoriska nyheter uppdaterar du webb adressen.Få en lista över alla webbplats nyheter.
- Project Server-webbplatser måste kanske val IDE ras för att säkerställa att de är korrekt kopplade.
