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
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996648"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook kan inte ansluta till gemensamma mappar

Om den gemensamma mappåtkomsten inte fungerar för vissa användare kan du prova följande:

Anslut till EXO PowerShell och konfigurera parametern DefaultPublicFolderMailbox för det aktuella användarkontot så att de matchar parametern i ett fungerande användarkonto.

Exempel:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Vänta i minst en timme innan ändringen verkställs.

Om problemet kvarstår följer du den [här proceduren för att](https://aka.ms/pfcte) felsöka åtkomstproblem med gemensamma mappar med hjälp Outlook.
 
**Så här styr du vilka användare som kan komma åt gemensamma mappar Outlook:**

1.  Använd Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true eller $false  
      
    $true: Tillåt användare att använda gemensamma mappar i Outlook  
      
    $false: Förhindra att användare kommer åt gemensamma mappar i Outlook. Det här är standardvärdet.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Obs!** Den här proceduren kan bara styra anslutningar Outlook skrivbordet för Windows klienter. En användare kan fortsätta komma åt gemensamma mappar med hjälp av OWA eller Outlook för Mac.
 
Mer information finns i [Vi presenterar stöd för kontrollerade anslutningar till gemensamma mappar i Outlook.](https://aka.ms/controlpf)