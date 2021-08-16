---
title: Problem med integrering av sömlös SSO med mina lokala appar
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028310"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problem med integrering av sömlös SSO med mina lokala appar

Så här felsöker du problem med integrering av sömlös enkel inloggning i lokala program:

**Rekommenderade steg**

1. Information om hur **du konfigurerar ett** lokalt program för enkel inloggning via programproxy finns i Lösenordsvalv för enkel inloggning med [programproxy.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) 
1. **Felsöka problem med** programproxy: Vi rekommenderar att du börjar med att granska felsökningsflödet och felsöka problem med [programproxykoppling](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)för att avgöra om programproxyanslutningar är konfigurerade på rätt sätt. Om du fortfarande har problem med att ansluta till programmet följer du felsökningsstegen i [Felsöka programproxyproblem.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Du kan [identifiera KORS-problem](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) med hjälp av följande felsökningsverktyg för webbläsare:
    1. Starta webbläsaren och bläddra till webbappen.
    1. Tryck **på F12** för att få fram felsökningskonsolen.
    1. Försök återskapa transaktionen och granska konsolmeddelandet. En KORS-överträdelse ger upphov till ett konsolfel om ursprung.
    1. Vissa KORS-problem kan inte lösas, till exempel när programmet omdirigerar till login.microsoftonline.com autentisera och åtkomsttoken upphör att gälla. Kors-samtalet misslyckas då. En lösning för det här scenariot är att förlänga livslängden för åtkomsttoken, för att förhindra att den går ut under en användares session. Mer information om hur du gör detta finns i [Konfigurerbara tokenlivslängder i Microsofts identitetsplattform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Rekommenderade dokument**

- [Konfigurera enkel inloggning till ett programproxyprogram](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [ENKEL INLOGGNING MED SAML för lokala program med programproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Förstå och lösa Azure Active Directory med programproxy-KORS-problem](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Felsöka konfigurationer med begränsad delegering av Kerberos för programproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)