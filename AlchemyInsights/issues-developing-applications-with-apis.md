---
title: 'Problem med att utveckla program med API: er'
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975019"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="af09f-102">Problem med att utveckla program med API: er</span><span class="sxs-lookup"><span data-stu-id="af09f-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="af09f-103">Om du vill börja använda Azure Active Directory Graph API läser du [snabb starts guiden för Azure AD Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) eller Visa den [interaktiva dokumentationen för Azure AD Graph API Reference](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span><span class="sxs-lookup"><span data-stu-id="af09f-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="af09f-104">**Slut på stöd för Azure Active Directory-autentiseringspaketet (ADAL) och Azure AD Graph API (AAD-diagram)**</span><span class="sxs-lookup"><span data-stu-id="af09f-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="af09f-105">**Från den 30 juni 2020,** lägger vi inte till några nya funktioner i ADAL och Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="af09f-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="af09f-106">Vi fortsätter att tillhandahålla tekniska support-och säkerhets uppdateringar men tillhandahåller inte längre funktions uppdateringar.</span><span class="sxs-lookup"><span data-stu-id="af09f-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="af09f-107">**Från den 30 juni, 2022**, kommer vi att få support för ADAL och Azure AD-graf och inte längre erbjuda teknisk support eller säkerhets uppdateringar.</span><span class="sxs-lookup"><span data-stu-id="af09f-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="af09f-108">Program som använder ADAL i befintliga OS-versioner fortsätter att fungera efter den här tiden men kommer inte att få teknisk support eller säkerhets uppdateringar.</span><span class="sxs-lookup"><span data-stu-id="af09f-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="af09f-109">Appar som använder Azure AD Graph efter den här tiden kan inte längre få svar från slut punkten för Azure AD-diagrammet.</span><span class="sxs-lookup"><span data-stu-id="af09f-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="af09f-110">**ADAL migrering**</span><span class="sxs-lookup"><span data-stu-id="af09f-110">**ADAL Migration**</span></span>

<span data-ttu-id="af09f-111">Vi rekommenderar att du uppdaterar till [Microsoft-autentiseringspaketet (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), som har de senaste funktionerna och säkerhets uppdateringarna.</span><span class="sxs-lookup"><span data-stu-id="af09f-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="af09f-112">Om du använder Microsoft-appar är det viktigt att Microsoft håller på att migrera sina program till MSAL efter slut för ande av supporten, vilket garanterar att de kommer att få ut så mycket som möjligt av säkerhets-och funktions förbättringar i MSAL.</span><span class="sxs-lookup"><span data-stu-id="af09f-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="af09f-113">[Läs vanliga frågor om ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="af09f-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="af09f-114">[Lär dig mer om hur du migrerar appar per plattform](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="af09f-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="af09f-115">Om du behöver hjälp med att förstå vilka av dina program som använder ADAL rekommenderar vi att du granskar alla dina programs källkod och om tillämpligt, nås till alla ISV-eller app-leverantörer.</span><span class="sxs-lookup"><span data-stu-id="af09f-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="af09f-116">Microsoft Support tillhandahåller också en lista över alla ADAL-appar som inte kommer från Microsoft i din klient organisation.</span><span class="sxs-lookup"><span data-stu-id="af09f-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="af09f-117">**Migrering av AAD-Graf**</span><span class="sxs-lookup"><span data-stu-id="af09f-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="af09f-118">För program som använder Azure AD Graph följer du våra råd för att migrera [Azure AD-graf-appar till Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="af09f-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="af09f-119">[Vår check lista för migrering innehåller en komma igång-plats](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="af09f-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="af09f-120">Registrerings portalen för Azure-appen visar vilka program som använder AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="af09f-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="af09f-121">Vi rekommenderar att du granskar alla dina programs källkod och om tillämpligt, nås till alla ISV-eller app-leverantörer.</span><span class="sxs-lookup"><span data-stu-id="af09f-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="af09f-122">Microsoft-supporten kan också tillhandahålla en lista över alla funktioner i AAD-diagram i klient organisationen.</span><span class="sxs-lookup"><span data-stu-id="af09f-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="af09f-123">För att ditt program ska kunna komma åt data i Microsoft Graph måste användaren eller administratören ge den rätt behörighet genom godkännande processen.</span><span class="sxs-lookup"><span data-stu-id="af09f-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="af09f-124">[Behörighets referensen för Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) visar de behörigheter som är kopplade till varje huvud uppsättning med Microsoft Graph API: er.</span><span class="sxs-lookup"><span data-stu-id="af09f-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="af09f-125">Det ger också vägledning om hur du använder behörigheterna.</span><span class="sxs-lookup"><span data-stu-id="af09f-125">It also provides guidance about how to use the permissions.</span></span>
