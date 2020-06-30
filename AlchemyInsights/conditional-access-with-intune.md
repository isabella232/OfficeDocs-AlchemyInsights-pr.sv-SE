---
title: Villkorlig åtkomst med Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931454"
---
# <a name="conditional-access-with-intune"></a>Villkorlig åtkomst med Intune

Om du använder **villkorlig åtkomst** med Intune krävs 3 steg:

- Skapa en **efterlevnadsprincip** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) för att definiera inställningar som måste uppfyllas innan enheten anses vara kompatibel. En enhet måste till exempel ha en stift på minst 6 siffror innan den anses vara kompatibel.
- Skapa en **princip för villkorlig åtkomst** som definierar vilka resurser som skyddas och vilka villkor som måste uppfyllas för att komma åt dessa resurser.  [En](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) enhet måste till exempel vara kompatibel innan den får åtkomst till företagets e-post.
- Se till att både **efterlevnadsprinciper** och **principer för villkorlig åtkomst** är inriktade på önskade grupper av användare. Detta kan kräva att du skapar specifika grupper av användare i Azure Active Directory.

**Användbara länkar:**

[Översikt över enhetsefterlevnad](https://docs.microsoft.com/intune/device-compliance-get-started)

[Felsöka certifikatutfärdar](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Felsökningsprincip](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

För att skydda e-post (Exchange online) från åtkomst av icke-kompatibla enheter måste båda dokumenten följas:

1. [Skydda e-poståtkomst från enheter som använder EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Skydda e-poståtkomst från enheter med moderna autentiseringsklienter som Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)