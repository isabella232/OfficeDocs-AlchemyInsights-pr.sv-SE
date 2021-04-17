---
title: Hantera synkroniserad användare
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823985"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Det går inte att ange en primär e-postadress, ändra användarattribut eller ta bort en synkroniserad användare

Om katalogsynkronisering är aktiverad för din miljö kan vissa användar- eller objektattribut inte ändras med hjälp av administrationscentret för Microsoft 365.

Om du vill hantera synkroniserade användare och alla deras attribut fullt ut använder du den lokala konsolen för hantering av Active Directory-användare och grupper (adsiedit.msc).  

Du kan också ändra enskilda användare eller attribut för synkroniserade användare med powershell, som i de här vanliga exemplen:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
