---
title: Konfigurera sömlös enkel inloggning (SSO)
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
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: 62f667cccd0761e081b3f651709fadfec12500e76fd8e30b8649a28e99001e4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966055"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Konfigurera sömlös enkel inloggning (SSO)

**Konfigurera program**

1. Du bör få värdena från programleverantören. Du kan manuellt ange värdena eller ladda upp en metadatafil för att extrahera värdet i fälten.
2. Många appar har redan konfigurerats för att fungera med Azure AD. De här apparna visas i galleriet med appar som du kan bläddra i när du lägger till en app i Azure AD-klientorganisationen. I [snabbstartserien](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) får du hjälp med processen.
3. Om du vill skapa ett program som inte är galleriprogram kan du klicka på + Skapa din egen **programknapp** och ge programmet ett namn.
    - Som standard markeras **Integrera andra program** som du inte hittar i galleriet, vilket är det rätta alternativet för program som inte är gallerier.
    - När du trycker **på** Skapa efter att ha lagt till namnet på programmet skapas ett nytt Företagsprogram som inte är galleri.
    - Du kan sedan gå till **enkel** inloggning **under** Hantera av programmet och du kommer att kunna se olika tekniker för implementering i din miljö.

**Konfigurera sömlös enkel inloggning för ett visst program**

För apparna i galleriet hittar du detaljerade anvisningar steg för steg. För att komma åt stegen kan du bläddra i en lista över alla självstudiekurser om appkonfiguration på [självstudiekurserna om appkonfiguration för SaaS.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**Konfigurera SAML-baserad SSO**

1. [Snabbstart: Konfigurera SAML-baserad](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)enkel inloggning (SSO) för ett program i din Azure Active Directory (Azure AD) klientorganisation.
2. Mer information om det SAML-baserade alternativet för enkel inloggning finns i [Förstå SAML-baserad enkel inloggning.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. Mer information om SAML 2.0-autentiseringsförfrågningar och -svar som Azure Active Directory (Azure AD) har stöd för enkel Sign-On (SSO) finns i [Enkel Sign-On SAML-protokoll.](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
4. Information om hur du skapar och konfigurerar en SAML-baserad enkel inloggning (SSO) för ditt program i Azure Active Directory (Azure AD) med Microsoft Graph API finns i Konfigurera [SAML-baserad](https://docs.microsoft.com/graph/application-saml-sso-configure-api)enkel inloggning för programmet med Hjälp av Microsofts API Graph.
5. Mer information om hur Azure AD använder SAML-protokollet finns i [Microsofts identitetsplattform använder SAML-protokollet.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Konfigurera token och anspråk**

1. [Så här gör du för att anpassa anspråk som utfärdats med SAML-token för företagsprogram.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. Mer information om hur du konfigurerar anspråk med hjälp av PowerShell finns i Så här gör du: Anpassa anspråk användarspecifika i token för en viss app i en [klientorganisation (förhandsversion).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
3. Mer information om hur du konfigurerar valfria anspråk finns [i Så här gör du: Uppge valfria anspråk för din app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Mer information om hur du använder attribut för katalogschematillägg för att skicka användardata till program i tokenanspråk finns i Använda attribut för katalogschematillägg [i anspråk.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)
5. Mer information om hur du konfigurerar tokenlivslängder finns i [Konfigurerbara tokenlivslängder i Microsofts identitetsplattform (förhandsversion)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
6. [Konfigurera principer för tokenlivslängd (förhandsversion)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) – I den här artikeln går vi igenom ett vanligt principscenario som kan hjälpa dig att införa nya regler för tokenlivslängd. I det här exemplet får du lära dig hur du skapar en princip som kräver att användarna autentiserar oftare i webbprogrammet.

**Felsöka SSO-konfiguration**

- Vanliga frågor och svar om Azure Active Directory sömlös enkel Sign-On inloggning (sömlös enkel inloggning) Azure Active Directory sömlös enkel [inloggning: Vanliga frågor och svar.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)
- Mer information om felsökning av vanliga problem Azure Active Directory (Azure AD) sömlös enkel Sign-On (Sömlös SSO) finns i Felsöka Azure Active Directory sömlös [enkel inloggning.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)
