---
title: Teams för Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: c9c4eb811c93f6d11ebf606ba4bd20cddc2901d6616700ebfe6ef597dd8dc006
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940693"
---
# <a name="teams-add-in-for-mac"></a>Teams för Mac

Så här felsöker du Teams tillägg för Mac-operativsystemanvändare:

**Steg 1:** Om du har hybrid-Exchange lokalt (2016 CU3 eller senare krävs) använder du verktyget Test-HMA.ps1 för att bekräfta att modern hybridautentisering är korrekt konfigurerad. Mer information finns i Validera [modern hybridautentiseringskonfiguration för Outlook för iOS och Android.](https://aka.ms/TestHMAEAS)  

**Obs!** Använd UPN-adressformatet (till exempel [username@contoso.com](mailto:username@contoso.com)), inte domän\användarnamn. Gör detta även för användare Exchange Online postlådor.

**Steg 2:** Be användaren gå till **Verktygskonton**  >  ... i Outlook för Mac, och leta reda på och markera kontot. Bekräfta att användarnamnet som visas är i UPN-format (till exempel [username@contoso.com](mailto:username@contoso.com)).

**Steg 3:** Bekräfta att användaren är en licensierad Microsoft Teams användare. Användaren måste använda Office 365 Mac-prenumeration, produktversion 16.24 eller senare.