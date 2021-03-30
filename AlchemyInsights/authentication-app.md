---
title: Autentiseringsapp
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405682"
---
# <a name="authentication-app"></a>Autentiseringsapp

Om du är global administratör kan du snabbt ta reda på vad som har hänt eller diagnostisera problem relaterade till inloggning med [inloggningsdiagnostik.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Starta diagnostiken genom att klicka på knappen[Starta](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)diagnostik. 
1. Leta reda på händelsen du vill analysera genom att ange den information du har om användaren, programmet, tiden för inloggning, begärans-ID eller korrelations-ID.
1. Granska diagnostikresultatet som visar information om vad som har hänt och vilka åtgärder du kan vidta för att göra ändringar, om några ändringar behövs.

**Kontrollera det scenario som är tillämpligt:**

1. Om en användare inte får ett push-meddelande i Microsoft Authenticator-appen kontrollerar du att de inte visas under MFA-blockerade användare enligt beskrivningen i Blockera och tillåta [användare.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Om användaren inte blockeras för MFA men inte får ett push-meddelande kan de öppna appen Microsoft Authenticator, vilket hämtar väntande godkännandebegäranden.
1. Som alternativ inloggningsmetod kan användaren även klicka på Logga in på ett annat sätt och välja att använda en verifieringskod från min mobilapp.
1. Appen Microsoft Authenticator är den enda metoden för många användare. [Läs mer om standardinställningar för säkerhet](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), läs Vanliga frågor och svar om [Authenticator-appen](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) för vanliga frågor och hur du löser dem.
 
**Rekommenderade videor**

[Konfigurera Authenticator-appen på en ny telefon (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
