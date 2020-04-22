---
title: ATP för SharePoint, OneDrive och Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 28046c61e1aedbb2c07cca3fc01b118d0dc3c143
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sv-SE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43712476"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="63c5c-102">ATP för SharePoint, OneDrive och Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="63c5c-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="63c5c-103">Så här aktiverar du Avancerat skydd mot hot:</span><span class="sxs-lookup"><span data-stu-id="63c5c-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="63c5c-104">Gå [https://protection.office.com](https://protection.office.com) till och logga in med ett globalt administratörs- eller säkerhetsadministratörskonto.</span><span class="sxs-lookup"><span data-stu-id="63c5c-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="63c5c-105">Välj **Principsäkra** \> bilagor i det vänstra **navigeringsfönstret**under **Hothantering**.</span><span class="sxs-lookup"><span data-stu-id="63c5c-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="63c5c-106">Välj **Aktivera ATP för SharePoint, OneDrive och Microsoft Teams**.</span><span class="sxs-lookup"><span data-stu-id="63c5c-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="63c5c-107">[Skapa en aktivitetsaviseringsprincip](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) för att ta emot meddelanden när vi upptäcker skadliga filer.</span><span class="sxs-lookup"><span data-stu-id="63c5c-107">[Create an activity alert policy](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="63c5c-108">Fullständiga instruktioner finns i det här [avsnittet](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="63c5c-108">For complete instructions, see this [topic](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="63c5c-109">**Atp**genom design söker inte igenom varenda fil i SharePoint Online, OneDrive för företag eller Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="63c5c-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="63c5c-110">Filer genomsöks asynkront av en process som använder delningsaktivitet, gästaktivitet och hotsignaler för att identifiera skadliga filer.</span><span class="sxs-lookup"><span data-stu-id="63c5c-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="63c5c-111">Mer information finns i det här [avsnittet](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="63c5c-111">For more information, see this [topic](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
