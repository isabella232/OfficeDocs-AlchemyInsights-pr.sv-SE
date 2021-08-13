---
title: Problem med aktivering/inloggning – fel i modulen för betrodd plattform
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
- "3406"
- "9001429"
ms.openlocfilehash: 90fc3135dcde5073330abb7cfe0e45c799e2154d9cd27c075c2c9ac89c18a641
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53937299"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Åtgärda meddelandet Microsoft 365 om att datorns modul för betrodd plattform inte fungerar korrekt

Lös problemet genom att prova med följande:

1. Öppna en Office-app och [logga ut](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) från befintliga användarkonton.   
2. Med Windows **Inställningar**  >  **e-postkonton**  >  **& ta bort** befintliga arbetskonton. 
3. Med Windows **Inställningar**  >  **åtkomst till konton**  >  **(arbete eller skola) kopplas befintliga** konton bort. 
4. Återställ Office-aktiveringsstatus. [Läs mer](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
).
5. Prova [återställningsprocessen för användare för](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) att åtgärda TPM-fel (Trusted Platform Module).