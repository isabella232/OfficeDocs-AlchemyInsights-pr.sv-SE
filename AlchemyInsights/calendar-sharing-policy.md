---
title: Kalender delnings princip för 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684248"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Princip fel när du delar en kalender

1. Gör något av följande, efter behov:
    - Ansluta till Exchange Online med fjärr-PowerShell. Mer information finns i [ansluta till Exchange Online med fjärr-PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Öppna Exchange Management Shell på den lokala servern.
2. Ta reda på vilken delnings princip som är tilldelad användaren. Det gör du genom att köra följande kommando och notera att principen returneras:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Uppdatera delnings principen för användaren. Gör så här:
    - Öppna administrationscentret för Exchange.
    - Klicka på **organisation**och dubbelklicka sedan på den princip som är tilldelad användaren under **individuell delning**. Det här är den princip som returnerades i steg 2.
    - På sidan delnings regel väljer du den delnings nivå som du vill tillåta under **Ange vilken information du vill dela**. Klicka på **Spara**.

Mer information finns i: ["principen tillåter inte att behörigheter på den här nivån beviljar åtkomst på denna nivå till en eller flera av mottagarna" när användaren försöker dela kalendern](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
