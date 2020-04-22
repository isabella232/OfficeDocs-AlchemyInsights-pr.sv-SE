---
title: Felsöka problem - Användaren hittades inte i katalogen
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702756"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="668ca-102">Felsöka problem - Användaren hittades inte i katalogen</span><span class="sxs-lookup"><span data-stu-id="668ca-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="668ca-103">Om användarna får felmeddelandet "användaren kan inte hittas" i katalogen, försök igen där ärendetypen är Användaren inte i katalogen.</span><span class="sxs-lookup"><span data-stu-id="668ca-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="668ca-104">Följande steg kan slutföras för att felsöka problemet.</span><span class="sxs-lookup"><span data-stu-id="668ca-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="668ca-105">Kontrollera att kontot som accepterade e-postbjudan är samma konto som används för att logga in senare.</span><span class="sxs-lookup"><span data-stu-id="668ca-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="668ca-106">Kontrollera att användaren använder samma konto för att acceptera inbjudan och logga in på webbplatsen.</span><span class="sxs-lookup"><span data-stu-id="668ca-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="668ca-107">Mer information finns i [Så här hanterar</a> du alias för ditt Microsoft-konto för att hantera Microsoft 365-inloggningen](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="668ca-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="668ca-108">Bläddra till varje webbplats där användaren tar emot felet.</span><span class="sxs-lookup"><span data-stu-id="668ca-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="668ca-109">Lägg till "/_layouts/15/people.aspx/membershipgroupid=0" (inom dubbelcitat) i slutet av webbadressen.</span><span class="sxs-lookup"><span data-stu-id="668ca-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="668ca-110">Exempel: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="668ca-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="668ca-111">Välj användaren i listan.</span><span class="sxs-lookup"><span data-stu-id="668ca-111">Select the user from the list.</span></span>

- <span data-ttu-id="668ca-112">Klicka på **Ta bort användarbehörigheter** från menyfliksområdet.</span><span class="sxs-lookup"><span data-stu-id="668ca-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="668ca-113">Lägg tillbaka användaren och skicka inbjudan igen till användaren.</span><span class="sxs-lookup"><span data-stu-id="668ca-113">Add back the User and Resend the invite to the user.</span></span>

