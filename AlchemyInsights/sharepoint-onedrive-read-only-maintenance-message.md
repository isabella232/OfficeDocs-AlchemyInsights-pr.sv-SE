---
title: Skrivskyddad för underhåll meddelande när du försöker använda SharePoint eller OneDrive
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620741"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Skrivskyddad för underhåll meddelande när du försöker använda SharePoint eller OneDrive

Användare får ett meddelande **Skrivskyddad för underhåll** vid försök att använda SharePoint- eller OneDrive för något av följande scenarier. 

-   Planerade eller aktiva underhållsåtgärd.  Kontrollera dem genom att navigera till [Message Center](https://portal.office.com/adminportal/home#/messagecenter).
-   En hög prioritet, aktiv tjänst tillbud som kan ske. Kontrollera alla rekommendationerna/incidenter genom att navigera till [Tjänsten hälsa](https://portal.office.com/adminportal/home#/servicehealth).
-   En mindre smart automatisk återställningsscenario som kan bero på grund av oväntade händelser på servrar som kan pågå i minst 30 min eller så. 
    
    Det finns inga Message Center eller tjänsten hälsa bokförs för dessa mindre återställningar, men du bör vara tillbaka till normal mycket snart.

Vid mycket få tillfällen observerade vi att en av tre scenarier som anges ovan har varit orsaken, och tjänsten har återställts, men användare webbläsarens cacheminne har rensats.

Försök att rensa webbläsarens cacheminne innan navigera till webbplatsen.

1. I webbläsaren Microsoft Edge, Välj **Inställningar**och välj **Sekretess och säkerhet**.
2. Markera under **Rensa bläddring**, **välja vad du vill ta bort**.
3. Välj **Cookies och sparade webbplats data**och välj **Radera**.

>[!Note] 
> Stegen kan skilja sig när du använder andra webbläsare som Mozilla Firefox eller Google Chrome.

>[!Note] 
> Ett annat alternativ är att öppna din SharePoint-webbplats eller en OneDrive i ett nytt InPrivate-fönster.