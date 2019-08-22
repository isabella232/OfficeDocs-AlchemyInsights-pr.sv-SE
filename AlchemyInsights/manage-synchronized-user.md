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
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="edd2b-102">Det går inte att ange primär e-postadress eller ändra användarattribut</span><span class="sxs-lookup"><span data-stu-id="edd2b-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="edd2b-103">Om katalogsynkronisering är aktiverat för din miljö, kan inte vissa användar- eller attribut ändras med hjälp av Microsoft 365 administratörscenter.</span><span class="sxs-lookup"><span data-stu-id="edd2b-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="edd2b-104">Använd din lokala active directory hanteringskonsolen användare och grupper (adsiedit.msc) för att hantera helt synkroniserade användare och deras attribut.</span><span class="sxs-lookup"><span data-stu-id="edd2b-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="edd2b-105">Du kan också ändra attributen för synkroniserade användare med hjälp av powershell som visas i exemplen gemensamma eller enskilda användare:</span><span class="sxs-lookup"><span data-stu-id="edd2b-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="edd2b-106">Set-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="edd2b-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="edd2b-107">Set-MsolUser - UserPrincipalName ”user@yourdomain.onmicrosoft.com” - DisplayName ”användare” - efternamn ”användare”-rubrik ”chef”-avdelning ”HR”</span><span class="sxs-lookup"><span data-stu-id="edd2b-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="edd2b-108">Ta bort MsolUser - UserPrincipalName ”user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="edd2b-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>