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
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955984"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Felsökning av säkerhetstips vid identifiering av bedrägerier

Om du får ett säkerhetstips där det står "Avsändaren misslyckades med våra identifieringskontroller för bedrägerier och kanske inte är den som de verkar vara", så kunde avsändaren inte överföra antingen DKIM- eller SPF-autentiseringskontroller. Den bästa metoden för att lösa det här är att avsändaren godkänner sig själv. Om avsändaren skickar åt dig måste du auktorisera dem genom att lägga till avsändarens IP-adress till SPF-posten.
  
Mer [information finns i Felsökning av den röda säkerhetstips för](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) identifiering av bedrägerier.
  
Här är några andra länkar som kan vara till hjälp:
  
- [Hur Microsoft använder Sender Policy Framework (SPF) för att förhindra förfalskning](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Konfigurera SPF för att förhindra förfalskning](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
