---
title: Använda Exchange Online PowerShell för att aktivera DKIM för en viss domän
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525245"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Använda Exchange Online PowerShell för att aktivera DKIM för en viss domän

Om du inte kan skapa DKIM DNS-posterna i administrationscentret kan du prova att använda Exchange Online PowerShell. 

Så här skapar du en DKIM DNS-post med Exchange Online PowerShell:

1. Öppna Windows PowerShell som administratör och kör följande kommandon i den ordning som beskrivs:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Om du har problem med att ansluta till Exchange Online PowerShell kan du [gå till Ansluta till Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. När du är ansluten till Exchange Online PowerShell kör du följande kommando:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. När kommandot ovan har körts kör du följande kommando för att avsluta Exchange Online PowerShell-sessionen:

    `Remove-PSSession $Session` 



