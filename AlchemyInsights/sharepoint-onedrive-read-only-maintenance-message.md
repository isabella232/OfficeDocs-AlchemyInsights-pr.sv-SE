---
title: Skrivskyddad för underhåll meddelande när du försöker använda SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051299"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Skrivskyddad för underhåll meddelande när du försöker använda SharePoint eller OneDrive

Användare kan få en **skrivskyddad för underhåll** meddelande när du försöker använda SharePoint eller OneDrive för något av följande scenarier. 

-   En planerad eller aktiv underhållsaktivitet.  Sök efter dem genom att navigera till [meddelandecentret](https://portal.office.com/adminportal/home#/messagecenter).
-   En hög prioritet, aktiv tjänst incident som kan inträffa. Kontrollera om det finns några bulletiner/incidenter genom att navigera till [tjänstens hälsa](https://portal.office.com/adminportal/home#/servicehealth).
-   En mindre Auto-Healing återhämtning scenario som kan hända på grund av oväntade händelser på servrarna som kan pågå i mindre än 30 min eller så. 
    
    Det finns inga meddelanden Center eller Tjänsthälsa inlägg för dessa mindre återvinningar men du bör vara tillbaka till det normala mycket snart.

Vid mycket få tillfällen konstaterade vi att en av de tre scenarierna som anges ovan har varit orsaken, och tjänsten har återställts, men användarnas webbläsarens cacheminne inte har klarats upp.

Försök att rensa webbläsarens cacheminne innan du navigerar till webbplatsen.

1. Välj **Inställningar**i webbläsaren Microsoft Edge och välj sedan **Sekretess och säkerhet**.
2. Under **Rensa bläddring**väljer du **Välj vad du vill rensa**.
3. Välj **cookies och sparade webbplatsdata**och välj **Rensa**.

>[!Note] 
> Dessa steg kan skilja sig åt när du använder andra webbläsare som Mozilla Firefox eller Google Chrome.

>[!Note] 
> Ett annat alternativ är att öppna SharePoint-webbplatsen eller OneDrive i ett nytt InPrivate-fönster.