---
title: Kontrollerar säkerheten felsökningstips för spårning av bedrägerier
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: ab7bd3ec66640d66e5f1ea7c1eeee0a1a9510241
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353267"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Kontrollerar säkerheten felsökningstips för spårning av bedrägerier

Om du får ett tips om säkerhet som säger ”avsändaren misslyckades våra bedrägeri identifiering kontroller och kanske inte som de verkar vara” sedan avsändaren gick inte att överföra DKIM eller SPF verifieringskontroller. Det bästa sättet att lösa detta är att auktorisera sig avsändaren. Om avsändaren skickar för din räkning, måste du ge dem genom att lägga till avsändarens IP-adress till SPF-post.
  
Mer information finns i [felsökningstips röd (misstänkta) säkerhet för spårning av bedrägerier kontrolleras](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .
  
Här följer några länkar som kan hjälpa:
  
- [Hur Office 365 använder avsändaren policy framework (SPF) för att förhindra förfalskningar](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [Konfigurera SPF i Office 365 för att förhindra förfalskning](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
