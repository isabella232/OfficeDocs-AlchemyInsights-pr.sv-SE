---
title: Hantera synkroniserade användare
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
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36542035"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Det går inte att ange primär e-postadress eller ändra användarattribut

Om katalogsynkronisering är aktiverat för din miljö, kan inte vissa användar- eller attribut ändras med hjälp av Microsoft 365 administratörscenter.

Använd din lokala active directory hanteringskonsolen användare och grupper (adsiedit.msc) för att hantera helt synkroniserade användare och deras attribut.  

Du kan också ändra attributen för synkroniserade användare med hjälp av powershell som visas i exemplen gemensamma eller enskilda användare: 
- Set-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Set-MsolUser - UserPrincipalName ”user@yourdomain.onmicrosoft.com” - DisplayName ”användare” - efternamn ”användare”-rubrik ”chef”-avdelning ”HR”
- Ta bort MsolUser - UserPrincipalName ”user@yourdomain.onmicrosoft.com