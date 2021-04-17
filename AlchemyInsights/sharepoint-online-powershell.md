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
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="c8102-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="c8102-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="c8102-103">Arbetar du med PowerShell eller skript i Sharepoint Online?</span><span class="sxs-lookup"><span data-stu-id="c8102-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="c8102-104">Gå till länkarna nedan för mer information.</span><span class="sxs-lookup"><span data-stu-id="c8102-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="c8102-105">Komma igång med SharePoint Online Management Shell</span><span class="sxs-lookup"><span data-stu-id="c8102-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="c8102-106">Ansluta till SPO PowerShell med multifaktorautentisering (MFA)</span><span class="sxs-lookup"><span data-stu-id="c8102-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="c8102-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) innehåller ett bibliotek med PowerShell-kommandon som gör att du kan utföra komplexa hanteringsåtgärder mot SPO.</span><span class="sxs-lookup"><span data-stu-id="c8102-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="c8102-108">Om du har problem med att ansluta med SPO-hanteringsgränssnittet kontrollerar du [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) att du har uppdaterat till den senaste versionen och försöker importera om modulen med hjälp av *"Import-Module Microsoft.Online.SharePoint.PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="c8102-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="c8102-109">Om du försöker köra skript på klientsidans objektmodell måste du ha [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installerat på den lokala datorn.</span><span class="sxs-lookup"><span data-stu-id="c8102-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="c8102-110">Om du har problem med att köra skript från PowerShell kan du överväga att köra PowerShell som administratör och ändra [körningsprincipen.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)</span><span class="sxs-lookup"><span data-stu-id="c8102-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>