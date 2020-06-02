---
title: Identifiera IP-adress och klient i granskningsloggar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508934"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="f2d60-102">Identifiera IP-adress och klient i granskningsloggar</span><span class="sxs-lookup"><span data-stu-id="f2d60-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="f2d60-103">IP-adressen som motsvarar en aktivitet av en Microsoft 365-användare eller administratör visas i granskningsloggarna.</span><span class="sxs-lookup"><span data-stu-id="f2d60-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="f2d60-104">Klientinformationen loggas också.</span><span class="sxs-lookup"><span data-stu-id="f2d60-104">The client information is also logged.</span></span> <span data-ttu-id="f2d60-105">Här är stegen för att identifiera sådan information</span><span class="sxs-lookup"><span data-stu-id="f2d60-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="f2d60-106">Logga in på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="f2d60-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="f2d60-107">Gå till söksidan **för sökfunktionen i**  >  **sökgranskning.**</span><span class="sxs-lookup"><span data-stu-id="f2d60-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="f2d60-108">Om du är intresserad av en viss aktivitet väljer du den i **listan Aktiviteter.**</span><span class="sxs-lookup"><span data-stu-id="f2d60-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="f2d60-109">Om inte, returneras alla aktiviteter för den valda användaren (standardinställning).</span><span class="sxs-lookup"><span data-stu-id="f2d60-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="f2d60-110">**Obs:** Vissa aktiviteter kanske inte är tillgängliga i **menyn Aktiviteter.** Dessa granskningsobjekt returneras dock om **Visa resultat för alla aktiviteter** är markerat (standardinställning).</span><span class="sxs-lookup"><span data-stu-id="f2d60-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="f2d60-111">Ange användarnamnet i fältet **Användare,** välj lämpligt datumintervall för aktiviteten och klicka sedan på **Sök**.</span><span class="sxs-lookup"><span data-stu-id="f2d60-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="f2d60-112">I resultaten kan du se IP-adressen för den aktiviteten i resultatfönstret.</span><span class="sxs-lookup"><span data-stu-id="f2d60-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="f2d60-113">Välj granskningsposten om du vill visa detaljerad information i **informationsutfällningen** (till exempel Klient, Användare som utförde åtgärden osv.).</span><span class="sxs-lookup"><span data-stu-id="f2d60-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="f2d60-114">Mer information finns [i Hitta IP-adressen för den dator som används för att komma åt ett komprometterat konto](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="f2d60-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
