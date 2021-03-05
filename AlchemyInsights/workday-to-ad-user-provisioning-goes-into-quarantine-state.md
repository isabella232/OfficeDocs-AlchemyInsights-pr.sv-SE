---
title: Arbetsdagar till AD-användaretablering sätts i karantän
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482905"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="58b43-102">Arbetsdagar till AD-användaretablering sätts i karantän</span><span class="sxs-lookup"><span data-stu-id="58b43-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="58b43-103">**Arbetsdagar till AD-användaretablering sätts i karantän och inga användare skapas i AD**</span><span class="sxs-lookup"><span data-stu-id="58b43-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="58b43-104">Jobbet för etablering av användare i AD har satts i karantän och granskningsloggarna visar exportfelhändelser med felmeddelandet **Fel: OperationsError-SvcErr: Ett åtgärdsfel inträffade. Ingen överordnad referens har konfigurerats för katalogtjänsten. Katalogtjänsten kan därför inte utfärda referenser till objekt utanför** den här skogen.</span><span class="sxs-lookup"><span data-stu-id="58b43-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="58b43-105">Det här felet visas vanligtvis om OU för Active Directory-behållaren inte är korrekt inställd eller om det uppstår problem med uttrycksmappningen som används för **parentEstinguishedName.**</span><span class="sxs-lookup"><span data-stu-id="58b43-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="58b43-106">Kontrollera om det finns stavfel **i standard-OU:n** för parametern Nya användare.</span><span class="sxs-lookup"><span data-stu-id="58b43-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="58b43-107">Kontrollera att den angivna OU:n redan finns i AD.</span><span class="sxs-lookup"><span data-stu-id="58b43-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="58b43-108">Om du använder **parentDistinguishedName** i attributmappningen ska du se till att det alltid utvärderas till en känd behållare i AD-domänen.</span><span class="sxs-lookup"><span data-stu-id="58b43-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="58b43-109">Kontrollera exporthändelsen i granskningsloggarna för att se det genererade värdet.</span><span class="sxs-lookup"><span data-stu-id="58b43-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="58b43-110">Mer information om hur du konfigurerar arbetsdagar för automatisk etablering finns i [Självstudiekurs: Konfigurera arbetsdagar för automatisk användaretablering.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="58b43-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

