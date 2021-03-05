---
title: Problem med attribut- och scopingfilter
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
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482923"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="7f946-102">Problem med attribut- och scopingfilter</span><span class="sxs-lookup"><span data-stu-id="7f946-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="7f946-103">**Problem med upn-värden i konflikt**</span><span class="sxs-lookup"><span data-stu-id="7f946-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="7f946-104">Arbetsdagar till AD-användaretablering – arbetsdagar till AD-användaretablering visar **felmeddelandet HybridSynkroniseringActiveDirectoryUserPrincipalNameNotUnique.**</span><span class="sxs-lookup"><span data-stu-id="7f946-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="7f946-105">Åtgärden misslyckades eftersom UPN-värde som angetts för tillägg/ändring inte är unikt för hela skogen.</span><span class="sxs-lookup"><span data-stu-id="7f946-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="7f946-106">Felinformation: **CONSTRAINT_ATT_TYPE – userPrincipalName.**</span><span class="sxs-lookup"><span data-stu-id="7f946-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="7f946-107">Värdet **för userPrincipalName** som Workday-kopplingen försöker ange när AD-användarkontot skapas finns redan i AD-måldomänen.</span><span class="sxs-lookup"><span data-stu-id="7f946-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="7f946-108">Detta antyder att antingen (1) användaren redan finns och att den matchande ID-kontrollen misslyckades för användaren eller (2) genererade UPN-regeln ett värde i konflikt.</span><span class="sxs-lookup"><span data-stu-id="7f946-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="7f946-109">Här är de föreslagna lösningsstegen:</span><span class="sxs-lookup"><span data-stu-id="7f946-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="7f946-110">Om det inte gick att länka arbetsdagar-kontot till Active Directory-kontot och det inte gick att länka det matchande ID-attributet (normalt anställnings-ID) i både Arbetsdagar och AD om det redan finns en exakt matchning.</span><span class="sxs-lookup"><span data-stu-id="7f946-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="7f946-111">Om de inte har någon matchning är det ett dataproblem som måste åtgärdas.</span><span class="sxs-lookup"><span data-stu-id="7f946-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="7f946-112">Om anställnings-ID:t i Arbetsdagar till exempel är 001052 och i AD är det 1052 går det inte att länka de två kontona och försöker skapa en användare som redan finns.</span><span class="sxs-lookup"><span data-stu-id="7f946-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="7f946-113">Lösningen i det här fallet är att ändra värdet för **Anställnings-ID** i AD så att inledande nollor inkluderas så att det blir 001052.</span><span class="sxs-lookup"><span data-stu-id="7f946-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="7f946-114">Om UPN-genererande uttryck inte genererar ett unikt värde bör du överväga att använda avdupliceringsfunktionen **SelectUniqueValue** för att generera ett unikt värde varje gång.</span><span class="sxs-lookup"><span data-stu-id="7f946-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="7f946-115">**Arbetsdagar till AD-användaretablering anger inte managerattributvärdet för AD-användarkontot**</span><span class="sxs-lookup"><span data-stu-id="7f946-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="7f946-116">Arbetsdagar till AD-jobbet för användaretablering anger inte **managerattributvärdet** för AD-användarkonton.</span><span class="sxs-lookup"><span data-stu-id="7f946-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="7f946-117">Det finns två möjliga scenarier när det här beteendet visas:</span><span class="sxs-lookup"><span data-stu-id="7f946-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="7f946-118">Chefen under Arbetsdagar kan inte matchas med ett motsvarande AD-användarkonto eftersom chefen inte omfattas.</span><span class="sxs-lookup"><span data-stu-id="7f946-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="7f946-119">I ett **scenario med flera AD-domäner** finns inte chefen i Arbetsdag i samma domän som användaren.</span><span class="sxs-lookup"><span data-stu-id="7f946-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="7f946-120">Prova följande för att lösa problemet:</span><span class="sxs-lookup"><span data-stu-id="7f946-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="7f946-121">Om du har definierat omfattningsfilter kontrollerar du först om chefen ingår i omfattningen och att den uppfyller omfattningssatsen.</span><span class="sxs-lookup"><span data-stu-id="7f946-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="7f946-122">Om chefen inte uppfyller omfattningen för filtret ändrar du filtret så att chefen också omfattas av etableringsåtgärden.</span><span class="sxs-lookup"><span data-stu-id="7f946-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="7f946-123">Om du har flera AD-domäner har kopplingen en känd begränsning av att det inte går att lösa referenser till flera domänhanterare.</span><span class="sxs-lookup"><span data-stu-id="7f946-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="7f946-124">Mer information om hur du konfigurerar arbetsdagar för automatisk etablering finns i [Självstudiekurs: Konfigurera arbetsdagar för automatisk användaretablering.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="7f946-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













