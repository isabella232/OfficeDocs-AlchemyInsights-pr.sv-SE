---
title: Villkorsstyrd åtkomst med Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704804"
---
# <a name="conditional-access-with-intune"></a>Villkorsstyrd åtkomst med Intune

För  **användning av villkorsstyrd**  åtkomst med Intune krävs tre steg:

- Skapa en  **efterlevnadsprincip** [(Android,](https://docs.microsoft.com/intune/compliance-policy-create-android)  [iOS,](https://docs.microsoft.com/intune/compliance-policy-create-ios)  [Windows)](https://docs.microsoft.com//intune/compliance-policy-create-windows)för att definiera inställningar som måste uppfyllas innan enheten anses vara kompatibel. En enhet måste ha en PIN-kod med minst 6 siffror innan den anses vara kompatibel.
- Skapa en **princip för villkorsstyrd**  åtkomst som definierar vilka resurser som ska skyddas och vilka villkor som måste uppfyllas för att komma åt dessa resurser.  [En enhet måste till](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  exempel vara kompatibel innan åtkomst ges till företagets e-post.
- Se till **att både efterlevnadsprinciper**  **och villkorsstyrda**  åtkomstprinciper är riktade till önskade grupper av användare. Det kan kräva att du skapar särskilda grupper av användare i Azure Active Directory.

**Användbara länkar:**

[Översikt över enhetsefterlevnad](https://docs.microsoft.com/intune/device-compliance-get-started)

[Felsökning av certifikatutfärdare](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Felsökningsprincip](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

För att skydda e-post (Exchange online) från åtkomst från enheter som inte är kompatibla måste båda dokumenten följas:

1. [Skydda e-poståtkomst från enheter med EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Skydda e-poståtkomst från enheter som använder moderna autentiseringsklienter som Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)