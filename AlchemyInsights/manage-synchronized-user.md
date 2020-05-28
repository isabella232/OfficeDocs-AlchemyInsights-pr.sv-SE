---
title: Hantera synkroniserad användare
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 84e337a7224fdd3c3ab7ad0f61240692fe007d5a
ms.sourcegitcommit: 82af227ac6d075e748e27c4ce6bdcf56628559cb
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/28/2020
ms.locfileid: "44407368"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Det går inte att ange primär e-postadress, ändra användarattribut eller ta bort/ta bort en synkroniserad användare

Om katalogsynkronisering är aktiverat för din miljö kan vissa användar- eller objektattribut inte ändras med hjälp av administrationscentret för Microsoft 365.

Om du vill hantera synkroniserade användare och alla deras attribut fullständigt använder du den lokala active directory-användar- och grupphanteringskonsolen (adsiedit.msc).  

Du kan också ändra enskilda användare eller attribut för synkroniserade användare med powershell, till exempel i de här vanliga exemplen: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
