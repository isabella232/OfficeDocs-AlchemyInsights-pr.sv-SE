---
title: Problem med integrering av sömlös SSO med lokala appar
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
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868768"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problem med integrering av sömlös SSO med lokala appar

Så här felsöker du problem med att integrera sömlös SSO med lokala program:

**Rekommenderade steg**

1. Om du vill konfigurera ett **lokalt program** för **enkel inloggning via tillämpningsproxy** läser du [lösen ords valv för enkel inloggning med programproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Felsöka problem med programproxy**: Vi rekommenderar att du börjar med att granska fel söknings flödet, [Felsöka Application Proxy Connector-problem](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)för att avgöra om programproxy-kopplingar är korrekt konfigurerade. Om du fortfarande har problem med att ansluta till programmet följer du fel söknings stegen i [program för fel söknings program](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Du kan [identifiera CORS-problem](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) genom att använda följande webb läsar verktyg:
    1. Starta webbläsaren och gå till webb programmet.
    1. Tryck på **F12** för att visa fel söknings konsolen.
    1. Försök att återskapa transaktionen och granska konsol meddelandet. En CORS-överträdelse skapar ett konsol fel om ursprung.
    1. Vissa CORS-problem kan inte lösas, till exempel när din app dirigerar om till login.microsoftonline.com, och åtkomsttoken upphör. CORS-samtalet Miss lyckas. En lösning på det här scenariot är att förlänga livs längden för åtkomsttoken, för att förhindra att den upphör att gälla under en användares session. Mer information om hur du gör detta finns i [konfigurations bara livs längder för token i Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Rekommenderade dokument**

- [Konfigurera enkel inloggning i ett program för programproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Enkel inloggning med SAML för lokala program med programproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Förstå och lös Azure Active Directory Application Proxy CORS-frågor](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Felsöka konfigurationer med restriktioner för delegering av Kerberos för tillämpningsproxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)