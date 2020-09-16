---
title: 2681 angrepps Simulator i Microsoft 365
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
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759237"
---
# <a name="attack-simulator-in-microsoft-365"></a>Angrepps Simulator i Microsoft 365

- Saknar du angrepps Simulator? För angrepps Simulator krävs **office 365 Advanced Threat Protection Plan 2 (ATP-abonnemang 2)** eller **Office 365 Enterprise E5**. Angrepps Simulator ingår **inte** i Office 365 Avancerat skydds abonnemang 1 (ATP-abonnemang 1), Office 365 Enterprise E3 eller något Microsoft 365-program för Business-prenumerationer.

- Det konto som du använder för att starta simulerade attacker kräver den globala administratören eller säkerhets administratören och multifaktorautentisering. Mer information om krav för attack simulatorn finns i [det här avsnittet](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Viktiga saker du bör veta om att simulering av **lösen ords attacker är brutet** :

  - Om det finns MFA aktiverat för mål kontot och lösen ordet har gissats till är det inte säkert att kontot påverkas (den andra autentiseringsprocessen är ofullständigt).

  - Lösen ords filen får inte vara större än 10 MB. Använd ett lösen ord per rad och inkludera en tom rad (rad matning) efter det senaste lösen ordet i listan.

- Viktiga saker du bör veta om **Spear nät fiske** :

  - Efter design kan du inte ange ett anpassat värde för **URL-adressen till nätfiske-inloggningen**.

  - Om en mottagare använder [tillägget aktivera rapport meddelande](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) om du vill rapportera meddelandet som nätfiske kanske du inte får aviseringar om meddelandet (eftersom det är ett simulerat angrepp).

- Rapporter: när det simulerade angreppet är slutfört kan du klicka på **angrepps information** för att visa rapporten.

- Detaljerade instruktioner och nya funktioner i angrepps Simulator finns i [angrepps Simulator i Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
