---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 839a70282b4dd619e9dbe8167ef0e409e468b1ad
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830600"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

Arbetar du med PowerShell eller skript i Sharepoint Online? Gå till länkarna nedan för mer information.
- [Komma igång med SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Ansluta till SPO PowerShell med multifaktorautentisering (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) innehåller ett bibliotek med PowerShell-kommandon som gör att du kan utföra komplexa hanteringsåtgärder mot SPO.

> [!NOTE]
> - Om du har problem med att ansluta med SPO-hanteringsgränssnittet kontrollerar du [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) att du har uppdaterat till den senaste versionen och försöker importera om modulen med hjälp av *"Import-Module Microsoft.Online.SharePoint.PowerShell".*
> - Om du försöker köra skript på klientsidans objektmodell måste du ha [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installerat på den lokala datorn.
> - Om du har problem med att köra skript från PowerShell kan du överväga att köra PowerShell som administratör och ändra [körningsprincipen.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)