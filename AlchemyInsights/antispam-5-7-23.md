---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717343"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Korrigera problem med e-postleverans för felkod 5.7.23

Verifiera SPF DNS-posten för din domän hos en offentlig tillgänglig SPF-eller DNS-postkontroll på webben.

Kontrol lera att det utgående meddelandet inte identifierades som skräp post av Microsoft och dirigeras via [poolen med högrisk leveranser](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Meddelanden i poolen med hög risk skickar inte SPF-kontroller och kommer därför inte att accepteras av mål-e-postorganisationen.

Om problemet kvarstår kan du behöva kontakta administratören hos e-postvärden som du försöker skicka e-post till. Anteckna det detaljerade externa felet som är tillgängligt i studs meddelandet. Microsoft Support kanske inte kan hjälpa till.
