---
title: Ändra e-postadress för en Microsoft 365-grupp eller Microsoft Teams
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
ms.openlocfilehash: acb343553bfb7e100c03d0e7046ed5cbdd6b739b9a61e3faf17768bd8aadff34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995640"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Ändra e-postadress för en Microsoft 365-grupp eller Microsoft Teams

Du kan ändra e-postadressen i en Microsoft 365-grupp eller Microsoft Teams med hjälp av [administratörscenter för Microsoft 365](https://admin.microsoft.com/). Välj bara gruppen och välj @redigera e-postadress.

Du kan också använda följande EXO PowerShell-kommando för att ändra den primära SMTP-adressen för en Microsoft 365-grupp/Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Exempel:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
