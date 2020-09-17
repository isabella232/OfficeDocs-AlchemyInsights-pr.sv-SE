---
title: Identifiera aktivitet för inkorgstransaktion i gransknings loggar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779069"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="57c35-102">Identifiera aktivitet för inkorgstransaktion i gransknings loggar</span><span class="sxs-lookup"><span data-stu-id="57c35-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="57c35-103">Du kan använda gransknings loggs ökning i Microsoft 365 Security & Compliance Center för att visa händelser för Inkorgshanteraren (skapa, ändra och ta bort regler för Inkorgen).</span><span class="sxs-lookup"><span data-stu-id="57c35-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="57c35-104">Logga in på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="57c35-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="57c35-105">Gå till sidan **Sök**  >  **gransknings loggs sökning** .</span><span class="sxs-lookup"><span data-stu-id="57c35-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="57c35-106">Välj datum intervall i fälten **start datum** och **slutdatum** .</span><span class="sxs-lookup"><span data-stu-id="57c35-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="57c35-107">Under **Exchange-postaktiviteter**kontrollerar du att fältet **aktiviteter** är inställt på **ny-InboxRule skapa/ändra/Aktivera/inaktivera regler för Inkorgen**.</span><span class="sxs-lookup"><span data-stu-id="57c35-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="57c35-108">Klicka på **Sök**.</span><span class="sxs-lookup"><span data-stu-id="57c35-108">Click **Search**.</span></span>

<span data-ttu-id="57c35-109">Välj en gransknings post i resultatet.</span><span class="sxs-lookup"><span data-stu-id="57c35-109">In the results, select an audit record.</span></span> <span data-ttu-id="57c35-110">I den utfällbara informationen klickar du på **Mer information**.</span><span class="sxs-lookup"><span data-stu-id="57c35-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="57c35-111">Information om inställningarna för regel för Inkorgen visas i **parameter** fältet.</span><span class="sxs-lookup"><span data-stu-id="57c35-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="57c35-112">Mer information finns i [avgöra om en användare har skapat en regel för Inkorgen](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="57c35-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
