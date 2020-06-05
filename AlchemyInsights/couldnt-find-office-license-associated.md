---
title: Åtgärda Microsoft 365-appar Kunde inte hitta associerat meddelande om office-licenser
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 65ffae1a784f841cb08a5df52b02671a4526d9d4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580459"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Åtgärda meddelandet "Det gick inte att hitta associerade office-licenser" i Microsoft 365-apparna

Om du får det här meddelandet kan du prova följande:

1. Kontrollera brandväggen, antivirusprogrammet och proxyinställningarna för att bekräfta att de inte blockerar Internetåtkomst till Microsoft 365-appar. Se [Microsoft 365-URL:er och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Ta bort och [tilldela office-licensen](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) för den berörda användaren. 
3. Öppna ett Office-program och [logga ut](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) från befintliga användarkonton.
4. Gå till Windows-inställningar **Accounts**>  >  **Konton e-& konton**och ta bort alla arbetskonton utom det berörda kontot.
5. Gå till Windows-inställningar > **Konton**  >  **Access-arbete eller skola**och koppla från alla arbetskonton utom det berörda kontot.
6. Återställ Office-aktiveringsstatusen. [Läs mer](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Logga in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med det berörda användarkontot.

Ytterligare felsökningslösningar finns [i Olicensierade produkt- och aktiveringsfel i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).