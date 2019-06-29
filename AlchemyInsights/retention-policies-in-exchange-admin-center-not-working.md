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
ms.openlocfilehash: 9f4a175239bc20aaf489615da63ef35002030a70
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35369683"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Lagringsprinciper i Exchange Admin Center

 **Problemet:** Nyskapade eller uppdaterade lagringsprinciper i Exchange Admin Center tillämpa inte för postlådor eller objekt inte har flyttat till arkivet postlåda eller tagits bort. 
  
 **Rotorsaker:**
  
- Detta kan bero på **Hanterade Mapphanteraren** inte bearbetats av användarens postlåda. Hanterade Mapphanteraren försöker bearbeta alla postlådor i organisationen molnbaserad var sjunde dag. Om du ändrar taggen bibehålla eller tillämpa en annan bevarandeprincip på en postlåda kan vänta tills mappen hanterade bistå bearbetar postlådan, eller du kan köra cmdlet Start-ManagedFolderAssistant om du vill starta hanteras Mapphanteraren att bearbeta en viss e-postlådan. Kör denna cmdlet är användbart för testning eller felsökning av en bevarandeprincip eller loggperioder tagg. Mer information finns i [Kör hanterade Mapphanteraren](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Lösning:** Kör följande kommando för att starta hanteras Mapphanteraren för en viss postlåda:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Detta kan också inträffa om **RetentionHold** har **aktiverats** på postlådan. Om postlådan har placerats i en RetentionHold, bearbetas inte bevarandeprincipen på postlådan under den tiden. För mer information om RetentionHold inställning finns: [Postlåda kvarhållande håller](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Lösning:**
    
  - Kontrollera status för RetentionHold inställningen för en viss postlåda i [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Kör följande kommando för att **Inaktivera** RetentionHold för en viss postlåda:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Kör nu mappen hanterade assistenten igen:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Observera:** Om en postlåda är mindre än 10 MB bearbetar hanteras Mapphanteraren inte automatiskt postlådan.
  