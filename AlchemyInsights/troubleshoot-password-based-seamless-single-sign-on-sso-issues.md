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
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972842"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Felsöka lösenordsbaserade problem med enkel inloggning (SSO)

Mer information om grunderna i lösenordsbaserad SSO finns [i Lösenordsbaserad autentisering med Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)

**Konfigurera lösenordsbaserad SSO**

1. [Konfigurera lösenordsbaserad enkel inloggning – Den](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) här artikeln går in på mer information om det lösenordsbaserade SSO-alternativet. Om programmet du ska lägga till kräver anpassad konfiguration och du behöver använda lösenordsbaserad SSO är den här artikeln för dig.
2. [Konfigurera lösenordsbaserad enkel inloggning för on-prem-appar](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) – Programproxy har stöd för flera lägen för enkel inloggning. Lösenordsbaserad inloggning är avsedd för program som använder ett användarnamn eller en lösenordskombination för autentisering. När du konfigurerar lösenordsbaserad inloggning för programmet måste användarna logga in i det lokala programmet en gång. Därefter lagras Azure Active Directory inloggningsinformationen och tilldelas automatiskt till programmet när användarna har fjärråtkomst till den.
    - Du bör redan ha publicerat och testat appen med Programproxy. Om inte följer du stegen i Publicera program med Azure AD-programproxy och fortsätter sedan konfigurationen av lösenordsbaserad SSO för on-prem-appar. [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application)

Information om hur du felsöker lösenordsbaserad SSO finns i [Felsöka lösenordsbaserad enkel inloggning i Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
