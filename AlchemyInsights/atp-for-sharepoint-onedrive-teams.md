---
title: ATP för SharePoint, OneDrive och Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715579"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>ATP för SharePoint, OneDrive och Microsoft Teams

Följ de här anvisningarna för att aktivera avancerat skydd:

1. Gå till [https://protection.office.com](https://protection.office.com) och logga in med en global administratör eller ett säkerhets administratörs konto.

2. I det vänstra navigerings fönstret under **Threat Management**väljer du **policy** \> **Safe Attachments**.

3. Välj **Aktivera ATP för SharePoint, OneDrive och Microsoft Teams**.

4. [Skapa en aktivitets aviserings princip](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) för att få aviseringar när vi upptäcker skadliga filer.

Anvisningar finns i det här [avsnittet](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Obs!** med ATP genomsöks inte alla filer i SharePoint Online, OneDrive för företag eller Microsoft Teams. Filer skannas asynkront av en process som använder delnings aktivitet, gäst aktivitet och hot signaler för att identifiera skadliga filer. Mer information finns i det här [avsnittet](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
