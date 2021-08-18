---
title: Byt ut den klassiska rotwebbplatsen mot en modern webbplats
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
ms.openlocfilehash: e8501414498bf1937e98abaca32987e3276bb54e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316158"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Byt ut den klassiska rotwebbplatsen mot en modern webbplats

Om din miljö konfigurerades före april 2019 kan du ändra rotwebbplatsen till en modern webbplats med hjälp av Microsoft PowerShell:

- Om du har en annan webbplats som du vill använda som rotwebbplats kan du ersätta [(byta) rotwebbplatsen](https://docs.microsoft.com/sharepoint/modern-root-site) med den. 
    - Använd [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) för att växla plats för en webbplats med en annan webbplats medan den ursprungliga webbplatsen arkiveras. Tillgängligt för både gruppwebbplats (inte ansluten till en grupp) och kommunikationswebbplats. 

- Ytterligare funktioner kommer snart att introduceras som gör att du kan fortsätta använda innehållet på webbplatsen, men konvertera den befintliga webbplatsen till en kommunikationswebbplats. 

**Viktigt!** De här funktionerna distribueras gradvis. Fortsätt att söka efter uppdateringar i Meddelandecenter. 

## <a name="known-issues-with-swapping-sites"></a>Kända problem med webbplatsbyte

- Målwebbplatsen kan returnera ett "hittades inte" (HTTP 404)-fel under en kort tidsperiod.
- Innehållet måste omsökas för att uppdatera sökindexet. Du behöver inte göra något manuellt – det här görs automatiskt.
- Allt som är beroende av "statiska" länkar (till exempel filsynkronisering OneNote filer) behöver korrigeras manuellt.
- Om källwebbplatsen var en nyhetswebbplats för organisationen uppdaterar du URL:en. Visa en lista över alla webbplatser för organisationsnyheter.
- Project Serverwebbplatser kan behöva verifieras för att säkerställa att de fortfarande är korrekt associerade.
