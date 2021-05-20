---
title: 2491 Avisering e-postmeddelanden från principen "Phish Delivered due to tenant or user override"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544596"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Avisering e-postmeddelanden från principen "Phish Delivered due to tenant or user override"

En standardaviseringsprincip med namnet "Phish Delivered due to tenant or user override" har distribuerats till klientorganisationen med Microsoft Defender för Office 365 P1- och P2-licenser. Om du fick det här aviseringen finns det anvisningar för att undersöka detta:

1. Från varningsmeddelandet klickar du **på Visa avisering** för **att** gå till sidan Aviseringar i & säkerhets- och efterlevnadscenter.

2. Välj aviseringen om du vill se alternativet **Visa meddelandelista eller** **Visa meddelanden i Utforskaren**. Båda dessa alternativ tar dig till meddelandets information, som innehåller Meddelande-ID. Observera att länken Hotutforskaren automatiskt filtrerar meddelanden som matchar aviseringskriterierna. Du kan behöva justera datumfiltret i Hotutforskaren.

Nätfiskemeddelandet levererades på grund av en manuellt konfigurerad åsidosättning:

- En tillåten avsändare eller domän som har angetts av användaren.

- En tillåten avsändare eller domän som anges av administratören i en princip mot skräppost.

- En tillåten IP-adress i en princip för anslutningsfilter.

- En e-postflödesregel (kallas även transportregel) som är konfigurerad för att tillåta meddelanden.

Om du anser att meddelandet felaktigt har markerats som phish använder du tillägget Outlook [Report Message](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) för att skicka exempel på meddelanden till Microsoft.
