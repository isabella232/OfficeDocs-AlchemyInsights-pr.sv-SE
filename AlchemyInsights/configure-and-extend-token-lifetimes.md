---
title: Konfigurera och förläng livs längd för token
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917198"
---
# <a name="configure-and-extend-token-lifetimes"></a>Konfigurera och förläng livs längd för token

Du kan ange livs längden för en åtkomst-, SAML-eller ID-token som utfärdas av Microsoft Identity Platform. Du kan ange livs längd för alla program i organisationen, för ett program med flera innehavare (flera organisationer) eller för ett specifikt tjänst huvud i organisationen. Mer information finns i [konfigurations bara livs längder för token](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

Exempel [på hur du konfigurerar livs längd för token](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes)finns i exempel.

Information om hur du konfigurerar livs längd och kompatibilitet för ett token i Azure Active Directory-B2C (Azure AD B2C) finns i avsnittet [Konfigurera tokens i Azure Active Directory-B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

I artikeln [Konfigurera session i Azure Active Directory-B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) beskrivs de metoder för enkel inloggning (SSO) som används i Azure AD B2C och som hjälper dig att välja den lämpligaste SSO-metoden när du konfigurerar principen.

**Hur länge tar tokens efter namn? Hur länge är de giltiga för?**

Livstiden för token är 1 timme och sessionens livstid är 24 timmar. Det innebär att om inga förfrågningar har gjorts inom 24 timmar måste du logga in igen innan du begär en ny token.

> [!NOTE]
> Efter den 30 maj 2020 kan ingen ny klient organisation använda principer för konfigurerings bar token för att konfigurera sessions-och uppdateringstoken. Utfasningen sker inom några månader efter det, vilket innebär att vi slutar att uppfylla befintliga sessioner för session och uppdatering av token. Du kan fortfarande konfigurera livs längd för åtkomsttoken efter utfasningen.






