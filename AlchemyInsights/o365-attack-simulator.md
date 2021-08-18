---
title: 2681 Attack Attack in Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: f6e221cc82a1b707f6acc457cb78db743521d859
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325089"
---
# <a name="attack-simulator-in-microsoft-365"></a>Attack Attack i Microsoft 365

- Saknar du Attack Attack? Attack Attack Attack kräver **Microsoft Defender för Office 365 abonnemang 2** eller Office 365 Enterprise **E5.** Attack Attack Attack **ingår inte** i Microsoft Defender för Office 365 abonnemang 1, Office 365 Enterprise E3 eller andra Microsoft 365-applikationer för affärsverksamhet prenumerationer.

- Det konto du använder för att starta simulerade attacker kräver global administratör eller säkerhetsadministratörsbehörighet och multifaktorautentisering (MFA). Mer information om attackkraven finns i det [här avsnittet.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)

- Viktiga saker att veta om **Råstyrt lösenord-attack** simuleringar:

  - Om målkontot har MFA aktiverat och lösenordet gissades rätt visas inte kontot som komprometterat (den andra autentiseringsfaktorn är ofullständig).

  - Lösenordsfilen får inte vara större än 10 MB. Använd ett lösenord per rad och ta med en tom rad (vagnretur) efter det sista lösenordet i listan.

- Viktiga saker att veta om **simuleringar av nätfiske:**

  - Som design kan du inte ange ett anpassat värde för URL för **nätfiskeinloggningsserver.**

  - Om en mottagare [](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) använder tillägget Aktivera rapportmeddelandet för att rapportera meddelandet som nätfiske kanske du inte får aviseringar om meddelandet (eftersom det är en simulerad attack).

- Rapporter: När den simulerade attacken är slutförd kan du klicka på **Attackinformation** för att se rapporten.

- Detaljerade instruktioner och nya funktioner i Attack Attack Attack finns i [Attack Attack in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
