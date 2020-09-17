---
title: Villkorlig åtkomst med Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807677"
---
# <a name="conditional-access-with-intune"></a>Villkorlig åtkomst med Intune

Användning av  **villkorsstyrd åtkomst**  med Intune kräver tre steg:

- Skapa en  **efterlevnadsprincip**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) för att definiera inställningar som måste uppfyllas innan enheten anses uppfylla kraven. En enhet måste till exempel ha en PIN-kod på minst 6 siffror innan den anses vara kompatibel.
- Skapa en **princip för villkorsstyrd åtkomst**  som definierar vilka resurser som skyddas och vilka villkor som måste uppfyllas för att få åtkomst till resurserna.  En enhet måste [till exempel](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) vara kompatibel innan du kan komma åt företagets e-post.
- Se till att båda reglerna för **efterlevnad**  och  **villkorsstyrd åtkomst**  är riktade till önskade grupper av användare. Detta kan kräva att specifika användar grupper skapas i Azure Active Directory.

**Användbara länkar:**

[Översikt över enhetens efterlevnad](https://docs.microsoft.com/intune/device-compliance-get-started)

[Felsöka CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Fel söknings princip](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

För att skydda e-post (Exchange Online) från åtkomst via icke-kompatibla enheter måste båda dokumenten följas:

1. [Skydda e-poståtkomst från enheter med hjälp av EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Skydda e-poståtkomst från enheter med moderna klienter som Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)