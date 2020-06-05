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
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580675"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Ändra e-postadress för en Microsoft 365-grupp

Du kan ändra e-postadressen för en Microsoft 365-grupp med hjälp av administrationscentret. Välj bara gruppen och välj @edit e-postadress.

Du kan också använda följande EXO PowerShell-kommando för att ändra den primära SMTP-adressen för en Microsoft 365-grupp:

Ange unifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address>

Exempel:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
