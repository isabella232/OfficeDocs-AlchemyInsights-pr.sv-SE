---
title: Lagringsprinciper i Exchange Admin Center fungerar inte
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 5d7b62546397c13b37540e8797b31123b2880280
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551361"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="b7cf4-102">Lagringsprinciper i Exchange Admin Center</span><span class="sxs-lookup"><span data-stu-id="b7cf4-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="b7cf4-103">**Problemet:** Nyskapade eller uppdaterade lagringsprinciper i Exchange Admin Center tillämpa inte för postlådor eller objekt inte har flyttat till arkivet postlåda eller tagits bort.</span><span class="sxs-lookup"><span data-stu-id="b7cf4-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="b7cf4-104">**Rotorsaker:**</span><span class="sxs-lookup"><span data-stu-id="b7cf4-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="b7cf4-105">Detta kan bero på **Hanterade Mapphanteraren** inte bearbetats av användarens postlåda.</span><span class="sxs-lookup"><span data-stu-id="b7cf4-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="b7cf4-106">Hanterade Mapphanteraren försöker bearbeta alla postlådor i organisationen molnbaserad var sjunde dag.</span><span class="sxs-lookup"><span data-stu-id="b7cf4-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="b7cf4-107">Om du ändrar taggen bibehålla eller tillämpa en annan bevarandeprincip på en postlåda kan vänta tills mappen hanterade bistå bearbetar postlådan, eller du kan köra cmdlet Start-ManagedFolderAssistant om du vill starta hanteras Mapphanteraren att bearbeta en viss e-postlådan.</span><span class="sxs-lookup"><span data-stu-id="b7cf4-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="b7cf4-108">Kör denna cmdlet är användbart för testning eller felsökning av en bevarandeprincip eller loggperioder tagg.</span><span class="sxs-lookup"><span data-stu-id="b7cf4-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="b7cf4-109">Mer information finns i [Kör hanterade Mapphanteraren](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="b7cf4-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="b7cf4-110">**Lösning:** Kör följande kommando för att starta hanteras Mapphanteraren för en viss postlåda:</span><span class="sxs-lookup"><span data-stu-id="b7cf4-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="b7cf4-111">Detta kan också inträffa om **RetentionHold** har **aktiverats** på postlådan.</span><span class="sxs-lookup"><span data-stu-id="b7cf4-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="b7cf4-112">Om postlådan har placerats i en RetentionHold, bearbetas inte bevarandeprincipen på postlådan under den tiden.</span><span class="sxs-lookup"><span data-stu-id="b7cf4-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="b7cf4-113">För mer information om RetentionHold inställning finns: [Postlåda kvarhållande håller](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="b7cf4-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="b7cf4-114">**Lösning:**</span><span class="sxs-lookup"><span data-stu-id="b7cf4-114">**Solution:**</span></span>
    
  - <span data-ttu-id="b7cf4-115">Kontrollera status för RetentionHold inställningen för en viss postlåda i [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="b7cf4-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="b7cf4-116">Kör följande kommando för att **Inaktivera** RetentionHold för en viss postlåda:</span><span class="sxs-lookup"><span data-stu-id="b7cf4-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="b7cf4-117">Kör nu mappen hanterade assistenten igen:</span><span class="sxs-lookup"><span data-stu-id="b7cf4-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="b7cf4-118">**Observera:** Om en postlåda är mindre än 10 MB bearbetar hanteras Mapphanteraren inte automatiskt postlådan.</span><span class="sxs-lookup"><span data-stu-id="b7cf4-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="b7cf4-119">Mer information om lagringsprinciper i Exchange Admin Center finns:</span><span class="sxs-lookup"><span data-stu-id="b7cf4-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="b7cf4-120">Taggar för bevarande och bevarandeprinciper</span><span class="sxs-lookup"><span data-stu-id="b7cf4-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="b7cf4-121">Tillämpa en princip för loggperiod till postlådor</span><span class="sxs-lookup"><span data-stu-id="b7cf4-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="b7cf4-122">Lägga till eller ta bort taggar för bevarande</span><span class="sxs-lookup"><span data-stu-id="b7cf4-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="b7cf4-123">Så här identifierar du vilken typ av undantag som placeras på en postlåda</span><span class="sxs-lookup"><span data-stu-id="b7cf4-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
