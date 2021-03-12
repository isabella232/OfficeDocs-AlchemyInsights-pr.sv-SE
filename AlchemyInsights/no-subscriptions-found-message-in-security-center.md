---
title: Inga prenumerationer hittades i Säkerhetscenter
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "50714389"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>Inga prenumerationer hittades i Säkerhetscenter

Om du får meddelandet "Inga prenumerationer hittades" när du öppnar Microsoft Defender Säkerhetscenter innebär det att Azure Active Directory (AAD) som används för att logga in användaren på portalen inte har någon Microsoft Defender ATP-licens.  

Licenserna för Windows E5 och Office E5 är separata licenser.

Öppna ett supportärende om licensen har köpts men inte etablerats i den här AAD-instansen. Antingen har du: <br/>
-   Ett möjligt problem med licensetablering.<br/>
-   Du har oavsiktligt etablerat licensen till en annan Microsoft AAD än den som används för autentisering i tjänsten.