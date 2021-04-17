---
title: Det går inte att komma åt gemensamma mappar
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819530"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="4e602-102">Outlook kan inte ansluta till gemensamma mappar</span><span class="sxs-lookup"><span data-stu-id="4e602-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="4e602-103">Om den gemensamma mappåtkomsten inte fungerar för vissa användare kan du prova följande:</span><span class="sxs-lookup"><span data-stu-id="4e602-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="4e602-104">Anslut till EXO PowerShell och konfigurera parametern DefaultPublicFolderMailbox för det problemanvändarkonto som matchar parametern på ett fungerande användarkonto.</span><span class="sxs-lookup"><span data-stu-id="4e602-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="4e602-105">Exempel:</span><span class="sxs-lookup"><span data-stu-id="4e602-105">Example:</span></span>

<span data-ttu-id="4e602-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="4e602-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="4e602-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="4e602-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="4e602-108">Vänta i minst en timme innan ändringen verkställs.</span><span class="sxs-lookup"><span data-stu-id="4e602-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="4e602-109">Om problemet kvarstår följer du den här [proceduren för att](https://aka.ms/pfcte) felsöka problem med åtkomst till gemensamma mappar med Hjälp av Outlook.</span><span class="sxs-lookup"><span data-stu-id="4e602-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="4e602-110">**Så här styr du vilka användare som kan komma åt gemensamma mappar i Outlook:**</span><span class="sxs-lookup"><span data-stu-id="4e602-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="4e602-111">Använd Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true eller $false</span><span class="sxs-lookup"><span data-stu-id="4e602-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="4e602-112">$true: Tillåta användare åtkomst till gemensamma mappar i Outlook</span><span class="sxs-lookup"><span data-stu-id="4e602-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="4e602-113">$false: Förhindra att användare kommer åt gemensamma mappar i Outlook.</span><span class="sxs-lookup"><span data-stu-id="4e602-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="4e602-114">Det här är standardvärdet.</span><span class="sxs-lookup"><span data-stu-id="4e602-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="4e602-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="4e602-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="4e602-116">**Obs!** Den här proceduren kan bara styra anslutningar med Outlook för Windows-klienter.</span><span class="sxs-lookup"><span data-stu-id="4e602-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="4e602-117">En användare kan fortsätta komma åt gemensamma mappar med hjälp av OWA eller Outlook för Mac.</span><span class="sxs-lookup"><span data-stu-id="4e602-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="4e602-118">Mer information finns i [Vi presenterar stöd för kontrollerade anslutningar till gemensamma mappar i Outlook.](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="4e602-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>