---
title: Hitta IP-adressen i granskningsloggen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483716"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="e6f72-102">Hitta IP-adressen i granskningsloggen</span><span class="sxs-lookup"><span data-stu-id="e6f72-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="e6f72-103">IP-adressen som motsvarar en aktivitet som utförts av en användare eller administratör visas i granskningsloggarna.</span><span class="sxs-lookup"><span data-stu-id="e6f72-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="e6f72-104">Klientinformationen loggas också.</span><span class="sxs-lookup"><span data-stu-id="e6f72-104">The client information is also logged.</span></span> <span data-ttu-id="e6f72-105">Så här identifierar du IP-adressen:</span><span class="sxs-lookup"><span data-stu-id="e6f72-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="e6f72-106">Gå till [Säkerhets- och & Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="e6f72-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="e6f72-107">Välj **Sök**  >  **[granskningsloggsökning.](https://go.microsoft.com/fwlink/?linkid=2103759)**</span><span class="sxs-lookup"><span data-stu-id="e6f72-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="e6f72-108">Om du ser ett meddelande om att du måste aktivera granskning kan du aktivera den nu.</span><span class="sxs-lookup"><span data-stu-id="e6f72-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="e6f72-109">Om den här funktionen inte är aktiverad kan inte sökresultatet hämta data från tidigare datum.</span><span class="sxs-lookup"><span data-stu-id="e6f72-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="e6f72-110">Om du är intresserad av en viss aktivitet väljer du den i **aktivitetslistan.** annars returneras alla aktiviteter för den valda användaren som standard.</span><span class="sxs-lookup"><span data-stu-id="e6f72-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="e6f72-111">Observera att vissa aktiviteter kanske inte är tillgängliga för markering från **menyn** Aktiviteter. Granskningsobjekten returneras emellertid om Visa resultat **för alla aktiviteter är** markerat (standardinställning).</span><span class="sxs-lookup"><span data-stu-id="e6f72-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="e6f72-112">Ange datumintervallet och välj **användarnamnet för** den användare du vill undersöka i fältet Användare.</span><span class="sxs-lookup"><span data-stu-id="e6f72-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="e6f72-113">Välj **Sök.**</span><span class="sxs-lookup"><span data-stu-id="e6f72-113">Select **Search**.</span></span> <span data-ttu-id="e6f72-114">Aktiviteterna visas under **Resultat.**</span><span class="sxs-lookup"><span data-stu-id="e6f72-114">The activities appear under **Results**.</span></span> <span data-ttu-id="e6f72-115">Du kan se IP-adressen för varje aktivitet.</span><span class="sxs-lookup"><span data-stu-id="e6f72-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="e6f72-116">Om du vill visa information väljer du en aktivitet och sedan **Mer information.**</span><span class="sxs-lookup"><span data-stu-id="e6f72-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="e6f72-117">Mer information finns i Söka i [Office 365-granskningsloggen för att felsöka vanliga scenarier.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="e6f72-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>