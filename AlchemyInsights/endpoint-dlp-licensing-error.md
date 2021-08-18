---
title: Slutpunkt DLP-licensfel
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
ms.openlocfilehash: c32ab88a72c265be411350e50756f5b2e1e3337c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322149"
---
# <a name="endpoint-dlp-licensing-error"></a>Slutpunkt DLP-licensieringsfel

Om du får följande felmeddelande när du försöker konfigurera slutpunkt DLP:

`Your organization is missing the licenses required to manage these devices`.

Kontrollera att du har någon av följande prenumerationer eller tillägg:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Microsoft 365 E5 Compliance
- Microsoft 365 A5 Compliance
- Microsoft 365 E5 – Informationsskydd och styrning
- Microsoft 365 A5 – Informationsskydd och styrning

**Obs!** Det här fungerar inte för licenskombinationer som: Win E5 + O365 E5 + EMS E5. Du måste ha en licens för endast M365 E5 för att kunna konfigurera den här funktionen.

Mer information om Endpoint DLP-licensiering finns i [Endpoint DLP-licensiering.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
