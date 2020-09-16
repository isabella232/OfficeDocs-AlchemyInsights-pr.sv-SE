---
title: Problem med SharePoint Designer
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
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727189"
---
# <a name="sharepoint-designer-connection-issues"></a>Problem med SharePoint Designer 

Om SharePoint-Designer har problem med anslutningen till SharePoint-webbplatser kan du försöka med följande vanliga lösningar.

Steg 1: kontrol lera att SharePoint Designer 2013 har uppdaterats med [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) och den [2 augusti 2016-uppdateringen för SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Steg 2: Rensa lokala cache-filer:

1. Stäng SharePoint Designer 2013.

2. På den lokala datorn tar du bort alla filer som finns i följande mappar.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Öppna SharePoint Designer 2013 och ange kontot igen för att se om det fungerar.

Steg 3: [Aktivera modern auktorisering för Office 2013 på Windows-enheter](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Steg 4: administratörer måste **tillåta anpassat skript** i inställningarna för SharePoint Admin Center för att tillåta SharePoint Designer-anslutningen. Se [Tillåt eller förhindra anpassat skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) för mer information.


