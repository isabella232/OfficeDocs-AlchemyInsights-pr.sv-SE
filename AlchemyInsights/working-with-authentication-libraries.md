---
title: Arbeta med autentiseringsbibliotek
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
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036867"
---
# <a name="working-with-authentication-libraries"></a>Arbeta med autentiseringsbibliotek

Lös problemet med Microsoft Authentication Library (MSAL) genom att utföra följande rekommenderade steg:

1. **Arbeta med MSAL**: [Autentiseringsbibliotek för Microsoft-identitetsplattform](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) – Den här artikeln visar stöd för Microsoft-autentiseringsbibliotek för flera programtyper. Den innehåller länkar till bibliotekskälla. var du hämtar paketet för appens projekt; och om biblioteket stöder inloggning (autentisering), åtkomst till skyddade webb-API:er (auktorisering) eller både och.

2. **Felsöka autentisering:** MSAL har stöd för flera autentiseringsflöden för användning i olika programscenarier. Beroende på hur klientprogrammet är uppbyggt kan MSAL använda en eller flera av de autentiseringsflöden som stöds av Microsofts identitetsplattform. Flöden kan producera flera typer av token och auktoriseringskoder och kräver olika token för att de ska fungera.

3. **Åtkomsttoken:** [Åtkomsttoken för Microsoft-identitetsplattform](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Lär dig hur ditt API kan verifiera och använda anspråk i en åtkomsttoken. All dokumentation i den här artikeln, förutom där inget anges, gäller endast för token som utfärdats för API:er som du har registrerat. Den gäller inte för token som utfärdats för API:er som ägs av Microsoft och inte heller för att verifiera hur Microsoft-identitetsplattformen kommer att utfärda token för ett API som du skapar.

**Supporten för Azure Active Directory Authentication Library (ADAL) har upphöra**

- **Från och med den 30 juni 2020** kommer vi inte längre att lägga till nya funktioner i ADAL och Azure AD Graph. Vi kommer att fortsätta att tillhandahålla teknisk support och säkerhetsuppdateringar men tillhandahåller inte längre funktionsuppdateringar.
- **Med start den 30 juni 2022** kommer vi att avsluta supporten för ADAL och Azure AD Graph och kommer inte längre att tillhandahålla teknisk support eller säkerhetsuppdateringar.
- Appar som använder ADAL på befintliga OS-versioner fortsätter att fungera efter denna tid men får *ingen teknisk support eller säkerhetsuppdateringar.*
- Appar som använder Azure AD Graph efter den här tiden kanske inte längre får svar från Azure AD Graph-slutpunkten.

**ADAL-migrering**

- Vi rekommenderar att du uppdaterar till MSAL, som har de senaste funktionerna och säkerhetsuppdateringarna.
- Om du använder Microsoft-appar vet du att Microsoft håller på att migrera sina appar till MSAL innan supporten har löpt ut, vilket säkerställer att de kommer att dra nytta av de kontinuerliga förbättringarna av säkerhet och funktioner i MSAL.

1. [Läs vanliga frågor och svar om ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Läs mer om hur du migrerar appar per plattform.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance)
3. Om du har fler frågor efter att ha läst guiden för din appplattform kan du publicera något på [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) med taggen [azure-ad-adal-deprecation] eller öppna ett problem på bibliotekets GitHub-lagringsplats. I avsnittet [Språk och ramverk i översiktsartikeln](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) för **MSAL** finns länkar till varje biblioteks lagringsdel.
4. **Om du behöver hjälp med att förstå vilken av dina appar** som använder ADAL rekommenderar vi att du granskar alla dina appars källkod. Om tillämpligt kan du kontakta oberoende programvaruleverantörer (ISV) eller appleverantörer. Microsoft support kan också ge dig en lista med alla ADAL-appar som inte kommer från Microsoft i din klientorganisation.







