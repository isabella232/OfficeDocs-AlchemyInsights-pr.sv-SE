---
title: 2491 Varning e-postmeddelanden från "Phish Levereras på grund av klient eller användare åsidosätta" politik
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758952"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Avisera e-postmeddelanden från principen "Phish Delivered på grund av klient- eller användaridosättning"

En standardaviseringsprincip med namnet "Phish Delivered på grund av klient- eller användar åsidosättning" har distribuerats till klienter med Office 365 ATP P1- och P2-licenser. Om du har fått den här aviseringen är det här stegen för att undersöka:

1. Klicka på Visa **avisering** från **varningsmeddelandet** för att gå till sidan Aviseringar i säkerhets- & compliance center.

2. Markera aviseringen om du vill visa alternativet **Visa meddelandelista** eller **Visa meddelanden i Utforskaren**. Båda dessa alternativ tar dig till informationen om meddelandet, som innehåller meddelande-ID. Observera att länken Threat Explorer automatiskt filtrerar de meddelanden som matchar varningsvillkoren. Du kan behöva justera datumfiltret i Threat Explorer.

Nätfiskemeddelandet levererades på grund av en manuellt konfigurerad åsidosättning:

- En tillåten avsändare eller domän som angetts av användaren.

- En tillåten avsändare eller domän som angetts av administratören i en policy mot skräppost.

- En tillåten IP-adress i en anslutningsfilterprincip.

- En regel för e-postflöde (kallas även en transportregel) som är konfigurerad för att tillåta meddelanden i.

Om du tror att meddelandet har markerats felaktigt som phish använder du [tillägget Outlook-rapportmeddelande](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) för att skicka meddelandeexempel till Microsoft.
