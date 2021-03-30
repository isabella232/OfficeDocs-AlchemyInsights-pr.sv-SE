---
title: Problem med appregistreringsklienthemlighet eller certifikat
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
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405331"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="1ae05-102">Problem med appregistreringsklienthemlighet eller certifikat</span><span class="sxs-lookup"><span data-stu-id="1ae05-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="1ae05-103">Går programhemligheten ut?</span><span class="sxs-lookup"><span data-stu-id="1ae05-103">Application client secret expiring?</span></span>

<span data-ttu-id="1ae05-104">Oavsett hur det registrerade programmet skapades, oavsett om det är genom standardregistreringsprocessen i registreringsportalen för appar eller om Service Principal skapades i klientorganisationen med hjälp av programmedgivande, måste en ny klienthemlighet skapas före utgångsdatumet för den aktuella och uppdateras i den relaterade programkoden.</span><span class="sxs-lookup"><span data-stu-id="1ae05-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="1ae05-105">Max giltighetsperioden är 2 år.</span><span class="sxs-lookup"><span data-stu-id="1ae05-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="1ae05-106">Som en påminnelse måste det hemliga värdet registreras eftersom det inte längre visas när du lämnar registreringssidan för appen i portalen.</span><span class="sxs-lookup"><span data-stu-id="1ae05-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="1ae05-107">Mer information finns i [Snabbstart: Registrera en app på Microsoft-identitetsplattformen](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) och [Metodtips för Microsofts identitetsplattform.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)</span><span class="sxs-lookup"><span data-stu-id="1ae05-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="1ae05-108">Mer information finns i Skapa [en Azure AD-app & tjänstens huvudnamn i portalen – Microsoft-identitetsplattformen.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)</span><span class="sxs-lookup"><span data-stu-id="1ae05-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
