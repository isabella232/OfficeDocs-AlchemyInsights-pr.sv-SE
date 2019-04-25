---
title: Aktivera Office 365 tillgängligt att LOVA för SharePoint, OneDrive och Microsoft-team
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403051"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Aktivera Office 365 avancerade Threat Protection for SharePoint Online, OneDrive och Microsoft-team

1. Gå till https://protection.office.com och logga in.
2. Välj **Threat management** > **Policy** > **Säkra bifogade filer**.
3. Markera **Aktivera ATP för SharePoint, OneDrive, och Microsoft team**och klicka sedan på **Spara**.
4. (Rekommenderas) Som global administratör eller en SharePoint Online-administratör som kör cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) med parametern **DisallowInfectedFileDownload** har värdet *true*.
5. (Rekommenderas) [Ställ in varningar](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) för identifierade filer.

> [!NOTE]
> ATP kommer nFör skanna varje enskild fil i SharePoint Online, OneDrive eller Microsoft Teams. Filer genomsöks asynkront, genom en process som använder fildelning och Gäst aktivitetshändelser, intelligent heuristik och hot-signaler för att identifiera skadliga filer. Se [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).