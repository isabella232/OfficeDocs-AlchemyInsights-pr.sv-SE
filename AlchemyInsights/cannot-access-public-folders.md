---
title: Kan inte komma åt gemensamma mappar
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
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341421"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="6e2f2-102">Det går inte att ansluta till gemensamma mappar i Outlook</span><span class="sxs-lookup"><span data-stu-id="6e2f2-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="6e2f2-103">Om det inte går att använda offentlig mappåtkomst för vissa användare kan du prova följande:</span><span class="sxs-lookup"><span data-stu-id="6e2f2-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="6e2f2-104">Anslut till EXO PowerShell och konfigurera parametern DefaultPublicFolderMailbox i användar kontot för problem för att matcha parametern på ett fungerande användar konto.</span><span class="sxs-lookup"><span data-stu-id="6e2f2-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="6e2f2-105">Exempel:</span><span class="sxs-lookup"><span data-stu-id="6e2f2-105">Example:</span></span>

<span data-ttu-id="6e2f2-106">Get-Mailbox WorkingUser | FT-DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="6e2f2-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="6e2f2-107">Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="6e2f2-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="6e2f2-108">Vänta i minst en timme innan ändringen börjar gälla.</span><span class="sxs-lookup"><span data-stu-id="6e2f2-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="6e2f2-109">Om problemet kvarstår följer du [den här proceduren](https://aka.ms/pfcte) för att felsöka åtkomst problem för offentliga mappar med hjälp av Outlook.</span><span class="sxs-lookup"><span data-stu-id="6e2f2-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="6e2f2-110">**Så här kontrollerar du vilka användare som kan komma åt gemensamma mappar med hjälp av Outlook**:</span><span class="sxs-lookup"><span data-stu-id="6e2f2-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="6e2f2-111">Använd set-CASMailbox cmdlethttps <mailboxname> -PublicFolderClientAccess $true eller $false</span><span class="sxs-lookup"><span data-stu-id="6e2f2-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="6e2f2-112">$true: Tillåt användare att komma åt gemensamma mappar i Outlook</span><span class="sxs-lookup"><span data-stu-id="6e2f2-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="6e2f2-113">$false: förhindra användares åtkomst till gemensamma mappar i Outlook.</span><span class="sxs-lookup"><span data-stu-id="6e2f2-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="6e2f2-114">Det här är standardvärdet.</span><span class="sxs-lookup"><span data-stu-id="6e2f2-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="6e2f2-115">Set-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="6e2f2-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="6e2f2-116">**Obs!** Den här proceduren kan endast styra anslutningar med Outlook Desktop för Windows-klienter.</span><span class="sxs-lookup"><span data-stu-id="6e2f2-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="6e2f2-117">En användare kan fortsätta att komma åt gemensamma mappar med OWA eller Outlook för Mac.</span><span class="sxs-lookup"><span data-stu-id="6e2f2-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="6e2f2-118">Mer information finns i artikeln [om stöd för kontrollerade anslutningar till gemensamma mappar i Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="6e2f2-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>