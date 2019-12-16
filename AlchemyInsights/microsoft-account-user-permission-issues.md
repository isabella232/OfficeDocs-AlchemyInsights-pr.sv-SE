---
title: Felsöka problem-användare hittades inte i katalogen
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0f1e427801107109e31486a4d300f53084880caf
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054828"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="05336-102">Felsöka problem-användare hittades inte i katalogen</span><span class="sxs-lookup"><span data-stu-id="05336-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="05336-103">Om användare får felmeddelandet "användaren kan inte hittas" i katalogen, vänligen försök igen där problemtypen är användaren inte i katalogen.</span><span class="sxs-lookup"><span data-stu-id="05336-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="05336-104">Följande steg kan slutföras för att felsöka problemet.</span><span class="sxs-lookup"><span data-stu-id="05336-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="05336-105">Se till att kontot som accepterade e-postinbjudan är samma konto som används för att logga in senare.</span><span class="sxs-lookup"><span data-stu-id="05336-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="05336-106">Kontrollera att användaren använder samma konto för att acceptera inbjudan och logga in på webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="05336-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="05336-107">Mer information finns i hantera [alias för ditt Microsoft-konto</a> för att hantera Office 365-inloggningen](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="05336-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="05336-108">Bläddra till varje plats (er) där användaren får felet.</span><span class="sxs-lookup"><span data-stu-id="05336-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="05336-109">Lägg till "/_layouts/15/People.aspx/MembershipGroupId = 0" (inom dubbla citationstecken) i slutet av webbplatsens URL.</span><span class="sxs-lookup"><span data-stu-id="05336-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="05336-110">Exempel: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="05336-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="05336-111">Markera användaren i listan.</span><span class="sxs-lookup"><span data-stu-id="05336-111">Select the user from the list.</span></span>

- <span data-ttu-id="05336-112">Klicka på **ta bort användarbehörigheter** från menyfliksområdet.</span><span class="sxs-lookup"><span data-stu-id="05336-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="05336-113">Lägg tillbaka användaren och skicka inbjudan till användaren igen.</span><span class="sxs-lookup"><span data-stu-id="05336-113">Add back the User and Resend the invite to the user.</span></span>

