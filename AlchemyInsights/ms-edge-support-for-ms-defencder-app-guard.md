---
title: Microsoft Edge-support för Microsoft Defender Application Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584009"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Microsoft Edge-support för Microsoft Defender Application Guard

Application Guard är utformat för Windows 10 och Microsoft Edge och använder ett maskin varu isolerings sätt som låter en användare navigera från en icke betrodd webbplats i en isolerad, Hyper-V-aktiverad behållare, avgränsas från operativ systemet.

En företags administratör definierar en lista över tillförlitliga webbplatser, moln resurser och interna nätverk. När en användare besöker en webbplats som inte finns med i listan öppnar Microsoft Edge webbplatsen i behållaren. Det innebär att om webbplatsen blir skadlig kan värddatorn vara skyddad och angripare kommer inte till företags data.

Installation av tillägg i behållaren stöds enligt Microsoft Edge version 81 och kan styras via en princip. Den updateURL-adress som används i ExtensionInstallForcelist-principen ska läggas till som en neutral resurs i principerna för nätverks isolering som används av Application Guard.

Mer information finns i [Microsoft Edge support för Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).
