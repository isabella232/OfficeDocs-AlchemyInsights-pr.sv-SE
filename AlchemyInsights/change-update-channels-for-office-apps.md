---
title: Ändra uppdateringskanaler för Office-appar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440022"
---
# <a name="change-update-channels-for-office-apps"></a>Ändra uppdateringskanaler för Office-appar

För nya Office-installationer använder du Hämtningsinställningar för Office-program för att välja önskad uppdateringskanal och installerar (eller installerar om) Office-program. Mer information finns [i Hantera inställningar för hämtning av programvara i Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**Anm.)** Den uppdateringskanal som valts med hjälp av inställningarna för hämtning av Office-programvara gäller för alla användare som utför nya installationer med O365-portalen. Mer information finns i [Ladda ned och installera eller installera om Microsoft 365 eller Office 2019 på en PC eller Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

För befintliga Office-installationer använder du OFFICE Deployment Tool (ODT) för att växla till en annan uppdateringskanal:  

1. Hämta den senaste versionen av Office Deployment Tool (setup.exe) från [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. Identifiera namnet på den kanal som du vill växla till. Mer information finns [i Konfigurationsalternativ för Distributionsverktyget för Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Skapa en XML-fil för konfiguration som anger lämpligt kanalnamn, till exempel update.xml.  
    a. <Configuration>  
    b. <uppdaterar **Channel="Monthly"** />  
    c. </Configuration>
4. Från en upphöjd kommandotolk växlar du till mappplatsen där setup.exe finns och kör följande kommando:  
    a. setup.exe /configure update.xml
5. Starta ett Office-program (till exempel **File**Excel) och välj sedan  >  **Filkonto**. I avsnittet Produktinformation väljer du Uppdatera **alternativ**  >  **Uppdatera nu**.

Mer information finns i [Så här byter du uppdateringskanaler för befintliga Office Apps](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

Konfigurera inställningen Uppdatera kanal med hjälp av grupp av användare eller med hjälp av Configuration Manager (SCCM) med hjälp av grupprincipobjekt. Mer information finns i [Översikt över uppdateringskanaler för Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). Mer information finns i [Så här hanterar du Office 365 ProPlus-kanaler för IT-proffs](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) och hantera uppdateringar av Microsoft [365-appar med Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).