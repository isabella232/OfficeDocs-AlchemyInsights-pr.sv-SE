---
title: Innehåll Sök inga resultat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800634"
---
# <a name="no-results-from-content-searchexports"></a>Inga resultat från innehåll Sök/export

Problem med innehåll Sök/export inte returnerar några data kan bero på att vissa krav säkerhetsfilter som installerades av en viss Admin och kommunicerar inte till alla administratörer.

Kontrollera om det finns några efterföljande säkerhetsfilter som kan orsaka det här problemet:
1. Ansluta till säkerhet och regelefterlevnadscentret Powershell
2. Kör följande kommandon:
<br>$org = ”yourdomain.com”
<br>Get-ComplianceSecurityFilter-organisation $org