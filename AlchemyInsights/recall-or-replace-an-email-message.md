---
title: Återkalla eller ersätta ett e-postmeddelande
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024404"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Återkalla eller ersätta ett e-postmeddelande i Microsoft 365

- Du kan **bara återkalla meddelanden som skickas till personer i din organisation.** Om meddelandet till exempel skickades till en Gmail-adress kan du inte återkalla den.
- Du kan **bara återkalla meddelanden som skickats Outlook för pc.** Om en användare skickar ett meddelande med Outlook för Mac eller Outlook på webben kan du inte återkalla det.
- Som innehavaradministratör kan du återkalla meddelanden för användares räkning genom att använda **PowerShell** (Mer information finns i: Söka efter och [ta bort e-postmeddelanden](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- Du kan inte återkalla meddelanden från administrationscentret. Rulla ned till "Sök efter och ta bort e-postmeddelanden i organisationen" för mer information.

**Återkalla eller ersätta ett e-postmeddelande som du har skickat**

1. I mappfönstret till vänster i Outlook väljer du mappen Skickat.
2. Öppna meddelandet som du vill återkalla. Du måste dubbelklicka för att öppna meddelandet. Du kan inte återkalla meddelandet genom att markera det så att det visas i läsfönstret.
3. Välj Åtgärder Återkalla detta meddelande **på**  >  **fliken Meddelande.**
4. Välj **Ta bort olästa exemplar av detta meddelande** eller Ta bort **olästa exemplar och ersätta med ett nytt** meddelande och välj sedan **OK.**
5. Om du skickar ett ersättningsmeddelande skriver du meddelandet och väljer sedan **Skicka**.
6. Om det går att återkalla ett meddelande eller inte beror på mottagarnas inställningar i Outlook.

Mer information, inklusive hur du kontrollerar återkallelsen, finns i Återkalla [eller ersätta ett e-postmeddelande som du har skickat.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

***Om du vill söka efter och ta bort e-postmeddelanden*** i organisationen är det enklast om du är global administratör. Om du inte är global administratör måste ditt konto läggas till i rollgruppen för eDiscovery Manager eller i rollen för efterlevnadssökningshantering. Om du vill ta bort meddelanden måste du gå med i rollgruppen Organisationshantering eller rollen för hantering av sökning och rensning. Behörigheter till dessa roller tilldelas i [Säkerhets- & kompatibilitetscenter.](https://protection.office.com/)

1. [Skapa en innehållssökning för](https://docs.microsoft.com/microsoft-365/compliance/content-search) att hitta det meddelande du vill ta bort.
2. [Anslut till Säkerhets- och efterlevnadscenter PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Om du använder MFA (multifaktorautentisering) kan du Anslut till Microsoft 365 Säkerhets- & PowerShell för [multifaktorautentisering.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
