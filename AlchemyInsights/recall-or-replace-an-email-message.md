---
title: Återkalla eller ersätta ett e-postmeddelande
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: e541620a499b02a7206579ffcc505ceb4e632a4c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742773"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Återkalla eller ersätta ett e-postmeddelande i Microsoft 365

- Du kan **bara återkalla meddelanden som skickas till personer i organisationen**. Om meddelandet till exempel skickades till en Gmail-adress kan du inte komma ihåg det.
- Du kan **bara återkalla meddelanden som skickats från Outlook 2016 för datorn**. Om en användare skickar ett meddelande med Outlook för Mac eller Outlook på webben kan du inte återkalla det.
- Om du är administratör kan du **återkalla meddelanden för användarnas räkning med hjälp av PowerShell**. Du kan inte återkalla meddelanden från administrationscentret. Bläddra ned till "Sök efter och ta bort e-postmeddelanden i organisationen" för mer information.

**Återkalla eller ersätta ett e-postmeddelande som du har skickat**

1. Välj mappen Skickat i mappfönstret till vänster om Outlook-fönstret.
2. Öppna meddelandet som du vill återkalla. Du måste dubbelklicka för att kunna öppna meddelandet. Om du markerar meddelandet så att det visas i läsfönstret kan du inte återkalla meddelandet.
3. Välj **Åtgärder** > **återkalla det här meddelandet på**fliken Meddelande .
4. Välj **Ta bort olästa kopior av det här meddelandet** eller Ta bort **olästa kopior och ersätt med ett nytt meddelande**och välj sedan **OK**.
5. Om du skickar ett ersättningsmeddelande skriver du meddelandet och väljer sedan **Skicka**.
6. Hur ett meddelande återkallas eller misslyckas beror på mottagarnas inställningar i Outlook.

Mer information, inklusive hur du kontrollerar återkallandet, finns i [Återkalla eller ersätta ett e-postmeddelande som du skickade](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Söka efter och ta bort e-postmeddelanden i organisationen*** Om du vill söka efter och ta bort e-postmeddelanden i organisationen är det enklast om du är global administratör. Om du inte är global administratör måste ditt konto läggas till i rollgruppen eDiscovery Manager eller i rollen hantering av efterlevnadssökning. Om du vill ta bort meddelanden måste du gå med i rollgruppen Organisationshantering eller hanteringsrollen Sök och rensa. Behörigheter till dessa roller tilldelas i [säkerhets- & efterlevnadscenter](https://protection.office.com/).

1. [Skapa en innehållssökning](https://docs.microsoft.com/office365/securitycompliance/content-search) för att hitta meddelandet som ska tas bort.
2. [Anslut till Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Om du använder MFA läser du [Anslut till Microsoft 365-säkerhet & Compliance Center PowerShell med multifaktorautentisering](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
