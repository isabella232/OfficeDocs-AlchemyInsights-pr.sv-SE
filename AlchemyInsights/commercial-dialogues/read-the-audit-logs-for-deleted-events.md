---
title: Läsa granskningsloggarna för borttagna händelser
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483319"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="dfc5d-102">Läsa granskningsloggarna för borttagna händelser</span><span class="sxs-lookup"><span data-stu-id="dfc5d-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="dfc5d-103">Gör så här:</span><span class="sxs-lookup"><span data-stu-id="dfc5d-103">Here's how to do this:</span></span>

1. <span data-ttu-id="dfc5d-104">Gå till [Säkerhets- och & Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="dfc5d-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="dfc5d-105">Välj **Sök**  >  [**granskningsloggsökning.**](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="dfc5d-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="dfc5d-106">Om du ser ett meddelande om att du måste aktivera funktionen kan du aktivera den nu.</span><span class="sxs-lookup"><span data-stu-id="dfc5d-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="dfc5d-107">Om funktionen inte är aktiverad kan inte sökresultat hämta data från tidigare datum.</span><span class="sxs-lookup"><span data-stu-id="dfc5d-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="dfc5d-108">Välj **Aktiviteter** och sök sedan efter **aktiviteter i Exchange-postlådan.**</span><span class="sxs-lookup"><span data-stu-id="dfc5d-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="dfc5d-109">Välj **borttagna meddelanden från mappen Borttaget** och **flyttade meddelanden till mappalternativen Borttaget.**</span><span class="sxs-lookup"><span data-stu-id="dfc5d-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="dfc5d-110">När du är klar klickar du utanför fönstret för att minimera **fönstret** Aktiviteter.</span><span class="sxs-lookup"><span data-stu-id="dfc5d-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="dfc5d-111">Ange datumintervallet och välj sedan **användarnamnet** för den användare du vill undersöka i rutan Användare.</span><span class="sxs-lookup"><span data-stu-id="dfc5d-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="dfc5d-112">Du kan välja flera användare åt gången.</span><span class="sxs-lookup"><span data-stu-id="dfc5d-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="dfc5d-113">Välj **Sök.**</span><span class="sxs-lookup"><span data-stu-id="dfc5d-113">Select **Search**.</span></span> <span data-ttu-id="dfc5d-114">Aktiviteterna visas under **Resultat.**</span><span class="sxs-lookup"><span data-stu-id="dfc5d-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="dfc5d-115">Om du vill visa informationen väljer du en aktivitet och sedan **Mer information.**</span><span class="sxs-lookup"><span data-stu-id="dfc5d-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="dfc5d-116">Mer information om det borttagna objektet, till exempel ämnesraden och objektets plats när det togs bort, visas i fältet **AffectedItems.**</span><span class="sxs-lookup"><span data-stu-id="dfc5d-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="dfc5d-117">Du kan inte återställa borttagna objekt med hjälp av granskningsloggfunktionen.</span><span class="sxs-lookup"><span data-stu-id="dfc5d-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="dfc5d-118">Information om hur du återställer borttagna objekt [finns i Återskapa borttagna objekt eller e-post i Outlook Web App.](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="dfc5d-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="dfc5d-119">Mer information finns i Söka [i Office 365-granskningsloggen för att felsöka vanliga scenarier.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="dfc5d-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
