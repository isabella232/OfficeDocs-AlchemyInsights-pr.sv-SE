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
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="49f1a-102">Fråga Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="49f1a-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="49f1a-103">Det här avsnittet kan även gälla utvecklare som fortfarande använder Azure AD Graph API.</span><span class="sxs-lookup"><span data-stu-id="49f1a-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="49f1a-104">Men **vi rekommenderar att** du använder Microsoft Graph för alla scenarier med katalog-, identitets-och åtkomst hantering.</span><span class="sxs-lookup"><span data-stu-id="49f1a-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="49f1a-105">**Autentiserings-eller auktoriseringsfel**</span><span class="sxs-lookup"><span data-stu-id="49f1a-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="49f1a-106">Om appen inte kan **Hämta tokens** för att ringa till Microsoft Graph kan du välja **ett problem med att hämta en** Microsoft Graph-kategori för att få mer specifikt hjälp och support för det här avsnittet.</span><span class="sxs-lookup"><span data-stu-id="49f1a-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="49f1a-107">Om ditt program **tar emot 401-eller 403-auktoriseringsfel** när du anropar Microsoft Graph väljer du Microsoft Graph API-kategorin **få ett fel meddelande om nekad åtkomst (Authorization)** i det här avsnittet.</span><span class="sxs-lookup"><span data-stu-id="49f1a-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="49f1a-108">**Jag vill använda Microsoft Graph men inte vet var du ska börja**</span><span class="sxs-lookup"><span data-stu-id="49f1a-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="49f1a-109">Mer information om Microsoft Graph finns i:</span><span class="sxs-lookup"><span data-stu-id="49f1a-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="49f1a-110">Översikt över Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="49f1a-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="49f1a-111">Översikt över identitets-och åtkomst hantering i Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="49f1a-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="49f1a-112">Komma igång med att bygga Microsoft Graph-appar</span><span class="sxs-lookup"><span data-stu-id="49f1a-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="49f1a-113">**Microsoft Graph-Utforskaren** – testa Microsoft Graph API: er i din klient organisation eller en demo klient organisation</span><span class="sxs-lookup"><span data-stu-id="49f1a-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="49f1a-114">**Jag vill använda Microsoft Graph men stöder det v 1.0-katalog-API: erna jag behöver?**</span><span class="sxs-lookup"><span data-stu-id="49f1a-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="49f1a-115">Microsoft Graph är den rekommenderade API för katalog, identitet och åtkomst hantering.</span><span class="sxs-lookup"><span data-stu-id="49f1a-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="49f1a-116">Det finns emellertid ett fåtal luckor mellan vad som är möjligt i Azure AD Graph och Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="49f1a-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="49f1a-117">Läs följande artiklar som markerar de senaste skillnaderna för att hjälpa dig.</span><span class="sxs-lookup"><span data-stu-id="49f1a-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="49f1a-118">Resurs typs skillnader mellan Azure AD Graph och Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="49f1a-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="49f1a-119">Skillnader mellan Azure AD Graph och Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="49f1a-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="49f1a-120">Metod skillnader mellan Azure AD och Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="49f1a-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="49f1a-121">**När jag frågar *användarobjektet* saknas många av dess egenskaper**</span><span class="sxs-lookup"><span data-stu-id="49f1a-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="49f1a-122">`GET https://graph.microsoft.com/v1.0/users` returnerar endast 11 egenskaper som Microsoft Graph Auto-väljer en standard uppsättning med *användar* egenskaper som ska returneras.</span><span class="sxs-lookup"><span data-stu-id="49f1a-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="49f1a-123">Om du behöver andra *användar* egenskaper kan du använda $SELECT för att välja vilka egenskaper som krävs.</span><span class="sxs-lookup"><span data-stu-id="49f1a-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="49f1a-124">Prova först i **Microsoft graphs Utforskare** .</span><span class="sxs-lookup"><span data-stu-id="49f1a-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="49f1a-125">**Vissa värden för användar egenskaper är *Null* trots att jag vet att de är inställda**</span><span class="sxs-lookup"><span data-stu-id="49f1a-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="49f1a-126">Den mest sannolika förklaringen är att programmet har tilldelats *användaren. ReadBasic. all* behörighet.</span><span class="sxs-lookup"><span data-stu-id="49f1a-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="49f1a-127">Detta gör att programmet kan läsa en begränsad uppsättning användar egenskaper och returnerar alla andra egenskaper som null även om de redan har angetts.</span><span class="sxs-lookup"><span data-stu-id="49f1a-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="49f1a-128">Prova att tilldela program *användaren. Läs alla* behörigheter i stället.</span><span class="sxs-lookup"><span data-stu-id="49f1a-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="49f1a-129">Mer information finns i [användar behörigheter för Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span><span class="sxs-lookup"><span data-stu-id="49f1a-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="49f1a-130">**Jag har problem med att använda OData-frågeparametrar för att filtrera data i Mina förfrågningar**</span><span class="sxs-lookup"><span data-stu-id="49f1a-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="49f1a-131">Även om Microsoft Graph har stöd för en mängd olika OData-frågeparametrar stöds inte många av dessa parametrar fullt av katalog tjänster (resurser som ärver från *directoryObject*) i Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="49f1a-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="49f1a-132">Samma begränsningar som fanns i Azure AD Graph finns kvar för den mesta delen i Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="49f1a-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="49f1a-133">**Stöds inte**: $count, $search och $filter värden för *Null* eller *icke-null*</span><span class="sxs-lookup"><span data-stu-id="49f1a-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="49f1a-134">**Stöds inte**: $filter på vissa egenskaper (se resurs avsnitt där egenskaper är filterade)</span><span class="sxs-lookup"><span data-stu-id="49f1a-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="49f1a-135">**Stöds inte**: växling, filtrering och sortering samtidigt</span><span class="sxs-lookup"><span data-stu-id="49f1a-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="49f1a-136">**Stöds inte**: filtrering för en relation.</span><span class="sxs-lookup"><span data-stu-id="49f1a-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="49f1a-137">Till exempel – hitta alla medlemmar i ingenjörs gruppen i Storbritannien.</span><span class="sxs-lookup"><span data-stu-id="49f1a-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="49f1a-138">**Delvis stöd**: $OrderBy på *användare* (DisplayName och userPrincipalName) och *grupp*</span><span class="sxs-lookup"><span data-stu-id="49f1a-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="49f1a-139">**Delvis stöd**: $filter (stöd för endast *EQ*-, *StartsWith*- *eller*, *and*-and *-Limit-* funktioner) kan $Expand (när du expanderar ett enskilt objekts relationer returneras alla relationer, men expanderar en samling med objekts relationer är begränsad)</span><span class="sxs-lookup"><span data-stu-id="49f1a-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="49f1a-140">Mer information finns i [Anpassa svar med frågeparametrar](https://docs.microsoft.com/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="49f1a-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="49f1a-141">**Det API jag ringer fungerar inte-var kan jag testa mer?**</span><span class="sxs-lookup"><span data-stu-id="49f1a-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="49f1a-142">**Microsoft Graph-Utforskaren** – testa Microsoft Graph API: er i din klient organisation eller en demo klient organisation och kontrol lera **exempel frågorna** i Microsoft Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="49f1a-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="49f1a-143">**När jag frågar för att få en ofullständig data uppsättning tillbaka**</span><span class="sxs-lookup"><span data-stu-id="49f1a-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="49f1a-144">Om du frågar en samling (som *användare*) används sid begränsningar i Microsoft Graph så att resultaten alltid returneras med en standard sid storlek.</span><span class="sxs-lookup"><span data-stu-id="49f1a-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="49f1a-145">Programmet bör alltid förvänta sig att bläddra igenom de samlingar som returneras från tjänsten.</span><span class="sxs-lookup"><span data-stu-id="49f1a-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="49f1a-146">Mer information finns i:</span><span class="sxs-lookup"><span data-stu-id="49f1a-146">For more information, see:</span></span>

- [<span data-ttu-id="49f1a-147">Metod tips för Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="49f1a-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="49f1a-148">Växling av Microsoft Graph-data i din app</span><span class="sxs-lookup"><span data-stu-id="49f1a-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="49f1a-149">**Mitt program är för långsamt och får också begränsat. Vilka förbättringar kan jag göra?**</span><span class="sxs-lookup"><span data-stu-id="49f1a-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="49f1a-150">Beroende på ditt scenario finns det en mängd olika alternativ som du kan använda för att göra ditt program mer gjort och i vissa fall mindre känsligt för tjänsten (när du gör för många samtal).</span><span class="sxs-lookup"><span data-stu-id="49f1a-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="49f1a-151">Mer information finns i:</span><span class="sxs-lookup"><span data-stu-id="49f1a-151">To learn more, see:</span></span>

- [<span data-ttu-id="49f1a-152">Metod tips för Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="49f1a-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="49f1a-153">Gruppbegäran</span><span class="sxs-lookup"><span data-stu-id="49f1a-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="49f1a-154">Spåra ändringar via delta-frågor</span><span class="sxs-lookup"><span data-stu-id="49f1a-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="49f1a-155">Få meddelanden om ändringar via webhookar</span><span class="sxs-lookup"><span data-stu-id="49f1a-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="49f1a-156">Begränsnings vägledning</span><span class="sxs-lookup"><span data-stu-id="49f1a-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="49f1a-157">**Var hittar jag mer information om fel och kända problem?**</span><span class="sxs-lookup"><span data-stu-id="49f1a-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="49f1a-158">Information om felsvar i Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="49f1a-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="49f1a-159">Kända problem med Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="49f1a-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="49f1a-160">**Var kan jag kontrol lera status för tjänst tillgänglighet och anslutnings barhet?**</span><span class="sxs-lookup"><span data-stu-id="49f1a-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="49f1a-161">Tjänst tillgänglighet och anslutnings barhet för de underliggande tjänsterna som kan nås via Microsoft Graph kan påverka den allmänna tillgängligheten och prestandan i Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="49f1a-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="49f1a-162">För Azure Active Directory-tjänstens hälsa kontrollerar du status för säkerhets-och **identitets** tjänster som visas på sidan för [Azure-status](https://azure.microsoft.com/status/).</span><span class="sxs-lookup"><span data-stu-id="49f1a-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="49f1a-163">För Office-tjänster som bidrar till Microsoft Graph bör du kontrol lera status för tjänsterna i [instrument panelen för Office-tjänsten](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="49f1a-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
