---
title: Problem med att utveckla program
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974766"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="79f27-102">Problem med att utveckla program</span><span class="sxs-lookup"><span data-stu-id="79f27-102">Issues developing applications</span></span>

<span data-ttu-id="79f27-103">För att felsöka de vanligaste problemen när du skapar Azure Active Directory (AD)-program kan du läsa följande artiklar:</span><span class="sxs-lookup"><span data-stu-id="79f27-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="79f27-104">Jag ser problem med att logga in på program via Chrome-webbläsaren</span><span class="sxs-lookup"><span data-stu-id="79f27-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="79f27-105">Jag vet inte hur man ändrar token för Tokenbegäran för mitt program</span><span class="sxs-lookup"><span data-stu-id="79f27-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="79f27-106">Jag har förvirrat till hur program medgivande fungerar</span><span class="sxs-lookup"><span data-stu-id="79f27-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="79f27-107">Jag vet inte hur jag ger behörighet till mitt program</span><span class="sxs-lookup"><span data-stu-id="79f27-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="79f27-108">Jag förstår inte skillnaden mellan delegerade och program behörigheter</span><span class="sxs-lookup"><span data-stu-id="79f27-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="79f27-109">\***Slut på stöd för Azure Active Directory-autentiseringspaketet (ADAL) och Azure AD Graph API (AAD-diagram)** _</span><span class="sxs-lookup"><span data-stu-id="79f27-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="79f27-110">Från den 30 juni 2020 lägger vi inte längre till några nya funktioner i Azure Active Directory-autentiseringspaketet (ADAL) och Azure AD Graph API (AAD-diagram).</span><span class="sxs-lookup"><span data-stu-id="79f27-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="79f27-111">Vi fortsätter att tillhandahålla tekniska support-och säkerhets uppdateringar men tillhandahåller inte längre funktions uppdateringar.</span><span class="sxs-lookup"><span data-stu-id="79f27-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="79f27-112">Från och med den 30 juni 2022 kommer vi att få support för ADAL och AAD-graf och inte längre erbjuda teknisk support eller säkerhets uppdateringar.</span><span class="sxs-lookup"><span data-stu-id="79f27-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="79f27-113">Som ett resultat av detta villkor gäller följande:</span><span class="sxs-lookup"><span data-stu-id="79f27-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="79f27-114">Program som använder ADAL i befintliga OS-versioner fortsätter att fungera efter den här tiden men kommer inte att få teknisk support eller säkerhets uppdateringar.</span><span class="sxs-lookup"><span data-stu-id="79f27-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="79f27-115">Appar som använder AAD Graph efter den här tiden får inte längre svar från slut punkten för en AAD-Graf</span><span class="sxs-lookup"><span data-stu-id="79f27-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="79f27-116">_ *ADAL-migrering*\*</span><span class="sxs-lookup"><span data-stu-id="79f27-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="79f27-117">Om du använder Microsoft-appar rekommenderar vi att du uppdaterar till Microsoft-autentiseringspaketet (MSAL), som har de senaste funktionerna och säkerhets uppdateringarna.</span><span class="sxs-lookup"><span data-stu-id="79f27-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="79f27-118">Denna rekommendation är att Microsoft initierar processen att migrera sina appar till MSAL efter tids fri sten för support.</span><span class="sxs-lookup"><span data-stu-id="79f27-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="79f27-119">Migreringen från Microsoft av sina program till MSAL säkerställer att apparna förbehåller sig från MSALs säkerhets-och funktions förbättringar.</span><span class="sxs-lookup"><span data-stu-id="79f27-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="79f27-120">Läs vanliga frågor om ADAL</span><span class="sxs-lookup"><span data-stu-id="79f27-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="79f27-121">Lär dig hur du migrerar appar per plattform</span><span class="sxs-lookup"><span data-stu-id="79f27-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="79f27-122">Om du behöver hjälp med att förstå vilka av dina program som använder ADAL rekommenderar vi att du granskar alla dina programs källkod och, om tillämpligt, kommer ut till någon oberoende program varu leverantör (ISV) eller program leverantör.</span><span class="sxs-lookup"><span data-stu-id="79f27-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="79f27-123">Microsoft Support tillhandahåller också en lista över alla ADAL-appar som inte kommer från Microsoft i din klient organisation.</span><span class="sxs-lookup"><span data-stu-id="79f27-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="79f27-124">**Migrering av AAD-Graf**</span><span class="sxs-lookup"><span data-stu-id="79f27-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="79f27-125">För program som använder AAD-diagram följer du vår vägledning för att migrera AAD Graph-appar till Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="79f27-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="79f27-126">[Vår check lista för migrering innehåller en komma igång-plats](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="79f27-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="79f27-127">Registrerings portalen för Azure-appen visar vilka program som använder AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="79f27-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="79f27-128">Vi rekommenderar att du granskar alla dina programs källkod och, om tillämpligt, kommer ut till oberoende program varu leverantörer eller program leverantörer.</span><span class="sxs-lookup"><span data-stu-id="79f27-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="79f27-129">Microsoft-supporten kan också tillhandahålla information om användning av AAD Graph i din klient organisation.</span><span class="sxs-lookup"><span data-stu-id="79f27-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







