---
title: Kalender-ikonen visas inte i Teams-klienten
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819971"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="9aa00-102">Kalender-ikonen visas inte i Teams-klienten</span><span class="sxs-lookup"><span data-stu-id="9aa00-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="9aa00-103">Fliken Kalender i Teams kräver åtkomst till en Exchange-postlåda via Exchange webbtjänster.</span><span class="sxs-lookup"><span data-stu-id="9aa00-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="9aa00-104">Exchange-postlådan kan vara online eller lokal.</span><span class="sxs-lookup"><span data-stu-id="9aa00-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="9aa00-105">För online-användare som inte kan se fliken Kalender ser du till att de [har licens för en Exchange Online-postlåda och att postlådan är aktiverad](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="9aa00-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="9aa00-106">Det kan vara problem med nätverket om användaren har en giltig postlåda i Exchange Online men fortfarande inte kan se fliken Kalender.</span><span class="sxs-lookup"><span data-stu-id="9aa00-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="9aa00-107">Använd [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) och kör **Anslutningstest för Microsoft Exchange webbtjänster** för den påverkade användaren.</span><span class="sxs-lookup"><span data-stu-id="9aa00-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="9aa00-108">Kontrollera slutligen [Teams-appar – principer för programkonfiguration](https://admin.teams.microsoft.com/policies/app-setup) för att säkerställa att kalenderprogrammet inte har tagits bort från principen som används för användaren (troligen **globala (standard för hela organisationen)**.</span><span class="sxs-lookup"><span data-stu-id="9aa00-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="9aa00-109">Om användarna är finns lokalt måste du bekräfta att hybridkonfigurationen är felfri.</span><span class="sxs-lookup"><span data-stu-id="9aa00-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="9aa00-110">Använd [Guiden för hybridkonfiguration](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) för felsökning.</span><span class="sxs-lookup"><span data-stu-id="9aa00-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="9aa00-111">Observera att [Teams kräver Exchange 2016 CU3 eller senare](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="9aa00-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
