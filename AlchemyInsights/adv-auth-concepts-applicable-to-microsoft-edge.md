---
title: Avancerade autentiseringskoncept som tillämpas på Microsoft Edge
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
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934383"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Avancerade autentiseringskoncept som tillämpas på Microsoft Edge

Här följer de avancerade autentiseringsbegreppen som gäller för Microsoft Edge:

**Proaktiv autentisering**

När du aktiverar [principen ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) försöker Microsoft Edge proaktivt autentisera inloggade användare via Microsoft-tjänster. Med jämna mellanrum används en onlinetjänst för att söka efter ett uppdaterat manifest som innehåller konfiguration som reglerar proaktiv autentisering.

Fördelar: Proaktiv autentisering aktiverar autentisering till nyckeltjänster, till exempel sidan Office ny flik. Om du Bing sökmotor förbättrar proaktiv autentisering adressfältets prestanda och genererar sökresultat som är anpassade efter behoven i ditt företag.

**Windows Hello CredUI för NTLM-autentisering**

Om enkel inloggning (SSO) inte är tillgänglig när en webbplats försöker logga in på användaren via NTLM- eller förhandlasmekanismen gör den här funktionen att användaren kan dela os-autentiseringsuppgifterna med webbplatsen och uppfylla autentiseringsutmaningen med hjälp av Windows Hello Cred UI. Det här inloggningsflödet visas bara i Windows 10 och bara för användare som inte får SSO under en NTLM- eller en förhandlans utmaning.

**Använd sparade lösenord för att logga in automatiskt**

Användare som sparar lösenord i Microsoft Edge kan aktivera automatisk inloggning på webbplatser där de har sparat autentiseringsuppgifter. Användare kan aktivera eller inaktivera den här funktionen i edge://settings/passwords, och du kan konfigurera den i [lösenordshanterarens](https://go.microsoft.com/fwlink/?linkid=2134622) principer.
