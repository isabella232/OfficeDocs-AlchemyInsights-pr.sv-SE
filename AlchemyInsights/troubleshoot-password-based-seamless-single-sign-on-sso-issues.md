---
title: Felsöka lösenordsbaserade problem med enkel inloggning (SSO)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714888"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Felsöka lösenordsbaserade problem med enkel inloggning (SSO)

Mer information om grunderna i lösenordsbaserad SSO finns i [Lösenordsbaserad autentisering med Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)

**Konfigurera lösenordsbaserad SSO**

1. [Konfigurera lösenordsbaserad enkel inloggning – i](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) den här artikeln finns mer information om det lösenordsbaserade SSO-alternativet. Om programmet du lägger till kräver anpassad konfiguration och du behöver använda lösenordsbaserad SSO är den här artikeln för dig.
2. [Konfigurera lösenordsbaserad enkel inloggning för on-prem-appar](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) – Programproxy har stöd för flera lägen för enkel inloggning. Lösenordsbaserad inloggning är avsedd för program som använder ett användarnamn/lösenord för autentisering. När du konfigurerar lösenordsbaserad inloggning för programmet måste användarna logga in på det lokala programmet en gång. Därefter lagras inloggningsinformationen i Azure Active Directory och tilldelas automatiskt till programmet när användarna öppnar det via fjärråtkomst.
    - Du bör redan ha publicerat och testat programmet med Programproxy. Om inte, följer du stegen i Publicera program med Azure AD-programproxy och fortsätter sedan konfigurationen av lösenordsbaserade SSO för on-prem-appar. [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application)

Information om hur du felsöker lösenordsbaserad SSO finns i [Felsöka lösenordsbaserad enkel inloggning i Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
