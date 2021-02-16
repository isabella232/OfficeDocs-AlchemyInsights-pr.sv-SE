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
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256970"
---
# <a name="device-writeback"></a>Tillbakaskrivning av enhet

Tillbakaskrivning av enhet används i följande scenarier:

- Aktivera [Windows Hello för företag med hjälp av distribution av hybridcertifikatförtroende](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)
- Aktivera villkorsstyrd åtkomst baserat på enheter med ADFS (2012 R2 eller senare) skyddade program (med tredjepartsförtroende)

    > [!NOTE]
    > En prenumeration på Azure AD Premium krävs för återskrivning av enhet.

Det ger ytterligare säkerhet och garanti för att åtkomst till program endast beviljas betrodda enheter. Mer information om villkorsstyrd åtkomst finns i [Hantera risker](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) med villkorsstyrd åtkomst och konfigurera lokal villkorsstyrd [åtkomst med hjälp av Azure Active Directory-enhetsregistrering.](https://docs.microsoft.com/azure/active-directory/devices/overview)

Mer information om hur du aktiverar tillbakaskrivning av enheter för enheter finns i [Aktivera enhetsskrivning.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)
