---
title: Åtgärda Office-appar Det gick inte att hitta associerat meddelande om office-licenser
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
ms.openlocfilehash: 565df0a05baa974a6cbac58ac6be8d78470dbc5d
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715650"
---
# <a name="fixing-the-office-apps-couldnt-find-office-licenses-associated-message"></a>Åtgärda meddelandet "Det gick inte att hitta associerade office-licenser"

Om du får det här meddelandet kan du prova följande:

1. Kontrollera brandväggen, antivirusprogrammet och proxyinställningarna för att bekräfta att de inte blockerar Internetåtkomst till Office-appar. Se [Microsoft 365-URL:er och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Ta bort och [tilldela office-licensen](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) för den berörda användaren. 
3. Öppna ett Office-program och [logga ut](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) från befintliga användarkonton.
4. Gå till Windows-inställningar > **Konton** > **e-post & konton**och ta bort alla arbetskonton utom det berörda kontot.
5. Gå till Windows-inställningar > **Konton** > **Access-arbete eller skola**och koppla från alla arbetskonton utom det berörda kontot.
6. Återställ aktiveringstillståndet för Office. [Läs mer](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Logga in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med det berörda användarkontot.

Ytterligare felsökningslösningar finns [i Olicensierade produkt- och aktiveringsfel i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).