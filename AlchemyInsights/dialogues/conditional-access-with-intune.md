---
title: Använda villkorsstyrd åtkomst med Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694715"
---
# <a name="using-conditional-access-with-intune"></a>Använda villkorsstyrd åtkomst med Intune

Användning av villkorsstyrd åtkomst med Intune kräver tre steg:

- [Skapa en efterlevnadsprincip för att definiera inställningar som måste uppfyllas innan enheten anses vara kompatibel. En enhet måste ha en PIN-kod med minst 6 siffror innan den anses vara kompatibel.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Skapa en princip för villkorsstyrd åtkomst som definierar vilka resurser som ska skyddas och vilka villkor som måste uppfyllas för att komma åt dessa resurser. En enhet måste till exempel vara kompatibel innan åtkomst ges till företagets e-post.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Se till att både efterlevnadsprinciper och villkorsstyrda åtkomstprinciper är riktade till önskade grupper av användare. Det kan kräva att du skapar särskilda grupper av användare i Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Läs mer...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
