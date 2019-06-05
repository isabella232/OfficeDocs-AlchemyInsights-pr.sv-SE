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
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716909"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer-anslutningsproblem 

<p>Om SharePoint Designer har uppstått anslutningsproblem med till SharePoint-webbplatser, försök följande vanliga lösningar.</p> <p><strong>Steg 1:</strong> <strong>Verifiera SharePoint Designer uppdateras&nbsp; </strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">SharePoint Designer servicepack 1 (SP1)</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">Uppdatering för SharePoint Designer 2013 (KB3114721)</a></li> </ul> <p><strong>Steg 2:</strong> <strong>Ta bort lokala cachefiler</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">Stäng SharePoint Designer 2013.&nbsp;</li> <li style="font-weight: 400;">Bläddra till följande mappar att ta bort cachelagrade filer på den lokala datorn.&nbsp;</li> <li style="font-weight: 400;">Klicka på <strong>Start -&gt; kör</strong> och ta bort alla filer som hittats under var och en av de under platser.&nbsp;<br /><br />%APPDATA%\Microsoft\Web server Extensions\Cache<br />%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">Öppna SharePoint Designer 2013 och ange konto igen för att se om det fungerar.</li> </ol> <p><strong>Steg 3:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide"> <strong>Aktivera moderna autentisering för Office 2013 på Windows-enheter</strong></a>&nbsp;</p> <p><strong>Steg 4:</strong> <strong>Administratörer behöver för att tillåta anpassat skript så att SharePoint Designer-anslutning</strong>.</p> <p>Detaljerade anvisningar, exempel och överväganden finns <a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">Tillåt eller förhindra att skriptet</a>.&nbsp;</p>


