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
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749975"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Ange ClientAccessServerEnabled till True

Om du inte kan öppna ett krypterat e-postmeddelande och i stället ser en **bifogad rpms gör** du så här:

1. Ansluta till Exchange Online PowerShell.

> [!NOTE]
> Om du vill ansluta till Exchange Online PowerShell måste du logga in med en global administratör eller ett Exchange-administratörskonto.

   a. Öppna Windows PowerShell och kör sedan följande kommando: `$UserCredential = Get-Credential`
b. I dialogrutan **Begäran om autentiseringsuppgifter för Windows PowerShell** anger du ditt arbets- eller skolkonto och ditt lösenord, c. Klicka på **OK**. 

2. Kör följande kommando för att skapa en ny session:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Kör följande kommando:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Kommandot `Get-IRMConfiguration` Kör.

4. Kontrollera **inställningen ClientAccessServerEnabled.** 

    a. Om **inställningen ClientAccessServerEnabled** är inställd **på False** kör du följande cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Stäng alltid PowerShell-sessionen med följande kommando: `Remove-PSSession $Session`

Mer information finns i [Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

