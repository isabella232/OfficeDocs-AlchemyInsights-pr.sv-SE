---
title: Ändra e-postadressen för en Microsoft 365 grupp
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 6bd9301b983d09f6a0058fee17577b9fc695458ed205f96aacf79a87e4a91e34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930747"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Ändra e-postadressen för en Microsoft 365 grupp

Du kan ändra e-postadressen för Microsoft 365 grupp med hjälp av administrationscentret. Välj bara gruppen och välj @redigera e-postadress.

Du kan också använda följande EXO PowerShell-kommando för att ändra den primära SMTP-adressen för en Microsoft 365 grupp:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Exempel:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
