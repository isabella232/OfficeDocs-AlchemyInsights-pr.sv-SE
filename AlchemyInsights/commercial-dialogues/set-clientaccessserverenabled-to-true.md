---
title: Ange ClientAccessServerEnabled till True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: fc953813a94c9ed3226f81f776d6085e12a6cafc
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320374"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Ange ClientAccessServerEnabled till True

Om du inte kan öppna ett krypterat e-postmeddelande och i stället ser en **bifogad rpms gör** du så här:

1. Ansluta till Exchange Online PowerShell.

    **Obs!** Om du vill ansluta Exchange Online PowerShell måste du logga in med en global administratör Exchange administratörskonto.

   a. Öppna Windows PowerShell och kör sedan följande kommando:`$UserCredential = Get-Credential`
   b. I dialogrutan **Windows PowerShell Begäran om autentiseringsuppgifter anger** du ditt arbets- eller skolkonto och lösenord, c. Klicka på **OK**. 

2. Kör följande kommando för att skapa en ny session:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Kör följande kommando:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Kommandot `Get-IRMConfiguration` Kör.

4. Kontrollera **inställningen ClientAccessServerEnabled.** 

    a. Om **inställningen ClientAccessServerEnabled** är inställd **på False** kör du följande cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

**Tips:** Stäng alltid PowerShell-sessionen med följande kommando: `Remove-PSSession $Session`

Mer information finns i [Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

