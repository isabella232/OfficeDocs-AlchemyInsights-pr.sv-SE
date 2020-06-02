---
title: Återkalla eller ersätta ett e-postmeddelande i Outlook Desktop
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: bb84363ae7d3c91750d5de789c091c7cebbbedc2
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502337"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Återkalla eller ersätta ett Outlook-e-postmeddelande

- Som administratör kan du **återkalla meddelanden för användare som använder PowerShell**. Du kan inte återkalla meddelanden från administrationscentret.
- Du kan **bara återkalla meddelanden som skickas till personer i organisationen**. Om meddelandet till exempel skickades till en Gmail-adress kan du inte komma ihåg det.
- Du kan **bara återkalla meddelanden som skickas från Outlook 2016 på datorn**. Om en användare skickar ett meddelande med Outlook för Mac eller Outlook på webben kan du inte återkalla det.

Så här återkallar eller ersätter du ett e-postmeddelande:

1. Välj mappen Skickat i mappfönstret till vänster om Outlook-fönstret.
1. Dubbelklicka på meddelandet som du vill återkalla för att öppna det.
1. Markera fliken **Meddelande** och välj sedan **Åtgärder**  >  **återkalla det här meddelandet**.
1. Välj **Ta bort olästa kopior av meddelandet** eller Ta bort **olästa kopior och ersätt med ett nytt meddelande**och välj sedan **OK**.
1. Om du skickar ett ersättningsmeddelande skriver du meddelandet och väljer sedan **Skicka**.
1. Hur ett meddelande återkallas eller misslyckas beror på mottagarens inställningar i Outlook. Steg för att kontrollera återkallandet finns i den [här artikeln](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Söka efter och ta bort e-postmeddelanden i organisationen

- Om du inte är global administratör måste ditt konto läggas till i rollen eDiscovery Manager eller hanteringsrollen för efterlevnadssökning för att söka efter meddelanden. Om du vill ta bort meddelanden måste du gå med i rollgruppen Organisationshantering eller hanteringsrollen Sök och rensa. Behörigheter för dessa roller tilldelas i [säkerhets- och efterlevnadscentret](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Skapa en innehållssökning](https://docs.microsoft.com/microsoft-365/compliance/content-search) för att hitta meddelandet som ska tas bort.
- [Anslut till Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Om du använder multifaktorautentisering läser du [Anslut till Microsoft 365 security and Compliance Center PowerShell med multifaktorautentisering](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).