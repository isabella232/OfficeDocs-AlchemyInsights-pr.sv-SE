---
title: Flytta e-postmeddelanden till arkivpostlådan
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
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822180"
---
# <a name="move-email-to-the-archive-mailbox"></a>Flytta e-post till arkivpostlådan

1. Bekräfta att en **arkivpostlåda** har aktiverats. Om inte, Använd stegen i [den här artikeln](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) för att aktivera arkivpostlådan.

2. Om du vill arkivera meddelanden automatiskt till arkivpostlådan måste en kvarhållningstagg med åtgärden **Flytta till Arkiv** vara inställd på **tillämpas automatiskt på hela postlådan (standard)-taggen**. Använd stegen här för att skapa taggen: [Arkiv standard tagg](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Lägg sedan till **arkivtaggen** i din bevarandeprincip. I Exchange administratörscenter, Välj **bevarandeprinciper** > Lägg till **Flytta till arkivtagg** till principen > **Spara**.

4. [Tilldela nu bevarandeprincipen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) till den specifika användarens postlåda. Samma princip kommer att tillämpas på både den **primära** och **arkivera** postlådan.

Det kan vara nödvändigt att tvinga assistenten för hanterade mappar (MFA) att köra och tillämpa de nya inställningarna på användarens postlåda. Kör följande kommando när du [är ansluten till EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) för att starta assistenten för hanterade mappar för en viss postlåda:
  
Start-ManagedFolderAssistant-identitet<name of the mailbox>

Mer information om hur du konfigurerar en arkivprincip finns [i ställa in en Arkiv-och Borttagningsprincip för postlådor](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  