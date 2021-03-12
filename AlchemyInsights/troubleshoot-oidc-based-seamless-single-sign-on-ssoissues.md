---
title: Felsöka OIDC-baserade problem med enkel inloggning (SSO)
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
- "9375"
ms.openlocfilehash: e4ddde6176d9ab021b93e23b3cb363e10b1c1048
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747132"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Felsöka OIDC-baserade problem med enkel inloggning (SSO)

- Mer information om hur du lägger till en OIDC-baserad app i din Azure-klientorganisation finns i [Snabbstart: Konfigurera OIDC-baserad](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)enkel inloggning (SSO) för ett program i Azure Active Directory-klienten (Azure AD).
- Mer information om appar som använder OpenID Connect-standarden för att implementera enkel inloggning finns i [Förstå OIDC-baserad enkel inloggning.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)
- Mer information finns i [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)och OpenID Connect-protokoll på Microsofts identitetsplattform om du väljer att skriva koden direkt genom att skicka och hantera HTTP-begäranden direkt, eller använda ett bibliotek med öppen källkod från tredje part i stället för att använda ett av våra bibliotek med öppen källkod.

**Protokoll**

1. [Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) och implicit grant flow – Den implicita grantens definierande egenskap är att token (ID-token eller åtkomsttoken) returneras direkt från /auktorisera slutpunkten i stället för /token-slutpunkten. Det här används ofta som en del av auktoriseringskodflödet, i det som kallas "hybridflödet", och hämtar ID-token för /auktoriseringsbegäran tillsammans med **en auktoriseringskod.** I den här artikeln beskrivs hur du programar direkt mot protokollet i programmet för att begära token från Azure AD.
2. Microsoft Identity Platform och [OAuth 2.0-auktoriseringskodflöde](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – OAuth 2.0-auktoriseringskodsauktoriseringen kan användas i appar som installeras på en enhet för att få åtkomst till skyddade resurser, till exempel webb-API:er. Med implementering av Microsoft-identitetsplattformen för OAuth 2.0 kan du lägga till inloggning och API-åtkomst till **dina mobil- och skrivbordsappar.** I den här artikeln beskrivs hur du programar direkt mot protokollet i programmet på val annat språk.
3. [Microsoft Identity Platform och OpenID Connect-protokollet](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) – När du använder Microsoft Identity-plattformens implementering av OpenID Connect kan du lägga till inloggnings- och API-åtkomst till dina appar. I den här artikeln beskrivs hur du gör detta oberoende av språk och hur du skickar och tar emot HTTP-meddelanden utan att **använda Microsofts bibliotek för öppen källkod.**
4. Microsoft-identitetsplattformen och flödet för [OAuth 2.0-klientautentiseringsuppgifter](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – Du kan använda autentiseringsuppgifterna för OAuth 2.0 som anges i RFC 6749, som ibland kallas **tvåbenta OAuth,** för att komma åt webbaserade resurser genom att använda identiteten för ett program. Den här typen av beviljande används ofta för interaktion mellan server och server som måste köras i bakgrunden, utan omedelbar interaktion med en användare. Dessa typer av program kallas ofta **daemons eller** **tjänstkonton.** I den här artikeln beskrivs hur du programmerar direkt mot protokollet i programmet.
