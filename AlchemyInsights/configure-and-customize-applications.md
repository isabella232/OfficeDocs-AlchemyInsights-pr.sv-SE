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
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54045006"
---
# <a name="configure-and-customize-applications"></a>Konfigurera och anpassa program

**Konfigurera program**

1. [Snabbstart: Konfigurera egenskaper för](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) ett program i Azure Active Directory-klientorganisationen (Azure AD) visar hur du konfigurerar vissa egenskaper för ett program.
2. För att integrera dina program med Azure Active Directory har vi utvecklat en samling [självstudiekurser](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) som väg väg för dig genom konfigurationen.
3. [Så här konfigurerar du ett](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) programproxyprogram får du hjälp att förstå hur du konfigurerar ett programproxyprogram i Azure AD så att dina lokala program visas i molnet.
4. [Ladda ned PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)och konfigurera programmet: Följ anvisningarna i Konfigurera *PingAccess* för Azure AD för att skydda program som publiceras med Microsoft Azure AD-programproxy på webbplatsen Ping Identity och ladda ned den senaste versionen av PingAccess.

**Felkonfigurerat programfel (AADSTS650056)**

1. Se till att du öppnar programmet från inloggningsadressen som tillhandahålls av programmets ägare. Annars kan du logga in i programmet på det sätt som är normalt. I de flesta fall löses problemet automatiskt automatiskt. Om det inte gör det kan det här inlägget hjälpa dig felsöka och lösa det.
2. **Om din organisation äger programmet (det vill** säga registrering av program finns i din organisation):
    - Vi rekommenderade åtminstone det eller `User.Read` `openid` delegerade behörighetstillståndet **från Microsoft Graph** till.
    - Se till att programmet och alla dess behörigheter godkänns. Du kan verifiera det genom att titta i **kolumnen Status** för programregistreringen i **API-behörigheter.**
    - I vissa fall kan programmet vara tredje part, men det kan vara registrerat i din organisation. Bekräfta om det här programmet finns med i dina appregistreringar (inte Enterprise-program).
    - Om du fortsätter att se det här felmeddelandet. Sedan kan du behöva skapa medgivande-URL:en som beskrivs i **steg 4.**
3. **Om din organisation inte är programägaren och använder det som ett tredjepartsprogram:**
    - Om du är global administratör/företagsadministratör bör du se medgivandeskärmen. Se till att du markerar kryssrutan **för "Godkännande för din organisations räkning".**
    - Om du inte ser skärmen med medgivande tar du bort Enterprise-programmet och försöker igen.
    - Om du fortsätter att se det här felmeddelandet. Sedan kan du behöva skapa medgivande-URL:en som beskrivs i **steg 4.**
4. Skapa **medgivande-URL:en** manuellt för att användas: Om programmet är utformat för att komma åt en viss resurs kanske du inte kan använda medgivandeknapparna från Azure Portal. Du måste manuellt generera din egen medgivande-URL och använda detta.
    - Du måste hämta och `{App-Id}` från `{App-Uri-Id}` programmets ägare. `{Tenant-Id}` som klientorganisationsidentifierare. Detta blir antingen `yourdomain.onmicrosoft.com` ditt katalog-ID eller det.
    - Om programmet öppnar sig själv för resursen är `{App-Id}` och kommer det att vara `{App-Uri-Id}` detsamma.
5. Mer information finns i Problem [med att logga in på SAML-baserade enkel inloggning på konfigurerade appar.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Anpassa program**

- [Lägga till profilering](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) på organisationens inloggningssida i Azure Active Directory – Använd organisationens logotyp och anpassade färgscheman för att ge dina inloggningssidor i Azure Active Directory (Azure AD) ett enhetligt utseende.
- [Lägg till ditt domännamn med hjälp Azure Active Directory portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) – Varje ny Azure AD-klientorganisation levereras med ett initialt domännamn. Du kan inte ändra eller ta bort det ursprungliga domännamnet, men du kan lägga till organisationens namn. Om du lägger till egna domännamn kan du skapa användarnamn som användarna känner till.
