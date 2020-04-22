---
title: Aktivera Office 365 ATP för SharePoint, OneDrive och Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703444"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivera avancerat skydd mot office 365 för SharePoint Online, OneDrive och Microsoft Teams

1. Gå https://protection.office.com till och logga in.
2. Välj Säkra bilagor **för hothanteringsprincip** > **Policy** > **.**
3. Välj **Aktivera ATP för SharePoint, OneDrive och Microsoft Teams**och klicka sedan på **Spara**.
4. (Rekommenderas) Som global administratör eller SharePoint Online-administratör kör du cmdleten [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) med parametern **DisallowInfectedFileDownload** inställd på *true*.
5. (Rekommenderas) [Ställ in aviseringar](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) för identifierade filer.

> [!NOTE]
> ATP kommer att skanna varenda fil i SharePoint Online, OneDrive eller Microsoft Teams. Filer skannas asynkront, genom en process som använder delnings- och gästaktivitetshändelser, tillsammans med smarta heuristik och hotsignaler för att identifiera skadliga filer. Se [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).