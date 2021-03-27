---
title: Avancerade autentiseringsbegrepp som är tillämpliga i Microsoft Edge
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
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398603"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Avancerade autentiseringsbegrepp som är tillämpliga i Microsoft Edge

Här följer de avancerade autentiseringsbegreppen som gäller för Microsoft Edge:

**Proaktiv autentisering**

När du aktiverar [principen ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) försöker Microsoft Edge proaktivt autentisera inloggade användare via Microsoft-tjänster. Med jämna mellanrum används en onlinetjänst för att söka efter ett uppdaterat manifest som innehåller konfiguration som reglerar proaktiv autentisering.

Fördelar: Proaktiv autentisering möjliggör autentisering till nyckeltjänster, till exempel sidan Ny flik i Office. Om Bing används som sökmotor förbättrar proaktiv autentisering prestandan i adressfältet och hjälper till att generera sökresultat som är anpassade efter behoven i ditt företag.

**Windows Hello CredUI för NTLM-autentisering**

Om enkel inloggning (SSO) inte är tillgänglig när en webbplats försöker logga in på användaren via NTLM- eller förhandlasmekanismen gör den här funktionen att användaren kan dela operativsystemets autentiseringsuppgifter med webbplatsen och uppfylla autentiseringsutmaningen med hjälp av windows Hello-gränssnittet i Cred. Det här inloggningsflödet visas bara i Windows 10 och bara för användare som inte får SSO under en NTLM- eller en förhandlans utmaning.

**Använd sparade lösenord för att logga in automatiskt**

Användare som sparar lösenord i Microsoft Edge kan aktivera automatisk inloggning på webbplatser där de har sparat autentiseringsuppgifter. Användare kan aktivera eller inaktivera den här funktionen i edge://settings/passwords, och du kan konfigurera den i [lösenordshanterarens](https://go.microsoft.com/fwlink/?linkid=2134622) principer.
