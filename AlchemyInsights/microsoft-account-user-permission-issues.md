---
title: Felsöka problem-användare hittades inte i katalogen
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754210"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="b29c3-102">Felsöka problem-användare hittades inte i katalogen</span><span class="sxs-lookup"><span data-stu-id="b29c3-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="b29c3-103">Om användare får felmeddelandet "användaren kan inte hittas" i katalogen.</span><span class="sxs-lookup"><span data-stu-id="b29c3-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="b29c3-104">Försök igen där problemtypen är användare inte i katalogen.</span><span class="sxs-lookup"><span data-stu-id="b29c3-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="b29c3-105">Följande steg kan slutföras för att felsöka problemet.</span><span class="sxs-lookup"><span data-stu-id="b29c3-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="b29c3-106">Se till att kontot som accepterade e-postinbjudan är samma konto som används för att logga in senare.</span><span class="sxs-lookup"><span data-stu-id="b29c3-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="b29c3-107">Kontrollera att användaren använder samma konto för att acceptera inbjudan och logga in på webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="b29c3-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="b29c3-108">Mer information finns i hantera [alias för ditt Microsoft-konto</a> för att hantera Office 365-inloggningen](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="b29c3-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="b29c3-109">Bläddra till varje plats (er) där användaren får felet.</span><span class="sxs-lookup"><span data-stu-id="b29c3-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="b29c3-110">Lägg till "/_layouts/15/People.aspx/MembershipGroupId = 0" (inom dubbla citationstecken) i slutet av webbplatsens URL.</span><span class="sxs-lookup"><span data-stu-id="b29c3-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="b29c3-111">Exempel: https://_ lt _ "contoso">. SharePoint. com/_ Layouts/15/People. aspx/membershipGroupId = 0.</span><span class="sxs-lookup"><span data-stu-id="b29c3-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="b29c3-112">Markera användaren i listan.</span><span class="sxs-lookup"><span data-stu-id="b29c3-112">Select the user from the list.</span></span>

- <span data-ttu-id="b29c3-113">Klicka på **ta bort användarbehörigheter** från menyfliksområdet.</span><span class="sxs-lookup"><span data-stu-id="b29c3-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="b29c3-114">Lägg tillbaka användaren och skicka inbjudan till användaren igen.</span><span class="sxs-lookup"><span data-stu-id="b29c3-114">Add back the User and Resend the invite to the user.</span></span>

