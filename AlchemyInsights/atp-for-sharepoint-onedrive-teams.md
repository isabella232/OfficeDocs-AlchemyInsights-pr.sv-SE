---
title: Tillgängligt att LOVA för SharePoint, OneDrive och Microsoft-team
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: b304f6c7d9959e49a8152c03f11c6c864a154ea5
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765454"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="a0219-102">Tillgängligt att LOVA för SharePoint, OneDrive och Microsoft-team</span><span class="sxs-lookup"><span data-stu-id="a0219-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="a0219-103">Gör så här om du vill aktivera avancerade Threat Protection:</span><span class="sxs-lookup"><span data-stu-id="a0219-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="a0219-104">Gå till [https://protection.office.com](https://protection.office.com) och logga in med en global administratör eller administratörskontot för säkerhet.</span><span class="sxs-lookup"><span data-stu-id="a0219-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="a0219-105">Välj **principen** i det vänstra navigeringsfönstret under **hantering av hot** \> **Säkra bifogade filer**.</span><span class="sxs-lookup"><span data-stu-id="a0219-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="a0219-106">Markera **Aktivera ATP för SharePoint, OneDrive, och Microsoft team**.</span><span class="sxs-lookup"><span data-stu-id="a0219-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="a0219-107">[Skapa en avisering principen aktiviteten](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) att ta emot meddelanden när vi identifiera skadliga filer.</span><span class="sxs-lookup"><span data-stu-id="a0219-107">[Create an activity alert policy](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="a0219-108">Fullständiga instruktioner finns i det här [avsnittet](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="a0219-108">For complete instructions, see this [topic](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="a0219-109">**Anmärkning**: avsiktligt ATP söker inte igenom varje enskild fil i SharePoint Online, OneDrive för företag eller Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a0219-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="a0219-110">Skannade filer asynkront med en process som använder en delad aktivitet, Gäst aktivitet och hot signalerar att identifiera skadliga filer.</span><span class="sxs-lookup"><span data-stu-id="a0219-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="a0219-111">Mer information finns i det här [avsnittet](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="a0219-111">For more information, see this [topic](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
