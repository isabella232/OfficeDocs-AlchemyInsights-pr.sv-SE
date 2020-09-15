---
title: Problem med att logga in i Microsoft 365-appar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: da1437ae8b09139b531deb8930d5648f908fae93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677008"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Problem med att logga in på Microsoft 365-appar

För att åtgärda inloggnings problem med Microsoft 365-appar kan du försöka med följande alternativ på den påverkade datorn:  

- För Windows, se [rekommendationer för att åtgärda vanliga inloggnings problem](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- För Mac kan  [du läsa det går inte att logga in i en Office 2016 för Mac-App](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Obs!**  **Det rekommenderas inte**att inaktivera modern INLOGGNINGSAUTENTISERING (ADAL) eller Web Account Management (WAM) för att åtgärda inloggnings-eller aktiverings problem. Om felen uppträder när du ansluter till Microsoft 365 med Office 2013 kontrollerar du att du [aktiverar modern auktorisering](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  för Office-klienten.

Specifika fel söknings åtgärder finns i:

[Anslutningsproblem vid inloggning efter uppdatering av Office 2016 build 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Det går inte att logga in på ditt organisations konto, till exempel Office 365, Azure eller Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Felsöka program som inte är webbläsare som inte kan logga in på Office 365, Azure eller Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Upprepade gånger ombeds att ange autentiseringsuppgifter i Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)