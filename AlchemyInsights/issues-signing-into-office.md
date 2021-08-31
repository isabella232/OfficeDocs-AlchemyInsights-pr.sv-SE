---
title: Problem med att logga in Microsoft 365 appar
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
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744664"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Problem med inloggning på Microsoft 365-applikationer

Obs! Om du använder en äldre version av Windows (t.ex. Windows 7 SP1, Windows Server 2008 R2) använder du den enkla [korrigeringen](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) för att aktivera TLS 1.2 som standard. Mer information finns i Uppdatering för att aktivera [TLS 1.1 och TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)som standard säkra protokoll i WinHTTP i Windows.

För att åtgärda inloggningsproblem med Microsoft 365-appar kan du försöka med följande alternativ på den berörda datorn:  

- Mer Windows finns [Rekommendationer hur du löser vanliga inloggningsproblem](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- För Mac, se [Det går inte att logga in på en Office 2016 för Mac program](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Tips** På Windows-datorer kan vi diagnostisera och automatiskt korrigera flera vanliga inloggningsproblem för Office åt dig. Ladda ned och kör **[Support- och återställningsassistenten](https://aka.ms/SaRA-OfficeSignInScenario)** om du vill använda vårt automatiska verktyg.

**Obs!** Du bör inte inaktivera ADAL (Modern Authentication) eller Web Account Management (WAM) för att åtgärda inloggnings- eller **aktiveringsproblem.** Om felen uppstår när du ansluter till en Microsoft 365 med Office 2013 bör du aktivera [modern](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) autentisering för Office klient.

Specifika felsökningsåtgärder finns i:

[Anslutningsproblem vid inloggning efter uppdatering av Office 2016 build 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Du kan inte logga in på ditt organisationskonto, till exempel Office 365, Azure eller Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Felsöka appar som inte är webbläsarbaserade och som inte kan logga in på Office 365, Azure eller Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Uppmanas upprepade gånger att ange autentiseringsuppgifter i Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)