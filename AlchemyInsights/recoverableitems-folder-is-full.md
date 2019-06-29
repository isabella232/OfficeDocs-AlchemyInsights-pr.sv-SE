---
title: 1336 RecoverableItems mappen är full
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 05e7b47a2200c3b0500e7d786166966ea301179a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35370405"
---
# <a name="the-recoverable-items-folder-is-full"></a>Objekt som kan återskapas mappen är full

För Exchange Online-postlådor i Office 365 är standard lagringsgränsen för objekt som kan återskapas mappen 30 GB. Lagringsgränsen för objekt som kan återskapas mappen ökar automatiskt till 100 GB om postlådan placeras på rättstvist håller e-informationsavslöjande Håll eller tilldelas en bevarandeprincip för Office 365.

När objekt som kan återskapas mappen överskrider lagringsgränsen, påverkas postlåda funktioner på följande sätt:

- Användaren kan inte ta bort objekt från postlådan.

- Hanterade Mapphanteraren kan inte radera objekt baserat på kvarhållande tagg eller inställningar för hanterade mappar.

- Kopiera-on-write sidan skydd processen inte kan upprätthålla versioner av objekt redigeras av användaren för postlådor som har enstaka objekt återställning aktiverat eller har spärrats.

- För postlådor som har postlådan granskningsloggning aktiverats kan ingen logg granskningsposter postlåda sparas i revisioner undermapp i mappen objekt som kan återskapas.

Administratörer kan använda för postlådor som inte är spärrade, de `Search-Mailbox -SearchDumpsterOnly -DeleteContent` i Exchange Online PowerShell för att ta bort objekt i mappen objekt som kan återskapas. Mer information finns i följande avsnitt:

- [Söka efter och ta bort meddelanden](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [Sök-postlåda](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Administratörer måste ta bort spärren innan de kan borttagna objekt från mappen objekt som kan återskapas för postlådor som är spärrade. Mer information finns i [Ta bort objekt i objekt som kan återskapas mappen för molnbaserade postlådor på Håll](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

För att förhindra att objekt som kan återskapas mappen blir full, kan administratörer öka lagringsgränsen för de objekt som kan återskapas mappen för postlådor på Håll och ställa in en bevarandeprincip för postlådan som flyttar objekt från mappen objekt som kan återskapas till användarens Arkiv e-postlådan. Se [öka objekt som kan återskapas kvoten för postlådor på Håll](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
