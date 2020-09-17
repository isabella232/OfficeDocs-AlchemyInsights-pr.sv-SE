---
title: Flytta e-postmeddelanden till Arkiv post lådan
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
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799798"
---
# <a name="move-email-to-the-archive-mailbox"></a>Flytta e-post till Arkiv post lådan

Om du vill att vi ska köra automatisk kontroll för de inställningar som beskrivs nedan, väljer du knappen tillbaka <--överst på den här sidan och anger sedan e-postadressen för den användare som har problem med att flytta e-post till deras Arkiv post låda.

1. Bekräfta att en **Arkiv post låda** har Aktiver ATS. Om inte, Använd anvisningarna i [den här artikeln](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) för att aktivera Arkiv post lådan.

2. Om du vill att meddelanden ska arkiveras automatiskt i Arkiv post lådan måste en bevarande tagg med åtgärden **Flytta till Arkiv** -uppgift vara inställd på att **tillämpas automatiskt på hela post låda (standard)**. Följ stegen här för att skapa taggen: [arkivera standard märke](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Lägg sedan till **Arkiv** tag gen i bevarande princip. I administrations centret för Exchange väljer du **bevarande principer** > lägger till **taggen flytta till Arkiv** till den princip > **Spara**.

4. [Tilldela bevarande principen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) till den specifika användarens post låda. Samma policy kommer att tillämpas på både den **primära** och **Arkiv** post lådan.

Det kan vara nödvändigt att tvinga den Managed mapp Assistant (MFA) att köras och tillämpa de nya inställningarna på användarens post låda. Kör följande kommando när du [är ansluten till EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) för att starta assistenten för hanterade mappar för en viss post låda:
  
Start-ManagedFolderAssistant-Identity <name of the mailbox>

Mer information om hur du konfigurerar en Arkiv princip finns i [Konfigurera en arkiverings-och borttagnings princip för post lådor](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  