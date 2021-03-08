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
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525960"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="1c452-102">Ange ClientAccessServerEnabled till True</span><span class="sxs-lookup"><span data-stu-id="1c452-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="1c452-103">Om du inte kan öppna ett krypterat e-postmeddelande och i stället ser en **rpmsg-bilaga** gör du så här:</span><span class="sxs-lookup"><span data-stu-id="1c452-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="1c452-104">Ansluta till Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="1c452-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="1c452-105">Om du vill ansluta till Exchange Online PowerShell måste du logga in med en global administratör eller ett Exchange-administratörskonto.</span><span class="sxs-lookup"><span data-stu-id="1c452-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="1c452-106">a.</span><span class="sxs-lookup"><span data-stu-id="1c452-106">a.</span></span> <span data-ttu-id="1c452-107">Öppna Windows PowerShell och kör sedan följande kommando: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="1c452-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="1c452-108">b.</span><span class="sxs-lookup"><span data-stu-id="1c452-108">b.</span></span> <span data-ttu-id="1c452-109">I dialogrutan **Autentiseringsbegäran för Windows PowerShell** anger du ditt arbets- eller skolkonto och lösenord, c.</span><span class="sxs-lookup"><span data-stu-id="1c452-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="1c452-110">Klicka på **OK**.</span><span class="sxs-lookup"><span data-stu-id="1c452-110">Click **OK**.</span></span> 

2. <span data-ttu-id="1c452-111">Kör följande kommando för att skapa en ny session:</span><span class="sxs-lookup"><span data-stu-id="1c452-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="1c452-112">a.</span><span class="sxs-lookup"><span data-stu-id="1c452-112">a.</span></span> <span data-ttu-id="1c452-113">Kör följande kommando:</span><span class="sxs-lookup"><span data-stu-id="1c452-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="1c452-114">Kommandot `Get-IRMConfiguration` Kör.</span><span class="sxs-lookup"><span data-stu-id="1c452-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="1c452-115">Kontrollera **inställningen ClientAccessServerEnabled.**</span><span class="sxs-lookup"><span data-stu-id="1c452-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="1c452-116">a.</span><span class="sxs-lookup"><span data-stu-id="1c452-116">a.</span></span> <span data-ttu-id="1c452-117">Om **inställningen ClientAccessServerEnabled** är inställd **på False** kör du följande cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="1c452-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="1c452-118">Stäng alltid PowerShell-sessionen med följande kommando: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="1c452-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="1c452-119">Mer information finns i [Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="1c452-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

