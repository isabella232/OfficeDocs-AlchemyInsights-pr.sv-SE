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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891767"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="9fefd-102">Det går inte att ansluta till gemensamma mappar</span><span class="sxs-lookup"><span data-stu-id="9fefd-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="9fefd-103">Om åtkomst till gemensamma mappar inte fungerar för vissa användare kan du prova följande:</span><span class="sxs-lookup"><span data-stu-id="9fefd-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="9fefd-104">Anslut till EXO PowerShell och konfigurera parametern DefaultPublicFolderMailbox på problemet användarkontot så att den matchar parametern på ett fungerande användarkonto.</span><span class="sxs-lookup"><span data-stu-id="9fefd-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="9fefd-105">Exempel:</span><span class="sxs-lookup"><span data-stu-id="9fefd-105">Example:</span></span>

<span data-ttu-id="9fefd-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="9fefd-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="9fefd-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox-värde \<från föregående kommando></span><span class="sxs-lookup"><span data-stu-id="9fefd-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="9fefd-108">Vänta minst en timme innan ändringen börjar gälla.</span><span class="sxs-lookup"><span data-stu-id="9fefd-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="9fefd-109">Om problemet kvarstår följer du [den här proceduren](https://aka.ms/pfcte) för att felsöka problem med åtkomst till gemensamma mappar med Outlook.</span><span class="sxs-lookup"><span data-stu-id="9fefd-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>