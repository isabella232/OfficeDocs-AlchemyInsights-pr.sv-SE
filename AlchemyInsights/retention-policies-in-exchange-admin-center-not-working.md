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
# <a name="retention-policies-in-exchange-admin-center"></a>Bevarandeprinciper i Administrationscenter för Exchange

 **Problem:** Nyligen skapade eller uppdaterade bevarandeprinciper i Administrationscenter för Exchange gäller inte för postlådor eller objekt som inte flyttas till arkivpostlådan eller tas bort. 
  
 **Grundorsakerna:**
  
- Det kan bero på att **assistenten för hanterade mappar** inte har bearbetat användarens postlåda. Assistenten för hanterade mappar försöker bearbeta alla postlådor i din molnbaserade organisation en gång var sjunde dag. Om du ändrar en kvarhållningstagg eller tillämpar en annan bevarandeprincip på en postlåda kan du vänta tills den hanterade mappassistenten bearbetar postlådan eller köra cmdleten Start-ManagedFolderAssistant för att starta assistenten Hanterad mapp för att bearbeta en viss postlåda. Köra den här cmdlet är användbart för att testa eller felsöka en bevarandeprincip eller inställningar för kvarhållningstagg. Mer information finns i [Kör assistenten För hanterade mappar](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Lösning:** Kör följande kommando för att starta assistenten För hanterade mappar för en viss postlåda:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Detta kan också inträffa om **RetentionHold** har **aktiverats** på postlådan. Om postlådan har placerats på en RetentionHold bearbetas inte bevarandeprincipen för postlådan under den tiden. Mer informaton på inställningen RetentionHold finns i: [Bevarande av postlådan håll](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Lösning:**
    
  - Kontrollera status för inställningen RetentionHold på den specifika postlådan i [EXO powershell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Kör följande kommando för att **inaktivera** RetentionHold på en viss postlåda:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Kör nu den hanterade mappassistenten igen:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Anm.:** Om en postlåda är mindre än 10 MB bearbetas inte postlådan automatiskt i assistenten.
 
Mer information om bevarandeprinciper i Administrationscenter för Exchange finns i:
- [Bevarandetaggar och bevarandeprinciper](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Tillämpa en bevarandeprincip på postlådor](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Lägga till eller ta bort kvarhållningstaggar](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Så här identifierar du vilken typ av spärr som placeras på en postlåda](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
