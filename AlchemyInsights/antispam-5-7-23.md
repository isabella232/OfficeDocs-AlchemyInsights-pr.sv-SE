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
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506461"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Åtgärda problem med e-postleverans för felkod 5.7.23

Verifiera SPF DNS-posten för din domän vid en allmänt tillgänglig SPF- eller DNS-inspelningskontroll på webben.

Kontrollera att det utgående meddelandet inte identifierades som skräppost av Microsoft och dirigerades via [högriskleveranspoolen](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Meddelanden i högriskleveranspoolen klarar inte SPF-kontroller och accepteras därför inte av e-postorganisationen för målet.

Om problemet kvarstår kan du behöva kontakta administratören för den e-postvärd som du försöker skicka e-post till. Anteckna det detaljerade externa felet i avvisningsmeddelandet. Microsoft-supporten kanske inte kan hjälpa till ytterligare.
