---
title: Microsoft Defender för Office 365 för SharePoint, OneDrive och Microsoft Teams
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
ms.openlocfilehash: 7d2ed7bc4c7d99cd01dadc12e38762903d6d8ab3
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543595"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a>Microsoft Defender för Office 365 för SharePoint, OneDrive och Microsoft Teams

Följ anvisningarna för att aktivera Microsoft Defender för Office 365:

1. Gå till [https://protection.office.com](https://protection.office.com) och logga in med en global administratör eller ett säkerhetsadministratörskonto.

2. I det vänstra navigeringsfönstret under **Hothantering** väljer du **Policy för** \> **Valv bilagor**.

3. Välj **Aktivera Defender för Office 365 för SharePoint, OneDrive och Microsoft Teams**.

4. [Skapa en princip för aktivitetsavisering](/microsoft-365/compliance/create-activity-alerts) för att få aviseringar när vi upptäcker skadliga filer.

Fullständiga instruktioner finns i aktivera [aktivera Valv för SharePoint, OneDrive och Microsoft Teams](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Obs!** Som design söker inte Microsoft Defender för Office 365 igenom alla filer i SharePoint Online, OneDrive för företag eller Microsoft Teams. Filer genomsöks asynkront av en process som använder delningsaktivitet, gästaktivitet och hot-signaler för att identifiera skadliga filer. Mer information finns i Bifoga [Valv för SharePoint, OneDrive och Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
