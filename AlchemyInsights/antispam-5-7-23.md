---
title: Antispam-5.7.23
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
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682316"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Åtgärda problem med e-postleverans för felkod 5.7.23

Kontrollera SPF DNS-posten för din domän på en offentligt tillgänglig SPF eller DNS-post Checker på webben.

Kontrollera att det utgående meddelandet inte identifierades som skräppost av Office 365 och dirigeras via [poolen med hög risk](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Meddelanden i poolen med hög risk skickar inte SPF-kontroller och godkänns därför inte av destinations organisationen för e-post.

Om problemet kvarstår kan du behöva kontakta administratören för den e-postvärd som du försöker skicka e-post till. Anteckna det detaljerade externa fel som finns i avvisningsmeddelandet.  Support för Office 365 kanske inte kan hjälpa till ytterligare.