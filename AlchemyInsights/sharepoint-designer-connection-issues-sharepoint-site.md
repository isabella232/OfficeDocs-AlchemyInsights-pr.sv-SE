---
title: Anslutningsproblem med SharePoint Designer
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
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511562"
---
# <a name="sharepoint-designer-connection-issues"></a>Anslutningsproblem med SharePoint Designer 

Om Det finns anslutningsproblem med SharePoint Designer på SharePoint-webbplatser kan du prova följande vanliga lösningar.

Steg 1: Kontrollera att SharePoint Designer 2013 har uppdaterats med [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) och [den 2 augusti 2016-uppdateringen för SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Steg 2: Rensa de lokala cachefilerna:

1. Stäng SharePoint Designer 2013.

2. På den lokala datorn tar du bort alla filer som finns i var och en av följande mappar.

    - %APPDATA%\Microsoft\Webbservertillägg\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Lokal\Microsoft\WebbplatsCache

3. Öppna SharePoint Designer 2013 och ange kontot igen för att se om det fungerar.

Steg 3: [Aktivera modern autentisering för Office 2013 på Windows-enheter](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Steg 4: Administratörer måste **tillåta anpassade skript** i SharePoint Admin Center-inställningarna för att tillåta SharePoint Designer-anslutningen. Mer information finns i [Tillåt eller förhindra anpassat skript.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


