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
ms.openlocfilehash: 23afea21668191093d612d68ca6e9ab2a844f4a14977631d33f4fd956fc3c4e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005792"
---
# <a name="using-conditional-access-with-intune"></a>Använda villkorsstyrd åtkomst med Intune

Användning av villkorsstyrd åtkomst med Intune kräver 3 steg:

- [Skapa en efterlevnadsprincip för att definiera inställningar som måste uppfyllas för att enheten ska anses vara kompatibel. En enhet måste ha en PIN-kod med minst 6 siffror innan den anses vara kompatibel.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Skapa en princip för villkorsstyrd åtkomst som definierar vilka resurser som ska skyddas och vilka villkor som måste uppfyllas för att komma åt dessa resurser. En enhet måste till exempel vara kompatibel innan åtkomst ges till företagets e-post.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Se till att både efterlevnadsprinciper och villkorsstyrda åtkomstprinciper är riktade till önskade grupper av användare. Det kan kräva att du skapar särskilda grupper med användare i Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Läs mer...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
