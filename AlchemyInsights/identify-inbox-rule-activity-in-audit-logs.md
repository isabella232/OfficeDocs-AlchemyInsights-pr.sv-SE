---
title: Identifiera regelaktivitet i inkorgsregel i granskningsloggar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716442"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="787a7-102">Identifiera regelaktivitet i inkorgsregel i granskningsloggar</span><span class="sxs-lookup"><span data-stu-id="787a7-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="787a7-103">Du kan använda granskningsloggsökning i Microsoft 365 Security & Compliance Center för att visa inkorgsregelhändelser (skapa, ändra och ta bort inkorgsregler).</span><span class="sxs-lookup"><span data-stu-id="787a7-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="787a7-104">Logga in på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="787a7-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="787a7-105">Gå till söksidan **för sökfunktionen i** > **sökgranskning.**</span><span class="sxs-lookup"><span data-stu-id="787a7-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="787a7-106">Välj datumintervall i fälten **Startdatum** och **Slutdatum.**</span><span class="sxs-lookup"><span data-stu-id="787a7-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="787a7-107">Kontrollera **Exchange Mailbox Activities**att fältet **Aktiviteter** är inställt på Regel för **Ny inkorgRule Skapa/ändra/aktivera/inaktivera inkorgsregeln**.</span><span class="sxs-lookup"><span data-stu-id="787a7-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="787a7-108">Klicka på **Sök**.</span><span class="sxs-lookup"><span data-stu-id="787a7-108">Click **Search**.</span></span>

<span data-ttu-id="787a7-109">Välj en granskningspost i resultatet.</span><span class="sxs-lookup"><span data-stu-id="787a7-109">In the results, select an audit record.</span></span> <span data-ttu-id="787a7-110">Klicka på **Mer information**i informationsutfällbara.</span><span class="sxs-lookup"><span data-stu-id="787a7-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="787a7-111">Information om inkorgsregelinställningarna visas i fältet **Parametrar.**</span><span class="sxs-lookup"><span data-stu-id="787a7-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="787a7-112">Mer information finns i [Bestämma om en användare har skapat en inkorgsregel](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="787a7-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
