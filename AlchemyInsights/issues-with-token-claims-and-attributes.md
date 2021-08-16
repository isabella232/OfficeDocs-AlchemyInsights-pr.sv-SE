---
title: Problem med tokenanspråk och attribut
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
- "9004347"
- "7761"
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012902"
---
# <a name="issues-with-token-claims-and-attributes"></a>Problem med tokenanspråk och attribut

**Uppdatera, konfigurera eller ta bort tokenanspråk**

1. Med hjälp Azure Active Directory (Azure AD) [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) kan du anpassa anspråkstypen för rollanspråk i den svarstoken som du får när du har auktoriserat en app.
2. Programutvecklare kan använda valfria anspråk i sina Azure AD-program för att ange vilka anspråk de vill ha i token som skickas till programmet. Mer information finns i [Tillhandahålla valfria anspråk för din app.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Konfigurera gruppanspråk för program med Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Om du använder sömlös enkel inloggning i programmet kan du se anpassa anspråk som [utfärdats i SAML-token för företagsprogram.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Mappning av anspråksattribut**

1. Information om hur du konfigurerar principen för anspråksmappning med hjälp av PowerShell finns i Anpassa anspråk i token för en viss app i en [klientorganisation (förhandsversion).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Attribut för katalogschematillägg är ett sätt att lagra ytterligare data i Azure Active Directory användarobjekt och andra katalogobjekt, till exempel grupper, information om klientorganisationen och tjänstens huvudnamn. Endast tilläggsattribut för användarobjekt kan användas för att avge anspråk till program. [Med hjälp av attribut för katalogschematillägg i](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) anspråk beskrivs hur du använder attribut för katalogschematillägg för att skicka användardata till program i tokenanspråk.

Mer information om tokenanspråk finns i:

- [Anspråk i åtkomsttoken](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Anspråk i en id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Anspråk som](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) du kan förvänta dig i ID-token och åtkomsttoken som utfärdats av Azure AD B2C
- [Anspråksreferens för SAML token](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
