---
title: Tillbakaskrivning av enhet
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: c069d0b4588e53250d6cc1f3a66c744ea5c12ae4
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320104"
---
# <a name="device-writeback"></a>Tillbakaskrivning av enhet

Tillbakaskrivning av enhet används i följande scenarier:

- Aktivera [Windows Hello för företag med hjälp av distribution av betrodda hybridcertifikat](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- Aktivera villkorsstyrd åtkomst baserat på enheter till ADFS-skyddade program (2012 R2 eller senare) (beroende på partens förtroenden)

    **Obs!** En prenumeration på Azure AD Premium krävs för tillbakaskrivning av enhet.

Detta ger ytterligare säkerhet och garanti för att åtkomst till program endast beviljas betrodda enheter. Mer information om villkorsstyrd åtkomst finns i Hantera [risker](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) med villkorsstyrd åtkomst och konfigurera villkorlig åtkomst lokalt med [hjälp Azure Active Directory enhetsregistrering.](https://docs.microsoft.com/azure/active-directory/devices/overview)

Mer information om hur du aktiverar enhets tillbakaskrivning för enheter finns i [Aktivera tillbakaskrivning av enhet.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)
