---
title: Flera aktiva sessioner till samma postlåda
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1836"
- "9000248"
ms.openlocfilehash: d2fd3f20346012baed21efd4900ca4cf73391d91
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439722"
---
# <a name="multiple-active-sessions-to-the-same-mailbox"></a><span data-ttu-id="fe521-102">Flera aktiva sessioner till samma postlåda</span><span class="sxs-lookup"><span data-stu-id="fe521-102">Multiple active sessions to the same mailbox</span></span>

<span data-ttu-id="fe521-103">För att styra användningen av Exchange-resurser har en postlåda en "budget".</span><span class="sxs-lookup"><span data-stu-id="fe521-103">To control usage of Exchange resources, a mailbox has a "budget."</span></span>

<span data-ttu-id="fe521-104">Undantaget över budget kan utlösas av, men är inte begränsat till, följande omständigheter:</span><span class="sxs-lookup"><span data-stu-id="fe521-104">The over-budget exception can be triggered by, but is not limited to, the following circumstances:</span></span>

- <span data-ttu-id="fe521-105">Några webbläsarflikar öppnas i samma Outlook Web App-session.</span><span class="sxs-lookup"><span data-stu-id="fe521-105">A few browser tabs are opened within the same Outlook Web App session.</span></span>

- <span data-ttu-id="fe521-106">Några aktiva Outlook Web App-sessioner till samma postlåda.</span><span class="sxs-lookup"><span data-stu-id="fe521-106">A few active Outlook Web App sessions to the same mailbox.</span></span>

- <span data-ttu-id="fe521-107">Några andra klientprogram (Outlook, Outlook Mobile, en klientapp från tredje part) har åtkomst till postlådan samtidigt.</span><span class="sxs-lookup"><span data-stu-id="fe521-107">A few other client applications (Outlook, Outlook Mobile, a third party client app) access the mailbox at the same time.</span></span>

- <span data-ttu-id="fe521-108">Tidskrävande åtgärder, till exempel att köra sökbegäranden, utförs från en annan aktiv postlådesession.</span><span class="sxs-lookup"><span data-stu-id="fe521-108">Long running operations, such as executing search requests, are performed from another active mailbox session.</span></span>

