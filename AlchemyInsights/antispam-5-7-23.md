---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676515"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Åtgärda problem med e-postleverans för felkod 5.7.23

Verifiera SPF DNS-posten för din domän vid en allmänt tillgänglig SPF- eller DNS-inspelningskontroll på webben.

Kontrollera att det utgående meddelandet inte identifierades som skräppost av Microsoft och dirigerades via [högriskleveranspoolen](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Meddelanden i högriskleveranspoolen klarar inte SPF-kontroller och accepteras därför inte av e-postorganisationen för målet.

Om problemet kvarstår kan du behöva kontakta administratören för den e-postvärd som du försöker skicka e-post till. Anteckna det detaljerade externa felet i avvisningsmeddelandet. Microsoft-supporten kanske inte kan hjälpa till ytterligare.
