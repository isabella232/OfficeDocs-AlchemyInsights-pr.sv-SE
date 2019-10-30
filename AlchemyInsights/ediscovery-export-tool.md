---
title: exportverktyg för e-informationsavslöjande
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 7e2964ef0a44ddf421e4aae007acbdbda196e20f
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/29/2019
ms.locfileid: "37769321"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Kan du inte installera eller köra e-informationsavslöjande export verktyg?

Om du inte kan installera eller köra Office 365 e-informationsavslöjande export verktyg för att hämta sökresultat, kontrollera följande saker:
  
- Den dator du använder uppfyller dessa förutsättningar:

  - 32-eller 64-bitars versioner av Windows 7 och senare versioner

  - Microsoft.NET Framework 4,7

  - En webbläsare som stöds:

  - Microsoft Edge

    Eller

  - Internet Explorer 10 och senare versioner

    Andra webbläsare, till exempel Google Chrome och Mozilla Firefox stöds inte.

- Din organisation kan ansluta till slutpunkten i Azure, vilket är ** \*. blob.Core.Windows.net** (jokertecknet representerar en unik identifierare för ditt exportjobb).

- Du har tilldelats rollen export i säkerhets &amp; regelefterlevnadscentret för Office 365. Som standard är den här rollen endast tilldelad till rollgruppen eDiscovery Manager. Se [tilldela eDiscovery-behörigheter](https://docs.microsoft.com/office365/securitycompliance/assign-ediscovery-permissions).

Mer information finns i [Exportera innehåll sökresultat](https://docs.microsoft.com/office365/securitycompliance/export-search-results).
  