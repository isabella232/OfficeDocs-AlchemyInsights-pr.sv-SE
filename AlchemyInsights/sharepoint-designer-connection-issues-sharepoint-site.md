---
title: Behörighetsnivåer för SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760710"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer-anslutningsproblem 

Om SharePoint Designer har uppstått anslutningsproblem med till SharePoint-webbplatser, försök följande vanliga lösningar.

Steg 1: Verifiera SharePoint Designer har uppdaterats.

- [SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [SharePoint Designer servicepack 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [Uppdatering för SharePoint Designer 2013 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

Steg 2: Ta bort lokala cachefiler

- Stäng SharePoint Designer 2013.

- Bläddra till följande mappar att ta bort cachelagrade filer på den lokala datorn.

- Klicka på Start, kör och ta bort alla filer som finns under var och en av de nedan platser.

%APPDATA%\Microsoft\Web server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

Öppna SharePoint Designer 2013 och ange konto igen för att se om det fungerar.

Steg 3: [Aktivera moderna autentisering för Office 2013 på Windows-enheter](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

Steg 4: Administratörer behöver du tillåta anpassat skript så att SharePoint Designer-anslutning.

Detaljerade anvisningar, exempel och överväganden finns [Tillåt eller förhindra att skriptet](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


