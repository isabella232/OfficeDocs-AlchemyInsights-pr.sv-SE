---
title: Flytta e-postmeddelanden till arkivpostlådan
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522789"
---
# <a name="move-email-to-the-archive-mailbox"></a>Flytta e-post till arkivpostlådan

Om du vill att vi ska köra automatiska kontroller för de inställningar som nämns nedan, välj bakåtknappen < - högst upp på den här sidan och ange sedan e-postadressen till den användare som har problem med att flytta e-post till sin arkivpostlåda.

1. Bekräfta att en **arkivpostlåda** har aktiverats. Om inte, gör du så här i den [här artikeln](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) för att aktivera arkivpostlådan.

2. Om du vill arkivera meddelanden automatiskt till arkivpostlådan måste en kvarhållningstagg med åtgärden **Flytta till arkiv** ställas in på att tillämpas automatiskt på hela **postlådetaggen (standard)**. Följ stegen här för att skapa taggen: [Arkiv standardtagg](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Lägg sedan till **arkivtaggen** i bevarandeprincipen. I administrationscentret för Exchange väljer du **Bevarandeprinciper** > lägga **till taggen Flytta i arkiv** i principen > **Spara**.

4. Tilldela [nu bevarandeprincipen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) till den specifika användarens postlåda. Samma princip tillämpas på både **postlådan Primär** och **Arkiv.**

Det kan vara nödvändigt att tvinga MFA (Managed Folder Assistant) att köra och tillämpa de nya inställningarna på användarens postlåda. Kör följande kommando när [du är ansluten till EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) för att starta assistenten för hanterade mappar för en viss postlåda:
  
Start-ManagedFolderAssistant -Identitet<name of the mailbox>

Mer information om hur du konfigurerar en arkivprincip finns i [Konfigurera en arkiv- och borttagningsprincip för postlådor](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  