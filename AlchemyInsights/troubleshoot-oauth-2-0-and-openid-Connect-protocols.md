---
title: Felsöka OAuth 2.0- och OpenID Connect-protokoll
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037697"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>Felsöka OAuth 2.0- och OpenID Connect-protokoll

Så här löser du problem med OAuth 2.0 och OpenID Connect:

Se följande artiklar om konfiguration och felsökning av OAuth 2.0- och OpenID Connect-protokoll:

- Microsoft Identity Platform och [OAuth 2.0-auktoriseringskodflöde](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – Den här artikeln beskriver hur du programmerar direkt mot programflödet **(PKCE)** i programmet, på vilket språk som helst.
- [Microsoft-identitetsplattformen](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) och flödet för OAuth 2.0-klientautentiseringsuppgifter – i den här artikeln beskrivs hur du programmerar direkt mot **klientautentiseringsflödet** i programmet.
- [Microsoft identity platform och OAuth 2.0 Resource Owner Password Credentials](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) – Den här artikeln beskriver hur du programmerar direkt mot **ROPC-flödet** i programmet.
    - Microsoft-identitetsplattformen stöder endast ROPC för Azure AD-innehavare och inte för personliga konton. Det innebär att du måste använda en klientspecifik slutpunkt **( eller https://login.microsoftonline.com/{TenantId_or_Name})** **organisationens slutpunkt.**
    - Personliga konton som bjuds in till en Azure AD-klientorganisation kan inte använda ROPC.
    - Konton som inte har lösenord kan inte logga in via ROPC. I det här scenariot rekommenderar vi att du använder ett annat flöde för appen i stället.
    - Om användare behöver använda [multifaktorautentisering (MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) för att logga in i programmet blockeras de.
    - ROPC stöds inte i [hybrididentitetsfederationsscenarier](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) (till exempel Azure AD och ADFS som används för att autentisera lokala konton). Om användare omdirigeras till en lokal identitetsleverantör kan Azure AD inte testa användarnamnet och lösenordet mot den identitetsleverantören. [Direktautentisering](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) stöds emellertid med ROPC.
    - Ett undantag från ett hybrididentitetsfederationsscenario skulle vara följande: Identifieringsprincip för hemsfär med **AllowCloudPasswordValidation** inställt på **SANT** gör att ROPC-flödet kan fungera för federerade användare när lokalt lösenord synkroniseras till molnet. Mer information finns i Aktivera [direkt ROPC-autentisering av federerade användare för äldre program](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- [Microsoft-identitetsplattformen och OAuth 2.0-flödet](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) för andra – den här artikeln beskriver hur du program direkt mot **OBO-flödet (OBO)** i programmet.
- Microsoft Identity Platform och [OpenID Connect-protokollet](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) – I den här artikeln beskrivs hur du implementerar OpenID Connect-protokollet oberoende av språk och hur du skickar och tar emot HTTP-meddelanden utan att använda Microsofts bibliotek för öppen källkod.

**Åtkomsttoken**

[Åtkomsttoken för Microsoft-identitetsplattform](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Lär dig hur ditt API kan verifiera och använda anspråk i en åtkomsttoken. All dokumentation i den här artikeln, förutom där inget anges, gäller endast för token som utfärdats för API:er som du har registrerat. Den gäller inte för token som utfärdats för API:er som ägs av Microsoft och inte heller för att verifiera hur Microsoft-identitetsplattformen kommer att utfärda token för ett API som du skapar.

**Programkonfiguration**

[Begränsningar och begränsningar för omdirigering av URI (svars-URL)](https://docs.microsoft.com/azure/active-directory/develop/reply-url) – Lär dig hur du konfigurerar din omdirigerings-URI (svars-URL). En omdirigerings-URI, eller svars-URL, är den plats där auktoriseringsservern skickar användaren när programmet har auktoriserats och beviljats en auktoriseringskod eller åtkomsttoken. Auktoriseringsservern skickar koden eller token till omdirigerings-URI: så det är viktigt att du registrerar rätt plats som en del av appregistreringsprocessen.

**Programetablering**

[Självstudiekurs:](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) Utveckla och planera etablering för en TIDM-slutpunkt – Den här artikeln beskriver hur du skapar en SAXM-slutpunkt och integrerar med AAD-etableringstjänsten.


