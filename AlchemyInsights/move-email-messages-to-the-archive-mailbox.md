---
title: Flytta e-postmeddelanden till arkivet postlåda
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a29fb799b68f5c187ca1d44aeaf94e6cd8760b0e
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35379515"
---
# <a name="move-email-to-the-archive-mailbox"></a>Flytta e-post till arkivet postlåda

1. Bekräfta att en **Arkivera postlåda** har aktiverats. Om så inte är fallet, följ instruktionerna i [den här artikeln](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) för att arkivera postlåda.

2. Om du vill arkivera meddelanden automatiskt till arkivet postlåda måste du ange taggen bevarande med åtgärden **Flytta Arkivera** tillämpas **automatiskt på hela postlådan (standard)-tagg**. Använd stegen här för att skapa taggen: [Arkivera standard tagg](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).

3. Lägg sedan till taggen **arkivet** princip för loggperiod. Välj **Lagringsprinciper** i Exchange administratörscenter, > lägga till **Flytta Arkivera-taggen** i princip-> **Spara**.

4. Nu [tilldela lagringsprincipen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) för användarens postlåda. Samma princip tillämpas på både det **primärt** och **Arkivera** postlåda.

Det kan vara nödvändigt att tvinga den hanterade mappen assistenten (MFA) att köra och använda de nya inställningarna till användarens postlåda. Kör följande kommando när [anslutet till EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) att starta hanteras Mapphanteraren för en viss postlåda:
  
Start-ManagedFolderAssistant-identitet<name of the mailbox>

Mer information om hur du konfigurerar en arkiveringsprincip finns i [Konfigurera en arkivera och ta bort princip för postlådor](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  