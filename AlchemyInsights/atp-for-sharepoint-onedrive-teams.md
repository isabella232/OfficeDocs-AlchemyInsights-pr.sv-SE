---
title: ATP för SharePoint, OneDrive och Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: e9437d04815d4ca2f55cf9133ef6a4b429cd2476
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508430"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>ATP för SharePoint, OneDrive och Microsoft Teams

Så här aktiverar du Avancerat skydd mot hot:

1. Gå till [https://protection.office.com](https://protection.office.com) och logga in med ett globalt administratörs- eller säkerhetsadministratörskonto.

2. Välj **Principsäkra** bilagor i det vänstra navigeringsfönstret under **Hothantering** \> **Safe Attachments**.

3. Välj **Aktivera ATP för SharePoint, OneDrive och Microsoft Teams**.

4. [Skapa en aktivitetsaviseringsprincip](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) för att ta emot meddelanden när vi upptäcker skadliga filer.

Fullständiga instruktioner finns i det här [avsnittet](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Atp**genom design söker inte igenom varenda fil i SharePoint Online, OneDrive för företag eller Microsoft Teams. Filer genomsöks asynkront av en process som använder delningsaktivitet, gästaktivitet och hotsignaler för att identifiera skadliga filer. Mer information finns i det här [avsnittet](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
