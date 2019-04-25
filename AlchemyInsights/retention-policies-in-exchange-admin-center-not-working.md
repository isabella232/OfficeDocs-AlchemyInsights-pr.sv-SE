---
title: Lagringsprinciper i Exchange Admin Center fungerar inte
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: c9061fa728edaab6575a7b1027783e56739a6d14
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371316"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="82aad-102">Lagringsprinciper i Exchange Admin Center</span><span class="sxs-lookup"><span data-stu-id="82aad-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="82aad-103">**Problemet:** Nyskapade eller uppdaterade lagringsprinciper i Exchange Admin Center tillämpa inte för postlådor eller objekt inte har flyttat till arkivet postlåda eller tagits bort.</span><span class="sxs-lookup"><span data-stu-id="82aad-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="82aad-104">**Rotorsaker:**</span><span class="sxs-lookup"><span data-stu-id="82aad-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="82aad-105">Detta kan bero på **Hanterade Mapphanteraren** inte bearbetats av användarens postlåda.</span><span class="sxs-lookup"><span data-stu-id="82aad-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="82aad-106">Hanterade Mapphanteraren försöker bearbeta alla postlådor i organisationen molnbaserad var sjunde dag.</span><span class="sxs-lookup"><span data-stu-id="82aad-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="82aad-107">Om du ändrar taggen bibehålla eller tillämpa en annan bevarandeprincip på en postlåda kan vänta tills mappen hanterade bistå bearbetar postlådan, eller du kan köra cmdlet Start-ManagedFolderAssistant om du vill starta hanteras Mapphanteraren att bearbeta en viss e-postlådan.</span><span class="sxs-lookup"><span data-stu-id="82aad-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="82aad-108">Kör denna cmdlet är användbart för testning eller felsökning av en bevarandeprincip eller loggperioder tagg.</span><span class="sxs-lookup"><span data-stu-id="82aad-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="82aad-109">Mer information finns i [Kör hanterade Mapphanteraren](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="82aad-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="82aad-110">**Lösning:** Kör följande kommando för att starta hanteras Mapphanteraren för en viss postlåda:</span><span class="sxs-lookup"><span data-stu-id="82aad-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="82aad-111">Detta kan också inträffa om **RetentionHold** har **aktiverats** på postlådan.</span><span class="sxs-lookup"><span data-stu-id="82aad-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="82aad-112">Om postlådan har placerats i en RetentionHold, bearbetas inte bevarandeprincipen på postlådan under den tiden.</span><span class="sxs-lookup"><span data-stu-id="82aad-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="82aad-113">För mer information om RetentionHold inställning finns: [Postlåda kvarhållande håller](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="82aad-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="82aad-114">**Lösning:**</span><span class="sxs-lookup"><span data-stu-id="82aad-114">**Solution:**</span></span>
    
  - <span data-ttu-id="82aad-115">Kontrollera status för RetentionHold inställningen för en viss postlåda i [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="82aad-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="82aad-116">Kör följande kommando för att **Inaktivera** RetentionHold för en viss postlåda:</span><span class="sxs-lookup"><span data-stu-id="82aad-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="82aad-117">Kör nu mappen hanterade assistenten igen:</span><span class="sxs-lookup"><span data-stu-id="82aad-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="82aad-118">**Observera:** Om en postlåda är mindre än 10 MB bearbetar hanteras Mapphanteraren inte automatiskt postlådan.</span><span class="sxs-lookup"><span data-stu-id="82aad-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

