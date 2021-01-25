---
title: 'Problem med länkar och URL: er'
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
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974755"
---
# <a name="issues-with-links-and-urls"></a>Problem med länkar och URL: er

Omdirigera URI/Reply URL-adresser (båda uttrycken är utbytbara) är URL-adresser som används av Microsoft Identity Platform för att returnera appen-begärda token. Information om dessa URL-adresser finns i följande artiklar:

- [Autentiseringsscheman och program scenarier](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) -information om hur du omdirigerar URI: er på **registrerings** sidan för varje scenario.
- [Omdirigera begränsningar och begränsningar för URI/Reply URL](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Jag vet inte hur jag registrerar rätt omdirigerande URI/Reply URL för mitt program**

När du loggar in med programmet du utvecklar, om dialog rutan inloggning visar **AADSTS50011: svars-URL-adressen som angavs i begäran inte stämmer överens med svar på URL- <your app ID> adresser som har kon figurer ATS för programmet**, måste du lägga till i din program registrering, omdirigerings-URI som används i Tokenbegäran till Microsoft Identity Platform.

Om du vill lägga till en svars-URL går du till fliken **Verifiera** på din **program registrerings** sida i Azure-portalen och lägger till en post i avsnittet **omdirigera URI: er** . Omdirigera URI: er skrivs (webb eller mobil/stationärt). Det värde du behöver ange beror på vilken typ av program du skapar, enligt beskrivningen nedan:

- För program med en enda sida och webbappar är svars-URL-adressen en URL-adress i programmet. Se [program registrering](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) för en sida eller [Registrera en Web App-app med Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- För skrivbordsappar är det värde som du måste välja beror på:
    - plattformen (MacOS skiljer sig från Windows eller Linux)
    - hur du erhåller token (interaktivt, med enhets kod flöde, integrerad Windows-autentisering [IWA] eller med användar namn/lösen ord).
    Mer information finns i [Desktop-appar-program registrering-omdirigera URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- För mobila program beror omdirigerings-URI på:
    - plattformen (iOS/Android/UWP)
    - informationen som används för att skapa din app, till exempel paket-ID i iOS, samt paket namnet och signatur-hashen för Android din app-registrering i Azure-portalen hjälper dig. För mer information, se [Platform Configuration och omdirigera URI: er](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Webb-API: er och vissa av de tysta sätten att förvärva token (IWA och username) kräver ingen omdirigerings-URI.

**Jag har distribuerat mitt webb program och när jag testar den distribuerade appen får jag ett svar på URL-matchningsfel**

Lägg till omdirigera URI: er för alla platser där du distribuerar webb programmet. Mer information finns i [Registrera en Web App-app med Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Lägg till Omdirigerad URI för en plats direkt efter att du har distribuerat programmet på den platsen.

**Jag kan inte registrera många svars-URL: er**

Du är en ISV och har en eller flera omdirigerings-URI: er till alla kunder. Du vill migrera från ADAL/Azure AD v 1.0 till MSAL/Microsofts identitets plattform och sedan trycka [maximalt antal omdirigerings-URI: er](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Lös problemet genom att [lägga till omdirigera URI: er till tjänstens huvud namn](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) som motsvarar var och en av dina kunder.
