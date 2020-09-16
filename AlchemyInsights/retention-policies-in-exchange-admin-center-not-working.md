---
title: Bevarande principer i Exchange Admin Center fungerar inte
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740528"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="424dc-102">Bevarande principer i administrations centret för Exchange</span><span class="sxs-lookup"><span data-stu-id="424dc-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="424dc-103">Om du vill att vi ska köra automatisk kontroll för de inställningar som nämns nedan, väljer du knappen tillbaka <--överst på den här sidan och anger sedan e-postadressen för den användare som har problem med bevarande principer.</span><span class="sxs-lookup"><span data-stu-id="424dc-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="424dc-104">**Problem:** Nyligen skapade eller uppdaterade bevarande principer i administrations centret för Exchange gäller inte för post lådor eller objekt flyttas inte till Arkiv post lådan eller tas bort.</span><span class="sxs-lookup"><span data-stu-id="424dc-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="424dc-105">**Rot orsaker:**</span><span class="sxs-lookup"><span data-stu-id="424dc-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="424dc-106">Det kan bero på att **assistenten för hanterade mappar** inte har bearbetat användarens post låda.</span><span class="sxs-lookup"><span data-stu-id="424dc-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="424dc-107">Managed Assistant försöker behandla alla post lådor i din molnbaserade organisation en gång i sju dagar.</span><span class="sxs-lookup"><span data-stu-id="424dc-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="424dc-108">Om du ändrar en behållnings tagg eller tillämpar en annan bevarande princip i en post låda kan du vänta tills den hanterade mappens stöd bearbetar post lådan, eller så kan du köra cmdleten Start-ManagedFolderAssistant för att starta assistenten för hanterade mappar för att bearbeta en viss post låda.</span><span class="sxs-lookup"><span data-stu-id="424dc-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="424dc-109">Att köra denna cmdlet är användbart för att testa eller felsöka en bevarande princip eller inställningar för bevarande märkning.</span><span class="sxs-lookup"><span data-stu-id="424dc-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="424dc-110">Om du vill ha mer information går [du till köra assistenten för hanterade mappar](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="424dc-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="424dc-111">**Lösning:** Kör följande kommando för att starta assistenten för hanterade mappar för en viss post låda:</span><span class="sxs-lookup"><span data-stu-id="424dc-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="424dc-112">Det kan också inträffa om **RetentionHold** har **Aktiver ATS** i post lådan.</span><span class="sxs-lookup"><span data-stu-id="424dc-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="424dc-113">Om post lådan har placerats på en RetentionHold bearbetas inte den bevarande principen för post lådan under den tiden.</span><span class="sxs-lookup"><span data-stu-id="424dc-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="424dc-114">Mer information för RetentionHold-inställningen finns i: [lagring av post lådor](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="424dc-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="424dc-115">**Lantansaltlösning**</span><span class="sxs-lookup"><span data-stu-id="424dc-115">**Solution:**</span></span>
    
  - <span data-ttu-id="424dc-116">Kontrol lera status för RetentionHold-inställningen i den specifika post lådan i [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="424dc-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="424dc-117">Kör följande kommando för att **inaktivera** RetentionHold för en viss post låda:</span><span class="sxs-lookup"><span data-stu-id="424dc-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="424dc-118">Kör sedan assistenten för hanterade mappar igen:</span><span class="sxs-lookup"><span data-stu-id="424dc-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="424dc-119">**Obs!** Om en post låda är mindre än 10 MB bearbetar inte post lådan automatiskt.</span><span class="sxs-lookup"><span data-stu-id="424dc-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="424dc-120">Mer information om bevarande principer i Exchange Admin Center finns i:</span><span class="sxs-lookup"><span data-stu-id="424dc-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="424dc-121">Bevarande märkning och bevarande principer</span><span class="sxs-lookup"><span data-stu-id="424dc-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="424dc-122">Tillämpa en bevarande princip på post lådor</span><span class="sxs-lookup"><span data-stu-id="424dc-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="424dc-123">Lägga till eller ta bort bevarande koder</span><span class="sxs-lookup"><span data-stu-id="424dc-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="424dc-124">Identifiera typen av undantag som tillämpas på en postlåda</span><span class="sxs-lookup"><span data-stu-id="424dc-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
