---
title: 618 Kalender delningspolicy
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373017"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Principfel vid delning av en kalender

1. Gör något av följande, beroende på din situation:
    - Anslut till Exchange Online med hjälp av Remote PowerShell. Mer information finns i [Anslut till Exchange Online med Fjärr-PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Öppna Exchange Management Shell på den lokala servern.
2. Bestäm delningsprincipen som har tilldelats användaren. Det gör du genom att köra följande kommando och notera att principen returneras:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Uppdatera delningsprincipen för användaren. Gör så här:
    - Öppna administrationscentret för Exchange.
    - Klicka på **Organisation**och dubbelklicka sedan på den princip som har tilldelats användaren under **Enskild delning**. Detta är den politik som returnerades i steg 2.
    - På sidan Delningsregel väljer du den kalenderdelningsnivå som du vill tillåta under **Ange vilken information du vill dela.** Klicka på **Spara**.

Mer information finns i: ["Principen tillåter inte att behörigheter på den här nivån beviljas ett eller flera av mottagarnas fel när användaren försöker dela kalendern](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
