---
title: Problem med token
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917215"
---
# <a name="issues-with-tokens"></a>Problem med token

Om du vill hantera problem relaterade till tokens kan du utföra följande steg:

1. Du kan ange livs längden för en åtkomst, ID eller SAML-token som utfärdas av Microsoft Identity Platform. Du kan ange livs längd för alla program i organisationen, för ett program med flera innehavare (flera organisationer) eller för ett specifikt tjänst huvud i organisationen. Mer information finns i [konfigurations bara livs längder för token i Microsoft Identity Platform (för hands version)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. Access-token gör att klienter säkert kan ringa skyddade webb-API: er och används av webb-API: er för autentisering och godkännande. Som en OAuth-specifikation är åtkomst till tokens ogenomskinliga strängar utan ett angivet format-vissa identitets leverantörer (IDPs) använder GUID, andra använder krypterade blob. I Microsoft Identity Platform används en mängd olika Access-Tokenbegäran beroende på konfigurationen för det API som accepterar token. Information om hur din API kan verifiera och använda anspråk i en åtkomsttoken finns i [Microsoft Identity Platform Access tokens](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).
3. Microsoft-autentiseringspaketet (MSAL) har stöd för flera autentiseringsscheman för användning i olika program scenarier. Mer information finns i [autentiseringsscheman](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. Granting Code för OAuth 2,0 kan användas i appar som är installerade på en enhet för att få åtkomst till skyddade resurser, till exempel webb-API: er. Om du använder Microsoft Identity Platform-implementeringen av OAuth 2,0 kan du lägga till inloggnings-och API-åtkomst till dina mobila och Station ära appar. Se [Microsoft Identity Platform och OAuth 2,0 Authorization Code](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) schema för hur du kan program mera direkt mot protokollet i programmet med något annat språk.
5. OpenID Connect (OIDC) är ett autentiseringsprotokoll inbyggt i OAuth 2,0 som du kan använda för att säkert logga in en användare i ett program. När du använder implementeringen av OpenID Connect i Microsoft Identity Platform kan du lägga till inloggnings-och API-åtkomst till dina appar. [Protokollet Microsoft Identity Platform och OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) visar hur du gör detta oberoende av språk och beskriver hur du skickar och tar emot http-meddelanden utan att använda Microsoft Open-source-bibliotek.
    - Användar slut punkten är en del av OIDC standard, utformad för att returnera anspråk för den användare som autentiserats. Mer information finns i [Microsoft Identity Platform UserInfo-slutpunkt](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - När du [anropar ett webb-API i ett webb program med hjälp av Azure AD och OpenID Connect](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) visas hur du skapar ett MVC-webbprogram som använder Azure AD för att logga in med hjälp av OpenID Connect-protokollet och sedan anropa ett webb-API under den inloggade användarens identitet med tokens som erhålls via OAuth 2,0. I det här exemplet används OpenID Connect .net OWIN-mellanvara och ADAL .net.
6. [Konfigurera ett program för att visa ett webb-API](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) -i det här snabb start programmet registrerar du ett webb-API med Microsoft Identity Platform och visar det för klient program genom att lägga till ett exempel på ett scope. När du registrerar ditt webb-API och visar det via omfattningar kan du ge behörighet till dess resurser till behöriga användare och klient program som har till gång till din API.
7. I Azure Active Directory-B2C (Azure AD B2C) är flödet för resurs ägar lösen ord (ROPC) ett OAuth-standardflöde. I det här flödet är ett program, även kallat förlitande part, en giltig identifiering för token. Uppgifterna inkluderar ett användar-ID och lösen ord. De tillgängliga tokens är en ID-token, Access-token och en uppdateringstoken. Mer information finns i [Konfigurera ett flöde för autentiseringsuppgifter för resurs ägare i Azure Active Directory-B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 

