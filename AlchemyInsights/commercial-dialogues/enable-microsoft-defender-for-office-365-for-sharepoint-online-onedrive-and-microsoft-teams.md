---
title: Aktivera Microsoft Defender för Office 365 för SharePoint Online, OneDrive och Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747739"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivera Microsoft Defender för Office 365 för SharePoint Online, OneDrive och Microsoft Teams

1. Använd dina autentiseringsuppgifter som global administratör eller säkerhetsadministratör och logga in på Säkerhets- och [efterlevnadscenter för Office 365.](https://protection.office.com/)
2. Välj **Hantering av hot** i den vänstra rutan och välj sedan Policy **Safe**  >  [attachments](https://protection.office.com/safeattachment).
3. Välj **Aktivera Microsoft Defender för Office 365 för SharePoint, OneDrive och Microsoft Teams** och välj sedan **Spara**.
    > [!TIP]
    >
    > - Som global administratör eller SharePoint Online-administratör kör du följande PowerShell-cmdlet med **parametern DisallowInfectedFileDownload** inställd på *sant:* [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Konfigurera aviseringar för identifierade filer](https://go.microsoft.com/fwlink/?linkid=2092110)

Mer information finns i [Microsoft Defender för Office 365 för SharePoint, OneDrive och Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
