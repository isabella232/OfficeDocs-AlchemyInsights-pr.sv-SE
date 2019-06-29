---
title: Återkalla eller ersätta ett e-postmeddelande
ms.author: daeite
author: daeite
manager: joallard
ms.date: 05/15/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 170fbd632f0289a45d9497ac26fbe7f90cf88318
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35356615"
---
# <a name="recall-or-replace-an-email-message"></a>Återkalla eller ersätta ett e-postmeddelande

- Du kan **bara återkalla meddelanden som skickas till personer i din organisation**. Om meddelandet har skickats till en Gmail-adress, till exempel du inte kommer ihåg den.
- Du kan **bara återkalla meddelanden som skickas från Outlook 2016 för PC**. Om en användare skickar ett meddelande med hjälp av Outlook för Mac eller Outlook på webben, du kan inte återkalla den.
- Om du är en administratör kan **Återkalla meddelanden för användare med hjälp av PowerShell**. Du kan inte återkalla meddelanden från administratörscenter. Rulla ned till ”Sök efter och ta bort e-postmeddelanden i organisationen” för mer information.

***Återkalla eller ersätta ett e-postmeddelande som skickades***

1. Välj mappen Skickat i mappfönstret till vänster i Outlook-fönstret.
2. Öppna det meddelande som du vill återkalla. Du måste dubbelklicka om du vill öppna meddelandet. Markera meddelandet så att det visas i läsfönstret kan du återkalla meddelandet inte.
3. Välj fliken meddelande **åtgärder** > **Återkalla detta meddelande**.
4. Välj **Ta bort olästa exemplar av meddelandet** eller **Ta bort olästa exemplar och ersätta med ett nytt meddelande**och klicka på **OK**.
5. Om du skickar ett meddelande med ersättning, skriva meddelandet och sedan **Skicka**.
6. Lyckades eller inte återkalla ett meddelande beror på mottagarens inställningar i Outlook.

För mer information, inklusive hur du kontrollerar återkallelsen finns [återkalla eller ersätta ett e-postmeddelande som du har skickat](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Söka efter och ta bort e-postmeddelanden i organisationen*** Om du vill söka efter och ta bort e-postmeddelanden i organisationen, är det enklast om du är en global administratör. Om du inte är en global administratör måste ditt konto läggas till e-informationsavslöjande Manager roll gruppen eller rollen management att söka. Om du vill ta bort meddelanden, måste du ansluta till organisationshantering roll gruppen eller rollen för sökning och rensa. Dessa roller behörigheter i [regelefterlevnadscentret för säkerhet &](https://protection.office.com/).

1. [Skapa ett innehåll söka](https://docs.microsoft.com/office365/securitycompliance/content-search) efter meddelandet om du vill ta bort.
2. [Ansluta till regelefterlevnadscentret PowerShell för säkerhet &](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Om du använder MFA finns i [Anslut till Office 365 säkerhet & Center PowerShell för att använda autentisering på flera plan](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
