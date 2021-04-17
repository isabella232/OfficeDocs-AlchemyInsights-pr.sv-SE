---
title: Problem med inloggning på Microsoft 365-appar
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 02841a1b4e92eec94fc6409941d91618f02518c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836621"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Problem med inloggning på Microsoft 365-appar

Prova följande alternativ på den aktuella datorn för att åtgärda inloggningsproblem med Microsoft 365-appar:  

- Windows finns i [Rekommendationer för att lösa vanliga inloggningsproblem](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- För Mac, se  [Det går inte att logga in på ett Office 2016 för Mac-program](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Tips** På Windows-datorer kan vi diagnostisera och automatiskt korrigera flera vanliga inloggningsproblem för Office åt dig. Ladda ned och kör **[Support- och återställningsassistenten](https://aka.ms/SaRA-OfficeSignInScenario)** om du vill använda vårt automatiska verktyg.

**Obs!** Du bör inte inaktivera ADAL (Modern Authentication) eller Web Account Management (WAM) för att åtgärda inloggnings- eller **aktiveringsproblem.** Om felen uppstår när du ansluter till Microsoft 365 med Office 2013 bör du aktivera [modern autentisering](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  för Office-klienten.

Specifika felsökningsåtgärder finns i:

[Anslutningsproblem vid inloggning efter uppdatering av Office 2016 build 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Du kan inte logga in på ditt organisationskonto, till exempel Office 365, Azure eller Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Felsöka appar som inte är webbläsarbaserade och som inte kan logga in på Office 365, Azure eller Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Uppmanas upprepade gånger att ange autentiseringsuppgifter i Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)