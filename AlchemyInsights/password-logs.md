---
title: Lösenordsloggar
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527183"
---
# <a name="password-logs"></a><span data-ttu-id="d65e0-102">Lösenordsloggar</span><span class="sxs-lookup"><span data-stu-id="d65e0-102">Password logs</span></span>

<span data-ttu-id="d65e0-103">**Jag har problem med att komma åt granskningsloggar för återställning av lösenord**</span><span class="sxs-lookup"><span data-stu-id="d65e0-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="d65e0-104">Så här felsöker du problem med åtkomst till granskningsloggar för återställning av lösenord:</span><span class="sxs-lookup"><span data-stu-id="d65e0-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="d65e0-105">Se till att du har behörighet att visa granskningsloggar.</span><span class="sxs-lookup"><span data-stu-id="d65e0-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="d65e0-106">Endast följande roller är behöriga:</span><span class="sxs-lookup"><span data-stu-id="d65e0-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="d65e0-107">Global administratör</span><span class="sxs-lookup"><span data-stu-id="d65e0-107">Global administrator</span></span>
 - <span data-ttu-id="d65e0-108">Säkerhetsadministratör</span><span class="sxs-lookup"><span data-stu-id="d65e0-108">Security administrator</span></span>
 - <span data-ttu-id="d65e0-109">Säkerhetsläsare</span><span class="sxs-lookup"><span data-stu-id="d65e0-109">Security reader</span></span>

<span data-ttu-id="d65e0-110">**Jag vill se alla granskningshändelser för återställning av lösenord från den tidpunkt jag först distribuerade**</span><span class="sxs-lookup"><span data-stu-id="d65e0-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="d65e0-111">Upp till 120 000 händelser för återställning av lösenord och registrering lagras i rapporter för de senaste 30 dagarna.</span><span class="sxs-lookup"><span data-stu-id="d65e0-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="d65e0-112">Den här maxgränsen gäller för användargränssnittet när CSV-filen laddas ned.</span><span class="sxs-lookup"><span data-stu-id="d65e0-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="d65e0-113">1 miljon händelser är tillgängliga via PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d65e0-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="d65e0-114">Mer information finns i länkarna nedan:</span><span class="sxs-lookup"><span data-stu-id="d65e0-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="d65e0-115">Självbetjäning för återställning av lösenord från API:t för Azure AD-rapporter och -händelser</span><span class="sxs-lookup"><span data-stu-id="d65e0-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="d65e0-116">Så här laddar du ned registreringshändelser för återställning av lösenord snabbt med PowerShell</span><span class="sxs-lookup"><span data-stu-id="d65e0-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="d65e0-117">**Jag vill veta mer om rapporteringsfunktioner för återställning av lösenord**</span><span class="sxs-lookup"><span data-stu-id="d65e0-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="d65e0-118">Kontrollera vem som registrerar eller återställer lösenord med granskningsloggar för återställning av lösenord i Azure-portalen under **Användare och grupper.**</span><span class="sxs-lookup"><span data-stu-id="d65e0-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="d65e0-119">Mer information finns i följande länkar:</span><span class="sxs-lookup"><span data-stu-id="d65e0-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="d65e0-120">Översikt över rapporter för återställning av lösenord</span><span class="sxs-lookup"><span data-stu-id="d65e0-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="d65e0-121">Så här visar du rapporter om återställning av lösenord i Azure Portal</span><span class="sxs-lookup"><span data-stu-id="d65e0-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="d65e0-122">Självbetjäning för återställning av lösenord från API:t för Azure AD-rapporter och -händelser</span><span class="sxs-lookup"><span data-stu-id="d65e0-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="d65e0-123">Så här laddar du ned registreringshändelser för återställning av lösenord snabbt med PowerShell</span><span class="sxs-lookup"><span data-stu-id="d65e0-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


