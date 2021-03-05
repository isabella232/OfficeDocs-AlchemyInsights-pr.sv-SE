---
title: Konfigurera etableringstjänsten
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
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484045"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="af19d-102">Konfigurera etableringstjänsten</span><span class="sxs-lookup"><span data-stu-id="af19d-102">Configuring the Provision service</span></span>

<span data-ttu-id="af19d-103">För att automatisera användaretablering ska fungera kräver Azure AD giltiga autentiseringsuppgifter som gör att det går att ansluta till API för arbetsdagar-webbtjänster.</span><span class="sxs-lookup"><span data-stu-id="af19d-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="af19d-104">Dessutom verifierar knappen Testanslutning i workday till AD-appen för användaretablering även om den kan ansluta till Azure AD Connect Provisioning Agent som är kopplad till AD-domänen.</span><span class="sxs-lookup"><span data-stu-id="af19d-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="af19d-105">Om Azure Portal returnerar ett fel när du sparar autentiseringsuppgifterna följer du de rekommenderade stegen nedan:</span><span class="sxs-lookup"><span data-stu-id="af19d-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="af19d-106">Bekräfta att du har konfigurerat användarkontot för Workday Integration System enligt i avsnittet Konfigurera [integreringssystemanvändare under Arbetsdagar.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="af19d-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="af19d-107">Kontrollera att Azure AD Connect Provisioning Agent Service är igång på din lokala Windows-server med services managementkonsolen.</span><span class="sxs-lookup"><span data-stu-id="af19d-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="af19d-108">Du kan också kontrollera status för agenten i Azure-portalen genom att klicka på knappen Visa lokala agenter.</span><span class="sxs-lookup"><span data-stu-id="af19d-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="af19d-109">Se till att du anger värdet för fältet "Användarnamn på arbetsdag" i formatet username@workday-klientorganisationsnamn.</span><span class="sxs-lookup"><span data-stu-id="af19d-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="af19d-110">Om arbetsdagens klientorganisationsnamn saknas misslyckas autentiseringen arbetsdagar.</span><span class="sxs-lookup"><span data-stu-id="af19d-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="af19d-111">Om du konfigurerar integreringen med workday-implementeringsklientorganisationen noterar du de schemalagda avbrottstimmarna för din arbetsdag-klientorganisation.</span><span class="sxs-lookup"><span data-stu-id="af19d-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="af19d-112">Arbetsdagar har planerat nedtid för sina implementeringsklienter under helger (vanligtvis från fredags kväll till lördag morgon) och anslutningsproblem under det här avbrottsfönstret är ett känt problem som automatiskt löses så snart implementeringsklienterna är online igen.</span><span class="sxs-lookup"><span data-stu-id="af19d-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="af19d-113">I sällsynta fall kan du även se det här felet om lösenordet för användaren av integrationssystemet har ändrats på grund av uppdatering av klientorganisationen eller om kontot är i låst eller utgånget läge.</span><span class="sxs-lookup"><span data-stu-id="af19d-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="af19d-114">Kontrollera statusen för användaren av integrationssystemet med din arbetsdagarsadministratör.</span><span class="sxs-lookup"><span data-stu-id="af19d-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="af19d-115">Mer information om hur du konfigurerar arbetsdagar för automatisk etablering finns i [Självstudiekurs: Konfigurera arbetsdagar för automatisk användaretablering.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="af19d-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
