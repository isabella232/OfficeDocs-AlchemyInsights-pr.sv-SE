---
title: Skriv bords versionen av Outlook eller ersätta ett e-postmeddelande
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
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664008"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Återkalla eller ersätta ett e-postmeddelande i Outlook

- Som administratör kan du **återkalla meddelanden åt användare med hjälp av PowerShell**. Du kan inte återkalla meddelanden från administrations centret.
- Du kan **bara återkalla meddelanden som skickas till personer i organisationen**. Om meddelandet skickades till en Gmail-adress, till exempel, kan du inte återkalla det.
- Du kan **bara återkalla meddelanden som skickats från Outlook 2016 på datorn**. Om en användare skickar ett meddelande med hjälp av Outlook för Mac eller Outlook på webben kan du inte återkalla det.

Så här återkallar eller ersätter du ett e-postmeddelande:

1. I mappfönstret till vänster i Outlook-fönstret väljer du mappen skickat.
1. Dubbelklicka på det meddelande som du vill återkalla för att öppna det.
1. Välj fliken **meddelande** och sedan **åtgärder**  >  **återkalla detta meddelande**.
1. Välj **ta bort olästa exemplar av detta meddelande** eller **ta bort olästa exemplar och ersätta med ett nytt meddelande**och välj sedan **OK**.
1. Om du skickar ett ersättnings meddelande skriver du meddelandet och väljer sedan **Skicka**.
1. Om du har problem med att återkalla meddelanden beror det på mottagarens inställningar i Outlook. Anvisningar för hur du kontrollerar åter kallelsen finns i [den här artikeln](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Söka efter och ta bort e-postmeddelanden i din organisation

- Om du inte är global administratör måste ditt konto läggas till i eDiscovery Manager-rollen eller för Sök hanterings rollen efterlevnad för att söka efter meddelanden. Om du vill ta bort meddelanden måste du gå med i roll gruppen organisations hantering eller rollen för sökning och rensning. Behörigheter för dessa roller är tilldelade i [säkerhets-och kompatibilitetstillstånd](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Skapa en innehålls sökning](https://docs.microsoft.com/microsoft-365/compliance/content-search) för att hitta meddelandet som ska tas bort.
- [Anslut till säkerhets-och Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Om du använder multifaktorautentisering läser du [ansluta till Microsoft 365 Security och Compliance Center PowerShell med multifaktorautentisering](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).