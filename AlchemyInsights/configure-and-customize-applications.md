---
title: Konfigurera och anpassa program
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
- "9004334"
- "7733"
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063710"
---
# <a name="configure-and-customize-applications"></a>Konfigurera och anpassa program

**Konfigurera program**

1. Snabbstart: Konfigurera egenskaper för ett program i [Azure Active Directory-klienten (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) visar hur du konfigurerar vissa egenskaper för ett program.
2. För att integrera dina program med Azure Active Directory har vi utvecklat en samling [självstudiekurser](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) som vägsöker dig genom konfigurationen.
3. [Om du konfigurerar ett](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) programproxyprogram får du hjälp att förstå hur du konfigurerar ett programproxyprogram i Azure AD så att dina lokala program exponeras i molnet.
4. [Ladda ned PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)och konfigurera programmet: Följ anvisningarna i *Konfigurera PingAccess* för Azure AD för att skydda program som publiceras med Microsoft Azure AD-programproxy på webbplatsen Ping Identity och hämta den senaste versionen av PingAccess.

**Felkonfigurerat programfel (AADSTS650056)**

1. Se till att du kommer åt programmet från inloggningsadressen som tillhandahålls av programägaren. Annars kan du logga in i programmet genom den vanliga processen. I de flesta fall löses problemet automatiskt. Om det inte gör det kan det här inlägget hjälpa dig felsöka och lösa det.
2. **Om din organisation äger programmet (vilket** innebär att programregistreringen finns i din organisation):
    - Vi rekommenderar åtminstone att det eller `User.Read` `openid` delegerade behörigheten från **Microsoft Graph** läggs till.
    - Se till att programmet och alla dess behörigheter godkänns. Du kan verifiera det genom att titta i **kolumnen Status** för programregistreringen i **API-behörigheter.**
    - I vissa fall kan programmet vara tredje part, men det kan vara registrerat i din organisation. Bekräfta om det här programmet finns med i dina appregistreringar (inte Enterprise-program).
    - Om du fortsätter att se det här felmeddelandet. Sedan kan du behöva skapa medgivande-URL:en som beskrivs i **steg 4.**
3. **Om din organisation inte är programägaren och använder den som ett tredjepartsprogram:**
    - Om du är global administratör/företagsadministratör bör du se medgivandeskärmen. Kontrollera att du markerar kryssrutan **för "Godkännande för din organisations räkning".**
    - Om du inte ser medgivandeskärmen tar du bort Enterprise-programmet och försöker igen.
    - Om du fortsätter att se det här felmeddelandet. Sedan kan du behöva skapa medgivande-URL:en som beskrivs i **steg 4.**
4. Skapa **medgivande-URL:en** manuellt som ska användas: Om programmet är utformat för att få åtkomst till en viss resurs kanske du inte kan använda knapparna för medgivande från Azure-portalen. Du måste manuellt generera URL-adressen till ditt medgivande och använda detta.
    - Du måste hämta och `{App-Id}` från `{App-Uri-Id}` programmets ägare. `{Tenant-Id}` blir din klientorganisationsidentifierare. Detta blir antingen `yourdomain.onmicrosoft.com` ditt katalog-ID eller ditt katalog-ID.
    - Om programmet öppnar sig själv för resursen gör det `{App-Id}` samma `{App-Uri-Id}` sak.
5. Mer information finns i Problem [med att logga in på SAML-baserade enkel inloggning för konfigurerade appar.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Anpassa program**

- Lägg [till profilering](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) på organisationens inloggningssida för Azure Active Directory – Använd organisationens logotyp och anpassade färgscheman för att ge dina Inloggningssidor i Azure Active Directory (Azure AD) ett enhetligt utseende.
- [Lägg till ditt eget domännamn med Hjälp av Azure Active Directory-portalen](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) – Alla nya Azure AD-klienter levereras med ett initialt domännamn. Du kan inte ändra eller ta bort det ursprungliga domännamnet, men du kan lägga till organisationens namn. Om du lägger till anpassade domännamn kan du skapa användarnamn som användarna känner till.
