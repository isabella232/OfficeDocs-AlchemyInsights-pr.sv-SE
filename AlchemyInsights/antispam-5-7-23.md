---
title: Skydd motspam – 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: cb9073306c65b09813290d6c8470d14395d2836fa3048f8ce0ecb8b06e71a010
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932187"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Korrigera problem med e-postleverans för felkod 5.7.23

Verifiera SPF DNS-posten för din domän på en offentligt tillgänglig SPF- eller DNS-postkontroll på webben.

Kontrollera att det utgående meddelandet inte identifierats som skräppost av Microsoft och dirigerats via [Högriskleveranspool.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Meddelanden i högriskleveranspoolen passerar inte SPF-kontroller och accepteras därför inte av mål-e-postorganisationen.

Om problemet kvarstår kan du behöva kontakta administratören för e-postvärden som du försöker skicka e-post till. Anteckna det detaljerade externa felet som finns i studsande meddelandet. Microsoft Support kanske inte kan hjälpa dig vidare.
