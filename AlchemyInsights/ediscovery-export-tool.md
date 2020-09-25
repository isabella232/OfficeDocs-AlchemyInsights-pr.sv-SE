---
title: verktyget för eDiscovery-export
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277936"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Kan du inte installera eller köra verktyget för eDiscovery-export?

Om du inte kan installera eller köra verktyget för eDiscovery-export för att hämta Sök resultat kan du kontrol lera följande:
  
- Den dator du använder uppfyller dessa krav:

  - 32-eller 64-bitars versioner av Windows 7 och senare versioner

  - Microsoft .NET Framework 4.7

  - En webbläsare som stöds:

  - Microsoft Edge

    Eller

  - Internet Explorer 10 och senare versioner

    Andra webbläsare, till exempel Google Chrome och Mozilla Firefox, stöds inte.

- Din organisation kan ansluta till slut punkten i Azure, som är ** \* . blob.Core.Windows.net** (jokertecknet representerar en unik identifierare för ditt export jobb).

- Du har tilldelats export rollen i Microsoft 365 Security &amp; Compliance Center. Som standard är den här rollen bara tilldelad till roll gruppen eDiscovery Manager. Se [tilldela eDiscovery-behörigheter](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Mer information finns i [Exportera innehålls Sök Resultat](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

Om du exporterar fler än 100K-postlådor måste du använda följande PowerShell för att ladda ned export resultaten:  [Exportera resultat från fler än 100K-postlådor](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).