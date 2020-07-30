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
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522825"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="3990d-102">Bevarandeprinciper i Administrationscenter för Exchange</span><span class="sxs-lookup"><span data-stu-id="3990d-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="3990d-103">Om du vill att vi ska köra automatiska kontroller för de inställningar som nämns nedan, välj bakåtknappen < - högst upp på den här sidan och ange sedan e-postadressen till den användare som har problem med bevarandeprinciper.</span><span class="sxs-lookup"><span data-stu-id="3990d-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="3990d-104">**Problem:** Nyligen skapade eller uppdaterade bevarandeprinciper i Administrationscenter för Exchange gäller inte för postlådor eller objekt som inte flyttas till arkivpostlådan eller tas bort.</span><span class="sxs-lookup"><span data-stu-id="3990d-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="3990d-105">**Grundorsakerna:**</span><span class="sxs-lookup"><span data-stu-id="3990d-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="3990d-106">Det kan bero på att **assistenten för hanterade mappar** inte har bearbetat användarens postlåda.</span><span class="sxs-lookup"><span data-stu-id="3990d-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="3990d-107">Assistenten för hanterade mappar försöker bearbeta alla postlådor i din molnbaserade organisation en gång var sjunde dag.</span><span class="sxs-lookup"><span data-stu-id="3990d-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="3990d-108">Om du ändrar en kvarhållningstagg eller tillämpar en annan bevarandeprincip på en postlåda kan du vänta tills den hanterade mappassistenten bearbetar postlådan eller köra cmdleten Start-ManagedFolderAssistant för att starta assistenten Hanterad mapp för att bearbeta en viss postlåda.</span><span class="sxs-lookup"><span data-stu-id="3990d-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="3990d-109">Köra den här cmdleten är användbart för att testa eller felsöka en bevarandeprincip eller inställningar för kvarhållningstagg.</span><span class="sxs-lookup"><span data-stu-id="3990d-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="3990d-110">Mer information finns i [Kör assistenten För hanterade mappar](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="3990d-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="3990d-111">**Lösning:** Kör följande kommando för att starta assistenten för hanterade mappar för en viss postlåda:</span><span class="sxs-lookup"><span data-stu-id="3990d-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="3990d-112">Detta kan också inträffa om **RetentionHold** har **aktiverats** på postlådan.</span><span class="sxs-lookup"><span data-stu-id="3990d-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="3990d-113">Om postlådan har placerats på en RetentionHold bearbetas inte bevarandeprincipen för postlådan under den tiden.</span><span class="sxs-lookup"><span data-stu-id="3990d-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="3990d-114">Mer informaton på inställningen RetentionHold finns i: [Bevarande av postlådan finns](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="3990d-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="3990d-115">**Lösning:**</span><span class="sxs-lookup"><span data-stu-id="3990d-115">**Solution:**</span></span>
    
  - <span data-ttu-id="3990d-116">Kontrollera status för inställningen RetentionHold på den specifika postlådan i [EXO powershell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="3990d-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="3990d-117">Kör följande kommando för att **inaktivera** RetentionHold på en viss postlåda:</span><span class="sxs-lookup"><span data-stu-id="3990d-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="3990d-118">Kör nu den hanterade mappassistenten igen:</span><span class="sxs-lookup"><span data-stu-id="3990d-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="3990d-119">**Obs:** Om en postlåda är mindre än 10 MB bearbetas postlådan inte automatiskt i assistenten.</span><span class="sxs-lookup"><span data-stu-id="3990d-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="3990d-120">Mer information om bevarandeprinciper i Administrationscenter för Exchange finns i:</span><span class="sxs-lookup"><span data-stu-id="3990d-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="3990d-121">Bevarandetaggar och bevarandeprinciper</span><span class="sxs-lookup"><span data-stu-id="3990d-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="3990d-122">Tillämpa en bevarandeprincip på postlådor</span><span class="sxs-lookup"><span data-stu-id="3990d-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="3990d-123">Lägga till eller ta bort kvarhållningstaggar</span><span class="sxs-lookup"><span data-stu-id="3990d-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="3990d-124">Identifiera typen av undantag som tillämpas på en postlåda</span><span class="sxs-lookup"><span data-stu-id="3990d-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
