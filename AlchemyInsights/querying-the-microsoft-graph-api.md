---
title: Fråga Microsoft Graph API
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
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974687"
---
# <a name="querying-the-microsoft-graph-api"></a>Fråga Microsoft Graph API

Det här avsnittet kan även gälla utvecklare som fortfarande använder Azure AD Graph API. Men **vi rekommenderar att** du använder Microsoft Graph för alla scenarier med katalog-, identitets-och åtkomst hantering.

**Autentiserings-eller auktoriseringsfel**

- Om appen inte kan **Hämta tokens** för att ringa till Microsoft Graph kan du välja **ett problem med att hämta en** Microsoft Graph-kategori för att få mer specifikt hjälp och support för det här avsnittet.
- Om ditt program **tar emot 401-eller 403-auktoriseringsfel** när du anropar Microsoft Graph väljer du Microsoft Graph API-kategorin **få ett fel meddelande om nekad åtkomst (Authorization)** i det här avsnittet.

**Jag vill använda Microsoft Graph men inte vet var du ska börja**

Mer information om Microsoft Graph finns i:

- [Översikt över Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Översikt över identitets-och åtkomst hantering i Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Komma igång med att bygga Microsoft Graph-appar](https://docs.microsoft.com/graph/)
- **Microsoft Graph-Utforskaren** – testa Microsoft Graph API: er i din klient organisation eller en demo klient organisation

**Jag vill använda Microsoft Graph men stöder det v 1.0-katalog-API: erna jag behöver?**

Microsoft Graph är den rekommenderade API för katalog, identitet och åtkomst hantering. Det finns emellertid ett fåtal luckor mellan vad som är möjligt i Azure AD Graph och Microsoft Graph. Läs följande artiklar som markerar de senaste skillnaderna för att hjälpa dig.

- [Resurs typs skillnader mellan Azure AD Graph och Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Skillnader mellan Azure AD Graph och Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Metod skillnader mellan Azure AD och Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**När jag frågar *användarobjektet* saknas många av dess egenskaper**

`GET https://graph.microsoft.com/v1.0/users` returnerar endast 11 egenskaper som Microsoft Graph Auto-väljer en standard uppsättning med *användar* egenskaper som ska returneras. Om du behöver andra *användar* egenskaper kan du använda $SELECT för att välja vilka egenskaper som krävs. Prova först i **Microsoft graphs Utforskare** .

**Vissa värden för användar egenskaper är *Null* trots att jag vet att de är inställda**

Den mest sannolika förklaringen är att programmet har tilldelats *användaren. ReadBasic. all* behörighet. Detta gör att programmet kan läsa en begränsad uppsättning användar egenskaper och returnerar alla andra egenskaper som null även om de redan har angetts. Prova att tilldela program *användaren. Läs alla* behörigheter i stället.

Mer information finns i [användar behörigheter för Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Jag har problem med att använda OData-frågeparametrar för att filtrera data i Mina förfrågningar**

Även om Microsoft Graph har stöd för en mängd olika OData-frågeparametrar stöds inte många av dessa parametrar fullt av katalog tjänster (resurser som ärver från *directoryObject*) i Microsoft Graph. Samma begränsningar som fanns i Azure AD Graph finns kvar för den mesta delen i Microsoft Graph:

1. **Stöds inte**: $count, $search och $filter värden för *Null* eller *icke-null*
2. **Stöds inte**: $filter på vissa egenskaper (se resurs avsnitt där egenskaper är filterade)
3. **Stöds inte**: växling, filtrering och sortering samtidigt
4. **Stöds inte**: filtrering för en relation. Till exempel – hitta alla medlemmar i ingenjörs gruppen i Storbritannien.
5. **Delvis stöd**: $OrderBy på *användare* (DisplayName och userPrincipalName) och *grupp*
6. **Delvis stöd**: $filter (stöd för endast *EQ*-, *StartsWith*- *eller*, *and*-and *-Limit-* funktioner) kan $Expand (när du expanderar ett enskilt objekts relationer returneras alla relationer, men expanderar en samling med objekts relationer är begränsad)

Mer information finns i [Anpassa svar med frågeparametrar](https://docs.microsoft.com/graph/query-parameters).

**Det API jag ringer fungerar inte-var kan jag testa mer?**

**Microsoft Graph-Utforskaren** – testa Microsoft Graph API: er i din klient organisation eller en demo klient organisation och kontrol lera **exempel frågorna** i Microsoft Graph Explorer.

**När jag frågar för att få en ofullständig data uppsättning tillbaka**

Om du frågar en samling (som *användare*) används sid begränsningar i Microsoft Graph så att resultaten alltid returneras med en standard sid storlek. Programmet bör alltid förvänta sig att bläddra igenom de samlingar som returneras från tjänsten.

Mer information finns i:

- [Metod tips för Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Växling av Microsoft Graph-data i din app](https://docs.microsoft.com/graph/paging)

**Mitt program är för långsamt och får också begränsat. Vilka förbättringar kan jag göra?**

Beroende på ditt scenario finns det en mängd olika alternativ som du kan använda för att göra ditt program mer gjort och i vissa fall mindre känsligt för tjänsten (när du gör för många samtal).

Mer information finns i:

- [Metod tips för Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Gruppbegäran](https://docs.microsoft.com/graph/json-batching)
- [Spåra ändringar via delta-frågor](https://docs.microsoft.com/graph/delta-query-overview)
- [Få meddelanden om ändringar via webhookar](https://docs.microsoft.com/graph/webhooks)
- [Begränsnings vägledning](https://docs.microsoft.com/graph/throttling)

**Var hittar jag mer information om fel och kända problem?**

- [Information om felsvar i Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Kända problem med Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Var kan jag kontrol lera status för tjänst tillgänglighet och anslutnings barhet?**

Tjänst tillgänglighet och anslutnings barhet för de underliggande tjänsterna som kan nås via Microsoft Graph kan påverka den allmänna tillgängligheten och prestandan i Microsoft Graph.

- För Azure Active Directory-tjänstens hälsa kontrollerar du status för säkerhets-och **identitets** tjänster som visas på sidan för [Azure-status](https://azure.microsoft.com/status/).
- För Office-tjänster som bidrar till Microsoft Graph bör du kontrol lera status för tjänsterna i [instrument panelen för Office-tjänsten](https://portal.office.com/adminportal/home#/servicehealth).
