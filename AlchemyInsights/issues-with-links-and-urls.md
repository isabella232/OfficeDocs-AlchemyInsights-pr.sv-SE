---
title: Problem med länkar och URL-adresser
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: f682afc2006957a83d02973d28e2a07ee63ac888
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707900"
---
# <a name="issues-with-links-and-urls"></a>Problem med länkar och URL-adresser

Omdirigerings-URI eller svars-URL (uttrycken är inte utbytbara) är dem URL-adresser som används av identitetsplattform för Microsoft för att returnera tokens som begärts av appar. Mer information om dessa URL-adresser finns i följande artiklar:

- [Autentiseringsflöden och programscenarier](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – information för varje scenario för omdirigerings-URI:er på sidan **Appregistrering**.
- [Restriktioner och begränsningar för omdirigerings-URI eller svars-URL](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Jag vet inte hur jag registrerar rätt omdirigerings-URI eller svars-URL för appen**

När du loggar in med det program du utvecklar och dialogrutan för inlogging visar **AADSTS50011: svars-URL:en som anges i begäran matchar inte svars-URL:en som har konfigurerats för programmet <your app ID>** så måste du lägga till den omdirigerings-URI som din kod använde när den begärde token till identitetsplattformen för Microsoft, detta gör du i programregistreringen.

Om du vill lägga till en svars-URL går du till fliken **Autentisering** på sidan för **Programregistrering** i Azure-portalen och lägger till en post i avsnittet **Omdirigerings-URI:er**. Värdet du behöver ange beror på vilken typ av program du skapar, se beskrivningen nedan:

- För ensidesapplikationer och webbappar är svars-URL:en en URL i applikationen. Se [Registrering av ensidesapplikationer](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) eller [Registrera en webbapp med hjälp av Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Vilket värde du behöver välja för skrivbordsappar beror på:
    - plattformen (MacOS skiljer sig från Windows och Linux)
    - Hur du hämtar token (interaktivt, med flöde för enhetskod, med integrerad Windows-autentisering [IWA] eller med användarnamn och lösenord).
    Mer information finns i [Skrivbordsappar, Appregistrering, Omdirigerings-URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- För mobilapplikationer beror omdirigerings-URI på:
    - plattformen (iOS/Android/UWP)
    - Den information som används för att skapa appen, till exempel paket-ID för iOS samt paketets namn och signatur med hashfunktion på Android, appregistreringen för Azure-portalen hjälper dig. Mer information finns i [Plattformskonfiguration och omdirigerings-URI:er](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Web API:er och några av de obevakade sätten att hämta tokens (IWA och användarnamn/lösenord) kräver inte en omdirigerings-URI.

**Jag har distribuerat webbapplikationen och när jag testar den distribuerade applikationen får jag en svars-URL om matchningsfel**

Lägg till omdirigerings-URI:er för alla platser som du distribuerar din webbapplikation till. Mer information finns i [Registrera en webbapp med Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Lägg till omdirigerings-URI för en plats direkt efter att du har distribuerat applikationen på den platsen.

**Jag kan inte registrera tillräckligt många svars-URL:er**

Du är en oberoende programvaruleverantör och har en eller flera omdirigerings-URI:er för varje kund. Du bör migrera från ADAL/Azure AD v1.0 till MSAL/identitetsplattformen för Microsoft för att få det [maximala antalet omdirigerings-URI:er](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Lös problemet genom att [lägga till omdirigerings-URI:er till tjänsthuvudnamn](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals), vilket motsvarar var och en av dina kunder.
