---
title: Tillgängligt att LOVA för SharePoint, OneDrive och Microsoft-team
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: b304f6c7d9959e49a8152c03f11c6c864a154ea5
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765454"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>Tillgängligt att LOVA för SharePoint, OneDrive och Microsoft-team

Gör så här om du vill aktivera avancerade Threat Protection:

1. Gå till [https://protection.office.com](https://protection.office.com) och logga in med en global administratör eller administratörskontot för säkerhet.

2. Välj **principen** i det vänstra navigeringsfönstret under **hantering av hot** \> **Säkra bifogade filer**.

3. Markera **Aktivera ATP för SharePoint, OneDrive, och Microsoft team**.

4. [Skapa en avisering principen aktiviteten](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) att ta emot meddelanden när vi identifiera skadliga filer.

Fullständiga instruktioner finns i det här [avsnittet](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).

**Anmärkning**: avsiktligt ATP söker inte igenom varje enskild fil i SharePoint Online, OneDrive för företag eller Microsoft Teams. Skannade filer asynkront med en process som använder en delad aktivitet, Gäst aktivitet och hot signalerar att identifiera skadliga filer. Mer information finns i det här [avsnittet](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).
