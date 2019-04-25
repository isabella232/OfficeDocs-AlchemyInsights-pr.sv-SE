---
title: Felsöka Lösenordssynkronisering
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 1320c0fe839337188162824439be6f15f86b6c90
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390465"
---
# <a name="troubleshoot-password-synchronization"></a>Felsöka Lösenordssynkronisering

Felsökning av problem där inga lösenord är synkroniserade med Azure AD Connect version 1.1.614.0 eller senare:
  
1. Öppna en ny Windows PowerShell-session på Azure AD Connect-servern med alternativet **Kör som administratör** . 
    
2. Kör **Ange körningsprincipen RemoteSigned** eller **Ange körningsprincipen obegränsad**. 
    
3. Starta guiden Azure AD Connect.
    
4. Navigera till den ** ytterligare aktiviteter ** anger ** felsöka **, och klicka på **Nästa**. 
    
5. Klicka på **Starta för att starta felsökning** -menyn i PowerShell på sidan felsökning. 
    
6. På huvudmenyn väljer du **Felsöka Lösenordssynkronisering**. 
    
7. Sub-menyn väljer du **Lösenordssynkronisering fungerar inte alls**. 
    
 **Förstå resultaten av felsökning aktivitet**
  
Felsökning uppgift utför följande kontroller:
  
- Kontrollerar att funktionen för synkronisering av lösenord är aktiverat för Azure AD-innehavare.
    
- Verifierar att Azure AD Connect-servern inte är i läget för mellanlagring.
    
- För varje befintlig lokal Active Directory connector (som motsvarar en befintlig Active Directory-skog):
    
- 
  - Kontrollerar att funktionen för synkronisering av lösenord är aktiverat.
    
  - Söker efter lösenord synkronisering heartbeat händelser i händelseloggarna för Windows-program.
    
  - För varje Active Directory-domän under lokal Active Directory-anslutningen:
    
  - Verifierar att domänen kan nås från Azure AD Connect-servern.
    
  - Verifierar att Active Directory DS (AD DS)-konton som används av lokal Active Directory-anslutningen har rätt användarnamn, lösenord och behörigheter som krävs för synkronisering av lösenord.
    
Mer hjälp med felsökning av synkronisering av lösenord, finns i [Felsöka Lösenordssynkronisering med Azure AD Connect-synkronisering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  

