---
title: Identifiera Inkorgen regeln aktivitet i granskningsloggar
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1201a625948743cacfaa58410abeb4108ed2eb56
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539191"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="2cc4a-102">Identifiera Inkorgen regeln aktivitet i granskningsloggar</span><span class="sxs-lookup"><span data-stu-id="2cc4a-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="2cc4a-103">Du kan använda Granska loggen Sök i Office 365 säkerhet & regelefterlevnadscentret Inkorgen regeln händelser (skapa, ändra och ta bort regler för Inkorgen).</span><span class="sxs-lookup"><span data-stu-id="2cc4a-103">You can use audit log search in the Office 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="2cc4a-104">Logga in på [Office 365 säkerhet & regelefterlevnadscentret](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="2cc4a-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="2cc4a-105">Gå till **Sök** > **Granska loggen** söksida.</span><span class="sxs-lookup"><span data-stu-id="2cc4a-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="2cc4a-106">Välj datumintervall i fälten **startdatum** och **slutdatum** .</span><span class="sxs-lookup"><span data-stu-id="2cc4a-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="2cc4a-107">Under **Aktiviteter för Exchange-postlåda**, Kontrollera fältet **aktiviteter** anges till **New-InboxRule skapa/ändra/aktivera/inaktivera Inkorgsregel**.</span><span class="sxs-lookup"><span data-stu-id="2cc4a-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="2cc4a-108">Klicka på **Sök**.</span><span class="sxs-lookup"><span data-stu-id="2cc4a-108">Click **Search**.</span></span>

<span data-ttu-id="2cc4a-109">Markera en granskningspost i resultatet.</span><span class="sxs-lookup"><span data-stu-id="2cc4a-109">In the results, select an audit record.</span></span> <span data-ttu-id="2cc4a-110">Klicka på **Mer Information**i information-utfällbar.</span><span class="sxs-lookup"><span data-stu-id="2cc4a-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="2cc4a-111">Information om inställningar för Inkorgen regeln visas i fältet **parametrar** .</span><span class="sxs-lookup"><span data-stu-id="2cc4a-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="2cc4a-112">Mer information finns i [fastställa om en användare har skapat en Inkorgsregel](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="2cc4a-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
