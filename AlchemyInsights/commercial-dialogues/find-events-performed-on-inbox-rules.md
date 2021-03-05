---
title: Hitta händelser som utförs för inkorgsregler
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483705"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="59b28-102">Hitta händelser som utförs för inkorgsregler</span><span class="sxs-lookup"><span data-stu-id="59b28-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="59b28-103">När regler för Inkorgen skapas, ändras eller tas bort registreras händelserna i granskningsloggen.</span><span class="sxs-lookup"><span data-stu-id="59b28-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="59b28-104">Så här granskar du dem:</span><span class="sxs-lookup"><span data-stu-id="59b28-104">Here's how to review them:</span></span>

1. <span data-ttu-id="59b28-105">Gå till [Säkerhets- och & Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="59b28-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="59b28-106">Välj Sök > granskningsloggsökning.</span><span class="sxs-lookup"><span data-stu-id="59b28-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="59b28-107">Om du ser ett meddelande om att du måste aktivera granskning kan du aktivera den nu.</span><span class="sxs-lookup"><span data-stu-id="59b28-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="59b28-108">Om den här funktionen inte är aktiverad kan inte sökresultat hämta data från tidigare datum.</span><span class="sxs-lookup"><span data-stu-id="59b28-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="59b28-109">Markera fältet Aktiviteter och sök efter Aktiviteter i Exchange-postlådan och välj sedan New-InboxRule skapa inkorgsregel från Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="59b28-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="59b28-110">När du är klar klickar du utanför fönstret för att minimera fönstret Aktiviteter.</span><span class="sxs-lookup"><span data-stu-id="59b28-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="59b28-111">Ange datumintervallet och välj sedan användarnamnet för den användare du vill undersöka i fältet Användare.</span><span class="sxs-lookup"><span data-stu-id="59b28-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="59b28-112">Du kan välja flera användare åt gången.</span><span class="sxs-lookup"><span data-stu-id="59b28-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="59b28-113">Välj Sök.</span><span class="sxs-lookup"><span data-stu-id="59b28-113">Select Search.</span></span> <span data-ttu-id="59b28-114">Aktiviteterna visas under Resultat.</span><span class="sxs-lookup"><span data-stu-id="59b28-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="59b28-115">Om du vill visa information väljer du en aktivitet och sedan Mer information.</span><span class="sxs-lookup"><span data-stu-id="59b28-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="59b28-116">Under avsnittet Parametrar ser du namnet på regeln, villkorsuppsättningen och de åtgärder som regeln kommer att vidta.</span><span class="sxs-lookup"><span data-stu-id="59b28-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="59b28-117">Mer information finns i Söka i Office 365-granskningsloggen för att felsöka vanliga scenarier.</span><span class="sxs-lookup"><span data-stu-id="59b28-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>