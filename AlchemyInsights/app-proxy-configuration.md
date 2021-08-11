---
title: Proxykonfiguration för app
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
- "9004356"
- "7800"
ms.openlocfilehash: 835bfc59f77b31dc9a37c98db911505e2c7a758b37406dfc4da2d139afa61db5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951583"
---
# <a name="app-proxy-configuration"></a>Proxykonfiguration för app

1. Information om hur du konfigurerar ett programproxyprogram i Azure AD för att visa dina lokala program i molnet finns i Konfigurera ett [programproxyprogram.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)
2. Med enkel inloggning (SSO) kan användarna komma åt ett program utan att autentisera flera gånger. Det gör att den enda autentiseringen sker i molnet, mot Azure Active Directory, och gör att tjänsten eller Anslutningen kan personifiera användaren för att slutföra alla ytterligare autentiseringsutmaningar från programmet. Mer information finns i Konfigurera [enkel inloggning till ett programproxyprogram](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).
3. Använd [den här artikeln](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) för att felsöka vanliga problem som människor ställs inför när du skapar ett nytt programproxyprogram.
4. Om du har problem med att konfigurera backend-autentisering i programmet kan du behöva Felsöka konfigurationer av [Kerberos-begränsade](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) ombud för Programproxy eller följa konfigurerar programmet med [PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) för att lösa problemet.
