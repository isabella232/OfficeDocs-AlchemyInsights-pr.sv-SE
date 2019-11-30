---
title: Fastställande Office apps kunde inte hitta Office-licenser associerade meddelande
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
ms.openlocfilehash: 1820cdb83a1adf36b4e7d0898ecdf8097eb6f0f3
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627936"
---
# <a name="fixing-the-office-apps-couldnt-find-office-licenses-associated-message"></a>Åtgärda Office-appar "Det gick inte att hitta Office-licenser associerade" meddelande

Om det här meddelandet visas provar du följande:

1. Kontrollera brandväggen, antivirusprogrammet och proxyinställningarna för att bekräfta att de inte blockerar Internet-åtkomst till Office-appar. Se [Office 365-URL: er och IP-adressintervall](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Ta bort och [omtilldela Office-licensen](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) för den berörda användaren. 
3. Öppna en Office-app och [Logga ut](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) från alla befintliga användarkonton.
4. Gå till Windows-inställningar > **konton** > **e-& konton**och ta bort alla arbetskonton utom det berörda kontot.
5. Gå till Windows-inställningar > **konton** > **tillgång till arbete eller skola**och koppla från alla arbetskonton utom det berörda kontot.
6. Återställ aktiveringstillståndet för Office. [Läs mer](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Logga in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med det aktuella användarkontot.

Ytterligare felsökningslösningar finns [i olicensierade produkt-och aktiveringsfel i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).