---
title: SAML assertions (tokens)
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
- "9004341"
- "7753"
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885677"
---
# <a name="saml-assertions-tokens"></a>SAML assertions (tokens)

1. (Security Assertion Markup Language) token är XML-representationer av anspråk. Som standard utfärdas tokens för SAML-token Windows Communication Foundation (WCF) i externa säkerhets scenarier. Mer information finns i [SAML-token och anspråk](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).
2. Microsoft Identity Platform har flera typer av säkerhetstoken i bearbetningen av varje autentiseringspaket. [Referens för SAML-Tokenbegäran](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) beskriver format, säkerhets egenskaper och innehållet i SAML 2,0-token.
3. Följ vägledningen i [konfigurations bara livs längder för token i Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) för att förstå hur du konfigurerar livs längd för token.
4. Följ de steg som beskrivs i [den här artikeln](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) för att förstå hur du konfigurerar Azure AD SAML token-kryptering.
5. I Azure AD kan du ställa in alternativ för certifikat signering och algoritm för certifikat signering. Mer information finns i [Avancerade alternativ för certifikat signering i SAML-token för Galleri-appar i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
