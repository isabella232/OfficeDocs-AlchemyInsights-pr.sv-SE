---
title: Aktivera Office 365 ATP för SharePoint, OneDrive och Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801093"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivera Microsoft Defender för Office 365 för SharePoint Online, OneDrive och Microsoft Teams

1. Gå till https://protection.office.com och logga in.
2. Välj **hot Management**  >  **policy** -  >  **säkra bifogade filer** .
3. Välj **Aktivera ATP för SharePoint, OneDrive och Microsoft Teams** och klicka sedan på **Spara** .
4. Lämpligt Som global administratör eller SharePoint Online-administratör kör du cmdleten [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) med parametern **DisallowInfectedFileDownload** angiven till *True* .
5. Lämpligt [Konfigurera aviseringar](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) för identifierade filer.

> [!NOTE]
> ATP kan du söka igenom alla filer i SharePoint Online, OneDrive eller Microsoft Teams. Filer skannas asynkront, genom en process där delnings-och gäst aktivitets händelser används tillsammans med smarta heuristik och hot signaler. Se [ATP för SharePoint, OneDrive och Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).