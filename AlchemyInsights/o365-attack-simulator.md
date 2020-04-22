---
title: 2681 Attack Simulator i Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713484"
---
# <a name="attack-simulator-in-microsoft-365"></a>Attack Simulator i Microsoft 365

- Saknar du Attack Simulator? Attack Simulator kräver **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** eller **Office 365 Enterprise E5**. Attack Simulator ingår **inte** i Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3 eller microsoft 365 Apps for business-prenumerationer.

- Kontot som du använder för att starta simulerade attacker kräver globala administratörs- eller säkerhetsadministratörsbehörigheter och MFA (Multifaktorautentisering). Mer information om attacksimulatorkrav finns i [det här avsnittet](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).

- Viktiga saker att veta om **Brute Force Password** attack simuleringar:

  - Om målkontot har MFA aktiverat och lösenordet gissades korrekt visas kontot inte som komprometterat (den andra autentiseringsfaktorn kommer att vara ofullständig).

  - Lösenordsfilen får inte vara större än 10 MB. Använd ett lösenord per rad och inkludera en tom rad (vagnretur) efter det sista lösenordet i listan.

- Viktiga saker att veta om **Spear Phishing** bifoga simuleringar:

  - Avsiktligt kan du inte ange ett anpassat värde för **webbloggningsserverns URL**.

  - Om en mottagare använder [tillägget Aktivera rapportmeddelande](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) för att rapportera meddelandet som nätfiske kanske du inte får aviseringar om meddelandet (eftersom det är en simulerad attack).

- Rapporter: När den simulerade attacken är klar kan du klicka på **Attackinformation** för att se rapporten.

- Detaljerade instruktioner och nya funktioner i Attack Simulator finns [i Attack Simulator i Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
