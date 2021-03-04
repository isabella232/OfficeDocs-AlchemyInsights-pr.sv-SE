---
title: Problem med en enskild användare
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
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430208"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="f1d54-102">Problem med en enskild användare</span><span class="sxs-lookup"><span data-stu-id="f1d54-102">Problem with single user</span></span>

- <span data-ttu-id="f1d54-103">Användaren kanske inte har etablerats eftersom tjänsten inte har haft möjlighet att utvärdera användaren ännu.</span><span class="sxs-lookup"><span data-stu-id="f1d54-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="f1d54-104">Läs vägledningen för hur lång tid etableringen tar samt förloppsfältet på konfigurationssidan för etablering.</span><span class="sxs-lookup"><span data-stu-id="f1d54-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="f1d54-105">Om den stadiga statusen som anges i avsnittet med ytterligare information ligger före datumet då användaren skapades/uppdaterades/togs bort, innebär det att vi inte har utvärderat användaren ännu.</span><span class="sxs-lookup"><span data-stu-id="f1d54-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="f1d54-106">I det här scenariot är det bäst att vänta till etableringstjänsten slutförs.</span><span class="sxs-lookup"><span data-stu-id="f1d54-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="f1d54-107">Observera att vår tjänst endast är medveten om ändringar för en användare i källsystemet (Cloud HR).</span><span class="sxs-lookup"><span data-stu-id="f1d54-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="f1d54-108">Det måste göras en giltig ändring i källsystemet för att Azure AD ska kunna identifiera ändringen och föra den till Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f1d54-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="f1d54-109">Etableringstjänsten utvärderade användaren och kom fram till att den inte bör tillhandahållas:</span><span class="sxs-lookup"><span data-stu-id="f1d54-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="f1d54-110">Om du har angett ett attributbaserat filter, kontrollera att användaren uppfyller de villkor som du har angett.</span><span class="sxs-lookup"><span data-stu-id="f1d54-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="f1d54-111">Om användarna redan finns i målsystemet och användarens status i källan och målmatchning kommer vi inte att vidta någon ytterligare åtgärd.</span><span class="sxs-lookup"><span data-stu-id="f1d54-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="f1d54-112">Etableringstjänsten försökte etablera användaren och misslyckades.</span><span class="sxs-lookup"><span data-stu-id="f1d54-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="f1d54-113">För dessa scenarier granskar du fliken felsökning och rekommendationer i etableringsloggarna:</span><span class="sxs-lookup"><span data-stu-id="f1d54-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="f1d54-114">Ett obligatoriskt attribut för användaren kanske saknas i lokal Active Directory eller Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f1d54-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="f1d54-115">Till exempel skapar inte reglerna för userPrincipalName eller sAMAccountName rätt värde.</span><span class="sxs-lookup"><span data-stu-id="f1d54-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="f1d54-116">Det matchande attributet (vanligtvis employeeId) löser inte mot en unik användare i en lokal Active Directory eller Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f1d54-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="f1d54-117">Det finns till exempel två användare med samma anställningsnr i AD och tjänsten returnerar en felkod som anger dubblettmålposter för samma källpost.</span><span class="sxs-lookup"><span data-stu-id="f1d54-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="f1d54-118">Om du vill granska loggar för enskild användare och grupper kan du [läsa i etableringsloggarna för ett problem med en viss användare.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)</span><span class="sxs-lookup"><span data-stu-id="f1d54-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
