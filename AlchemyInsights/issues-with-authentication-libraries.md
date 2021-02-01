---
title: Problem med autentiseringsbibliotek
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
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063700"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="a425d-102">Problem med autentiseringsbibliotek</span><span class="sxs-lookup"><span data-stu-id="a425d-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="a425d-103">[Autentiseringsbibliotek för Microsoft-identitetsplattformen](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) listar Microsoft-stödda och kompatibla bibliotek för klient- och mellanprogramsautentisering.</span><span class="sxs-lookup"><span data-stu-id="a425d-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="a425d-104">Microsoft Authentication Library (MSAL) har stöd för flera [autentiseringsflöden](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) för användning i olika programscenarier.</span><span class="sxs-lookup"><span data-stu-id="a425d-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="a425d-105">Om du vill autentisera och skaffa token initierar du ett nytt offentligt eller konfidentiellt klientprogram i koden.</span><span class="sxs-lookup"><span data-stu-id="a425d-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="a425d-106">Du kan ange flera konfigurationsalternativ när du initierar klientappen i Microsoft Authentication Library (MSAL).</span><span class="sxs-lookup"><span data-stu-id="a425d-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="a425d-107">Mer information finns i [Programkonfigurationsalternativ.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)</span><span class="sxs-lookup"><span data-stu-id="a425d-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="a425d-108">**Support för Azure Active Directory Authentication Library (ADAL) och Azure AD Graph API (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="a425d-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="a425d-109">**Från och med den 30 juni 2020** kommer vi inte längre att lägga till nya funktioner i ADAL och Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="a425d-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="a425d-110">Vi kommer att fortsätta att tillhandahålla teknisk support och säkerhetsuppdateringar men tillhandahåller inte längre funktionsuppdateringar.</span><span class="sxs-lookup"><span data-stu-id="a425d-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="a425d-111">**Med början den 30 juni 2022** kommer vi att avsluta supporten för ADAL och Azure AD Graph och kommer inte längre att tillhandahålla teknisk support eller säkerhetsuppdateringar.</span><span class="sxs-lookup"><span data-stu-id="a425d-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="a425d-112">Appar som använder ADAL på befintliga OS-versioner fortsätter att fungera efter den här tiden men får *ingen teknisk support eller säkerhetsuppdateringar.*</span><span class="sxs-lookup"><span data-stu-id="a425d-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="a425d-113">Appar som använder Azure AD Graph efter den här tiden kanske inte längre får svar från Azure AD Graph-slutpunkten.</span><span class="sxs-lookup"><span data-stu-id="a425d-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="a425d-114">**ADAL-migrering**</span><span class="sxs-lookup"><span data-stu-id="a425d-114">**ADAL Migration**</span></span>

<span data-ttu-id="a425d-115">Vi rekommenderar uppdatering till [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de senaste funktionerna och säkerhetsuppdateringarna.</span><span class="sxs-lookup"><span data-stu-id="a425d-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="a425d-116">Om du använder Microsoft-appar vet du att Microsoft arbetar med att migrera programmen till MSAL innan tidsgränsen för supporten löper ut, vilket säkerställer att de kommer att dra nytta av MSAL:s kontinuerliga förbättringar av säkerhet och funktioner.</span><span class="sxs-lookup"><span data-stu-id="a425d-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="a425d-117">Mer information finns i:</span><span class="sxs-lookup"><span data-stu-id="a425d-117">For more information, see:</span></span>

1. [<span data-ttu-id="a425d-118">Läs vanliga frågor och svar om ADAL</span><span class="sxs-lookup"><span data-stu-id="a425d-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="a425d-119">Läs mer om hur du migrerar appar per plattform</span><span class="sxs-lookup"><span data-stu-id="a425d-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="a425d-120">Om du behöver hjälp med att förstå vilka av dina appar som använder ADAL rekommenderar vi att du går igenom alla dina apps källkod och, om tillämpligt, kontakta internetleverantörer eller internetleverantörer.</span><span class="sxs-lookup"><span data-stu-id="a425d-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="a425d-121">Microsoft support kan också ge dig en lista med alla ADAL-appar som inte kommer från Microsoft i din klientorganisation.</span><span class="sxs-lookup"><span data-stu-id="a425d-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="a425d-122">**AAD Graph-migrering**</span><span class="sxs-lookup"><span data-stu-id="a425d-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="a425d-123">För program som använder Azure AD Graph följer du våra riktlinjer för att [migrera Azure AD Graph-appar till Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)</span><span class="sxs-lookup"><span data-stu-id="a425d-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="a425d-124">Vår migreringschecklista ger dig en utgångspunkt.</span><span class="sxs-lookup"><span data-stu-id="a425d-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="a425d-125">Azure-appregistreringsportalen visar vilka program som använder AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="a425d-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="a425d-126">Vi rekommenderar att du granskar alla dina appars källkod, och om tillämpligt kan du nå ut till ISV:er eller programleverantörer.</span><span class="sxs-lookup"><span data-stu-id="a425d-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="a425d-127">Microsofts support kan också ge dig en lista över all AAD Graph-användning i din klientorganisation.</span><span class="sxs-lookup"><span data-stu-id="a425d-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="a425d-128">För att appen ska kunna komma åt data i Microsoft Graph måste användaren eller administratören bevilja den rätt behörighet via en medgivandeprocess.</span><span class="sxs-lookup"><span data-stu-id="a425d-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="a425d-129">I [behörighetsreferensen för Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) visas behörigheterna som är kopplade till varje huvuduppsättning Microsoft Graph-API:er.</span><span class="sxs-lookup"><span data-stu-id="a425d-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="a425d-130">Den innehåller även vägledning om hur du använder behörigheterna.</span><span class="sxs-lookup"><span data-stu-id="a425d-130">It also provides guidance about how to use the permissions.</span></span>
