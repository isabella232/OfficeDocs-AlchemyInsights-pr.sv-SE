---
title: Anslutningsproblem för SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051731"
---
# <a name="sharepoint-designer-connection-issues"></a>Anslutningsproblem för SharePoint Designer 

Om SharePoint Designer har anslutningsproblem till SharePoint-webbplatser kan du prova följande gemensamma lösningar.

Steg 1: Kontrollera att SharePoint Designer 2013 har uppdaterats med [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) och den [2 augusti 2016 uppdatering för SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Steg 2: rensa de lokala cachefilerna:

1. Stäng SharePoint Designer 2013.

2. Ta bort alla filer som finns i följande mappar på den lokala datorn.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Öppna SharePoint Designer 2013 och ange kontot igen för att se om det fungerar.

Steg 3: [Aktivera modern autentisering för Office 2013 på Windows-enheter](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Steg 4: administratörer måste **tillåta anpassade skript** i SharePoint Admin Center-inställningar för att tillåta SharePoint Designer-anslutningen. Mer information finns i [Tillåt eller förhindra anpassat skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .


