---
title: 2491 Avisera e-postmeddelanden från principen "Phish som skickas på grund av klient-eller användar åsidosättningar"
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
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728629"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Avisera e-postmeddelanden från principen "Phish som skickas på grund av klient-eller användar åsidosättningar"

En standard aviserings princip med namnet "Phish levererad på grund av klient-eller användar åsidosättning" har distribuerats till klient organisationer med Office 365 ATP-och P2-licenser. Om du fick den här aviseringen kan du undersöka:

1. Klicka på **Visa varning** i aviserings meddelandet för att gå till sidan **aviseringar** i säkerhets & efterlevnad.

2. Välj varningen om du vill se alternativet att **Visa meddelande listan** eller **Visa meddelanden i Utforskaren**. Båda dessa alternativ tar dig till meddelandets information, som innehåller meddelande-ID. Observera att länken Threat Explorer automatiskt filtrerar meddelanden som matchar aviserings villkoren. Du kan behöva justera datum filtret i Threat Explorer.

Nät fiske meddelandet levererades på grund av en manuellt konfigurerad åsidosättning:

- En avsändare eller domän som anges av användaren.

- En avsändare eller domän som angetts av administratören i en policy för skräp post.

- En tillåten IP-adress i en anslutnings filter princip.

- En regel för e-postflöde (kallas även transport regel) som är konfigurerad för att tillåta meddelanden i.

Om du tror att meddelandet inte hade marker ATS som Phish kan du använda [tillägget Outlook rapportera meddelande](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) för att skicka meddelanden till Microsoft.
