---
title: Kontrollerar säkerheten felsökningstips för spårning av bedrägerier
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 24842e8cc5c6e47fb0eb637e6a3211637ede1ed8
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29492275"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Kontrollerar säkerheten felsökningstips för spårning av bedrägerier

Om du får ett tips om säkerhet som säger ”avsändaren misslyckades våra bedrägeri identifiering kontroller och kanske inte som de verkar vara” sedan avsändaren gick inte att överföra DKIM eller SPF verifieringskontroller. Det bästa sättet att lösa detta är att auktorisera sig avsändaren. Om avsändaren skickar för din räkning, måste du ge dem genom att lägga till avsändarens IP-adress till SPF-post.
  
Mer information finns i [felsökningstips röd (misstänkta) säkerhet för spårning av bedrägerier kontrolleras](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) . 
  
Här följer några länkar som kan hjälpa:
  
- [Hur Office 365 använder avsändaren policy framework (SPF) för att förhindra förfalskningar](https://docs.microsoft.com/en-us/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [Konfigurera SPF i Office 365 för att förhindra förfalskning](https://docs.microsoft.com/en-us/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

