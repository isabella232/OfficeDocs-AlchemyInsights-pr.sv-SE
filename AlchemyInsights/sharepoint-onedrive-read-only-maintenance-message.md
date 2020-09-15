---
title: Skriv skydd för underhålls meddelande när du försöker använda SharePoint eller OneDrive
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
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670850"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Skriv skydd för underhålls meddelande när du försöker använda SharePoint eller OneDrive

Användare kan få ett **skrivskyddat för underhålls** meddelande när de försöker använda SharePoint eller OneDrive för något av följande scenarier. 

-   En planerad eller aktiv underhålls aktivitet.  Leta efter dem genom att gå till [meddelande Center](https://portal.office.com/adminportal/home#/messagecenter).
-   Ett högprioriterat, aktivt tjänst problem som kan uppstå. Sök efter eventuella rådgivare/incidenter genom att gå till [tjänstens hälsa](https://portal.office.com/adminportal/home#/servicehealth).
-   Ett mindre automatiskt återställnings scenario som kan förekomma på grund av eventuella oväntade händelser på de servrar som eventuellt har varit mindre än 30 minuter. 
    
    Det finns inga poster för meddelande Center eller tjänstens hälsa för dessa mindre återställningar, men du bör vara tillbaka till normalt.

Under de senaste inloggningarna observerade vi att ett av de tre ovanstående scenarierna var orsaken och att tjänsten har återställts men att användarens webbläsare inte har rensats.

Försök rensa webbläsarens cache innan du navigerar till webbplatsen.

1. I webbläsaren Microsoft Edge väljer du **Inställningar**och sedan **Sekretess och säkerhet**.
2. Under **Rensa bläddring**väljer **du Välj vad du vill rensa**.
3. Välj **cookies och sparade webbplats data**och välj **Rensa**.

>[!Note] 
> De här stegen kan skilja sig från andra webbläsare, till exempel Mozilla Firefox och Google Chrome.

>[!Note] 
> Ett annat alternativ är att öppna SharePoint-webbplatsen eller OneDrive i ett nytt InPrivate-fönster.