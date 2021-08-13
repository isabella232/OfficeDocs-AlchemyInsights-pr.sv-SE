---
title: Outlook Återkalla eller ersätta ett e-postmeddelande på skrivbordet
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918413"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Återkalla eller ersätta ett e Outlook meddelande

- Som administratör kan du återkalla **meddelanden åt användare med hjälp av PowerShell.** Du kan inte återkalla meddelanden från administrationscentret.
- Du kan **bara återkalla meddelanden som skickas till personer i din organisation.** Om meddelandet till exempel skickades till en Gmail-adress kan du inte återkalla den.
- Du kan **bara återkalla meddelanden som skickats Outlook 2016 på datorn.** Om en användare skickar ett meddelande med Outlook för Mac eller Outlook på webben kan du inte återkalla det.

Så här återkallar eller ersätter du ett e-postmeddelande:

1. I mappfönstret till vänster i Outlook väljer du mappen Skickat.
1. Dubbelklicka på det meddelande som du vill återkalla för att öppna det.
1. Välj fliken **Meddelande** och välj sedan Åtgärder **Återkalla**  >  **detta meddelande.**
1. Välj **Ta bort olästa exemplar av detta meddelande** eller Ta bort **olästa exemplar och ersätta med ett** nytt meddelande och välj sedan **OK**.
1. Om du skickar ett ersättningsmeddelande skriver du meddelandet och väljer sedan **Skicka**.
1. Om det går att återkalla ett meddelande eller inte beror på mottagarens inställningar i Outlook. Information om hur du kontrollerar återkallelsen finns i [den här artikeln.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

Söka efter och ta bort e-postmeddelanden i din organisation

- Om du inte är global administratör måste ditt konto läggas till i rollen eDiscovery Manager eller rollen för efterlevnadssökning för att söka efter meddelanden. Om du vill ta bort meddelanden måste du gå med i rollgruppen Organisationshantering eller rollen för hantering av sökning och rensning. Behörigheter för de här rollerna tilldelas i [Säkerhets- och efterlevnadscenter.](https://go.microsoft.com/fwlink/?linkid=2083731)
- [Skapa en innehållssökning för](https://docs.microsoft.com/microsoft-365/compliance/content-search) att hitta det meddelande du vill ta bort.
- [Anslut till PowerShell för säkerhet- och efterlevnadscenter.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)

Om du använder multifaktorautentisering kan du Anslut till Microsoft 365 PowerShell för säkerhet och [efterlevnad med multifaktorautentisering.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)