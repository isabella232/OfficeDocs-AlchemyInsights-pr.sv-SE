---
title: 1048 5.7.750 Tjänsten är inte tillgänglig. Klient som blockerats från att skicka från oregistrerade domäner
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 0fd0fd730d562fa0313d61c1593d6eab91b3bc8cc15ba277e9cd4e4deb6901bd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919081"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a>5.7.750 Client blocked from sending from unregistered domain

Felet inträffar när en stor mängd meddelanden skickas från domäner som inte är etablerade i klientorganisationen (läggs till som godkända domäner och valideras).

Du kan undvika det här felet genom att använda en certifikatbaserad e-postflödeskoppling där certifikatets domän är en etableringsdomän, eller så kan du etablera alla avsändande domäner.

Mer information finns i Korrigera problem med e-postleverans för [felkoder mellan 5.7.700 och 5.7.750 i Exchange Online.](https://go.microsoft.com/fwlink/?linkid=2164955)