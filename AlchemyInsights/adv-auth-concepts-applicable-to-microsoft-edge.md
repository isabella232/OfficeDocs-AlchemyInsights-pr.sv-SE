---
title: Avancerade autentiseringsmetoder för Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573778"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Avancerade autentiseringsmetoder för Microsoft Edge

Nedan följer de avancerade autentiseringsmetoderna som gäller för Microsoft Edge:

**Proaktiv auktorisering**

När du aktiverar [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) -principen försöker Microsoft Edge proaktivt autentisera inloggade användare via Microsoft-tjänster. Med jämna mellanrum används en online tjänst för att söka efter ett uppdaterat manifest som innehåller konfigurationen som styr proaktiv-förauktoriseringen.

Fördelar: proaktivt-verifikation möjliggör till gång till viktiga tjänster, till exempel sidan ny flik i Office. Om Bing används som sökmotor förbättrar dessutom adress fältets prestanda och gör att Sök resultaten anpassas efter företagets behov?.

**Windows Hello-CredUI för NTLM-verifikation**

Om enkel inloggning (SSO) inte är tillgängligt när en webbplats försöker logga in användaren via NTLM eller Negotiate-mekanismen tillåter den här funktionen att användaren delar autentiseringsuppgifterna för operativ systemet med webbplatsen och för att uppfylla verifierings utmaningen genom att använda Windows Hello-gränssnittet. Det här inloggnings flödet visas bara i Windows 10 och endast för användare som inte behöver SSO under ett NTLM-eller Negotiate-anrop.

**Använda sparade lösen ord för att logga in automatiskt**

Användare som sparar lösen ord i Microsoft Edge kan aktivera automatisk inloggning på webbplatser där de har sparat sina autentiseringsuppgifter. Användare kan aktivera eller inaktivera den här funktionen i edge://settings/passwords och du kan konfigurera den i principer för [lösen ords hanteraren](https://go.microsoft.com/fwlink/?linkid=2134622) .
