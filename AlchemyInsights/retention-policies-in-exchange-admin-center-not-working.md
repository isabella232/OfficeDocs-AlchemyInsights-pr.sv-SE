---
title: Bevarandeprinciper i Administrationscenter för Exchange fungerar inte
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: e2fb22f872be0eefc3b4b78b18cd09baffa66cda
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742451"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="339d6-102">Bevarandeprinciper i Administrationscenter för Exchange</span><span class="sxs-lookup"><span data-stu-id="339d6-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="339d6-103">**Problem:** Nyligen skapade eller uppdaterade bevarandeprinciper i Administrationscenter för Exchange gäller inte för postlådor eller objekt som inte flyttas till arkivpostlådan eller tas bort.</span><span class="sxs-lookup"><span data-stu-id="339d6-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="339d6-104">**Grundorsakerna:**</span><span class="sxs-lookup"><span data-stu-id="339d6-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="339d6-105">Det kan bero på att **assistenten för hanterade mappar** inte har bearbetat användarens postlåda.</span><span class="sxs-lookup"><span data-stu-id="339d6-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="339d6-106">Assistenten för hanterade mappar försöker bearbeta alla postlådor i din molnbaserade organisation en gång var sjunde dag.</span><span class="sxs-lookup"><span data-stu-id="339d6-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="339d6-107">Om du ändrar en kvarhållningstagg eller tillämpar en annan bevarandeprincip på en postlåda kan du vänta tills den hanterade mappassistenten bearbetar postlådan eller köra cmdleten Start-ManagedFolderAssistant för att starta assistenten Hanterad mapp för att bearbeta en viss postlåda.</span><span class="sxs-lookup"><span data-stu-id="339d6-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="339d6-108">Köra den här cmdlet är användbart för att testa eller felsöka en bevarandeprincip eller inställningar för kvarhållningstagg.</span><span class="sxs-lookup"><span data-stu-id="339d6-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="339d6-109">Mer information finns i [Kör assistenten För hanterade mappar](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="339d6-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="339d6-110">**Lösning:** Kör följande kommando för att starta assistenten För hanterade mappar för en viss postlåda:</span><span class="sxs-lookup"><span data-stu-id="339d6-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="339d6-111">Detta kan också inträffa om **RetentionHold** har **aktiverats** på postlådan.</span><span class="sxs-lookup"><span data-stu-id="339d6-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="339d6-112">Om postlådan har placerats på en RetentionHold bearbetas inte bevarandeprincipen för postlådan under den tiden.</span><span class="sxs-lookup"><span data-stu-id="339d6-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="339d6-113">Mer informaton på inställningen RetentionHold finns i: [Bevarande av postlådan håll](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="339d6-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="339d6-114">**Lösning:**</span><span class="sxs-lookup"><span data-stu-id="339d6-114">**Solution:**</span></span>
    
  - <span data-ttu-id="339d6-115">Kontrollera status för inställningen RetentionHold på den specifika postlådan i [EXO powershell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="339d6-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="339d6-116">Kör följande kommando för att **inaktivera** RetentionHold på en viss postlåda:</span><span class="sxs-lookup"><span data-stu-id="339d6-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="339d6-117">Kör nu den hanterade mappassistenten igen:</span><span class="sxs-lookup"><span data-stu-id="339d6-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="339d6-118">**Anm.:** Om en postlåda är mindre än 10 MB bearbetas inte postlådan automatiskt i assistenten.</span><span class="sxs-lookup"><span data-stu-id="339d6-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="339d6-119">Mer information om bevarandeprinciper i Administrationscenter för Exchange finns i:</span><span class="sxs-lookup"><span data-stu-id="339d6-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="339d6-120">Bevarandetaggar och bevarandeprinciper</span><span class="sxs-lookup"><span data-stu-id="339d6-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="339d6-121">Tillämpa en bevarandeprincip på postlådor</span><span class="sxs-lookup"><span data-stu-id="339d6-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="339d6-122">Lägga till eller ta bort kvarhållningstaggar</span><span class="sxs-lookup"><span data-stu-id="339d6-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="339d6-123">Så här identifierar du vilken typ av spärr som placeras på en postlåda</span><span class="sxs-lookup"><span data-stu-id="339d6-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
