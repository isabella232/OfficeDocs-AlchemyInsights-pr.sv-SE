---
title: Hantera synkroniserad användare
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
- "9000609"
- "2444"
ms.openlocfilehash: 7bf7d3f00308ff6bc973cd52e09ca51c5fd0f45b
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451418"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Det går inte att ange primär e-postadress, ändra användarattribut eller ta bort/ta bort en synkroniserad användare

Om Active Directory-synkronisering är aktive rad för din miljö kan vissa användare eller objektattribut inte ändras med administrations centret för Microsoft 365.

Om du vill hantera synkroniserade användare och alla dess attribut fullt ut använder du din lokala Active Directory-användare och grupp hanterings konsol (adsiedit. msc).  

Du kan också ändra enskilda användare eller attribut för synkroniserade användare med hjälp av PowerShell som i följande exempel:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
