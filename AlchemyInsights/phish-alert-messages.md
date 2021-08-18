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
ms.openlocfilehash: 90b078147bbb1e60cba0a2de6e49a862469f93aa
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316376"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Avisering e-postmeddelanden från principen "Phish Delivered due to tenant or user override"

En standardaviseringsprincip **med namnet Phish Delivered** på grund av åsidosättning av klientorganisation eller användare finns tillgänglig i organisationer med Microsoft Defender för Office 365 P1- och P2-licenser. Om du fick det här aviseringen finns det anvisningar för att undersöka detta:

1. Klicka på Visa avisering i **varningsmeddelandet** för att gå till **sidan** Aviseringar Microsoft 365 Defender portalen.

2. Välj aviseringen om du vill se alternativet **Visa meddelandelista eller** **Visa meddelanden i Utforskaren**. Båda dessa alternativ tar dig till meddelandets information, som innehåller Meddelande-ID. Observera att länken Hotutforskaren automatiskt filtrerar meddelanden som matchar aviseringskriterierna. Du kan behöva justera datumfiltret i Hotutforskaren.

Nätfiskemeddelandet levererades på grund av en manuellt konfigurerad åsidosättning:

- En tillåten avsändare eller domän som har angetts av användaren.
- En tillåten avsändare eller domän som anges av administratören i en princip mot skräppost.
- En tillåten IP-adress i en princip för anslutningsfilter.
- En e-postflödesregel (kallas även transportregel) som är konfigurerad för att tillåta meddelanden.

Om du anser att meddelandet felaktigt har markerats som nätfiske använder du [administratörsinskick](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission) för att rapportera meddelandet till Microsoft.

Användarna kan använda [tilläggen Rapportmeddelande](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) eller Rapport nätfiske i Outlook skicka exempel på meddelanden till Microsoft.
