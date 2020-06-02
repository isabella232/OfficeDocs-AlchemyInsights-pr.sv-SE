---
title: Felsökning av säkerhetstipset för bedrägeriidentifieringskontroller
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505001"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Felsökning av säkerhetstipset för bedrägeriidentifieringskontroller

Om du får ett säkerhetstips som säger "Avsändaren misslyckades våra kontroller bedrägeri upptäckt och kanske inte vem de verkar vara", då avsändaren misslyckades med att passera antingen DKIM eller SPF autentisering kontroller. Den bästa metoden för att lösa detta är att avsändaren auktoriserar sig själva. Om avsändaren skickar för din räkning måste du auktorisera dem genom att lägga till avsändarens IP-adress i din SPF-post.
  
Mer information [finns i Felsökning av det röda (misstänkta) säkerhetstipset för kontroller av bedrägeriidentifiering.](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)
  
Här är några andra länkar som kan hjälpa:
  
- [Så här använder Microsoft avsändande principramverk (SPF) för att förhindra förfalskning](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Konfigurera SPF för att förhindra förfalskning](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
