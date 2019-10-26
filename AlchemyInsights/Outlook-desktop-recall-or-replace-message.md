---
title: Outlook-skrivbordet återkalla eller ersätta ett e-postmeddelande
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
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/25/2019
ms.locfileid: "36496129"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Återkalla eller ersätta ett Outlook-e-postmeddelande

- Som administratör kan du **återkalla meddelanden för användare med hjälp av PowerShell**. Du kan inte återkalla meddelanden från administratörscenter.
- Du kan **bara återkalla meddelanden som skickas till personer i din organisation**. Om meddelandet skickades till en Gmail-adress kan du till exempel inte återkalla det.
- Du kan **bara återkalla meddelanden som skickats från Outlook 2016 på datorn**. Om en användare skickar ett meddelande med Outlook för Mac eller Outlook på webben kan du inte återkalla det.

Så här återkallar eller ersätter du ett e-postmeddelande:

1. I mappfönstret till vänster i Outlook-fönstret väljer du mappen skickat.
1. Dubbelklicka på det meddelande som du vill återkalla för att öppna det.
1. Välj fliken **meddelande** och välj sedan **åtgärder** > **återkalla det här meddelandet**.
1. Välj **ta bort olästa kopior av det här meddelandet** eller **ta bort olästa kopior och Ersätt med ett nytt meddelande**och välj sedan **OK**.
1. Om du skickar ett ersättnings meddelande skriver du meddelandet och väljer sedan **Skicka**.
1. Lyckade eller misslyckade återkallningar av ett meddelande beror på mottagarens inställningar i Outlook. Anvisningar om hur du kontrollerar återkallningen finns i [den här artikeln](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Sök efter och ta bort e-postmeddelanden i din organisation

- Om du inte är global administratör måste ditt konto läggas till i rollen eDiscovery Manager-roll eller efterlevnadshantering för att söka efter meddelanden. Om du vill ta bort meddelanden måste du gå med i rollgruppen Organisationshantering eller rollen Sök-och rensnings hantering. Behörigheter för dessa roller tilldelas i säkerhets- [och Efterlevnadscenter](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Skapa en innehållssökning](https://docs.microsoft.com/office365/securitycompliance/content-search) för att hitta meddelandet att ta bort.
- [Anslut till Security och Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Om du använder multifaktorautentisering, se [ansluta till Office 365 Security och Compliance Center PowerShell med multifaktorautentisering](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).