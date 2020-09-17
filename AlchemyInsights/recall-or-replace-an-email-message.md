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
ms.openlocfilehash: 2e711679e7db7293d9e7e6f68d0662f03047c23d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799222"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Återkalla eller ersätta ett e-postmeddelande i Microsoft 365

- Du kan **bara återkalla meddelanden som skickas till personer i organisationen**. Om meddelandet skickades till en Gmail-adress, till exempel, kan du inte återkalla det.
- Du kan **bara återkalla meddelanden som skickats från Outlook 2016 för PC**. Om en användare skickar ett meddelande med hjälp av Outlook för Mac eller Outlook på webben kan du inte återkalla det.
- Om du är administratör kan du **återkalla meddelanden för användare med hjälp av PowerShell**. Du kan inte återkalla meddelanden från administrations centret. Bläddra ned till "Sök efter och ta bort e-postmeddelanden i din organisation" för mer information.

**Återkalla eller ersätta ett e-postmeddelande som du har skickat**

1. I mappfönstret till vänster i Outlook-fönstret väljer du mappen skickat.
2. Öppna meddelandet som du vill återkalla. Du måste dubbelklicka för att öppna meddelandet. Om du väljer meddelandet så att det visas i Läs fönstret kan du inte återkalla meddelandet.
3. Välj **åtgärder**  >  **återkalla detta meddelande**på fliken meddelande.
4. Välj **ta bort olästa exemplar av detta meddelande** eller **ta bort olästa exemplar och ersätta med ett nytt meddelande**och välj sedan **OK**.
5. Om du skickar ett ersättnings meddelande skriver du meddelandet och väljer sedan **Skicka**.
6. Om du har problem med att återkalla meddelanden beror det på mottagarens inställningar i Outlook.

Mer information om hur du kontrollerar åter kallelsen finns i [återkalla eller ersätta ett e-postmeddelande som du har skickat](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Söka efter och ta bort e-postmeddelanden i din organisation*** Om du är global administratör kan du söka efter och ta bort e-postmeddelanden i organisationen. Om du inte är global administratör måste ditt konto läggas till i roll gruppen för eDiscovery-hanteraren eller till en hanterings roll för Sök efter efterlevnad. Om du vill ta bort meddelanden måste du gå med i roll gruppen organisations hantering eller rollen för sökning och rensning. Behörigheter för dessa roller är tilldelade i [säkerhets & Compliance Center](https://protection.office.com/).

1. [Skapa en innehålls sökning](https://docs.microsoft.com/microsoft-365/compliance/content-search) för att hitta meddelandet som ska tas bort.
2. [Anslut till säkerhets & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Om du använder MFA kan du läsa [Anslut till Microsoft 365 security & Compliance Center PowerShell med multifaktorautentisering](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
