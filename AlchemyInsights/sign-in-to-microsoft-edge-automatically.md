---
title: Logga in automatiskt till Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398747"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Logga in automatiskt till Microsoft Edge

Microsoft Edge använder operativsystemets standardkonto för att automatiskt logga in en användare enligt hur användarens enhet har konfigurerats. 

Scenarierna för varje typ av enhetskonfiguration och dess beroende inloggningsprocess för användare beskrivs nedan:

- **Enheten är hybrid/AAD-J:** Det här alternativet är tillgängligt på Windows 10, i Windows på nedåtnivå och i motsvarande serverversioner. Användare loggas automatiskt in med sina Azure Active Directory-konton (AD).
- **Enheten är domän ansluten:** Det här alternativet är tillgängligt i Windows 10, Windows på nedåtnivå och motsvarande serverversioner. Användare med domänkonton loggas som standard inte in automatiskt. för att aktivera automatisk inloggning för dem, använder du **policyn ConfigureOnPremisesAccountAutoSignIn.** Om du vill aktivera automatisk inloggning för användare med Azure AD-konton kan du överväga att koppla en hybrid-anslutning till deras enheter.
- **Operativsystemets standardkonto** är ett Microsoft-konto: Det här alternativet är tillgängligt på Windows 10 RS3 (version 1709, version 10.0.16299) och senare versioner. Det är osannolikt att scenariot förekommer på företagsenheter. Men om standardkontot för operativsystemet är ett Microsoft-konto loggar Microsoft Edge automatiskt in användaren med Microsoft-kontot.
 
 
