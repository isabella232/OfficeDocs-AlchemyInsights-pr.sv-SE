---
title: Configuration Manager-enheter saknas i portalen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: 7a11ad3c6970be2c52a7cf0696bd3810b9bd665a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2020
ms.locfileid: "43790235"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="d817d-102">Configuration Manager-enheter saknas i portalen</span><span class="sxs-lookup"><span data-stu-id="d817d-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="d817d-103">För att enhetssynkronisering ska fungera måste [nödvändiga Internetslutpunkter](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) gå att nå från den lokala server som är värd för rollen Anslutningspunkt för tjänsten.</span><span class="sxs-lookup"><span data-stu-id="d817d-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="d817d-104">För att felsöka enhetssynkronisering läser du **CMGatewaySyncUploadWorker.log** som finns i anslutningspunkten för tjänsten.</span><span class="sxs-lookup"><span data-stu-id="d817d-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="d817d-105">Läs mer om [Klientanslutning i Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span><span class="sxs-lookup"><span data-stu-id="d817d-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
