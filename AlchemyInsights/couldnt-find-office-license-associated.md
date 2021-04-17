---
title: Åtgärda meddelandet om att Microsoft 365-appar inte kunde hitta associerade Office-licenser
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816506"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Åtgärdar meddelandet "Det gick inte att hitta associerade Office-licenser" för Microsoft 365-programmen

Om du får det här meddelandet kan du prova följande:

1. Kontrollera brandväggen, antivirusprogrammet och proxyinställningarna för att kontrollera att de inte blockerar Internetåtkomsten till Microsoft 365-appar. Se [URL-adresser och IP-adressintervall för Microsoft 365.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
2. Ta bort [och omtilldela Office-licensen](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) för den aktuella användaren. 
3. Öppna ett Office-program [och logga ut](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) från befintliga användarkonton.
4. Gå till Windows Inställningar >  >  **e-&-postkonton** och ta bort alla arbetskonton utom det aktuella kontot.
5. Gå till Windows Inställningar > **Konton Åtkomst till** arbete eller skola  >  **och** koppla bort alla arbetskonton utom det aktuella kontot.
6. Återställ Office-aktiveringsstatusen. [Läs mer](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Logga in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med det aktuella användarkontot.

Ytterligare felsökningslösningar finns i [Office-felmeddelanden om olicensierad produkt och aktivering.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)