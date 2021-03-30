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
# <a name="get-a-list-of-enterprise-applications"></a>Hämta en lista över Företagsprogram

1. En **lista** med företagsprogram (alla program eller filtrerade efter visningsnamn, ID, identifierar-URI:er osv.) via Powershell-kommandot finns i [Get-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)
2. En lista över tjänstens huvudobjekt (alla objekt eller filtrerade efter ID) via Powershell-kommandot finns i [Get-AzureADServicePrincipal (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)
3. Om du vill visa **en lista med SAML-konfigurerade appar kan följande PowerShell-skript** hjälpa dig:

    Varje program kan vara det en OAuth-app eller SAML-app (både galleri- och icke-galleriappar) skapa två objekt i AAD när registreringen sker. Det ena kallas Application Object och det andra är Service Principal-objektet. När dududumpar egenskaperna för ett Service Principal Object med PowerShell, kommer du att se att alla program har ett visst antal taggar som är kopplade till den.

    - OAuth-appar hade en tagg med namnet "**WindowsAzureActiveDirectoryIntegratedApp**"
    - SAML-galleriappar skulle ha en tagg med namnet "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - SAML-appar som inte är galleri skulle ha en tagg med namnet "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    Du kan använda de här taggarna och ta reda på vilken typ av app det är. Taggen "**WindowsAzureActiveDirectoryIntegratedApp**" är gemensam för alla typer av appar. Du kan använda följande avsnitt för att visa alla SAML-program (både galleri och icke-galleri):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Mer information finns i [Identifiera SAML-aktiverade appar i Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)

4. **Hitta och visa endast webbprogram:** Använd kommandot nedan för att få alla Azure AD-program med programtypen "Webbapp/API"

    Get-AzureADApplication -Alla:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Hitta och lista enbart interna program:** Kör följande kommando för att få alla ursprungliga klientprogram (stationära/mobila enheter).

    Get-AzureADApplication -Alla:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Exportera all registrerad Azure AD-programinformation till CSV:** Kommandot nedan exporterar alla Azure AD-appar med obligatorisk information till CSV-fil:

    - Get-AzureADApplication -Alla:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **Behöver exportera en lista över oanvända Azure-appar** – granskningsrapport

    Azure AD kan visa programloggar endast i upp till 30 dagar förutsatt att du har Azure AD Premium-licens.
    Det finns två alternativ för att behålla data i mer än 30 dagar. Du kan använda [Azure AD-rapport-API:er](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) för att hämta data programmässigt och lagra dem i en databas. Alternativt kan du integrera granskningsloggar i ett SIEM-system från tredje part.

    Du kan också ladda ned applistan för alla program och ägda program under Azure Active Directory>appregistreringar>Ladda ned>alla program/ägda program.

    En lista med program via MS Graph finns i [Listprogram – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) och [programresurstyp – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).
