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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749732"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a><span data-ttu-id="1e645-102">Använda Exchange Online PowerShell för att aktivera DKIM för en viss domän</span><span class="sxs-lookup"><span data-stu-id="1e645-102">Use Exchange Online PowerShell to enable DKIM for a specific domain</span></span>

<span data-ttu-id="1e645-103">Om du inte kan skapa DKIM DNS-posterna i administrationscentret kan du prova att använda Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="1e645-103">If you can't create the DKIM DNS records in the admin center, try using Exchange Online PowerShell.</span></span> 

<span data-ttu-id="1e645-104">Så här skapar du en DKIM DNS-post med Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="1e645-104">To create a DKIM DNS record using Exchange Online PowerShell, perform the following steps:</span></span>

1. <span data-ttu-id="1e645-105">Öppna Windows PowerShell som administratör och kör följande kommandon i den ordning som beskrivs:</span><span class="sxs-lookup"><span data-stu-id="1e645-105">Open Windows PowerShell as an administrator and run the following commands in the described sequence:</span></span>

    <span data-ttu-id="1e645-106">a.</span><span class="sxs-lookup"><span data-stu-id="1e645-106">a.</span></span> `$UserCredential = Get-Credential`

    <span data-ttu-id="1e645-107">b.</span><span class="sxs-lookup"><span data-stu-id="1e645-107">b.</span></span> `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="1e645-108">c.</span><span class="sxs-lookup"><span data-stu-id="1e645-108">c.</span></span> `Import-PSSession $Session -DisableNameChecking`
    
<span data-ttu-id="1e645-109">Om du har problem med att ansluta till Exchange Online PowerShell kan du [gå till Ansluta till Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="1e645-109">If you have trouble connecting to Exchange Online PowerShell, see [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="1e645-110">När du är ansluten till Exchange Online PowerShell kör du följande kommando:</span><span class="sxs-lookup"><span data-stu-id="1e645-110">Once you're connected to Exchange Online PowerShell, run the following command:</span></span>

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. <span data-ttu-id="1e645-111">När kommandot ovan har körts kör du följande kommando för att avsluta Exchange Online PowerShell-sessionen:</span><span class="sxs-lookup"><span data-stu-id="1e645-111">Once the above command has been successfully executed, run the following command to terminate the Exchange Online PowerShell session:</span></span>

    `Remove-PSSession $Session` 



