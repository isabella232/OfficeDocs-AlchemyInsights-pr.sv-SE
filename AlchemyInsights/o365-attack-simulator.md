---
title: 2681 attack Simulator i Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305349"
---
# <a name="attack-simulator-in-office-365"></a>Attack Simulator i Office 365

- Saknar du attack Simulator? Attack Simulator kräver **office 365 Advanced Threat Protection Plan 2 (ATP-plan 2)** eller **Office 365 Enterprise E5**. Attack Simulator ingår **inte** i Office 365 Advanced Threat Protection Plan 1 (ATP-plan 1), Office 365 Enterprise E3 eller Office 365 Business-prenumerationer.

- Det konto som du använder för att starta simulerade attacker kräver global administratör eller säkerhets administratörsbehörighet och multifaktorautentisering (MFA). Mer information om krav för attack Simulator finns i [det här avsnittet](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).

- Viktiga saker att veta om **brute force lösenord** attack simuleringar:

  - Om målkontot har MFA aktiverat och lösenordet gissades korrekt, visas kontot inte som komprometterad (den andra autentiseringsfaktorn blir ofullständig).

  - Lösenordsfilen får inte vara större än 10 MB. Använd ett lösenord per rad och inkludera en tom rad (vagnretur) efter det sista lösenordet i listan.

- Viktiga saker att veta om **spjut phishing** bifoga simuleringar:

  - Du kan inte ange ett anpassat värde för URL för **phishing-inloggningserver**.

  - Om en mottagare använder den [Aktivera rapportmeddelande tillägget](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) för att rapportera meddelandet som nätfiske, kanske du inte får aviseringar för meddelandet (eftersom detta är en simulerad attack).

- Rapporter: när den simulerade attacken är klar kan du klicka på **attack Detaljer** för att se rapporten.

- Detaljerade instruktioner och nya funktioner i attack Simulator finns i [attack Simulator i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
