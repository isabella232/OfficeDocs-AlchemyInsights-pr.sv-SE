---
title: Read-Only visas ett meddelande om underhåll när du försöker använda SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 376b653b18857103586e25edd0ad6801a7bbe0a1
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329466"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only visas ett meddelande om underhåll när du försöker använda SharePoint eller OneDrive

Användare kan få ett **meddelande om skrivskydd** för underhåll när de försöker använda SharePoint eller OneDrive något av följande scenarier. 

-   En planerad eller aktiv underhållsaktivitet.  Se om de finns i [meddelandecentret.](https://portal.office.com/adminportal/home#/messagecenter)
-   En aktiv tjänsthändelse med hög prioritet som kan inträffa. Leta efter rådgivningar/incidenter genom att gå till [Tjänstens hälsa.](https://portal.office.com/adminportal/home#/servicehealth)
-   Ett mindre scenario för automatisk återställning som kan inträffa på grund av oväntade händelser på servrarna som kan pågå i mindre än 30 minuter. 
    
    Det finns inga inlägg i Meddelandecenter eller Tjänstens hälsa för dessa mindre återställningar men du bör vara helt normal inom kort.

Vi har mycket få gånger observerat att något av de tre scenarierna ovan har varit orsaken och att tjänsten har återställts, men användarens webbläsarcache har inte rensats.

Försök rensa webbläsarens cache innan du navigerar till webbplatsen.

1. I din Microsoft Edge väljer du **Inställningar** och sedan Sekretess **och säkerhet.**
2. Under **Rensa surfning** väljer du **Välj vad som ska rensas.**
3. Välj **Cookies och sparade webbplatsdata** och välj **Rensa**.

**Obs!** De här stegen kan skilja sig när du använder andra webbläsare, till exempel Mozilla Firefox eller Google Chrome.

**Obs!** Ett annat alternativ är att öppna SharePoint-webbplatsen eller OneDrive i ett nytt InPrivate-fönster.