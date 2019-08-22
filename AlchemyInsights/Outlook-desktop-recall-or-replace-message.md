---
title: Outlook stationära återkalla eller ersätta ett e-postmeddelande
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496129"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Återkalla eller ersätta ett e-postmeddelande i Outlook

- Som administratör kan du **Återkalla meddelanden för användare med hjälp av PowerShell**. Du kan inte återkalla meddelanden från administratörscenter.
- Du kan **bara återkalla meddelanden som skickas till personer i din organisation**. Om meddelandet har skickats till en Gmail-adress, till exempel du inte kommer ihåg den.
- Du kan **bara återkalla meddelanden som skickas från Outlook 2016 på datorn**. Om en användare skickar ett meddelande med hjälp av Outlook för Mac eller Outlook på webben, du kan inte återkalla den.

Att återkalla eller ersätta ett e-postmeddelande:

1. Markera mappen Skickat i mappfönstret till vänster i Outlook-fönstret.
1. Dubbelklicka på meddelandet som du vill återkalla om du vill öppna den.
1. Klicka på fliken **meddelande** och välj **åtgärder** > **Återkalla detta meddelande**.
1. Välj **Ta bort olästa exemplar av meddelandet** eller **Ta bort olästa exemplar och ersätta med ett nytt meddelande**och välj sedan **OK**.
1. Om du skickar ett meddelande med ersättning, skriver meddelandet och välj sedan **Skicka**.
1. Lyckades eller inte återkalla ett meddelande beror på mottagarens inställningar i Outlook. Åtgärder för att kontrollera om återkallelsen, finns i [den här artikeln](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Söka efter och ta bort e-postmeddelanden i organisationen

- Om du inte är en global administratör måste ditt konto läggas till e-informationsavslöjande Manager roll eller överensstämmelse Search management rollen att söka efter meddelanden. Om du vill ta bort meddelanden, måste du ansluta till organisationshantering roll gruppen eller rollen för sökning och rensa. Behörigheter för rollerna tilldelas i [center för säkerhet och kompatibilitet](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Skapa ett innehåll söka](https://docs.microsoft.com/office365/securitycompliance/content-search) efter meddelandet om du vill ta bort.
- [Ansluta till säkerhet och PowerShell regelefterlevnadscentret](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Om du använder autentisering på flera plan finns i [Anslut till Office 365 säkerhet och regelefterlevnad Center PowerShell använda autentisering på flera plan](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).