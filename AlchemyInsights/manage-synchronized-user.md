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
ms.openlocfilehash: 53c188f6c6ab93bcc6f87d95717dc0d24d492bb7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47777695"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Det går inte att ange primär e-postadress, ändra användarattribut eller ta bort/ta bort en synkroniserad användare

Om Active Directory-synkronisering är aktive rad för din miljö kan vissa användare eller objektattribut inte ändras med administrations centret för Microsoft 365.

Om du vill hantera synkroniserade användare och alla dess attribut fullt ut använder du din lokala Active Directory-användare och grupp hanterings konsol (adsiedit. msc).  

Du kan också ändra enskilda användare eller attribut för synkroniserade användare med hjälp av PowerShell som i följande exempel: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
