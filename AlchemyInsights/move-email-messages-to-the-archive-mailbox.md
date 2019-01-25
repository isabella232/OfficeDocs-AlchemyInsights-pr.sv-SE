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
Problem Arkivera objekt med Arkivera postlådan. Kontrollera att du har utfört följande åtgärder:
  
1. Bekräfta att en **Arkivera postlåda** har aktiverats. Om du inte följer instruktionerna i [denna artikel](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) för att arkivera postlåda. 
    
2. I Exchange Admin Center, Välj **Kvarhållande taggar** under **Regelefterlevnadshantering**, skapa en **tagg för bevarande** med åtgärden **Flytta till Arkiv** som innehåller önskad **Kvarhållande ålder**.
    
3. Markera **Lagringsprinciper**i Exchange Admin Center, och skapa en **Princip för loggperiod** till din **Flytta till arkivet** innehållen tagg till principen. 
    
4. [Tilldela en princip för loggperiod](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) till användarens postlåda. Samma princip tillämpas på både det **primärt** och **Arkivera** postlåda. 
    
Användarens postlåda ska nu ha en arkiveringsprincip för att flytta objekt till arkivet postlåda. Det kan vara nödvändigt att tvinga den hanterade mappen assistenten (MFA) att köra och använda de nya inställningarna till användarens postlåda. Kör följande kommando när [anslutet till EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) att starta hanteras Mapphanteraren för en viss postlåda: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Om du vill ha mer information om att konfigurera en arkiveringsprincip finns i avsnittet [Konfigurera en arkivera och ta bort princip för postlådor](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

