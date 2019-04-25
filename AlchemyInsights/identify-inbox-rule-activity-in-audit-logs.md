---
title: Identifiera Inkorgen regeln aktivitet i granskningsloggar
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: 9339d9c58056f568dc994b75bffe39f2c8bbdd34
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417264"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="9e4e9-102">Identifiera Inkorgen regeln aktivitet i granskningsloggar</span><span class="sxs-lookup"><span data-stu-id="9e4e9-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="9e4e9-103">Du kan använda Granska loggen Sök i säkerhet & regelefterlevnadscentret Inkorgen regeln händelser (skapa, ändra och ta bort regler för Inkorgen).</span><span class="sxs-lookup"><span data-stu-id="9e4e9-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="9e4e9-104">Logga in på [Office 365 & överensstämmelse Säkerhetscenter](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="9e4e9-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="9e4e9-105">Klicka på **Sök och undersökningen** och välj **Granska loggen Sök**.</span><span class="sxs-lookup"><span data-stu-id="9e4e9-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="9e4e9-106">Välj datumintervall i fälten **startdatum** och **slutdatum** .</span><span class="sxs-lookup"><span data-stu-id="9e4e9-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="9e4e9-107">Under **Aktiviteter för Exchange-postlåda**, Kontrollera fältet **aktiviteter** anges till **New-InboxRule skapa/ändra/aktivera/inaktivera Inkorgsregel**.</span><span class="sxs-lookup"><span data-stu-id="9e4e9-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="9e4e9-108">Klicka på **Sök**.</span><span class="sxs-lookup"><span data-stu-id="9e4e9-108">Click **Search**.</span></span>

<span data-ttu-id="9e4e9-109">Markera en granskningspost i resultatet.</span><span class="sxs-lookup"><span data-stu-id="9e4e9-109">In the results, select an audit record.</span></span> <span data-ttu-id="9e4e9-110">Klicka på **Mer Information**i information-utfällbar.</span><span class="sxs-lookup"><span data-stu-id="9e4e9-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="9e4e9-111">Information om inställningar för Inkorgen regeln visas i fältet **parametrar** .</span><span class="sxs-lookup"><span data-stu-id="9e4e9-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="9e4e9-112">Mer information finns i [fastställa om en användare har skapat en Inkorgsregel](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="9e4e9-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
