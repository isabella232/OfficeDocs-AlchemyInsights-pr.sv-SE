---
title: Ändra e-postadress för en Microsoft 365-grupp eller Microsoft Teams
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
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756575"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Ändra e-postadress för en Microsoft 365-grupp eller Microsoft Teams

Du kan ändra e-postadressen i en Microsoft 365-grupp eller Microsoft Teams med hjälp av [administratörscenter för Microsoft 365](https://admin.microsoft.com/). Välj bara gruppen och välj @redigera e-postadress.

Du kan också använda följande EXO PowerShell-kommando för att ändra den primära SMTP-adressen för en Microsoft 365-grupp/Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Exempel:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
