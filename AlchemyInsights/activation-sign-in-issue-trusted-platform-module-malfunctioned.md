---
title: Aktivering/inloggnings problem – Trusted Platform Module fungerar inte
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
- "3406"
- "9001429"
ms.openlocfilehash: 13e6fcd18047e511452f0180dc2e4677466d4db3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697539"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Att åtgärda Microsoft 365-apparna "din dators betrodda plattformsmodulen fungerar inte korrekt"

Lös problemet genom att prova med följande:

1. Öppna en Office-app och [logga ut](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) från befintliga användarkonton.   
2. Använda Windows- **Inställningar**  >  **konton**  >  **e-** postkonton & konton, ta bort befintliga arbets konton. 
3. Använda Windows- **Inställningar**  >  **konton**  >  **arbets-eller skol**anslutningar, koppla bort befintliga konton. 
4. Återställ Office-aktiveringsstatus. [Läs mer](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
).
5. Pröva [användar återställnings processen](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) för att åtgärda fel i TPM (Trusted Platform Module).