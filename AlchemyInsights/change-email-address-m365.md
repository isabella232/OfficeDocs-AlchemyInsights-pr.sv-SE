---
title: Ändra e-postadressen för Microsoft 365-gruppen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: f54ca5df09d0604f6d58c6c8a41dc907485e1f04
ms.sourcegitcommit: beb9715ac0c8e8333fef6764ecd346b7401a2612
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/10/2020
ms.locfileid: "48462058"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Ändra e-postadress för en Microsoft 365-grupp

Du kan ändra e-postadressen för en Microsoft 365-grupp i administrations centret. Markera gruppen och välj @edit e-postadress.

Du kan också använda EXO PowerShell-kommandot för att ändra primär SMTP-adressen för en Microsoft 365-grupp:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Exempel:

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
