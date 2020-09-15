---
title: Innehålls sökning inga resultat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680665"
---
# <a name="no-results-from-content-searchexports"></a>Inga resultat från innehålls sökning/export

Problem med innehålls sökning/exporterar inte några data kan bero på vissa säkerhets filter för efterlevnad som konfigurerades av en viss administratör och inte kommunicerar med alla administratörer.

Lös problemet genom att kontrol lera om det finns några säkerhets filter för efterlevnad som kan orsaka detta:
1. Ansluta till säkerhets-och Compliance Center PowerShell
2. Kör följande cmdlets:
<br>$org = "yourdomain.com"
<br>Skaffa-ComplianceSecurityFilter-organisation $org