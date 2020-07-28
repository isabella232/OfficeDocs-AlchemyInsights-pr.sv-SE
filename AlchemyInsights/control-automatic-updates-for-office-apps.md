---
title: Styra automatiska uppdateringar för Office Apps
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
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439926"
---
# <a name="control-automatic-updates-for-office-apps"></a>Styra automatiska uppdateringar för Office Apps

Som standard hämtas uppdateringar för Office Apps automatiskt och tillämpas i bakgrunden utan att användaren behöver göra något. Administratörer kan dock styra hur uppdateringar tillämpas med hjälp av Office Update-inställningar. Med uppdateringsinställningarna kan administratörer aktivera eller inaktivera automatiska uppdateringar, visa eller dölja knappen **Uppdatera nu** i Office, ange tidsgränser för uppdateringar med mera. Detaljerad information finns i:

- [Konfigurera uppdateringsinställningar för Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Automatisk uppdatering för Office är inte aktiverat](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Definiera hur Office uppdateras när det har installerats](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Så här granskar du de befintliga uppdateringsinställningarna som tillämpas på en klientdator:

1. Öppna Registereditorn genom att gå till **Starta**  >  **Kör**  >  **regedit**.
2. Växla till följande plats och granska inställningarna för Office Update:  
    a. HKEY_LOCAL_MACHINE\PROGRAMVARA\Microsoft\Office\  
    b. Klicka på Tillrun\Konfiguration

**Anm.)**  Om OfficeMgmtCOM-nyckeln är inställd kan meddelandet "Uppdateringar hanteras av **Office**systemadministratören" visas i  >  **Account**  >  **Office-uppdateringar**för Office-konto . Mer information finns i [Hantera uppdateringar av Microsoft 365-appar med Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  