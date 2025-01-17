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
ms.openlocfilehash: 2d132101768e0a835d448604d684ec0c735e6628
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332177"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivera Microsoft Defender för Office 365 för SharePoint Online, OneDrive och Microsoft Teams

1. Gå till https://protection.office.com och logga in.
2. Välj **Policy för hantering** av  >  **hot** Valv bifogade  >  **filer**.
3. Välj **Aktivera Defender för Office 365 för SharePoint, OneDrive** och Microsoft Teams och klicka sedan på **Spara.**
4. (Rekommenderas) Som global administratör eller SharePoint Online-administratör kör du [cmdleten Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) med **parametern DisallowInfectedFileDownload** inställd på *sant.*
5. (Rekommenderas) [Konfigurera aviseringar för](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) identifierade filer.

**Obs!** Microsoft Defender för Office 365 genomsöker inte igenom alla filer i SharePoint Online, OneDrive eller Microsoft Teams. Filer skannas asynkront genom en process som använder delning och gästaktivitetshändelser, tillsammans med smart heuristics och hot- signaler för att identifiera skadliga filer. Se [Microsoft Defender för Office 365 för SharePoint, OneDrive och Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
