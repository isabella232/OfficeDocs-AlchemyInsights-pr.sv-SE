---
title: Slutpunkt DLP har inte distribuerats till användarens enhet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731869"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>Slutpunkt DLP har inte distribuerats till användarens enhet

Om DLP-inställningen (Endpoint data loss prevention) inte har tillämpats på en användares enhet bekräftar du att du uppfyller följande krav:

- Windows 10 x64 version 1809 eller senare installeras på enheten.
- Klientversion mot skadlig programvara version 4.18.2009.7 eller senare installeras.
- Enheten är **något av** följande:
    
    - Azure Active Directory (AAD)-ansluten
    - Hybrid Azure AD-ansluten
    - AAD-registrerad

- För att tillämpa principåtgärder ser du till att Microsoft Chromium Edge-webbläsaren är installerad på slutpunktsenheten.

Ytterligare krav för distribution av slutpunkt DLP finns i Komma [igång med dataförlustskydd i slutpunkten.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)