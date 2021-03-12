---
title: Problem med Microsoft Graph API
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
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/29/2021
ms.locfileid: "50714515"
---
# <a name="microsoft-graph-api-issues"></a><span data-ttu-id="1a5ea-102">Problem med Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="1a5ea-102">Microsoft Graph API issues</span></span>

<span data-ttu-id="1a5ea-103">Det här avsnittet kan även gälla för utvecklare som fortfarande använder Azure AD Graph API.</span><span class="sxs-lookup"><span data-stu-id="1a5ea-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="1a5ea-104">Vi rekommenderar dock **starkt att** du använder Microsoft Graph för alla scenarier för katalog-, identitets- och åtkomsthantering.</span><span class="sxs-lookup"><span data-stu-id="1a5ea-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="1a5ea-105">**Autentiserings- eller auktoriseringsproblem**</span><span class="sxs-lookup"><span data-stu-id="1a5ea-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="1a5ea-106">Om din app inte kan hämta **token för** att anropa Microsoft Graph väljer du Problem med att hämta en åtkomsttoken **(autentisering)** Microsoft Graph-kategori för att få mer specifik hjälp och support i det här avsnittet.</span><span class="sxs-lookup"><span data-stu-id="1a5ea-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="1a5ea-107">Om appen får **401- eller 403-auktoriseringsfel** när du ringer Microsoft Graph väljer du kategorin Få ett felmeddelande om nekad åtkomst **(auktorisering)** Microsoft Graph API för att få mer specifik hjälp och support för det här avsnittet.</span><span class="sxs-lookup"><span data-stu-id="1a5ea-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="1a5ea-108">**Jag vill använda Microsoft Graph, men vet inte var jag ska börja**</span><span class="sxs-lookup"><span data-stu-id="1a5ea-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

