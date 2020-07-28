---
title: Installera uppdateringar för Office-appar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1747"
- "9000140"
ms.openlocfilehash: b5952feaac7ac51faed2a3399c68a87a4227b165
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440153"
---
# <a name="apply-updates-for-office-apps"></a>Installera uppdateringar för Office-appar

Som standard är uppdateringar för Office Apps kostnadsfria, hämtade automatiskt och tillämpas i bakgrunden utan att användaren behöver göra något. Om du vill köra uppdateringar manuellt om du stöter på problem med att installera uppdateringar läser du [Installera Office-uppdateringar](https://support.office.com/article/install-office-updates-2ab296f3-7f03-43a2-8e50-46de917611c5). Mer information finns i [Felsöka installation av Office](https://support.microsoft.com/office/troubleshoot-installing-office-35ff2def-e0b2-4dac-9784-4cf212c1f6c2?ui=en-us&rs=en-us&ad=us#O365Plans=signinorgid).

Om du vill hantera Office-uppdateringar för användarna bör du tänka på följande:

- Välj rätt Office Update Channel för din organisation baserat på önskad frekvens av uppdateringar. Mer information finns i [Översikt över uppdateringskanaler för Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-of-update-channels-for-office-365-proplus).

- Bestäm om du vill installera uppdateringar automatiskt från internet eller från en lokal resurs. Mer information finns i [Välja hur du hanterar uppdateringar av Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/choose-how-to-manage-updates-to-office-365-proplus).

- Granska Office Update-inställningar för att styra hur uppdateringar tillämpas på slutanvändarens datorer:

    - [Konfigurera uppdateringsinställningar för Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus).
    - [Definiera hur Office uppdateras när det har installerats](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element).

När du distribuerar Office-appar till flera användare använder du verktyget Anpassning av Office för att skapa konfigurationsfiler för distribution och konfigurera Office-uppdateringar med hjälp av Office-distributionsverktyget. Mer information finns [i Översikt över Anpassningsverktyget för Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run) och [office-distributionsverktyget](https://go.microsoft.com/fwlink/p/?LinkID=626065).

- Ett exempel på hur du konfigurerar användargrupper för att distribuera Office-uppdateringar finns i [Distribuera Microsoft 365-appar från en lokal källa](https://docs.microsoft.com/deployoffice/deploy-office-365-proplus-from-a-local-source).
-   Överväg att använda ForceAppShutdown-inställningen om Office-uppdateringar inte tillämpas på några användare på grund av öppna Office-appar. Mer information finns i [egenskapen FORCEAPPSHUTDOWN (en del av egenskapselementet).](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#forceappshutdown-property-part-of-property-element) 

**Se även**

[Översikt över uppdateringsprocessen för Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-of-the-update-process-for-office-365-proplus).  
[Släpp information för uppdateringar till Microsoft 365 Apps](https://docs.microsoft.com/officeupdates/release-notes-office365-proplus).  
[Hantera uppdateringar av Microsoft 365-appar med Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager).  
