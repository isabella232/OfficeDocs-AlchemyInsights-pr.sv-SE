---
title: Flytta e-postmeddelanden till arkivpostlådan
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974975"
---
# <a name="move-email-to-the-archive-mailbox"></a>Flytta e-post till arkivpostlådan

Om du vill att vi ska köra automatiska kontroller för inställningarna som nämns nedan väljer du bakåtknappen < – högst upp på den här sidan och anger sedan e-postadressen till den användare som har problem med att flytta e-post till arkivpostlådan.

1. Bekräfta att en **arkivpostlåda** har aktiverats. Om det inte är det använder du stegen i [den här artikeln](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) för att aktivera arkivpostlådan.

2. Om du vill arkivera meddelanden automatiskt till  arkivpostlådan måste en bevarandetagg med åtgärden Flytta till arkiv ställas in så att den tillämpas automatiskt på hela postlådan **(standardtagg).** Använd stegen här för att skapa taggen: [Arkivera standardtaggen](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Lägg sedan till **arkiveringstaggen** i bevarandeprincipen. I Exchange väljer du Bevarandeprinciper och > till  taggen Flytta till arkiv i principen > **Spara.** 

4. Tilldela [bevarandeprincipen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) till den specifika användarens postlåda. Samma princip används för både den primära **postlådan och** **arkivpostlådan.**

Det kan vara nödvändigt att tvinga assistenten för hanterade mappar (MFA) att köra och tillämpa de nya inställningarna på användarens postlåda. Kör följande kommando när du är [ansluten till EXO PowerShell för](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) att starta assistenten för hanterade mappar för en viss postlåda:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

Mer information om hur du inställningar en arkiveringsprincip finns [i Konfigurera en princip för arkivering och borttagning för postlådor.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  