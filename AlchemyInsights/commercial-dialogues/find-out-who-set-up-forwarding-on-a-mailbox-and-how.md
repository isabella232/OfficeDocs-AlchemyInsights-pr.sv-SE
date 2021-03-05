---
title: Ta reda på vem som konfigurerade vidarebefordran för en postlåda och hur
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483355"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="b9b77-102">Ta reda på vem som konfigurerade vidarebefordran för en postlåda och hur</span><span class="sxs-lookup"><span data-stu-id="b9b77-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="b9b77-103">Om extern vidarebefordran har angetts för en postlåda granskas aktiviteten som en del av Set-Mailbox-cmdleten.</span><span class="sxs-lookup"><span data-stu-id="b9b77-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="b9b77-104">Så här hittar du aktiviteten i granskningsloggen:</span><span class="sxs-lookup"><span data-stu-id="b9b77-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="b9b77-105">Gå till [Säkerhets- och & Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="b9b77-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="b9b77-106">Välj **Sök** >  **granskningsloggsökning.**</span><span class="sxs-lookup"><span data-stu-id="b9b77-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="b9b77-107">Om du ser ett meddelande om att du måste aktivera granskning kan du aktivera den nu.</span><span class="sxs-lookup"><span data-stu-id="b9b77-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="b9b77-108">Om den här funktionen inte är aktiverad kan inte sökresultat hämta data från tidigare datum.</span><span class="sxs-lookup"><span data-stu-id="b9b77-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="b9b77-109">Kontrollera att fältet **Aktiviteter** är inställt på **Visa resultat för alla aktiviteter** (standard).</span><span class="sxs-lookup"><span data-stu-id="b9b77-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="b9b77-110">Ange datumintervallet.</span><span class="sxs-lookup"><span data-stu-id="b9b77-110">Specify the date range.</span></span> <span data-ttu-id="b9b77-111">Du behöver inte ange ett användarnamn.</span><span class="sxs-lookup"><span data-stu-id="b9b77-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="b9b77-112">Välj **Sök.**</span><span class="sxs-lookup"><span data-stu-id="b9b77-112">Select **Search**.</span></span> <span data-ttu-id="b9b77-113">Aktiviteterna visas under **Resultat.**</span><span class="sxs-lookup"><span data-stu-id="b9b77-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="b9b77-114">Välj **Filtrera resultat** och ange sedan Ange postlåda **i** fältet **Aktivitetsfilter.**</span><span class="sxs-lookup"><span data-stu-id="b9b77-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="b9b77-115">Då returneras **alla Aktiviteter för Uppsättningspostlåda.**</span><span class="sxs-lookup"><span data-stu-id="b9b77-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="b9b77-116">Om du vill visa informationen väljer du en aktivitet och sedan **Mer information.**</span><span class="sxs-lookup"><span data-stu-id="b9b77-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="b9b77-117">Under **Parametrar** kan du se vidarebefordran av e-postadressen som ställts in för postlådan.</span><span class="sxs-lookup"><span data-stu-id="b9b77-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="b9b77-118">**Användar-ID** representerar den användare som konfigurerade extern vidarebefordran för postlådan.</span><span class="sxs-lookup"><span data-stu-id="b9b77-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="b9b77-119">Mer information finns i Söka [i Office 365-granskningsloggen för att felsöka vanliga scenarier.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="b9b77-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>