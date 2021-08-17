---
title: Har användarna fått skadlig e-post
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 608e2226c055f58ecf4f62e3c913106a6d319190ed6b317508e41514c12ba5d0
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57893421"
---
# <a name="did-your-users-receive-malicious-email"></a>Har användarna fått skadlig e-post?

Du kan nu rapportera skadlig e-post till Microsoft med [hjälp av inskickade meddelanden Microsoft 365 Defender portal](https://sip.security.microsoft.com/reportsubmission?viewid=admin).

Meddelanden som skickas i [administrationsinskick genomsöks](https://security.microsoft.com/reportsubmission?viewid=admin) och följande resultat visas i den utfällkommning som visas:

- Om avsändarens e-postautentisering misslyckades vid leveransen.
- Information om politiska träffar som kan ha påverkat eller åsidosatt bedömningen av ett meddelande.
- Aktuella detonationsresultat för att se om webbadresserna eller filerna i meddelandet var skadliga eller inte.
- Feedback från klassare

Om en åsidosättning hittades bör omskanningen slutföras på några minuter. Om det inte uppstod något problem med e-postautentisering eller om leveransen inte påverkades av en åsidosättning, kan det ta upp till en dag för feedbacken från klasserna.

Om du inte håller med den slutliga domen om ett meddelande, URL eller fil (blockerad kontra inte blockerad), skicka meddelandet igen efter en dag för att skanna igen. Sannolikheten är stor för att domen skulle förändras efter att ha skickat meddelandet igen.

Under tiden kan du ta bort skadlig e-post från användarnas inkorgar genom att följa anvisningarna [i den här artikeln](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Kunder med Microsoft Defender för Office 365 kan:
  - Använda [Hotutforskaren för att hitta och ta bort misstänkta e-postmeddelanden](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [Använda Valv för att blockera åtkomst till](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links) en skadlig URL
  - Spåra användare som har klickat på och åtkomst till skadliga URL:er: Visa nätfiske-URL och [klicka på bedömningsdata](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)  &  [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - Starta [en automatiserad undersökning manuellt](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Du kan också skydda mot skadliga filer och URL-adresser genom att följa anvisningarna i [Skydd mot skadliga URL:er och filer](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).
