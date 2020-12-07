---
title: Kalender ikonen visas inte i Microsoft Teams-klienten
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583928"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a><span data-ttu-id="069d7-102">Kalender ikonen visas inte i Microsoft Teams-klienten</span><span class="sxs-lookup"><span data-stu-id="069d7-102">Calendar icon isn't showing in Microsoft Teams client</span></span>

<span data-ttu-id="069d7-103">Fliken **kalender** i Teams kräver åtkomst till en Exchange-postlåda via Exchange Web Services.</span><span class="sxs-lookup"><span data-stu-id="069d7-103">The **Calendar** Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="069d7-104">Exchange-postlådan kan vara online eller lokalt.</span><span class="sxs-lookup"><span data-stu-id="069d7-104">The Exchange mailbox can be Online, or On-Premises.</span></span> <span data-ttu-id="069d7-105">För onlineanvändare som inte ser fliken **kalender** kontrollerar du att de [är licensierade för en Exchange Online-postlåda och att post lådan är aktive rad](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="069d7-105">For Online users who do not see the **Calendar** Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span> <span data-ttu-id="069d7-106">Om användarna är lokala måste du bekräfta att din hybrid konfiguration är felfri.</span><span class="sxs-lookup"><span data-stu-id="069d7-106">If your users are homed On-Premises, you need to confirm that your Hybrid configuration is healthy.</span></span> <span data-ttu-id="069d7-107">Använd [Guiden för hybridkonfiguration](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) för felsökning.</span><span class="sxs-lookup"><span data-stu-id="069d7-107">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span> <span data-ttu-id="069d7-108">Observera att [Teams kräver Exchange 2016 CU3 eller senare](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="069d7-108">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>

<span data-ttu-id="069d7-109">Mer information och fel söknings anvisningar finns i [Felsöka problem med interaktioner i Microsoft Teams och Exchange Server](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span><span class="sxs-lookup"><span data-stu-id="069d7-109">For more information and troubleshooting steps, see [Troubleshoot Microsoft Teams and Exchange Server interaction issues](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span></span>
