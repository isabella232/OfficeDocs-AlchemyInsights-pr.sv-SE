---
title: 1336 RecoverableItems-mappen är full
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
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741285"
---
# <a name="the-recoverable-items-folder-is-full"></a>Mappen för återställnings bara objekt är full

För Exchange Online-postlådor är standard lagrings gränsen 30 GB för mappen för återställnings bara objekt. Gränsen för lagrings utrymmet för mappen för återställnings bara objekt höjs automatiskt till 100 GB om post lådan är placerad i en begränsnings spärr, eDiscovery-undantag eller är kopplad till en bevarande princip.

När mappen för återställnings bara objekt når lagrings gränsen påverkas funktionen för post lådor på följande sätt:

- Användaren kan inte ta bort objekt från post lådan.

- Assistenten för hanterade mappar kan inte ta bort objekt baserat på bevarande kod eller inställningar för hanterade mappar.

- För att post lådor med återställning av enskilt objekt är aktiverat eller parkerade kan inte kopierings skydds processen hantera de objekt som redigerats av användaren.

- För post lådor som har post lådans gransknings loggning aktive rad kan inga gransknings poster för post lådor sparas i undermappen revisioner i mappen återställnings bara objekt.

För brev lådor som inte är parkerade kan administratörer använda `Search-Mailbox -SearchDumpsterOnly -DeleteContent` kommandot i Exchange Online PowerShell för att ta bort objekt i mappen för återställnings bara objekt. Mer information finns i följande avsnitt:

- [Söka efter och ta bort meddelanden](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Sök-post låda](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

För att post lådor ska blockeras måste administratörer ta bort spärren innan de kan ta bort objekt från mappen för återställnings bara objekt. Mer information finns i [ta bort objekt i mappen för återställnings bara objekt i molnbaserade post lådor](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

För att förhindra att mappen återställnings bara objekt blir full kan administratörerna öka lagrings gränsen för mappen för återställnings bara objekt för post lådor med undantag och konfigurera en bevarande princip för post lådor som flyttar objekt från mappen för återställnings bara objekt till användarens arkiv post låda. Se [öka kvoten för återställnings bara objekt för post lådor](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
