---
title: Inga resultat som returneras under innehålls sökning
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680329"
---
# <a name="no-results-returned-during-content-searchexport"></a>Inga resultat som returneras under innehålls sökning

Om du har problem med följande eDiscovery-scenarier:

- Innehålls sökning/export returnerar inga data eller oväntade data
- eDiscovery-sökning eller export Miss lyckas

Detta kan bero på att vissa säkerhets filter för efterlevnad har ställts in av en viss administratör och inte har meddelats till alla administratörer.

Lös problemet genom att kontrol lera om det finns några säkerhets filter för efterlevnad som kan orsaka dessa problem:

1. Ansluta till säkerhets-och Compliance Center PowerShell
2. Kör följande cmdlets:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Mer information om säkerhets filter för efterlevnad finns i avsnittet [behörigheter för innehålls sökning](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
