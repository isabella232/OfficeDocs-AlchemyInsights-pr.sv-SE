---
title: Felsökning av säkerhetstips vid identifiering av bedrägerier
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834749"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Felsökning av säkerhetstips vid identifiering av bedrägerier

Om du får ett säkerhetstips där det står "Avsändaren misslyckades med våra kontroller för identifiering av bedrägerier och kanske inte är den som de verkar vara", så gick det inte att överföra antingen DKIM- eller SPF-autentiseringskontrollerna till avsändaren. Den bästa metoden för att lösa det här är att avsändaren godkänner sig själv. Om avsändaren skickar åt dig måste du auktorisera dem genom att lägga till avsändarens IP-adress till SPF-posten.
  
Mer [information finns i Felsökning av röda (misstänkta) säkerhetstips](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) för identifiering av bedrägerier.
  
Här är några andra länkar som kan vara till hjälp:
  
- [Hur Microsoft använder Sender Policy Framework (SPF) för att förhindra förfalskning](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Konfigurera SPF för att förhindra förfalskning](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
