---
title: Flytta e-postmeddelanden till arkivet postlåda
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29492335"
---
<span data-ttu-id="24104-p101">Problem Arkivera objekt med Arkivera postlådan. Kontrollera att du har utfört följande åtgärder:</span><span class="sxs-lookup"><span data-stu-id="24104-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="24104-p102">Bekräfta att en **Arkivera postlåda** har aktiverats. Om du inte följer instruktionerna i [denna artikel](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) för att arkivera postlåda.</span><span class="sxs-lookup"><span data-stu-id="24104-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="24104-106">I Exchange Admin Center, Välj **Kvarhållande taggar** under **Regelefterlevnadshantering**, skapa en **tagg för bevarande** med åtgärden **Flytta till Arkiv** som innehåller önskad **Kvarhållande ålder**.</span><span class="sxs-lookup"><span data-stu-id="24104-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="24104-107">Markera **Lagringsprinciper**i Exchange Admin Center, och skapa en **Princip för loggperiod** till din **Flytta till arkivet** innehållen tagg till principen.</span><span class="sxs-lookup"><span data-stu-id="24104-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="24104-p103">[Tilldela en princip för loggperiod](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) till användarens postlåda. Samma princip tillämpas på både det **primärt** och **Arkivera** postlåda.</span><span class="sxs-lookup"><span data-stu-id="24104-p103">[Assign the Retention Policy](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="24104-p104">Användarens postlåda ska nu ha en arkiveringsprincip för att flytta objekt till arkivet postlåda. Det kan vara nödvändigt att tvinga den hanterade mappen assistenten (MFA) att köra och använda de nya inställningarna till användarens postlåda. Kör följande kommando när [anslutet till EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) att starta hanteras Mapphanteraren för en viss postlåda:</span><span class="sxs-lookup"><span data-stu-id="24104-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="24104-113">Om du vill ha mer information om att konfigurera en arkiveringsprincip finns i avsnittet [Konfigurera en arkivera och ta bort princip för postlådor](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="24104-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

