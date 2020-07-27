---
title: Princip för programskydd
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423959"
---
# <a name="application-protection-policy"></a>Princip för programskydd

Om du inte har en ny till Application Protection Policy (APP) kan du läsa [översikten över appskyddsprinciper](https://docs.microsoft.com/intune/apps/app-protection-policy).

Lär dig hur du [skapar och tilldelar principer för appskydd](https://docs.microsoft.com/intune/app-protection-policies).

Krav på programskydd:

- Användaren har en Intune- eller EMS-licens.
- Användaren tillhör en grupp som omfattas av programskyddsprinciper.
- Endast en företagsanvändare är inloggad i skyddade appar på en enhet.
- Programmet har [implementerat Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started). En lista över appar som stöder SDK finns [i Microsoft Intune-skyddade appar](https://docs.microsoft.com/intune/apps-supported-intune-apps).

Principer gäller när en användare som uppfyller ovanstående krav loggar in på en Intune SDK-aktiverad app. Det enklaste sättet att avgöra om en princip tillämpas är genom att kräva att användaren anger en pin i principen. 

Mer information finns i:

[Vanliga frågor och svar om APP/MAM-felsökning](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[Så här validerar du principinställningarna för appskydd](https://docs.microsoft.com/intune/app-protection-policies-validate)

[Förstå leveranstid för appskyddsprincip](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[Så här övervakar du appskyddsprinciper](https://docs.microsoft.com/intune/app-protection-policies-monitor)