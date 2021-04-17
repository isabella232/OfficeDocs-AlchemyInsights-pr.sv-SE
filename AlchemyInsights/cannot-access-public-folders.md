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
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook kan inte ansluta till gemensamma mappar

Om den gemensamma mappåtkomsten inte fungerar för vissa användare kan du prova följande:

Anslut till EXO PowerShell och konfigurera parametern DefaultPublicFolderMailbox för det problemanvändarkonto som matchar parametern på ett fungerande användarkonto.

Exempel:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Vänta i minst en timme innan ändringen verkställs.

Om problemet kvarstår följer du den här [proceduren för att](https://aka.ms/pfcte) felsöka problem med åtkomst till gemensamma mappar med Hjälp av Outlook.
 
**Så här styr du vilka användare som kan komma åt gemensamma mappar i Outlook:**

1.  Använd Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true eller $false  
      
    $true: Tillåta användare åtkomst till gemensamma mappar i Outlook  
      
    $false: Förhindra att användare kommer åt gemensamma mappar i Outlook. Det här är standardvärdet.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Obs!** Den här proceduren kan bara styra anslutningar med Outlook för Windows-klienter. En användare kan fortsätta komma åt gemensamma mappar med hjälp av OWA eller Outlook för Mac.
 
Mer information finns i [Vi presenterar stöd för kontrollerade anslutningar till gemensamma mappar i Outlook.](https://aka.ms/controlpf)