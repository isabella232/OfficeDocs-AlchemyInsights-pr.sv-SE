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
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380523"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Det går inte att ange primär e-postadress eller ändra användarattribut

Om katalogsynkronisering är aktiverat för din miljö ändras inte vissa attribut för användar- eller med hjälp av Admin Center.
Använd din lokala active directory hanteringskonsolen användare och grupper (adsiedit.msc) för att hantera helt synkroniserade användare och deras attribut.  

Du kan också ändra attributen för synkroniserade användare med hjälp av powershell som visas i exemplen gemensamma eller enskilda användare: 
- Set-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Set-MsolUser - UserPrincipalName ”user@yourdomain.onmicrosoft.com” - DisplayName ”användare” - efternamn ”användare”-rubrik ”chef”-avdelning ”HR”
- Ta bort MsolUser - UserPrincipalName ”user@yourdomain.onmicrosoft.com