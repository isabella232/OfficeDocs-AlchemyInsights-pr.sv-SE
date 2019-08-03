---
title: Felsökning - användare som inte finns i katalogen
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0909edc581c811fdc4683b004e0df0adbac88d1c
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/26/2019
ms.locfileid: "35249931"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="f4a58-102">Felsökning - användare som inte finns i katalogen</span><span class="sxs-lookup"><span data-stu-id="f4a58-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="f4a58-103">Om användarna får fel meddelande ”användaren kan inte hittas” i katalogen.</span><span class="sxs-lookup"><span data-stu-id="f4a58-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="f4a58-104">Försök igen om den typ av fråga användaren inte är i katalogen.</span><span class="sxs-lookup"><span data-stu-id="f4a58-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="f4a58-105">Följande åtgärder kan utföras för felsökning av problemet.</span><span class="sxs-lookup"><span data-stu-id="f4a58-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="f4a58-106">Se till att det konto som har accepterat postinbjudan e-är samma konto som används för att logga in senare.</span><span class="sxs-lookup"><span data-stu-id="f4a58-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="f4a58-107">Kontrollera att användaren använder samma konto för att acceptera inbjudan och logga in på webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="f4a58-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="f4a58-108">Mer information finns i [hur du hanterar alias för ditt Microsoft-konto</a> att hantera Office 365-inloggning](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="f4a58-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="f4a58-109">Bläddra till varje plats där användaren får felet.</span><span class="sxs-lookup"><span data-stu-id="f4a58-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="f4a58-110">Lägga till ”/ _layouts/15/people.aspx/membershipgroupid=0” (inom citattecken) i slutet av webbplatsens URL.</span><span class="sxs-lookup"><span data-stu-id="f4a58-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="f4a58-111">Exempel: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="f4a58-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="f4a58-112">Markera användaren i listan.</span><span class="sxs-lookup"><span data-stu-id="f4a58-112">Select the user from the list.</span></span>

- <span data-ttu-id="f4a58-113">Klicka på **Ta bort användarbehörigheter** från menyfliken.</span><span class="sxs-lookup"><span data-stu-id="f4a58-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="f4a58-114">Lägg tillbaka till användaren och skicka inbjudan till användaren.</span><span class="sxs-lookup"><span data-stu-id="f4a58-114">Add back the User and Resend the invite to the user.</span></span>

