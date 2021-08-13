---
title: Configuration Manager-enheter saknas i portalen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: 358bb6aa0420a845e51e0b75049c2ae790daf3690e5cfb115b234d82a29e93a7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966127"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>Configuration Manager-enheter saknas i portalen

För att enhetssynkronisering ska fungera måste [nödvändiga Internetslutpunkter](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) gå att nå från den lokala server som är värd för rollen Anslutningspunkt för tjänsten. För att felsöka enhetssynkronisering läser du **CMGatewaySyncUploadWorker.log** som finns i anslutningspunkten för tjänsten.

Läs mer om [Klientanslutning i Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).
