---
title: Ändra e-postadressen för en Microsoft 365-grupp
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
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819062"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Ändra e-postadressen för en Microsoft 365-grupp

Du kan ändra e-postadressen för en Microsoft 365-grupp med hjälp av administrationscentret. Välj bara gruppen och välj @redigera e-postadress.

Du kan också använda följande EXO PowerShell-kommando för att ändra den primära SMTP-adressen för en Microsoft 365-grupp:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Exempel:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
