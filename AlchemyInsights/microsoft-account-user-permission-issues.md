---
title: Felsöka problem – användare finns inte i katalogen
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725425"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="6cf78-102">Felsöka problem – användare finns inte i katalogen</span><span class="sxs-lookup"><span data-stu-id="6cf78-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="6cf78-103">Om det visas ett fel meddelande om att det inte går att hitta användaren i katalogen, försök igen där ärende typen inte finns i katalogen.</span><span class="sxs-lookup"><span data-stu-id="6cf78-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="6cf78-104">Följ de här anvisningarna för att felsöka problemet.</span><span class="sxs-lookup"><span data-stu-id="6cf78-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="6cf78-105">Kontrol lera att kontot som godkände e-postinbjudanen är samma konto som används för att logga in senare.</span><span class="sxs-lookup"><span data-stu-id="6cf78-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="6cf78-106">Kontrol lera att användaren använder samma konto för att acceptera inbjudan och logga in på webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="6cf78-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="6cf78-107">Mer information finns i [hur du hanterar alias för ditt Microsoft-konto </a> för att hantera Microsoft 365-inloggningen](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="6cf78-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="6cf78-108">Bläddra till varje webbplats som användaren får felet från.</span><span class="sxs-lookup"><span data-stu-id="6cf78-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="6cf78-109">Lägg till "/_layouts/15/People.aspx/MembershipGroupId = 0" (inom dubbel citat tecken) i slutet av webbplats-URL: en.</span><span class="sxs-lookup"><span data-stu-id="6cf78-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="6cf78-110">Exempel: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="6cf78-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="6cf78-111">Välj användaren i listan.</span><span class="sxs-lookup"><span data-stu-id="6cf78-111">Select the user from the list.</span></span>

- <span data-ttu-id="6cf78-112">Klicka på **ta bort användar behörigheter** från menyfliksområdet.</span><span class="sxs-lookup"><span data-stu-id="6cf78-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="6cf78-113">Lägg till användaren tillbaka och skicka inbjudan till användaren igen.</span><span class="sxs-lookup"><span data-stu-id="6cf78-113">Add back the User and Resend the invite to the user.</span></span>

