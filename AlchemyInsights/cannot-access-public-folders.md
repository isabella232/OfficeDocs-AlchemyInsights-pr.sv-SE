---
title: Det går inte att komma åt gemensamma mappar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959512"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="1454b-102">Outlook kan inte ansluta till gemensamma mappar</span><span class="sxs-lookup"><span data-stu-id="1454b-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="1454b-103">Om åtkomst till gemensamma mappar inte fungerar för få användare kan du prova följande:</span><span class="sxs-lookup"><span data-stu-id="1454b-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="1454b-104">Anslut till EXO PowerShell och konfigurera DefaultPublicFolderMailbox på problem användarkontot så att det matchar ett på ett fungerande användarkonto.</span><span class="sxs-lookup"><span data-stu-id="1454b-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="1454b-105">Exempel:</span><span class="sxs-lookup"><span data-stu-id="1454b-105">Example:</span></span>

<span data-ttu-id="1454b-106">Hämta postlåda WorkingUser | FT DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="1454b-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="1454b-107">Ange postlåda ProblemUser-DefaultPublicFolderMailbox \<värde från föregående kommando></span><span class="sxs-lookup"><span data-stu-id="1454b-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="1454b-108">Vänta minst en timme innan ändringen träder i kraft.</span><span class="sxs-lookup"><span data-stu-id="1454b-108">Wait at least one hour for the change to take effect.</span></span>