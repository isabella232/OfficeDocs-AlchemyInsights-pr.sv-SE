---
title: Logga in i Microsoft Edge automatiskt
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
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678817"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Logga in i Microsoft Edge automatiskt

Microsoft Edge använder operativ systemets standard konto för att automatiskt logga in en användare baserat på hur användarens enhet är konfigurerad. 

Scenarierna för varje typ av enhets konfiguration och inloggnings process som tillhör ande användare beskrivs nedan:

1. **Enheten är hybrid/AAD-J**: det här alternativet är tillgängligt i Windows 10, Windows och motsvarande Server versioner. Användarna loggas automatiskt in med sina Azure Active Directory (AD)-konton.
2. **Enheten är** domänansluten: det här alternativet är tillgängligt i Windows 10, i Windows och motsvarande Server versioner. Som standard är användare med domän konton inte inloggade automatiskt; Använd **ConfigureOnPremisesAccountAutoSignIn** policy för att aktivera automatisk inloggning för dem. För att aktivera automatisk inloggning för användare med Azure AD-konton kan du välja att hybrid-ansluter till sina enheter.
3. **Operativ systemets standard konto är ett Microsoft-konto**: det här alternativet är tillgängligt på Windows 10 RS3 (version 1709, build 10.0.16299) och senare versioner. Det är osannolikt att scenariot inträffar på företags enheter. Om operativ systemets standard konto är ett Microsoft-konto loggar Microsoft Edge automatiskt in användaren med Microsoft-kontot.
 
 
