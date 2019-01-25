---
title: 1332 OWA - regler för Inkorgen inte körs för en postlåda
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f090d0a9d84bc6a4d1a1f4c0af55102d4b0ddfbe
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29492735"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>En Inkorgsregel fungerar inte som förväntat

Kontrollera följande inställningar:
  
- Ett meddelande kan omdirigeras, vidarebefordrade eller besvarade automatiskt baserat på regler för Inkorgen bara en gång. En regel som omdirigerar (en inkorg eller e-flöde regel, även kallad transport-regeln) kan lägga till högst tio mottagare för vidarebefordran till ett meddelande. Mer information finns i [Journal, Transport, och Inkorgen gränserna](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).
    
- Regler för Inkorgen fungerar inte på alternativa journal postlåda. Mer information om alternativa journaler postlådan finns [alternativa journal postlåda](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).
    
Om du vill lösa de här problemen finns i [KB 2829319](https://support.microsoft.com/kb/2829319).
  
Om följande problem inte gäller kör den diagnostiska rapporten Inkorgen regeln innan du eskalera problemet till Microsoft Support:
  
1. Öppna postlådan i Outlook på webben och klicka på **Inställningar** \> **Alternativ** \> **Ordna e-post** \> **regler för Inkorgen**.
    
2. Klicka på **om reglerna inte fungerar Klicka här för att generera en diagnostisk rapport**längst ned på sidan.
    

