---
title: Slut punkts licens fel för DLP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: d17c51177898d62c7c477460c8c26b4753bae65f
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564870"
---
# <a name="endpoint-dlp-licensing-error"></a>Slut punkts licens fel för DLP

Om du får följande fel meddelande när du försöker skapa Endpoint-DLP:

`Your organization is missing the licenses required to manage these devices`.

Kontrol lera att du har någon av följande prenumerationer eller tillägg:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Microsoft 365 E5-efterlevnad
- Microsoft 365 A5-efterlevnad
- Microsoft 365 E5 informations skydd och styrelse former
- Microsoft 365 A5 informations skydd och styrelse former

> [!NOTE]
> Detta fungerar inte för licens kombinationer som: Win E5 + O365 E5 + EMS E5. Du måste ha en ren M365 E5-licens för att kunna använda den här funktionen.

För mer information om DLP-licensiering för slut punkter, se [slut punkt för DLP-licensiering.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
