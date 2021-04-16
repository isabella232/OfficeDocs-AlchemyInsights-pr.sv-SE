---
title: eDiscovery-exportverktyg
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814606"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Kan du inte installera eller köra eDiscovery-exportverktyget?

Om du inte kan installera eller köra eDiscovery-exportverktyget för att ladda ned sökresultat kontrollerar du följande:
  
- Datorn du använder uppfyller dessa krav:

  - 32- eller 64-bitarsversioner av Windows 7 och senare versioner

  - Microsoft .NET Framework 4.7

  - En webbläsare som stöds:

  - Microsoft Edge

    Eller

  - Internet Explorer 10 och senare versioner

    Andra webbläsare, till exempel Google Chrome och Mozilla Firefox, stöds inte.

- Din organisation kan ansluta till slutpunkten i Azure, som är **\* .blob.core.windows.net** (jokertecknet representerar en unik identifierare för exportjobbet).

- Du har tilldelats exportrollen i Säkerhetsefterlevnadscenter för Microsoft 365. &amp; Som standard är den här rollen endast tilldelad rollgruppen för eDiscovery-hanteraren. Se [Tilldela eDiscovery-behörigheter](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Mer information finns i [Exportera resultat för innehållssökning.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

Om du exporterar fler än 100 000 postlådor måste du använda följande Powershell för att ladda ned exportresultatet: Exportera resultat från fler än [100 000 postlådor.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)