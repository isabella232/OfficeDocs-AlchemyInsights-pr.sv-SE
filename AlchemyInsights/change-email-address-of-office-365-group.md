---
title: Ändra e-postadress för en Microsoft 365-grupp
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/27/2020
ms.locfileid: "44283262"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a>Ändra e-postadress för en Microsoft 365-grupp

Du kan ändra e-postadressen för en Microsoft 365-grupp med hjälp av administrationscentret. Välj bara gruppen och välj @edit e-postadress.

Du kan också använda följande EXO PowerShell-kommando för att ändra den primära SMTP-adressen för en Microsoft 365-grupp:

Ange unifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address>

Exempel:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