- [<span data-ttu-id="1a5ea-109">Översikt över Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1a5ea-109">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="1a5ea-110">Översikt över hantering av identitet och åtkomst i Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1a5ea-110">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="1a5ea-111">Komma igång med att skapa Microsoft Graph-appar</span><span class="sxs-lookup"><span data-stu-id="1a5ea-111">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="1a5ea-112">**Microsoft Graph Explorer** – Testa Microsoft Graph-API:er i klientorganisationen eller en demoklientorganisation</span><span class="sxs-lookup"><span data-stu-id="1a5ea-112">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="1a5ea-113">**Jag vill använda Microsoft Graph, men har det stöd för de v1.0-katalog-API:er jag behöver?**</span><span class="sxs-lookup"><span data-stu-id="1a5ea-113">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="1a5ea-114">Microsoft Graph är det rekommenderade API:t för hantering av katalog, identitet och åtkomst.</span><span class="sxs-lookup"><span data-stu-id="1a5ea-114">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="1a5ea-115">Det finns dock fortfarande några luckor mellan vad som är möjligt i Azure AD Graph och Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1a5ea-115">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="1a5ea-116">Läs följande artiklar, som tar upp de senaste skillnaderna som kan vara till hjälp för ditt val:</span><span class="sxs-lookup"><span data-stu-id="1a5ea-116">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="1a5ea-117">Skillnader i resurstyper mellan Azure AD Graph och Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1a5ea-117">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="1a5ea-118">Skillnader i egenskap mellan Azure AD Graph och Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1a5ea-118">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="1a5ea-119">Skillnader i metod mellan Azure AD och Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1a5ea-119">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="1a5ea-120">**API:t som jag anropar fungerar inte – var kan jag testa mer?**</span><span class="sxs-lookup"><span data-stu-id="1a5ea-120">**The API I am calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="1a5ea-121">**Microsoft Graph Explorer** – Testa Microsoft Graph API:er i din klientorganisation eller en demoklientorganisation och ta även en titta på exempelfrågorna **i** Microsoft Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="1a5ea-121">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="1a5ea-122">**Min app är för långsam och begränsas också. Vilka förbättringar kan jag göra?**</span><span class="sxs-lookup"><span data-stu-id="1a5ea-122">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="1a5ea-123">Beroende på ditt scenario finns det ett antal olika alternativ som du har tillgång till för att göra programmet mer mer uttjänat, och i vissa fall mindre beivrat att begränsas av tjänsten (när du ringer för många samtal).</span><span class="sxs-lookup"><span data-stu-id="1a5ea-123">Depending on your scenario, there are a variety of options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

- [<span data-ttu-id="1a5ea-124">Metodtips för Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1a5ea-124">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="1a5ea-125">Grupperingsförfrågningar</span><span class="sxs-lookup"><span data-stu-id="1a5ea-125">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="1a5ea-126">Spåra ändringar via deltafråga</span><span class="sxs-lookup"><span data-stu-id="1a5ea-126">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="1a5ea-127">Få ett meddelande om ändringar via webhooks</span><span class="sxs-lookup"><span data-stu-id="1a5ea-127">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="1a5ea-128">Begränsningsvägledning</span><span class="sxs-lookup"><span data-stu-id="1a5ea-128">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="1a5ea-129">**Var hittar jag mer information om fel och kända problem?**</span><span class="sxs-lookup"><span data-stu-id="1a5ea-129">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="1a5ea-130">Information om Microsoft Graph-felsvar</span><span class="sxs-lookup"><span data-stu-id="1a5ea-130">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="1a5ea-131">Kända problem med Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1a5ea-131">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="1a5ea-132">**Var kan jag kontrollera status för tjänstens tillgänglighet och anslutning?**</span><span class="sxs-lookup"><span data-stu-id="1a5ea-132">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="1a5ea-133">Tjänstens tillgänglighet och anslutning för underliggande tjänster som kan nås via Microsoft Graph kan påverka den övergripande tillgängligheten och prestandan för Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1a5ea-133">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="1a5ea-134">För Azure Active Directory-tjänstens hälsa kontrollerar du statusen för **Säkerhets- och identitetstjänster** som visas på [Azure-statussidan.](https://azure.microsoft.com/status/)</span><span class="sxs-lookup"><span data-stu-id="1a5ea-134">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="1a5ea-135">För Office-tjänster som bidrar till Microsoft Graph kontrollerar du statusen för tjänster som visas på [Hälsoinstrumentpanelen för Office.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="1a5ea-135">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="1a5ea-136">Microsoft Graph-auktoriseringsfel kan vara ett resultat av flera olika problem, varav de flesta genererar ett 401- eller 403-fel.</span><span class="sxs-lookup"><span data-stu-id="1a5ea-136">Microsoft Graph authorization errors can be a result of several different issues, most of which generate a 401 or 403 error.</span></span> <span data-ttu-id="1a5ea-137">Följande kan till exempel leda till auktoriseringsfel:</span><span class="sxs-lookup"><span data-stu-id="1a5ea-137">For example, the following can all lead to authorization errors:</span></span>

- <span data-ttu-id="1a5ea-138">Felaktiga [förvärvsflöden av åtkomsttoken](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span><span class="sxs-lookup"><span data-stu-id="1a5ea-138">Incorrect [access token acquisition flows](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span></span>
- <span data-ttu-id="1a5ea-139">Dåligt konfigurerade [behörighetsomfattningar](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span><span class="sxs-lookup"><span data-stu-id="1a5ea-139">Poorly configured [permission scopes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span></span>
- <span data-ttu-id="1a5ea-140">Brist på [medgivande](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="1a5ea-140">Lack of [consent](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span></span>

<span data-ttu-id="1a5ea-141">\**_Supporten upphör för ADAL (Azure Active Directory Authentication Library) och Azure AD Graph API (AAD Graph)_* _</span><span class="sxs-lookup"><span data-stu-id="1a5ea-141">\**_End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)_* _</span></span>

<span data-ttu-id="1a5ea-142">_\*Från och med den 30 juni 2020\*\*, kommer vi inte längre att lägga till nya funktioner i ADAL och Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="1a5ea-142">_\*Starting June 30th, 2020\*\*, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="1a5ea-143">Vi kommer att fortsätta att tillhandahålla teknisk support och säkerhetsuppdateringar men tillhandahåller inte längre funktionsuppdateringar.</span><span class="sxs-lookup"><span data-stu-id="1a5ea-143">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="1a5ea-144">**Med början den 30 juni 2022** kommer vi att avsluta supporten för ADAL och Azure AD Graph och kommer inte längre att tillhandahålla teknisk support eller säkerhetsuppdateringar.</span><span class="sxs-lookup"><span data-stu-id="1a5ea-144">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="1a5ea-145">Appar som använder ADAL på befintliga OS-versioner fortsätter att fungera efter den här tiden men får *ingen teknisk support eller säkerhetsuppdateringar.*</span><span class="sxs-lookup"><span data-stu-id="1a5ea-145">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="1a5ea-146">Appar som använder Azure AD Graph efter den här tiden kanske inte längre får svar från Azure AD Graph-slutpunkten.</span><span class="sxs-lookup"><span data-stu-id="1a5ea-146">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="1a5ea-147">**ADAL-migrering**</span><span class="sxs-lookup"><span data-stu-id="1a5ea-147">**ADAL Migration**</span></span>

<span data-ttu-id="1a5ea-148">Vi rekommenderar uppdatering till [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de senaste funktionerna och säkerhetsuppdateringarna.</span><span class="sxs-lookup"><span data-stu-id="1a5ea-148">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="1a5ea-149">Om du använder Microsoft-appar vet du att Microsoft migrerar sina program till MSAL innan tidsgränsen för supporten löper ut, vilket säkerställer att de kommer att dra nytta av MSAL:s kontinuerliga förbättringar av säkerhet och funktioner.</span><span class="sxs-lookup"><span data-stu-id="1a5ea-149">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="1a5ea-150">Läs vanliga frågor och svar om ADAL</span><span class="sxs-lookup"><span data-stu-id="1a5ea-150">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="1a5ea-151">Läs mer om hur du migrerar appar per plattform</span><span class="sxs-lookup"><span data-stu-id="1a5ea-151">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="1a5ea-152">Om du behöver hjälp med att förstå vilka av dina appar som använder ADAL rekommenderar vi att du går igenom alla dina apps källkod och, om tillämpligt, kontakta internetleverantörer eller internetleverantörer.</span><span class="sxs-lookup"><span data-stu-id="1a5ea-152">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="1a5ea-153">Microsoft support kan också ge dig en lista med alla ADAL-appar som inte kommer från Microsoft i din klientorganisation.</span><span class="sxs-lookup"><span data-stu-id="1a5ea-153">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="1a5ea-154">**AAD Graph-migrering**</span><span class="sxs-lookup"><span data-stu-id="1a5ea-154">**AAD Graph Migration**</span></span>

<span data-ttu-id="1a5ea-155">För program som använder Azure AD Graph följer du våra riktlinjer för att [migrera Azure AD Graph-appar till Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)</span><span class="sxs-lookup"><span data-stu-id="1a5ea-155">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. <span data-ttu-id="1a5ea-156">[I vår checklista för migrering får du en punkt för att komma igång](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="1a5ea-156">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span>
2. <span data-ttu-id="1a5ea-157">Azure-appregistreringsportalen visar vilka program som använder AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="1a5ea-157">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="1a5ea-158">Vi rekommenderar att du granskar alla dina appars källkod, och om tillämpligt kan du nå ut till ISV:er eller programleverantörer.</span><span class="sxs-lookup"><span data-stu-id="1a5ea-158">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="1a5ea-159">Microsoft Support kan också ge dig en lista över all AAD Graph-användning i din klientorganisation.</span><span class="sxs-lookup"><span data-stu-id="1a5ea-159">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="1a5ea-160">För att appen ska kunna komma åt data i Microsoft Graph måste användaren eller administratören bevilja den rätt behörighet via en medgivandeprocess.</span><span class="sxs-lookup"><span data-stu-id="1a5ea-160">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="1a5ea-161">I [behörighetsreferensen för Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) visas behörigheterna som är kopplade till varje huvuduppsättning Microsoft Graph-API:er.</span><span class="sxs-lookup"><span data-stu-id="1a5ea-161">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="1a5ea-162">Den innehåller även vägledning om hur du använder behörigheterna.</span><span class="sxs-lookup"><span data-stu-id="1a5ea-162">It also provides guidance about how to use the permissions.</span></span>
