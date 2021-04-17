---
title: Innehållssökning inga resultat
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816866"
---
# <a name="no-results-from-content-searchexports"></a>Inga resultat från innehållssökning/-exporter

Problem med innehållssökning/exporter som inte returnerar några data kan bero på vissa säkerhetsfilter för efterlevnad som har ställts in av en viss administratör och inte meddelar dem till alla administratörer.

Lös problemet genom att kontrollera om det finns säkerhetsfilter för efterlevnad som kan orsaka följande:
1. Ansluta till Säkerhets- och efterlevnadscenter Powershell
2. Kör följande kommando:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter - $org