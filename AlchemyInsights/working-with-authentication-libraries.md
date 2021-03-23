---
title: Arbeta med autentiseringsbibliotek
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036867"
---
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="eb5bf-102">Arbeta med autentiseringsbibliotek</span><span class="sxs-lookup"><span data-stu-id="eb5bf-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="eb5bf-103">Lös problemet med Microsoft Authentication Library (MSAL) genom att utföra följande rekommenderade steg:</span><span class="sxs-lookup"><span data-stu-id="eb5bf-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="eb5bf-104">**Arbeta med MSAL**: [Autentiseringsbibliotek för Microsoft-identitetsplattform](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) – Den här artikeln visar stöd för Microsoft-autentiseringsbibliotek för flera programtyper.</span><span class="sxs-lookup"><span data-stu-id="eb5bf-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="eb5bf-105">Den innehåller länkar till bibliotekskälla. var du hämtar paketet för appens projekt; och om biblioteket stöder inloggning (autentisering), åtkomst till skyddade webb-API:er (auktorisering) eller både och.</span><span class="sxs-lookup"><span data-stu-id="eb5bf-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="eb5bf-106">**Felsöka autentisering:** MSAL har stöd för flera autentiseringsflöden för användning i olika programscenarier.</span><span class="sxs-lookup"><span data-stu-id="eb5bf-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="eb5bf-107">Beroende på hur klientprogrammet är uppbyggt kan MSAL använda en eller flera av de autentiseringsflöden som stöds av Microsofts identitetsplattform.</span><span class="sxs-lookup"><span data-stu-id="eb5bf-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="eb5bf-108">Flöden kan producera flera typer av token och auktoriseringskoder och kräver olika token för att de ska fungera.</span><span class="sxs-lookup"><span data-stu-id="eb5bf-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="eb5bf-109">**Åtkomsttoken:** [Åtkomsttoken för Microsoft-identitetsplattform](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Lär dig hur ditt API kan verifiera och använda anspråk i en åtkomsttoken.</span><span class="sxs-lookup"><span data-stu-id="eb5bf-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="eb5bf-110">All dokumentation i den här artikeln, förutom där inget anges, gäller endast för token som utfärdats för API:er som du har registrerat.</span><span class="sxs-lookup"><span data-stu-id="eb5bf-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="eb5bf-111">Den gäller inte för token som utfärdats för API:er som ägs av Microsoft och inte heller för att verifiera hur Microsoft-identitetsplattformen kommer att utfärda token för ett API som du skapar.</span><span class="sxs-lookup"><span data-stu-id="eb5bf-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="eb5bf-112">**Supporten för Azure Active Directory Authentication Library (ADAL) har upphöra**</span><span class="sxs-lookup"><span data-stu-id="eb5bf-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="eb5bf-113">**Från och med den 30 juni 2020** kommer vi inte längre att lägga till nya funktioner i ADAL och Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="eb5bf-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="eb5bf-114">Vi kommer att fortsätta att tillhandahålla teknisk support och säkerhetsuppdateringar men tillhandahåller inte längre funktionsuppdateringar.</span><span class="sxs-lookup"><span data-stu-id="eb5bf-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="eb5bf-115">**Med start den 30 juni 2022** kommer vi att avsluta supporten för ADAL och Azure AD Graph och kommer inte längre att tillhandahålla teknisk support eller säkerhetsuppdateringar.</span><span class="sxs-lookup"><span data-stu-id="eb5bf-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="eb5bf-116">Appar som använder ADAL på befintliga OS-versioner fortsätter att fungera efter denna tid men får *ingen teknisk support eller säkerhetsuppdateringar.*</span><span class="sxs-lookup"><span data-stu-id="eb5bf-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="eb5bf-117">Appar som använder Azure AD Graph efter den här tiden kanske inte längre får svar från Azure AD Graph-slutpunkten.</span><span class="sxs-lookup"><span data-stu-id="eb5bf-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="eb5bf-118">**ADAL-migrering**</span><span class="sxs-lookup"><span data-stu-id="eb5bf-118">**ADAL Migration**</span></span>

- <span data-ttu-id="eb5bf-119">Vi rekommenderar att du uppdaterar till MSAL, som har de senaste funktionerna och säkerhetsuppdateringarna.</span><span class="sxs-lookup"><span data-stu-id="eb5bf-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="eb5bf-120">Om du använder Microsoft-appar vet du att Microsoft håller på att migrera sina appar till MSAL innan supporten har löpt ut, vilket säkerställer att de kommer att dra nytta av de kontinuerliga förbättringarna av säkerhet och funktioner i MSAL.</span><span class="sxs-lookup"><span data-stu-id="eb5bf-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="eb5bf-121">[Läs vanliga frågor och svar om ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)</span><span class="sxs-lookup"><span data-stu-id="eb5bf-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="eb5bf-122">[Läs mer om hur du migrerar appar per plattform.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance)</span><span class="sxs-lookup"><span data-stu-id="eb5bf-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="eb5bf-123">Om du har fler frågor efter att ha läst guiden för din appplattform kan du publicera något på [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) med taggen [azure-ad-adal-deprecation] eller öppna ett problem på bibliotekets GitHub-lagringsplats.</span><span class="sxs-lookup"><span data-stu-id="eb5bf-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="eb5bf-124">I avsnittet [Språk och ramverk i översiktsartikeln](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) för **MSAL** finns länkar till varje biblioteks lagringsdel.</span><span class="sxs-lookup"><span data-stu-id="eb5bf-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="eb5bf-125">**Om du behöver hjälp med att förstå vilken av dina appar** som använder ADAL rekommenderar vi att du granskar alla dina appars källkod.</span><span class="sxs-lookup"><span data-stu-id="eb5bf-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="eb5bf-126">Om tillämpligt kan du kontakta oberoende programvaruleverantörer (ISV) eller appleverantörer.</span><span class="sxs-lookup"><span data-stu-id="eb5bf-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="eb5bf-127">Microsoft support kan också ge dig en lista med alla ADAL-appar som inte kommer från Microsoft i din klientorganisation.</span><span class="sxs-lookup"><span data-stu-id="eb5bf-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>







