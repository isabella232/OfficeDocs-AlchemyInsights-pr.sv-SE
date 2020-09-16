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
# <a name="retention-policies-in-exchange-admin-center"></a>Bevarande principer i administrations centret för Exchange

Om du vill att vi ska köra automatisk kontroll för de inställningar som nämns nedan, väljer du knappen tillbaka <--överst på den här sidan och anger sedan e-postadressen för den användare som har problem med bevarande principer.

 **Problem:** Nyligen skapade eller uppdaterade bevarande principer i administrations centret för Exchange gäller inte för post lådor eller objekt flyttas inte till Arkiv post lådan eller tas bort. 
  
 **Rot orsaker:**
  
- Det kan bero på att **assistenten för hanterade mappar** inte har bearbetat användarens post låda. Managed Assistant försöker behandla alla post lådor i din molnbaserade organisation en gång i sju dagar. Om du ändrar en behållnings tagg eller tillämpar en annan bevarande princip i en post låda kan du vänta tills den hanterade mappens stöd bearbetar post lådan, eller så kan du köra cmdleten Start-ManagedFolderAssistant för att starta assistenten för hanterade mappar för att bearbeta en viss post låda. Att köra denna cmdlet är användbart för att testa eller felsöka en bevarande princip eller inställningar för bevarande märkning. Om du vill ha mer information går [du till köra assistenten för hanterade mappar](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Lösning:** Kör följande kommando för att starta assistenten för hanterade mappar för en viss post låda:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Det kan också inträffa om **RetentionHold** har **Aktiver ATS** i post lådan. Om post lådan har placerats på en RetentionHold bearbetas inte den bevarande principen för post lådan under den tiden. Mer information för RetentionHold-inställningen finns i: [lagring av post lådor](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Lantansaltlösning**
    
  - Kontrol lera status för RetentionHold-inställningen i den specifika post lådan i [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Kör följande kommando för att **inaktivera** RetentionHold för en viss post låda:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Kör sedan assistenten för hanterade mappar igen:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Obs!** Om en post låda är mindre än 10 MB bearbetar inte post lådan automatiskt.
 
Mer information om bevarande principer i Exchange Admin Center finns i:
- [Bevarande märkning och bevarande principer](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Tillämpa en bevarande princip på post lådor](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Lägga till eller ta bort bevarande koder](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Identifiera typen av undantag som tillämpas på en postlåda](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
