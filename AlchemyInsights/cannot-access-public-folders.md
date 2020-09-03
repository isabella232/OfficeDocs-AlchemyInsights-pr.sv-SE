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
# <a name="outlook-cannot-connect-to-public-folders"></a>Det går inte att ansluta till gemensamma mappar i Outlook

Om det inte går att använda offentlig mappåtkomst för vissa användare kan du prova följande:

Anslut till EXO PowerShell och konfigurera parametern DefaultPublicFolderMailbox i användar kontot för problem för att matcha parametern på ett fungerande användar konto.

Exempel:

Get-Mailbox WorkingUser | FT-DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

Vänta i minst en timme innan ändringen börjar gälla.

Om problemet kvarstår följer du [den här proceduren](https://aka.ms/pfcte) för att felsöka åtkomst problem för offentliga mappar med hjälp av Outlook.
 
**Så här kontrollerar du vilka användare som kan komma åt gemensamma mappar med hjälp av Outlook**:

1.  Använd set-CASMailbox cmdlethttps <mailboxname> -PublicFolderClientAccess $true eller $false  
      
    $true: Tillåt användare att komma åt gemensamma mappar i Outlook  
      
    $false: förhindra användares åtkomst till gemensamma mappar i Outlook. Det här är standardvärdet.  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Obs!** Den här proceduren kan endast styra anslutningar med Outlook Desktop för Windows-klienter. En användare kan fortsätta att komma åt gemensamma mappar med OWA eller Outlook för Mac.
 
Mer information finns i artikeln [om stöd för kontrollerade anslutningar till gemensamma mappar i Outlook](https://aka.ms/controlpf).