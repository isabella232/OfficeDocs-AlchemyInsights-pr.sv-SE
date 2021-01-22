---
title: Problem med SSO-anslutning
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
- "9004357"
- "7810"
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935204"
---
# <a name="sso-connection-issues"></a>Problem med SSO-anslutning

1. Följ [Snabbstart: Konfigurera egenskaper för en programguide](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) för att konfigurera programmet.
2. Beroende på vilket program [och det enkel inloggningsalternativ du](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) har valt följer du lämplig vägledning nedan:
    - Information om hur **du** konfigurerar ett lokalt program för **SAML-baserad** enkel inloggning finns i SAML för enkel inloggning för lokala program [med Programproxy.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
    - Information om hur **du konfigurerar** ett molnprogram för **lösenordsbaserad enkel inloggning** finns i Konfigurera enkel inloggning med [lösenord.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Information om hur du  **konfigurerar ett** lokalt program för enkel inloggning via programproxy finns i Lösenordsvalv för enkel inloggning [med Programproxy.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. **Felsöka proxyproblem för** programmet: Vi rekommenderar att du börjar med att granska felsökningsflödet [och](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)felsöka proxyanslutningsproblem för programmet för att avgöra om programmets proxyanslutningar är korrekt konfigurerade. Om du fortfarande har problem med att ansluta till programmet följer du felsökningsflödet i [Felsöka programproxyprogramproblem.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Du kan [identifiera CORS-problem](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) med hjälp av felsökningsverktyg för webbläsare:
    - Starta webbläsaren och bläddra till webbappen.
    - Tryck **på F12** för att visa felsökningskonsolen.
    - Försök återskapa transaktionen och granska konsolmeddelandet. Ett KORS-brott ger ett konsolfel om ursprung.
    - Vissa KORS-problem kan inte lösas, till exempel när programmet omdirigerar till login.microsoft.com autentisera, och åtkomsttoken upphör att gälla. Kors-samtalet misslyckas då. En lösning på det här scenariot är att förlänga livslängden för åtkomsttoken, för att förhindra att den går ut under en användares session. Mer information om hur du gör detta finns i [Konfigurerbara tokenlivslängder i Microsoft-identitetsplattformen.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
4. **Felsöka SAML-baserad** enkel inloggning: Vi rekommenderar att du kontrollerar problem med att logga in på [SAML-baserad](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)enkel inloggning på konfigurerade appar för att hitta lösningar på de problem som du troligtvis stöter på.
5. **Felsökning av lösenordsbaserad** enkel inloggning: Vi rekommenderar att du felsöker lösenordsbaserad enkel inloggning i [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)för att hitta lösningar på de problem som du troligen stöter på.
6. Information om anslutningsproblem vid användning av VPN finns i Hur du använder enkel inloggning [(SSO) över VPN och Wi-Fi anslutningar.](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)
