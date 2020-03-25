---
title: Resursmigreringsbegränsning med 503 fel
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931676"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a>Resursmigreringsbegränsning med 503 fel

**Viktigt:** Många SharePoint Online- och OneDrive-kunder kör affärskritiska program mot tjänsten som körs i bakgrunden. Dessa inkluderar innehållsmigrering, DLP (Data Loss Prevention) och säkerhetskopieringslösningar. Under dessa exempellösa tider vidtar vi åtgärder för att se till att SharePoint Online- och OneDrive-tjänster förblir mycket tillgängliga och tillförlitliga för dina användare som är mer beroende av tjänsten i fjärrarbete.

Till stöd för detta mål har vi implementerat strängare begränsningsgränser för bakgrundsappar (migrering, DLP och säkerhetskopieringslösningar) under dagtid. Du bör förvänta dig att dessa appar kommer att uppnå mycket begränsad dataflöde under dessa tider. Under kvälls- och helgtimmar för regionen kommer tjänsten dock att vara redo att behandla en betydligt högre mängd förfrågningar från bakgrundsappar.

**503 fel vid migrering till SharePoint Online**

Det verkar som om du migrerar till SharePoint Online och tar emot 503 fel. Följ stegen nedan så att vi kan hjälpa dig så snart som möjligt. 

1. Klicka på **Kontakta support**och sedan på **Ny servicebegäran**.
2. Om du vill ange rubrik och beskrivning skriver du **SharePoint-migreringsbegränsning med 503**.
3. När biljetten har skickats, vänligen uppdatera den med följande information:
    - Hur mycket kvar av migrering (till exempel hur många TBs?).
    - Start- och slutdatum för migrering.
    - Beskriv var du migrerar ditt innehåll från, till exempel SharePoint Server, Box, GDrive, Filresurser osv..
    - Uppskatta antalet begränsningsfel (till exempel x begränsning per timme?) och när skedde begränsningen.
    - Vilket migreringsverktyg du använder (till exempel SPMT eller ShareGate).


