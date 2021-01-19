---
title: Inloggnings fel för användare
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7790"
- "9004355"
ms.openlocfilehash: 05bd31cb4afecf1342e040eecd9e58cd38bd8d49
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901252"
---
# <a name="user-sign-in-errors"></a>Inloggnings fel för användare

**Lösa problem med inloggnings diagnosen**

Utför följande steg för att upptäcka orsaken till att problem som är relaterade till inloggning för användare identifieras:

1. Starta [inloggnings diagnosen](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Hitta den händelse du vill analysera genom att ange informationen du har om användaren, programmet, tiden för inloggning, begärande-ID eller korrelations-ID.
3. Granska de diagnostiska resultaten som visar information om vad som hände och vilka åtgärder du kan vidta för att göra ändringar, om det behövs.

**Letar du efter information om AADSTS-felkoderna som returneras från Azure Active Directory (Azure AD) säkerhetstokentjänst?** Läs [den här artikeln](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) för att hitta AADSTS fel beskrivningar, korrigeringar och vissa föreslagna lösningar