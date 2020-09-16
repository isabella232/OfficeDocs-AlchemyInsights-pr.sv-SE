---
title: Reparera Microsoft 365-appar det gick inte att hitta det kopplade meddelandet för Office-licenser
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747713"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Åtgärda meddelande om att Microsoft 365-apparna inte hittade Office-licenser

Om du får det här meddelandet kan du prova följande:

1. Kontrol lera brand vägg, antivirus program och proxyinställningar för att bekräfta att de inte blockerar Internet åtkomst till Microsoft 365-appar. Se [Microsoft 365 URL: er och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Ta bort och [tilldela om Office-licensen](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) för den aktuella användaren. 
3. Öppna ett Office-program och [Logga ut](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) från befintliga användar konton.
4. Gå till Windows-inställningar > **konton**  >  **& konton**och ta bort alla arbets konton förutom det berörda kontot.
5. Gå till Windows-inställningar > **konton**  >  **åtkomst till arbets-eller skol arbete**och koppla från alla arbets konton förutom det berörda kontot.
6. Återställ Office-aktiveringsstatusen. [Läs mer](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Logga](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) in med det användar konto som påverkas.

Ytterligare lösningar för fel sökning finns i [olicensierad produkt och aktiverings fel i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).