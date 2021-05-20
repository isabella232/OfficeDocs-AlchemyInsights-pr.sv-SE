---
title: Inga prenumerationer hittades i säkerhetscentret
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
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544126"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>Inga prenumerationer hittades i säkerhetscentret

Om du får meddelandet "Inga prenumerationer hittades" när du öppnar Microsoft Defender Säkerhetscenter innebär det att den Azure Active Directory (AAD) som används för att logga in användaren på portalen inte har en Microsoft Defender ATP licens.  

Licenserna Windows E5 Office E5 är separata licenser.

Öppna ett supportärende om licensen har köpts men inte etablerats i den här AAD-instansen. Du har antingen: <br/>
-   Ett möjligt problem med licensetablering.<br/>
-   Du har oavsiktligt etablerat licensen till en annan Microsoft AAD än den som används för autentisering i tjänsten.