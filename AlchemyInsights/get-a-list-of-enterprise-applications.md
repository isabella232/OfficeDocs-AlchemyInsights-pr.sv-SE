---
title: Hämta en lista över Företagsprogram
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405511"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="ff67a-102">Hämta en lista över Företagsprogram</span><span class="sxs-lookup"><span data-stu-id="ff67a-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="ff67a-103">En **lista** med företagsprogram (alla program eller filtrerade efter visningsnamn, ID, identifierar-URI:er osv.) via Powershell-kommandot finns i [Get-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)</span><span class="sxs-lookup"><span data-stu-id="ff67a-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="ff67a-104">En lista över tjänstens huvudobjekt (alla objekt eller filtrerade efter ID) via Powershell-kommandot finns i [Get-AzureADServicePrincipal (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)</span><span class="sxs-lookup"><span data-stu-id="ff67a-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="ff67a-105">Om du vill visa **en lista med SAML-konfigurerade appar kan följande PowerShell-skript** hjälpa dig:</span><span class="sxs-lookup"><span data-stu-id="ff67a-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="ff67a-106">Varje program kan vara det en OAuth-app eller SAML-app (både galleri- och icke-galleriappar) skapa två objekt i AAD när registreringen sker.</span><span class="sxs-lookup"><span data-stu-id="ff67a-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="ff67a-107">Det ena kallas Application Object och det andra är Service Principal-objektet.</span><span class="sxs-lookup"><span data-stu-id="ff67a-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="ff67a-108">När dududumpar egenskaperna för ett Service Principal Object med PowerShell, kommer du att se att alla program har ett visst antal taggar som är kopplade till den.</span><span class="sxs-lookup"><span data-stu-id="ff67a-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="ff67a-109">OAuth-appar hade en tagg med namnet "**WindowsAzureActiveDirectoryIntegratedApp**"</span><span class="sxs-lookup"><span data-stu-id="ff67a-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="ff67a-110">SAML-galleriappar skulle ha en tagg med namnet "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span><span class="sxs-lookup"><span data-stu-id="ff67a-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="ff67a-111">SAML-appar som inte är galleri skulle ha en tagg med namnet "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span><span class="sxs-lookup"><span data-stu-id="ff67a-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="ff67a-112">Du kan använda de här taggarna och ta reda på vilken typ av app det är.</span><span class="sxs-lookup"><span data-stu-id="ff67a-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="ff67a-113">Taggen "**WindowsAzureActiveDirectoryIntegratedApp**" är gemensam för alla typer av appar.</span><span class="sxs-lookup"><span data-stu-id="ff67a-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="ff67a-114">Du kan använda följande avsnitt för att visa alla SAML-program (både galleri och icke-galleri):</span><span class="sxs-lookup"><span data-stu-id="ff67a-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="ff67a-115">Mer information finns i [Identifiera SAML-aktiverade appar i Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)</span><span class="sxs-lookup"><span data-stu-id="ff67a-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="ff67a-116">**Hitta och visa endast webbprogram:** Använd kommandot nedan för att få alla Azure AD-program med programtypen "Webbapp/API"</span><span class="sxs-lookup"><span data-stu-id="ff67a-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="ff67a-117">Get-AzureADApplication -Alla:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="ff67a-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="ff67a-118">**Hitta och lista enbart interna program:** Kör följande kommando för att få alla ursprungliga klientprogram (stationära/mobila enheter).</span><span class="sxs-lookup"><span data-stu-id="ff67a-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="ff67a-119">Get-AzureADApplication -Alla:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="ff67a-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="ff67a-120">**Exportera all registrerad Azure AD-programinformation till CSV:** Kommandot nedan exporterar alla Azure AD-appar med obligatorisk information till CSV-fil:</span><span class="sxs-lookup"><span data-stu-id="ff67a-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="ff67a-121">Get-AzureADApplication -Alla:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="ff67a-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="ff67a-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span><span class="sxs-lookup"><span data-stu-id="ff67a-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="ff67a-123">**Behöver exportera en lista över oanvända Azure-appar** – granskningsrapport</span><span class="sxs-lookup"><span data-stu-id="ff67a-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="ff67a-124">Azure AD kan visa programloggar endast i upp till 30 dagar förutsatt att du har Azure AD Premium-licens.</span><span class="sxs-lookup"><span data-stu-id="ff67a-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="ff67a-125">Det finns två alternativ för att behålla data i mer än 30 dagar.</span><span class="sxs-lookup"><span data-stu-id="ff67a-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="ff67a-126">Du kan använda [Azure AD-rapport-API:er](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) för att hämta data programmässigt och lagra dem i en databas.</span><span class="sxs-lookup"><span data-stu-id="ff67a-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="ff67a-127">Alternativt kan du integrera granskningsloggar i ett SIEM-system från tredje part.</span><span class="sxs-lookup"><span data-stu-id="ff67a-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="ff67a-128">Du kan också ladda ned applistan för alla program och ägda program under Azure Active Directory>appregistreringar>Ladda ned>alla program/ägda program.</span><span class="sxs-lookup"><span data-stu-id="ff67a-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="ff67a-129">En lista med program via MS Graph finns i [Listprogram – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) och [programresurstyp – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span><span class="sxs-lookup"><span data-stu-id="ff67a-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
