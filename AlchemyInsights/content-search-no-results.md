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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516797"
---
# <a name="no-results-from-content-searchexports"></a>Inga resultat från innehåll Sök/export

Problem med innehåll Sök/export inte returnerar några data kan bero på att vissa krav säkerhetsfilter som installerades av en viss Admin och kommunicerar inte till alla administratörer.

Kontrollera om det finns några efterföljande säkerhetsfilter som kan orsaka det här problemet:
1. Ansluta till säkerhet och regelefterlevnadscentret Powershell
2. Kör följande kommandon:
<br>$org = ”yourdomain.com”
<br>Get-ComplianceSecurityFilter-organisation $org