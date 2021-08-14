---
title: SharePoint Anslutningsproblem i Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942043"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Anslutningsproblem i Designer 

Om SharePoint Designer har anslutningsproblem med SharePoint kan du prova följande vanliga lösningar.

Steg 1: Kontrollera att SharePoint Designer 2013 är uppdaterat med [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) och uppdateringen från den 2 augusti [2016 för SharePoint Designer 2013.](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)



Steg 2: Rensa de lokala cachefilerna:

1. Stäng SharePoint Designer 2013.

2. Ta bort alla filer som hittas i följande mappar på den lokala datorn.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Öppna SharePoint Designer 2013 och ange kontot igen för att se om det fungerar.

Steg 3: [Aktivera modern autentisering för Office 2013 på Windows enheter.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

Steg 4: Administratörer måste tillåta **egna** skript i SharePoint Admin Center-inställningarna för att tillåta SharePoint Designer. Mer information [finns i Tillåta eller](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) förhindra egna skript.


