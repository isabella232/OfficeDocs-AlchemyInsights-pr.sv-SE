---
title: 1336 Mappen RecoverableItems är full
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720270"
---
# <a name="the-recoverable-items-folder-is-full"></a>Mappen Återställningsbara objekt är full

För Exchange Online-postlådor är standardlagringsgränsen för mappen Återställningsbara objekt 30 GB. Lagringsgränsen för mappen Återställningsbara objekt ökas automatiskt till 100 GB om postlådan placeras på bevarande av juridiska skäl, spärr för eDiscovery eller tilldelas en bevarandeprincip.

När mappen Återställningsbara objekt når lagringsgränsen påverkas postlådefunktionen på följande sätt:

- Användaren kan inte ta bort objekt från postlådan.

- Assistenten för hanterad mapp kan inte ta bort objekt baserat på kvarhållningstagg eller hanterade mappinställningar.

- För postlådor som har ensidig återställning av ett objekt aktiverat eller har spärrats kan sidskyddsprocessen för copy-on-write inte underhålla versioner av objekt som redigerats av användaren.

- För postlådor som har loggning av postlådegranskning aktiverat kan inga loggposter för postlådagranskning sparas i undermappen Granskningar i mappen Återställningsbara objekt.

För postlådor som inte är spärrade kan `Search-Mailbox -SearchDumpsterOnly -DeleteContent` administratörer använda kommandot i Exchange Online PowerShell för att ta bort objekt i mappen Återställningsbara objekt. Mer information finns i följande avsnitt:

- [Söka efter och ta bort meddelanden](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [Sök-brevlåda](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

För postlådor som är spärrade måste administratörer ta bort spärren innan de kan ta bort objekt från mappen Återställningsbara objekt. Mer information finns [i Ta bort objekt i mappen Återställningsbara objekt för molnbaserade postlådor som är spärrade](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

För att förhindra att mappen Återställningsbara objekt blir fullständig kan administratörer öka lagringsgränsen för mappen Återställningsbara objekt för spärrade postlådor och ställa in en bevarandeprincip för postlådan som flyttar objekt från mappen Återställningsbara objekt till användarens arkivpostlåda. Se [Öka kvoten För återställningsbara objekt för spärrade postlådor](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
