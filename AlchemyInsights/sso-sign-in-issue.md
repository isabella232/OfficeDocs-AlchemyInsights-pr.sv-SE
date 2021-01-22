---
title: Problem med sömlös SSO-inloggning
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
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935214"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Problem med sömlös SSO-inloggning

När användaren har autentiserats cachelagras användarens autentiseringsuppgifter i webbläsaren, så att programmet automatiskt loggar in med samma konto i samma webbläsare. Det kan göra det svårt för en annan användare eller en enskild användare att logga in på flera konton på en enhet. Lös det här: 1. Försök logga in på en annan webbläsare. 2. Rensa webbläsarens cache och/eller cookies och försök logga in igen.

Om du fortfarande har inloggningsproblem rekommenderar vi följande för att diagnostisera och automatisera lösningsstegen:

1. Installera tillägget [Mina program för säker](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) webbläsare om du vill att Azure Active Directory (Azure AD) ska ge bättre diagnos och lösningar när testupplevelsen används i Azure Portal.
2. Återskapa felet med testupplevelsen på appkonfigurationssidan i Azure-portalen. Mer information finns i [Felsöka SAML-baserade program för enkel inloggning.](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues)
3. Om du använder testupplevelsen i Azure-portalen med Tillägget Mina appar säker webbläsare kan du hoppa **över steg 4.**
4. Så här öppnar du den SAML-baserade konfigurationssidan för enkel inloggning:
    - Öppna [Azure-portalen](https://portal.azure.com/) och logga in som **global administratör** eller **Coadmin.**
    - Öppna **Azure Active Directory-tillägget** genom att **välja Alla** tjänster högst upp på den huvudsakliga vänstra navigeringsmenyn.
    - Skriv "Azure Active Directory" i filtersökrutan och välj **Azure Active Directory-objektet.**
    - Välj **Företagsprogram** på den vänstra navigeringsmenyn i Azure Active Directory.
    - Välj **Alla program** om du vill visa en lista över alla dina program. Om du inte ser det program du vill visa här använder  du **filterkontrollen** högst  upp i listan Alla program och ställer in alternativet Visa på **Alla program.**
    - Välj det program du vill konfigurera för enkel inloggning.
    - När programmet har laddats **in väljer du Enkel** inloggning på programmets vänstra navigeringsmeny.
    - Välj **SAML-baserad SSO.**
5. Mer information om rekommenderade steg att följa beror på felet i Problem med att logga in på [SAML-baserad](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)enkel inloggning på konfigurerade appar.
6. Information om hur du felsöker andra inloggningsproblem finns i följande vägledning:
    - [Enkel Sign-On SAML-protokoll](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Så här felsöker du inloggningsfel med Azure Active Directory-rapporter](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Uppmaning om oväntat medgivande](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Fel i användarens medgivande](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Problem med att logga in från Mina program](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Fel på inloggningssidan för program](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Problem med att logga in på en Microsoft-app](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
