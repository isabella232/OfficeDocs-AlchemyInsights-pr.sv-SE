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
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="1e8b0-102">Det går inte att ange primär e-postadress, ändra användarattribut eller ta bort/ta bort en synkroniserad användare</span><span class="sxs-lookup"><span data-stu-id="1e8b0-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="1e8b0-103">Om Active Directory-synkronisering är aktive rad för din miljö kan vissa användare eller objektattribut inte ändras med administrations centret för Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1e8b0-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="1e8b0-104">Om du vill hantera synkroniserade användare och alla dess attribut fullt ut använder du din lokala Active Directory-användare och grupp hanterings konsol (adsiedit. msc).</span><span class="sxs-lookup"><span data-stu-id="1e8b0-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="1e8b0-105">Du kan också ändra enskilda användare eller attribut för synkroniserade användare med hjälp av PowerShell som i följande exempel:</span><span class="sxs-lookup"><span data-stu-id="1e8b0-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span>

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
