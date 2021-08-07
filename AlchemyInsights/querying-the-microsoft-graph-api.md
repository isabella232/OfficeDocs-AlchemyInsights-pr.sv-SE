---
title: Fråga Microsofts Graph API
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
- "9004345"
- "7846"
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923257"
---
# <a name="querying-the-microsoft-graph-api"></a>Fråga Microsofts Graph API

Det här avsnittet kan även gälla för utvecklare som fortfarande använder Azure AD Graph API. Vi rekommenderar dock starkt **att** du använder Microsoft Graph för alla scenarier för hantering av katalog, identitet och åtkomst.

**Autentiserings- eller auktoriseringsproblem**

- Om appen inte kan hämta **token** för att ringa till Microsoft Graph väljer du Problem med att få en åtkomsttoken **(autentisering)** Microsoft Graph-kategori för att få mer specifik hjälp och support för det här avsnittet.
- Om appen får **401- eller 403-auktoriseringsfel** när du ringer Microsoft Graph väljer du kategorin Få åtkomst nekad **(Auktorisering)** Microsoft Graph API för att få mer specifik hjälp och support för det här avsnittet.

**Jag vill använda Microsoft Graph, men vet inte var jag ska börja**

Mer information om Microsoft Graph finns i:

- [Översikt över Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Översikt över identitets- och åtkomsthantering i Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Komma igång med att skapa Microsoft Graph appar](https://docs.microsoft.com/graph/)
- **Microsoft Graph –** testa Microsofts Graph-API:er i klientorganisationen eller en demoklientorganisation

**Jag vill använda Microsoft Graph, men stöder det de v1.0-katalog-API:er jag behöver?**

Microsoft Graph är det rekommenderade API:t för hantering av katalog, identitet och åtkomst. Det finns dock fortfarande några skillnader mellan vad som är möjligt i Azure AD Graph och Microsoft Graph. Läs följande artiklar, där du hittar de senaste skillnaderna som kan vara till hjälp:

- [Skillnader i resurstyp mellan Azure AD Graph och Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Skillnader i egenskap mellan Azure AD Graph och Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Skillnader i metod mellan Azure AD och Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**När jag frågar *användarobjektet* saknas många av dess egenskaper**

`GET https://graph.microsoft.com/v1.0/users`returnerar bara 11 egenskaper eftersom Microsoft Graph automatiskt väljer en standarduppsättning användaregenskaper *som* ska returneras. Om du behöver andra *användaregenskaper* kan $select för att välja de egenskaper som programmet behöver. Testa det först **i Microsoft Graph Explorer.**

**Vissa användaregenskapsvärden *är null* även om jag vet att de har angetts**

Den troligaste förklaringen är att programmet har beviljats *behörigheten User.ReadBasic.All.* Då kan programmet läsa en begränsad uppsättning användaregenskaper och returnera alla andra egenskaper som null även om de har angetts tidigare. Försök att ge programmet *behörigheten User.Read.All* i stället.

Mer information finns i [Microsoft Graph användarbehörigheter.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)

**Jag har problem med att använda OData-frågeparametrar för att filtrera data i mina begäranden**

Även om Microsoft Graph har stöd för ett brett utbud av OData-frågeparametrar stöds inte många av dessa parametrar helt av katalogtjänsterna (resurser som ärver från *katalogObjekt*) i Microsoft Graph. Samma begränsningar som fanns i Azure AD-Graph finns kvar, oftast i Microsoft Graph:

1. **Stöds inte:**$count, $search eller $filter *null-värden* eller *inte null-värden*
2. **Stöds inte:**$filter för vissa egenskaper (se resursavsnitt om vilka egenskaper som kan filtreras)
3. **Stöds inte:** sidnumrering, filtrering och sortering samtidigt
4. **Stöds inte:** filtrering av en relation. Till exempel – hitta alla medlemmar i teknikgruppen som finns i Storbritannien.
5. **Delvis stöd:**$orderby *användare* (endast displayName och userPrincipalName) och *grupp*
6. **Delvis stöd:**$filter (stöder endast *eq* ,  *startswith*, eller och begränsat stöd för *)*$expand (när du expanderar ett objekts relationer returneras alla relationer, men det är begränsat att expandera en samling av objektrelationer)

Mer information finns i Anpassa [svar med frågeparametrar](https://docs.microsoft.com/graph/query-parameters).

**API:t jag anropar fungerar inte – var kan jag testa mer?**

**Microsoft Graph Utforskaren** – testa Microsoft Graph-API:er i din klientorganisation eller  en demoklientorganisation och ta även en titta på exempelfrågorna i Microsoft Graph Explorer.

**När jag frågar efter data verkar det som om jag får tillbaka en ofullständig datauppsättning**

Om du avfrågar en samling (t.ex. användare) använder Microsoft Graph begränsningar på serversidan så att resultaten alltid returneras med en standardstorlek på sidan. Programmet bör alltid gå igenom samlingar som returneras från tjänsten.

Mer information finns i:

- [Microsoft Graph metodtips](https://docs.microsoft.com/graph/best-practices-concept)
- [Sidnumrering för Microsoft Graph data i appen](https://docs.microsoft.com/graph/paging)

**Min app är för långsam och begränsas också. Vilka förbättringar kan jag göra?**

Beroende på scenariot finns det en mängd olika alternativ som du har tillgång till för att göra programmet mer mer uttjänat, och i vissa fall är det mindre risk för att du begränsas av tjänsten (när du ringer för många samtal).

Mer information finns i:

- [Microsoft Graph metodtips](https://docs.microsoft.com/graph/best-practices-concept)
- [Grupperingsförfrågningar](https://docs.microsoft.com/graph/json-batching)
- [Spåra ändringar via deltafråga](https://docs.microsoft.com/graph/delta-query-overview)
- [Få ett meddelande om ändringar via webhooks](https://docs.microsoft.com/graph/webhooks)
- [Begränsningsvägledning](https://docs.microsoft.com/graph/throttling)

**Var hittar jag mer information om fel och kända problem?**

- [Microsoft Graph information om felsvar](https://docs.microsoft.com/graph/errors)
- [Kända problem med Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Var kan jag kontrollera status för tjänstens tillgänglighet och anslutning?**

Tjänstens tillgänglighet och anslutning för de underliggande tjänsterna som kan nås via Microsoft Graph kan påverka Microsofts övergripande tillgänglighet och prestanda Graph.

- För Azure Active Directory tjänstens hälsa kontrollerar du statusen för **säkerhets- och identitetstjänster** som visas på [Azure-statussidan.](https://azure.microsoft.com/status/)
- Om Office tjänster som kan bidra till Microsoft Graph kontrollerar du statusen för de tjänster [Office Hälsoinstrumentpanelen](https://portal.office.com/adminportal/home#/servicehealth).
